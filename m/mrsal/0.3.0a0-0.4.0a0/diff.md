# Comparing `tmp/mrsal-0.3.0a0.tar.gz` & `tmp/mrsal-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrsal-0.3.0a0.tar", max compression
+gzip compressed data, was "mrsal-0.4.0a0.tar", max compression
```

## Comparing `mrsal-0.3.0a0.tar` & `mrsal-0.4.0a0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.3.0a0/LICENSE.txt
--rw-r--r--   0        0        0     6681 2023-02-24 05:58:19.559374 mrsal-0.3.0a0/README.md
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.3.0a0/mrsal/__init__.py
--rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.3.0a0/mrsal/config/__init__.py
--rw-r--r--   0        0        0     1175 2023-02-16 07:01:55.359449 mrsal-0.3.0a0/mrsal/config/config.py
--rw-r--r--   0        0        0      286 2022-08-17 10:39:13.102254 mrsal-0.3.0a0/mrsal/config/exceptions.py
--rw-r--r--   0        0        0     2431 2022-08-17 10:39:13.102254 mrsal-0.3.0a0/mrsal/config/logging.py
--rw-r--r--   0        0        0    24628 2023-02-24 05:58:19.559374 mrsal-0.3.0a0/mrsal/mrsal.py
--rw-r--r--   0        0        0      666 2023-02-24 05:59:54.229388 mrsal-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 mrsal-0.3.0a0/setup.py
--rw-r--r--   0        0        0     7403 1970-01-01 00:00:00.000000 mrsal-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2022-09-08 10:55:29.050700 mrsal-0.4.0a0/LICENSE.txt
+-rw-r--r--   0        0        0     8649 2023-04-25 11:22:46.987597 mrsal-0.4.0a0/README.md
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.4.0a0/mrsal/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-17 10:39:13.102254 mrsal-0.4.0a0/mrsal/config/__init__.py
+-rw-r--r--   0        0        0     1175 2023-02-16 07:01:55.359449 mrsal-0.4.0a0/mrsal/config/config.py
+-rw-r--r--   0        0        0      286 2022-08-17 10:39:13.102254 mrsal-0.4.0a0/mrsal/config/exceptions.py
+-rw-r--r--   0        0        0     2431 2022-08-17 10:39:13.102254 mrsal-0.4.0a0/mrsal/config/logging.py
+-rw-r--r--   0        0        0    28079 2023-04-25 11:18:08.038376 mrsal-0.4.0a0/mrsal/mrsal.py
+-rw-r--r--   0        0        0      666 2023-04-25 09:09:38.522739 mrsal-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 mrsal-0.4.0a0/PKG-INFO
```

### Comparing `mrsal-0.3.0a0/LICENSE.txt` & `mrsal-0.4.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mrsal-0.3.0a0/README.md` & `mrsal-0.4.0a0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -141,10 +141,63 @@
         requeue=False,
         callback_with_delivery_info=True
     )
 ```
 
 Done! Your first message of friendship has been sent to the friendship queue on the exchange of friendship.
 
+
+### 3 Concurrent Consumers
+
+Sometimes we need to start multiple consumers to listen to the **same** **queue** and process received messages **concurrently**. 
+You can do that by calling `start_concurrence_consumer` which takes `total_threads` param in addition to the same parameters used in `start_consumer`.
+This method will create a **thread pool** and _spawn new_ `Mrsal` object and start **new consumer** for every thread. 
+
+```python
+import json
+import time
+
+import pika
+from pika.exchange_type import ExchangeType
+
+import mrsal.config.config as config
+import tests.config as test_config
+from mrsal.mrsal import Mrsal
+
+
+mrsal = Mrsal(host=test_config.HOST,
+              port=config.RABBITMQ_PORT,
+              credentials=config.RABBITMQ_CREDENTIALS,
+              virtual_host=config.V_HOST)
+mrsal.connect_to_server()
+
+APP_ID = "TEST_CONCURRENT_CONSUMERS"
+EXCHANGE = "BOOKS"
+EXCHANGE_TYPE = ExchangeType.direct
+QUEUE_EMERGENCY = "SORT_BOOKS"
+NUM_THREADS = 3
+NUM_MESSAGES = 3
+INACTIVITY_TIMEOUT = 3
+ROUTING_KEY = "PROCESS BOOK"
+MESSAGE_ID = "LIBRARY"
+
+def test_concurrent_consumer():
+    # Start concurrent consumers
+    mrsal.start_concurrence_consumer(total_threads=NUM_THREADS, queue=QUEUE_EMERGENCY,
+                                     callback=consumer_callback_with_delivery_info,
+                                     callback_args=(test_config.HOST, QUEUE_EMERGENCY),
+                                     exchange=EXCHANGE, exchange_type=EXCHANGE_TYPE,
+                                     routing_key=ROUTING_KEY,
+                                     inactivity_timeout=INACTIVITY_TIMEOUT,
+                                     callback_with_delivery_info=True)
+    print(f"Concurrent consumers are done")
+
+    mrsal.close_connection()
+
+def consumer_callback_with_delivery_info(host_param: str, queue_param: str, method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str):
+    time.sleep(5)
+    return True
+```
+
 That simple! You have now setup a full advanced message queueing protocol that you can use to promote friendship or other necessary communication between your services.
 
 ###### Note! Please refer to the full guide on how to use customize Mrsal to meet specific needs. There are many parameters and settings that you can use to set up a more sophisticated communication protocol.
```

### Comparing `mrsal-0.3.0a0/mrsal/config/config.py` & `mrsal-0.4.0a0/mrsal/config/config.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.3.0a0/mrsal/config/logging.py` & `mrsal-0.4.0a0/mrsal/config/logging.py`

 * *Files identical despite different names*

### Comparing `mrsal-0.3.0a0/mrsal/mrsal.py` & `mrsal-0.4.0a0/mrsal/mrsal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import concurrent.futures
 import json
 import os
-import pika
 import ssl
 from dataclasses import dataclass
 from socket import gaierror
-from typing import Callable, Dict, NoReturn, Tuple, Any
+from typing import Any, Callable, Dict, NoReturn, Tuple
+
+import pika
 from pika import SSLOptions
 from retry import retry
 
 from mrsal.config.logging import get_logger
 
 
 @dataclass
@@ -68,15 +70,15 @@
                     port=self.port,
                     ssl_options=ssl_options,
                     virtual_host=self.virtual_host,
                     credentials=credentials,
                     heartbeat=self.heartbeat,
                     blocked_connection_timeout=self.blocked_connection_timeout
                 ))
-            self._channel = self._connection.channel()
+            self._channel: pika.adapters.blocking_connection.BlockingChannel = self._connection.channel()
             # Note: prefetch is set to 1 here as an example only.
             # In production you will want to test with different prefetch values
             # to find which one provides the best performance and usability for your solution
             self._channel.basic_qos(prefetch_count=self.prefetch_count)
             self.log.success(f'Connection established with RabbitMQ on {connection_info}')
             return self._connection
         except TypeError as err:
@@ -218,24 +220,24 @@
         )
         context.load_cert_chain(
             certfile=os.environ.get('RABBITMQ_CERT'),
             keyfile=os.environ.get('RABBITMQ_KEY')
         )
         return context
 
-    def __stop_consuming(self, consumer_tag: str) -> NoReturn:
+    def stop_consuming(self, consumer_tag: str) -> NoReturn:
         self._channel.stop_consuming(consumer_tag=consumer_tag)
-        self.log.info('Consumer is stopped, carry on')
+        self.log.info(f'Consumer is stopped, carry on. consumer_tag={consumer_tag}')
 
-    def __close_channel(self) -> NoReturn:
+    def close_channel(self) -> NoReturn:
         self._channel.close()
         self.log.info('Channel is closed, carry on')
 
-    def __close_connection(self) -> NoReturn:
-        self.__close_channel()
+    def close_connection(self) -> NoReturn:
+        self.close_channel()
         self._connection.close()
         self.log.info('Connection is closed, carry on')
 
     def queue_delete(self, queue: str):
         self._channel.queue_delete(queue=queue)
 
     def exchange_delete(self, exchange: str):
@@ -280,18 +282,18 @@
                         self._channel.basic_ack(delivery_tag)
                 self.log.info('----------------------------------------------------')
         except FileNotFoundError as e:
             self.log.error(f'Connection closed with error: {e}')
             self._channel.stop_consuming()
 
     def start_consumer(
-            self, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None, 
+            self, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None,
             exchange: str = None, exchange_type: str = None, routing_key: str = None,
             inactivity_timeout: int = None, requeue: bool = False, fast_setup: bool = False,
-            callback_with_delivery_info: bool = False
+            callback_with_delivery_info: bool = False, thread_num: int = None
     ):
         """
         Setup consumer:
             1- Consumer start consuming the messages from the queue.
             2- If `inactivity_timeout` is given (in seconds) the consumer will be canceled when the time of inactivity 
                 exceeds inactivity_timeout.
             3- Send the consumed message to callback method to be processed, and then the message can be either:
@@ -318,20 +320,21 @@
                 - spec.BasicProperties: Captures the client message sent to the server. E.g:(CONTENT_TYPE, DELIVERY_MODE, MESSAGE_ID, APP_ID). 
         """
         if fast_setup:
             # setting up the necessary connections
             self.setup_exchange(exchange=exchange, exchange_type=exchange_type)
             self.setup_queue(queue=queue)
             self.setup_queue_binding(exchange=exchange, queue=queue, routing_key=routing_key)
-
-        self.log.info(f'Consuming messages: queue= {queue}, requeue= {requeue}, inactivity_timeout= {inactivity_timeout}')
+        print_thread_index = f"thread={str(thread_num)} -> " if thread_num is not None else ""
+        self.log.info(f'{print_thread_index} Consuming messages queue= {queue}, requeue= {requeue}, inactivity_timeout= {inactivity_timeout}')
 
         try:
-            method_frame: spec.Basic.Deliver 
-            prop: spec.BasicProperties 
+            self.consumer_tag = None
+            method_frame: spec.Basic.Deliver
+            prop: spec.BasicProperties
             body: Any
             for method_frame, properties, body in \
                     self._channel.consume(queue=queue, inactivity_timeout=inactivity_timeout):
                 try:
                     if (method_frame, properties, body) != (None, None, None):
                         consumer_tags = self._channel.consumer_tags
                         self.consumer_tag = method_frame.consumer_tag
@@ -349,42 +352,91 @@
                                 delivery_tag= {method_frame.delivery_tag},
                                 properties= {properties},
                                 consumer_tags= {consumer_tags},
                                 consumer_tag= {self.consumer_tag}
                                 """)
                         if callback_with_delivery_info:
                             is_processed = callback(*callback_args, method_frame, properties, body) if callback_args else callback(method_frame, properties, body)
-                        else:    
+                        else:
                             is_processed = callback(*callback_args, body) if callback_args else callback(body)
                         if is_processed:
                             self._channel.basic_ack(delivery_tag=method_frame.delivery_tag)
-                            self.log.info(f'Message coming from the app={app_id} with messageId={msg_id} is acknowledged.')
+                            self.log.info(f'{print_thread_index} Message coming from the app={app_id} with messageId={msg_id} is acknowledged.')
                         else:
-                            self.log.warning(f'Could not process the message coming from the app={app_id} with messageId={msg_id}. This will be rejected and sent to dead-letters-exchange if it configured or deleted if not.')
+                            self.log.warning(
+                                f'{print_thread_index} Could not process the message coming from the app={app_id} with messageId={msg_id}. This will be rejected and sent to dead-letters-exchange if it configured or deleted if not.')
                             self._channel.basic_nack(delivery_tag=method_frame.delivery_tag, requeue=requeue)
-                            self.log.warning('Message rejected')
+                            self.log.warning(f'{print_thread_index} Message rejected')
                             pass
-                        self.log.info(f'[*] keep listening on {queue}.')
+                        self.log.info(f'[*] {print_thread_index} keep listening on {queue}...')
                     else:
-                        self.log.warning(f'Given period of inactivity {inactivity_timeout} is exceeded. Cancel consumer.')
+                        self.log.warning(f'{print_thread_index} Given period of inactivity {inactivity_timeout} is exceeded. Cancel consumer.')
+                        self.stop_consuming(self.consumer_tag)
                         self._channel.cancel()
                 except (pika.exceptions.StreamLostError, pika.exceptions.ConnectionClosedByBroker, ValueError, TypeError):
-                    self.log.error('I lost the connection with the Mrsal.', exc_info=True)
+                    self.log.error(f'{print_thread_index} I lost the connection with the Mrsal.', exc_info=True)
                     pass
                 except KeyboardInterrupt:
-                    self.log('Stopping Mrsal consumption.')
-                    self.__stop_consuming(self.consumer_tag)
-                    self.__close_connection()
+                    self.log(f'{print_thread_index} Stopping Mrsal consumption.')
+                    self.stop_consuming(self.consumer_tag)
+                    self.close_connection()
                     break
         except pika.exceptions.ChannelClosed as err2:
-            self.log.error(f'ChannelClosed is caught while consuming. Channel is closed by broker. Cancel consumer. {str(err2)}')
+            self.log.error(f'{print_thread_index} ChannelClosed is caught while consuming. Channel is closed by broker. Cancel consumer. {str(err2)}')
             self._channel.cancel()
 
     # --------------------------------------------------------------
     # --------------------------------------------------------------
+    def _spawn_mrsal_and_start_new_consumer(self, thread_num: int, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None,
+                                            exchange: str = None, exchange_type: str = None, routing_key: str = None,
+                                            inactivity_timeout: int = None, requeue: bool = False, fast_setup: bool = False,
+                                            callback_with_delivery_info: bool = False):
+        try:
+            self.log.info(f"thread_num={thread_num} -> Start consumer")
+            mrsal_obj = Mrsal(host=self.host,
+                              port=self.port,
+                              credentials=self.credentials,
+                              virtual_host=self.virtual_host,
+                              ssl=self.ssl,
+                              verbose=self.verbose,
+                              prefetch_count=self.prefetch_count,
+                              heartbeat=self.heartbeat,
+                              blocked_connection_timeout=self.blocked_connection_timeout)
+            mrsal_obj.connect_to_server()
+
+            mrsal_obj.start_consumer(
+                callback=callback,
+                callback_args=callback_args,
+                queue=queue,
+                requeue=requeue,
+                exchange=exchange,
+                exchange_type=exchange_type,
+                routing_key=routing_key,
+                fast_setup=fast_setup,
+                inactivity_timeout=inactivity_timeout,
+                callback_with_delivery_info=callback_with_delivery_info,
+                thread_num=thread_num
+            )
+
+            mrsal_obj.stop_consuming(mrsal_obj.consumer_tag)
+            mrsal_obj.close_connection()
+            self.log.info(f"thread_num={thread_num} -> End consumer")
+        except Exception as e:
+            self.log.error(f"thread_num={thread_num} -> Failed to consumer: {e}")
+
+    def start_concurrence_consumer(self, total_threads: int, queue: str, callback: Callable, callback_args: Tuple[str, Any] = None,
+                                   exchange: str = None, exchange_type: str = None, routing_key: str = None,
+                                   inactivity_timeout: int = None, requeue: bool = False, fast_setup: bool = False,
+                                   callback_with_delivery_info: bool = False):
+        with concurrent.futures.ThreadPoolExecutor(max_workers=total_threads) as executor:
+            executor.map(self._spawn_mrsal_and_start_new_consumer, range(total_threads), [queue]*total_threads, [callback]*total_threads, [callback_args]*total_threads,
+                         [exchange]*total_threads, [exchange_type]*total_threads, [routing_key]*total_threads,
+                         [inactivity_timeout]*total_threads, [requeue]*total_threads, [fast_setup]*total_threads,
+                         [callback_with_delivery_info]*total_threads)
+
     @retry((pika.exceptions.UnroutableError), tries=2, delay=5, jitter=(1, 3))
     def publish_message(
             self, exchange: str, routing_key: str, message: Any, exchange_type: str = None,
             queue: str = None, fast_setup: bool = False, prop: pika.BasicProperties = None
     ):
         """Publish message to the exchange specifying routing key and properties.
```

### Comparing `mrsal-0.3.0a0/pyproject.toml` & `mrsal-0.4.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mrsal"
-version = "0.3.0-alpha"
+version = "0.4.0-alpha"
 description = "Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika."
 authors = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
 maintainers = ["Raafat <rafatzahran90@gmail.com>", "Jon E Nesvold <jnesvold@pm.me>"]
 keywords = ["RabbitMQ", "Pika", "Mrsal"]
 readme = "README.md"
 license = ""
```

### Comparing `mrsal-0.3.0a0/setup.py` & `mrsal-0.4.0a0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,224 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mrsal
+Version: 0.4.0a0
+Summary: Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika.
+Keywords: RabbitMQ,Pika,Mrsal
+Author: Raafat
+Author-email: rafatzahran90@gmail.com
+Maintainer: Raafat
+Maintainer-email: rafatzahran90@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: pika (>=1.3.0,<2.0.0)
+Requires-Dist: retry (>=0.9.2,<0.10.0)
+Description-Content-Type: text/markdown
+
+# MRSAL  <img align="right" width="125" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/187228621-af1d695d-29a3-4940-9a8c-c19bcd6421a5.png">
+<img src="https://img.shields.io/badge/release-v0.1.0--alpha-blue" height="20" /> [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/) 
+
+## Intro
+Mrsal is a simple to use message broker abstraction on top of [RabbitMQ](https://www.rabbitmq.com/) and [Pika](https://pika.readthedocs.io/en/stable/index.html). The goal is to make Mrsal trivial to re-use in all services of a distributed system and to make the use of advanced message queing protocols easy and safe. No more big chunks of repetive code across your services or bespoke solutions to handle dead letters. 
+
+###### Mrsal is Arabic for a small arrow and is used to describe something that performs a task with lightness and speed. 
+
+## Quick Start guide
+
+### 0. Install
+
+First things first: 
+
+```bash
+pip install mrsal
+```
+
+We need to install RabbitMQ to use Mrsal. Head over to [install](https://www.rabbitmq.com/download.html) RabbitMQ. Make sure to stick to the configuration that you give the installation throughout this guide. You can also use the [Dockerfile](https://github.com/NeoMedSys/mrsal/blob/main/Dockerfile) and the [docker-compose](https://github.com/NeoMedSys/mrsal/blob/main/docker-compose.yml) that we are using in the full guide.
+
+Next set the default username, password and servername for your RabbitMQ setup. It's advisable to use a `.env` script or the rc file for persistence.
+
+```bash
+[RabbitEnvVars]
+RABBITMQ_DEFAULT_USER=******
+RABBITMQ_DEFAULT_PASS=******
+RABBITMQ_DEFAULT_VHOST=******
+RABBITMQ_DOMAIN=******
+RABBITMQ_DOMAIN_TLS=******
+
+RABBITMQ_GUI_PORT=******
+RABBITMQ_PORT=******
+RABBITMQ_PORT_TLS=******
+
+# FOR TLS
+RABBITMQ_CAFILE=/path/to/file
+RABBITMQ_CERT=/path/to/file
+RABBITMQ_KEY=/path/to/file
+```
+
+Please read the [full guide](https://github.com/NeoMedSys/mrsal/blob/main/FullGuide.md) to understand what Mrsal currently can and can't do.
+
+###### Mrsal was first developed by NeoMedSys and the research group [CRAI](https://crai.no/) at the univeristy hospital of Oslo.
+
+### 1. Setup and connect
+
+
+The first thing we need to do is to setup our rabbit server before we can subscribe and publish to it. Lets set up a server on our localhost with the port and credentials we used when spinning up the docker-compose
+
+```python
+import json
+import pika
+from mrsal.mrsal import Mrsal
+
+# If you want to use SSL for external listening then set it to True
+SSL = False
+
+# Note RabbitMQ container is listening on:
+# 1. When SSL is False the default port 5672 which is exposed to RABBITMQ_PORT in docker-compose
+# 2. When SSL is True the default port 5671 which is exposed to RABBITMQ_PORT_TLS in docker-compose
+port = RABBITMQ_PORT_TLS if SSL else RABBITMQ_PORT
+host = RABBITMQ_DOMAIN_TLS if SSL else RABBITMQ_DOMAIN
+
+# It should match with the env specifications (RABBITMQ_DEFAULT_USER, RABBITMQ_DEFAULT_PASS)
+credentials=(RABBITMQ_DEFAULT_USER, RABBITMQ_DEFAULT_PASS)
+
+# It should match with the env specifications (RABBITMQ_DEFAULT_VHOST)
+v_host = RABBITMQ_DEFAULT_VHOST
+
+mrsal = Mrsal(
+    host=host,
+    port=port,
+    credentials=credentials,
+    virtual_host=v_host,
+    ssl=SSL
+)
+
+mrsal.connect_to_server()
+```
+
+### 2 Publish
+Now lets publish our message of friendship on the friendship exchange.
+Note: When `fast_setup=True` that means Mrsal will create the specified `exchange` and `queue`, then bind them together using `routing_key`.
+
+```python
+# BasicProperties is used to set the message properties
+prop = pika.BasicProperties(
+        app_id='friendship_app',
+        message_id='friendship_msg',
+        content_type='text/plain',
+        content_encoding='utf-8',
+        delivery_mode=pika.DeliveryMode.Persistent,
+        headers=None)
+
+message_body = 'Hello'
+
+# Publish the message to the exchange to be routed to queue
+mrsal.publish_message(exchange='friendship',
+                        exchange_type='direct',
+                        queue='friendship_queue',
+                        routing_key='friendship_key',
+                        message=json.dumps(message_body), 
+                        prop=prop,
+                        fast_setup=True)
+```
+
+### 3 Consume
+
+Now lets setup a consumer that will listen to our very important messages. If you are using scripts rather than notebooks then it's advisable to run consume and publish separately. We are going to need a callback function which is triggered upon receiving the message from the queue we subscribe to. You can use the callback function to activate something in your system.
+
+Note: 
+- If you start a consumer with `callback_with_delivery_info=True` then your callback function should have at least these params `(method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str)`. 
+- If not, then it should have at least `(message_param: str)`
+
+```python
+import json
+
+def consumer_callback_with_delivery_info(host_param: str, queue_param: str, method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str):
+    str_message = json.loads(message_param).replace('"', '')
+    if 'Hello' in str_message:
+        app_id = properties.app_id
+        msg_id = properties.message_id
+        print(f'app_id={app_id}, msg_id={msg_id}')
+        print('Salaam habibi')
+        return True  # Consumed message processed correctly
+    return False
+
+def consumer_callback(host_param: str, queue_param: str, message_param: str):
+    str_message = json.loads(message_param).replace('"', '')
+    if 'Hello' in str_message:
+        print('Salaam habibi')
+        return True  # Consumed message processed correctly
+    return False
+
+mrsal.start_consumer(
+        queue='friendship_queue',
+        callback=consumer_callback_with_delivery_info,
+        callback_args=(test_config.HOST, 'friendship_queue'),
+        inactivity_timeout=1,
+        requeue=False,
+        callback_with_delivery_info=True
+    )
+```
+
+Done! Your first message of friendship has been sent to the friendship queue on the exchange of friendship.
+
+
+### 3 Concurrent Consumers
+
+Sometimes we need to start multiple consumers to listen to the **same** **queue** and process received messages **concurrently**. 
+You can do that by calling `start_concurrence_consumer` which takes `total_threads` param in addition to the same parameters used in `start_consumer`.
+This method will create a **thread pool** and _spawn new_ `Mrsal` object and start **new consumer** for every thread. 
+
+```python
+import json
+import time
+
+import pika
+from pika.exchange_type import ExchangeType
+
+import mrsal.config.config as config
+import tests.config as test_config
+from mrsal.mrsal import Mrsal
+
+
+mrsal = Mrsal(host=test_config.HOST,
+              port=config.RABBITMQ_PORT,
+              credentials=config.RABBITMQ_CREDENTIALS,
+              virtual_host=config.V_HOST)
+mrsal.connect_to_server()
+
+APP_ID = "TEST_CONCURRENT_CONSUMERS"
+EXCHANGE = "BOOKS"
+EXCHANGE_TYPE = ExchangeType.direct
+QUEUE_EMERGENCY = "SORT_BOOKS"
+NUM_THREADS = 3
+NUM_MESSAGES = 3
+INACTIVITY_TIMEOUT = 3
+ROUTING_KEY = "PROCESS BOOK"
+MESSAGE_ID = "LIBRARY"
+
+def test_concurrent_consumer():
+    # Start concurrent consumers
+    mrsal.start_concurrence_consumer(total_threads=NUM_THREADS, queue=QUEUE_EMERGENCY,
+                                     callback=consumer_callback_with_delivery_info,
+                                     callback_args=(test_config.HOST, QUEUE_EMERGENCY),
+                                     exchange=EXCHANGE, exchange_type=EXCHANGE_TYPE,
+                                     routing_key=ROUTING_KEY,
+                                     inactivity_timeout=INACTIVITY_TIMEOUT,
+                                     callback_with_delivery_info=True)
+    print(f"Concurrent consumers are done")
+
+    mrsal.close_connection()
+
+def consumer_callback_with_delivery_info(host_param: str, queue_param: str, method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str):
+    time.sleep(5)
+    return True
+```
 
-packages = \
-['mrsal', 'mrsal.config']
+That simple! You have now setup a full advanced message queueing protocol that you can use to promote friendship or other necessary communication between your services.
 
-package_data = \
-{'': ['*']}
+###### Note! Please refer to the full guide on how to use customize Mrsal to meet specific needs. There are many parameters and settings that you can use to set up a more sophisticated communication protocol.
 
-install_requires = \
-['colorlog>=6.7.0,<7.0.0', 'pika>=1.3.0,<2.0.0', 'retry>=0.9.2,<0.10.0']
-
-setup_kwargs = {
-    'name': 'mrsal',
-    'version': '0.3.0a0',
-    'description': 'Mrsal is a simple to use message broker abstraction on top of RabbitMQ and Pika.',
-    'long_description': '# MRSAL  <img align="right" width="125" alt="20200907_104224" src="https://user-images.githubusercontent.com/29639563/187228621-af1d695d-29a3-4940-9a8c-c19bcd6421a5.png">\n<img src="https://img.shields.io/badge/release-v0.1.0--alpha-blue" height="20" /> [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)\n[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/) \n\n## Intro\nMrsal is a simple to use message broker abstraction on top of [RabbitMQ](https://www.rabbitmq.com/) and [Pika](https://pika.readthedocs.io/en/stable/index.html). The goal is to make Mrsal trivial to re-use in all services of a distributed system and to make the use of advanced message queing protocols easy and safe. No more big chunks of repetive code across your services or bespoke solutions to handle dead letters. \n\n###### Mrsal is Arabic for a small arrow and is used to describe something that performs a task with lightness and speed. \n\n## Quick Start guide\n\n### 0. Install\n\nFirst things first: \n\n```bash\npip install mrsal\n```\n\nWe need to install RabbitMQ to use Mrsal. Head over to [install](https://www.rabbitmq.com/download.html) RabbitMQ. Make sure to stick to the configuration that you give the installation throughout this guide. You can also use the [Dockerfile](https://github.com/NeoMedSys/mrsal/blob/main/Dockerfile) and the [docker-compose](https://github.com/NeoMedSys/mrsal/blob/main/docker-compose.yml) that we are using in the full guide.\n\nNext set the default username, password and servername for your RabbitMQ setup. It\'s advisable to use a `.env` script or the rc file for persistence.\n\n```bash\n[RabbitEnvVars]\nRABBITMQ_DEFAULT_USER=******\nRABBITMQ_DEFAULT_PASS=******\nRABBITMQ_DEFAULT_VHOST=******\nRABBITMQ_DOMAIN=******\nRABBITMQ_DOMAIN_TLS=******\n\nRABBITMQ_GUI_PORT=******\nRABBITMQ_PORT=******\nRABBITMQ_PORT_TLS=******\n\n# FOR TLS\nRABBITMQ_CAFILE=/path/to/file\nRABBITMQ_CERT=/path/to/file\nRABBITMQ_KEY=/path/to/file\n```\n\nPlease read the [full guide](https://github.com/NeoMedSys/mrsal/blob/main/FullGuide.md) to understand what Mrsal currently can and can\'t do.\n\n###### Mrsal was first developed by NeoMedSys and the research group [CRAI](https://crai.no/) at the univeristy hospital of Oslo.\n\n### 1. Setup and connect\n\n\nThe first thing we need to do is to setup our rabbit server before we can subscribe and publish to it. Lets set up a server on our localhost with the port and credentials we used when spinning up the docker-compose\n\n```python\nimport json\nimport pika\nfrom mrsal.mrsal import Mrsal\n\n# If you want to use SSL for external listening then set it to True\nSSL = False\n\n# Note RabbitMQ container is listening on:\n# 1. When SSL is False the default port 5672 which is exposed to RABBITMQ_PORT in docker-compose\n# 2. When SSL is True the default port 5671 which is exposed to RABBITMQ_PORT_TLS in docker-compose\nport = RABBITMQ_PORT_TLS if SSL else RABBITMQ_PORT\nhost = RABBITMQ_DOMAIN_TLS if SSL else RABBITMQ_DOMAIN\n\n# It should match with the env specifications (RABBITMQ_DEFAULT_USER, RABBITMQ_DEFAULT_PASS)\ncredentials=(RABBITMQ_DEFAULT_USER, RABBITMQ_DEFAULT_PASS)\n\n# It should match with the env specifications (RABBITMQ_DEFAULT_VHOST)\nv_host = RABBITMQ_DEFAULT_VHOST\n\nmrsal = Mrsal(\n    host=host,\n    port=port,\n    credentials=credentials,\n    virtual_host=v_host,\n    ssl=SSL\n)\n\nmrsal.connect_to_server()\n```\n\n### 2 Publish\nNow lets publish our message of friendship on the friendship exchange.\nNote: When `fast_setup=True` that means Mrsal will create the specified `exchange` and `queue`, then bind them together using `routing_key`.\n\n```python\n# BasicProperties is used to set the message properties\nprop = pika.BasicProperties(\n        app_id=\'friendship_app\',\n        message_id=\'friendship_msg\',\n        content_type=\'text/plain\',\n        content_encoding=\'utf-8\',\n        delivery_mode=pika.DeliveryMode.Persistent,\n        headers=None)\n\nmessage_body = \'Hello\'\n\n# Publish the message to the exchange to be routed to queue\nmrsal.publish_message(exchange=\'friendship\',\n                        exchange_type=\'direct\',\n                        queue=\'friendship_queue\',\n                        routing_key=\'friendship_key\',\n                        message=json.dumps(message_body), \n                        prop=prop,\n                        fast_setup=True)\n```\n\n### 3 Consume\n\nNow lets setup a consumer that will listen to our very important messages. If you are using scripts rather than notebooks then it\'s advisable to run consume and publish separately. We are going to need a callback function which is triggered upon receiving the message from the queue we subscribe to. You can use the callback function to activate something in your system.\n\nNote: \n- If you start a consumer with `callback_with_delivery_info=True` then your callback function should have at least these params `(method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str)`. \n- If not, then it should have at least `(message_param: str)`\n\n```python\nimport json\n\ndef consumer_callback_with_delivery_info(host_param: str, queue_param: str, method_frame: pika.spec.Basic.Deliver, properties: pika.spec.BasicProperties, message_param: str):\n    str_message = json.loads(message_param).replace(\'"\', \'\')\n    if \'Hello\' in str_message:\n        app_id = properties.app_id\n        msg_id = properties.message_id\n        print(f\'app_id={app_id}, msg_id={msg_id}\')\n        print(\'Salaam habibi\')\n        return True  # Consumed message processed correctly\n    return False\n\ndef consumer_callback(host_param: str, queue_param: str, message_param: str):\n    str_message = json.loads(message_param).replace(\'"\', \'\')\n    if \'Hello\' in str_message:\n        print(\'Salaam habibi\')\n        return True  # Consumed message processed correctly\n    return False\n\nmrsal.start_consumer(\n        queue=\'friendship_queue\',\n        callback=consumer_callback_with_delivery_info,\n        callback_args=(test_config.HOST, \'friendship_queue\'),\n        inactivity_timeout=1,\n        requeue=False,\n        callback_with_delivery_info=True\n    )\n```\n\nDone! Your first message of friendship has been sent to the friendship queue on the exchange of friendship.\n\nThat simple! You have now setup a full advanced message queueing protocol that you can use to promote friendship or other necessary communication between your services.\n\n###### Note! Please refer to the full guide on how to use customize Mrsal to meet specific needs. There are many parameters and settings that you can use to set up a more sophisticated communication protocol.\n',
-    'author': 'Raafat',
-    'author_email': 'rafatzahran90@gmail.com',
-    'maintainer': 'Raafat',
-    'maintainer_email': 'rafatzahran90@gmail.com',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

