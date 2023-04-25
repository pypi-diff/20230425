# Comparing `tmp/oxalis-0.5.3.tar.gz` & `tmp/oxalis-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.5.3.tar", max compression
+gzip compressed data, was "oxalis-0.5.4.tar", max compression
```

## Comparing `oxalis-0.5.3.tar` & `oxalis-0.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.3/LICENSE
--rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.5.3/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.3/oxalis/__init__.py
--rw-r--r--   0        0        0    10949 2023-04-20 05:15:02.504528 oxalis-0.5.3/oxalis/amqp.py
--rw-r--r--   0        0        0     6836 2023-04-20 05:15:02.504528 oxalis-0.5.3/oxalis/base.py
--rw-r--r--   0        0        0     1654 2022-07-12 02:08:37.164774 oxalis-0.5.3/oxalis/beater.py
--rw-r--r--   0        0        0     3621 2023-04-20 05:26:02.224743 oxalis-0.5.3/oxalis/kafka.py
--rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.5.3/oxalis/pool.py
--rw-r--r--   0        0        0     6575 2023-04-20 05:15:02.508527 oxalis-0.5.3/oxalis/redis.py
--rw-r--r--   0        0        0      972 2023-04-20 05:26:14.840442 oxalis-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     7859 1970-01-01 00:00:00.000000 oxalis-0.5.3/setup.py
--rw-r--r--   0        0        0     8003 1970-01-01 00:00:00.000000 oxalis-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.4/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.5.4/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.4/oxalis/__init__.py
+-rw-r--r--   0        0        0    10989 2023-04-24 10:09:33.396921 oxalis-0.5.4/oxalis/amqp.py
+-rw-r--r--   0        0        0     6939 2023-04-24 10:09:33.396921 oxalis-0.5.4/oxalis/base.py
+-rw-r--r--   0        0        0     1654 2022-07-12 02:08:37.164774 oxalis-0.5.4/oxalis/beater.py
+-rw-r--r--   0        0        0     3833 2023-04-24 10:09:33.396921 oxalis-0.5.4/oxalis/kafka.py
+-rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.5.4/oxalis/pool.py
+-rw-r--r--   0        0        0     6536 2023-04-24 10:09:33.396921 oxalis-0.5.4/oxalis/redis.py
+-rw-r--r--   0        0        0      972 2023-04-24 10:10:11.068009 oxalis-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7859 1970-01-01 00:00:00.000000 oxalis-0.5.4/setup.py
+-rw-r--r--   0        0        0     8003 1970-01-01 00:00:00.000000 oxalis-0.5.4/PKG-INFO
```

### Comparing `oxalis-0.5.3/LICENSE` & `oxalis-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.3/README.md` & `oxalis-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.3/oxalis/amqp.py` & `oxalis-0.5.4/oxalis/amqp.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,14 @@
             task_cls=task_cls,
             task_codec=task_codec,
             pool=pool,
             timeout=timeout,
             worker_num=worker_num,
             test=test,
         )
-        self.tasks: tp.Dict[str, Task] = {}  # type: ignore
         self.connection = connection
         self.default_exchange = default_exchange
         self.default_queue = default_queue
         if default_routing_key:
             self.default_exchange.default_routing_key = default_routing_key
         self.queues: tp.List[Queue] = [self.default_queue]
         self.exchanges: tp.List[Exchange] = [self.default_exchange]
@@ -161,22 +160,30 @@
         await self.declare(self.exchanges)
         for q, e, k in self.bindings:
             await self.bind(q, e, k)
 
     async def wait_close(self):
         for tag, queue in self.consumer_tags.items():
             await queue.cancel(tag, timeout=self.timeout)
-        await asyncio.sleep(self.timeout)  # waiting for reject message
+        await super().wait_close()
 
     async def disconnect(self):
         for channel in self.channels:
             await channel.close()
         await self.connection.close()
 
-    async def send_task(self, task: Task, *task_args, _delay: float = 0, _priority: int = 0, _headers: tp.Optional[tp.Dict] = None, **task_kwargs):  # type: ignore[override]
+    async def send_task(
+        self,
+        task: Task,
+        *task_args,
+        _delay: float = 0,
+        _priority: int = 0,
+        _headers: tp.Optional[tp.Dict] = None,
+        **task_kwargs,
+    ):
         if task.name not in self.tasks:
             raise ValueError(f"Task {task} not register")
         headers = _headers if _headers else {}
         if _delay:
             if task.exchange.type != ExchangeType.X_DELAYED_MESSAGE:
                 raise ValueError(
                     f"Task {task} with delay must go with 'x-delayed-message' exchange"
@@ -258,15 +265,15 @@
             _names.add(eq.name)
 
     async def bind(self, queue: Queue, exchange: Exchange, routing_key: str = ""):
         queue.set_channel(self.channel)
         exchange.set_channel(self.channel)
         await queue.bind(exchange, routing_key, timeout=self.timeout)
 
-    async def exec_task(self, task: Task, *args, **task_kwargs):  # type: ignore[override]
+    async def exec_task(self, task: Task, *args, **task_kwargs):
         message: aio_pika.IncomingMessage = args[0]
         task_args = args[1:]
         if not task.ack_later:
             await message.ack()
         try:
             await super().exec_task(task, *task_args, **task_kwargs)
         except Exception as e:
@@ -275,20 +282,24 @@
             elif task.ack_always and task.ack_later:
                 await message.ack()
             raise e from None
         if task.ack_later:
             await message.ack()
 
     async def _on_message_receive(self, message: aio_pika.abc.AbstractIncomingMessage):
-        task, spawned = await self.on_message_receive(message.body, message)
-        # reject after close
-        if not task:
-            await message.reject()
-        elif task and not spawned:
-            await message.reject(requeue=True)
+        self.consuming_count += 1
+        try:
+            task, spawned = await self.on_message_receive(message.body, message)
+            # reject after close
+            if not task:
+                await message.reject()
+            elif task and not spawned:
+                await message.reject(requeue=True)
+        finally:
+            self.consuming_count -= 1
 
     async def _receive_message(self, queue: Queue):
         channel = self.connection.channel()
         self.channels.append(channel)
         await channel.initialize()
         await channel.set_qos(
             prefetch_count=queue.consumer_prefetch_count,
```

### Comparing `oxalis-0.5.3/oxalis/base.py` & `oxalis-0.5.4/oxalis/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,59 +67,61 @@
         return json.dumps([task.name, list(task_args), task_kwargs]).encode()
 
     @classmethod
     def decode(cls, content: bytes) -> MESSAGE_TYPE:
         return json.loads(content)
 
 
-class Oxalis(abc.ABC):
+class Oxalis(abc.ABC, tp.Generic[TASK_TV]):
     def __init__(
         self,
-        task_cls: tp.Type[Task] = Task,
+        task_cls: tp.Type[TASK_TV],
         task_codec: TaskCodec = TaskCodec(),
         pool: Pool = Pool(),
         timeout: float = 5.0,
         worker_num: int = 0,
         test: bool = False,
     ) -> None:
         self.task_cls = task_cls
-        self.tasks: tp.Dict[str, Task] = {}
+        self.tasks: tp.Dict[str, TASK_TV] = {}
         self.task_codec = task_codec
         self.pools: tp.List[Pool] = [pool]
         self.running = False
         self.timeout = timeout
         self.test = test
         self._on_close_signal_count = 0
         self.worker_num = worker_num or os.cpu_count()
         self.is_worker = False
         self.pool_wait_spawn = True
+        self.consuming_count = 0
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(pid-{os.getpid()})>"
 
     async def connect(self):
         pass
 
     async def wait_close(self):
-        pass
+        while self.consuming_count:
+            await asyncio.sleep(self.timeout)
 
     async def disconnect(self):
         pass
 
     @abc.abstractmethod
     async def send_task(
         self,
-        task: Task,
+        task: TASK_TV,
         *task_args,
         _delay: float = 0,
         **task_kwargs,
     ):
         pass
 
-    async def exec_task(self, task: Task, *task_args, **task_kwargs):
+    async def exec_task(self, task: TASK_TV, *task_args, **task_kwargs):
         logger.debug(f"Worker {self} execute task {task}...")
         await task(*task_args, **task_kwargs)
 
     def run_worker_master(self):
         for task in self.tasks.values():
             logger.info(f"Registered Task: {task}")
 
@@ -149,50 +151,49 @@
     async def work(self):
         while self.running:
             await asyncio.sleep(self.timeout)
 
         await self.wait_close()
         await asyncio.wait(
             [asyncio.get_event_loop().create_task(p.wait_close()) for p in self.pools],
-            timeout=self.timeout,
         )
         await self.disconnect()
 
     def close_worker(self, force: bool = False):
         logger.info(f"Close worker{'(force)' if force else ''}: {self}...")
         self.running = False
         if force:
             logger.warning(f"Force close: {self}, may lose some message!")
             for p in self.pools:
                 p.force_close()
             sys.exit()
 
-    def register_task(self, task: Task):
+    def register_task(self, task: TASK_TV):
         if task.name in self.tasks:
             raise ValueError("double task, check task name")
         self.tasks[task.name] = task
 
     def register(
         self,
         *,
         task_name: str = "",
         timeout: float = -1,
         pool: tp.Optional[Pool] = None,
         **_,
-    ) -> tp.Callable[[tp.Callable], Task]:
+    ) -> tp.Callable[[tp.Callable], TASK_TV]:
         def wrapped(func):
             task = self.task_cls(self, func, name=task_name, timeout=timeout, pool=pool)
             self.register_task(task)
             return task
 
         return wrapped
 
     async def on_message_receive(
         self, content: bytes, *args
-    ) -> tp.Tuple[tp.Optional[Task], bool]:
+    ) -> tp.Tuple[tp.Optional[TASK_TV], bool]:
         try:
             task_name, task_args, task_kwargs = self.task_codec.decode(content)
         except Exception as e:
             logger.exception(e)
             return None, False
 
         if task_name not in self.tasks:
```

### Comparing `oxalis-0.5.3/oxalis/beater.py` & `oxalis-0.5.4/oxalis/beater.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.3/oxalis/kafka.py` & `oxalis-0.5.4/oxalis/kafka.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
+import typing
 import typing as tp
+from collections import defaultdict
 
 import aiokafka
 
 from .base import Oxalis as _Oxalis
 from .base import Task as _Task
 from .base import TaskCodec, logger
 from .pool import Pool
@@ -37,46 +39,41 @@
         worker_num: int = 0,
         test: bool = False,
         group="default_group",
         default_topic="default_topic",
         topics: tp.Sequence[str] = tuple(),
     ) -> None:
         super().__init__(
-            task_cls=task_cls,
+            task_cls,
             task_codec=task_codec,
             pool=pool,
             timeout=timeout,
             worker_num=worker_num,
             test=test,
         )
         self.pool_wait_spawn = True
         self.consuming = True
-        self.tasks: tp.Dict[str, Task] = {}  # type: ignore
         self.kafka_url = kafka_url
         self.default_topic = default_topic
         self.group = group
         self.topics = set(topics)
         self.topics.add(self.default_topic)
         self.producer: aiokafka.AIOKafkaConsumer
 
     async def connect(self):
         self.producer = aiokafka.AIOKafkaProducer(
             bootstrap_servers=self.kafka_url,
             request_timeout_ms=int(self.timeout * 1000),
         )
         await self.producer.start()
 
-    async def wait_close(self):
-        while self.consuming:
-            await asyncio.sleep(self.timeout)
-
     async def disconnect(self):
         await self.producer.stop()
 
-    async def send_task(self, task: Task, *task_args, _delay=0, **task_kwargs):  # type: ignore[override]
+    async def send_task(self, task: Task, *task_args, _delay=0, **task_kwargs):
         if task.name not in self.tasks:
             raise ValueError(f"Task {task} not register")
         logger.debug(f"Send task {task} to worker...")
         await self.producer.send_and_wait(
             task.topic, self.task_codec.encode(task, task_args, task_kwargs)
         )
 
@@ -98,26 +95,35 @@
             )
             self.register_task(task)
             self.topics.add(topic)
             return task
 
         return wrapped
 
-    async def _start_consumer(self):
-        self.consuming = True
+    async def _start_consumer(self, topics: typing.List[str]):
+        self.consuming_count += 1
         try:
             consumer = aiokafka.AIOKafkaConsumer(
-                *self.topics, bootstrap_servers=self.kafka_url, group_id=self.group
+                *topics,
+                bootstrap_servers=self.kafka_url,
+                group_id=self.group,
+                enable_auto_commit=False,
             )
             await consumer.start()
             while self.running:
                 with contextlib.suppress(asyncio.TimeoutError):
                     msg = await asyncio.wait_for(
                         consumer.getone(), timeout=self.timeout
                     )
-                    await self.on_message_receive(msg.value)
+                    _, spowned = await self.on_message_receive(msg.value)
+                    if spowned:
+                        await consumer.commit()
             await consumer.stop()
         finally:
-            self.consuming = False
+            self.consuming_count -= 1
 
     def _run_worker(self):
-        asyncio.ensure_future(self._start_consumer())
+        topics = defaultdict(list)
+        for task in self.tasks.values():
+            topics[id(task.pool)].append(task.topic)
+        for ts in topics.values():
+            asyncio.ensure_future(self._start_consumer(ts))
```

### Comparing `oxalis-0.5.3/oxalis/pool.py` & `oxalis-0.5.4/oxalis/pool.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.3/oxalis/redis.py` & `oxalis-0.5.4/oxalis/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,21 +68,20 @@
 
     async def connect(self):
         await self.client.initialize()
 
     async def wait_close(self):
         while self.pubsub.connection is not None:
             await asyncio.sleep(self.timeout)
-        while self._receiving:
-            await asyncio.sleep(self.timeout)
+        await super().wait_close()
 
     async def disconnect(self):
         await self.client.close()
 
-    async def send_task(self, task: Task, *task_args, _delay: float = 0, **task_kwargs):  # type: ignore[override]
+    async def send_task(self, task: Task, *task_args, _delay: float = 0, **task_kwargs):
         if task.name not in self.tasks:
             raise ValueError(f"Task {task} not register")
         content = self.task_codec.encode(task, task_args, task_kwargs)
         if _delay:
             logger.debug(f"Send task {task} to worker with {_delay}s delay...")
             await self.client.zadd(
                 self.delay_queue.name,
@@ -139,50 +138,52 @@
                     try:
                         content = content[16:]
                         task_name, _, _ = self.task_codec.decode(content)
                         if task_name not in self.tasks:
                             logger.warning(f"Received task {task_name} not found")
                         else:
                             task = self.tasks[task_name]
-                            if isinstance(task.queue, PubsubQueue):  # type: ignore
-                                await self.client.publish(task.queue.name, content)  # type: ignore
+                            if isinstance(task.queue, PubsubQueue):
+                                await self.client.publish(task.queue.name, content)
                             else:
-                                await self.client.rpush(task.queue.name, content)  # type: ignore
+                                await self.client.rpush(task.queue.name, content)
                     except Exception as e:
                         logger.exception(e)
             if count < fetch_count:
                 await asyncio.sleep(time_offset)
 
     async def _receive_message(self, queue_names: tp.Set[str]):
-        self._receiving = True
+        self.consuming_count += 1
         try:
             while self.running:
                 content = await self.client.blpop(
                     list(queue_names), timeout=self.timeout
                 )
                 if not content:
                     continue
                 else:
                     await self.on_message_receive(content[1])
         finally:
-            self._receiving = False
+            self.consuming_count -= 1
 
     async def _receive_pubsub_message(self, queue_names: tp.Set[str]):
+        self.consuming_count += 1
         try:
             while self.running:
                 if not self.pubsub.subscribed:
                     await self.pubsub.subscribe(*queue_names)
                 content = await self.pubsub.get_message(
                     ignore_subscribe_messages=True, timeout=self.timeout
                 )
                 if not content:
                     continue
                 else:
                     await self.on_message_receive(content["data"])
         finally:
+            self.consuming_count -= 1
             await self.pubsub.close()
 
     def _run_worker(self):
         """
         Limit queue consume concurrency by pool
         """
         queue_names = defaultdict(set)
```

### Comparing `oxalis-0.5.3/pyproject.toml` & `oxalis-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.5.3"
+version = "0.5.4"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.7",
```

### Comparing `oxalis-0.5.3/setup.py` & `oxalis-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aio-pika>=8.0.3', 'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1']
 
 setup_kwargs = {
     'name': 'oxalis',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'Distributed async task/job queue',
     'long_description': '<p>\n<a href="https://pypi.org/project/oxalis/">\n    <img src="https://badge.fury.io/py/oxalis.svg" alt="Package version">\n</a>\n</p>\n\n# Oxalis  \n\nDistributed async task/job queue, like Celery for `asyncio` world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ) support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis backend\n\nDefine task:\n```python\nfrom redis.asyncio.client import Redis\nfrom oxalis.redis import Oxalis\n\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")))\n\n@oxalis.register()\nasync def hello_task():\n    print("Hello oxalis")\n```\n\nRun worker(consumer):\n```python\noxalis.run_worker_master()\n```\n\n```shell\npython ex.py\nINFO:oxalis:Registered Task: <Task(hello_task)>\nINFO:oxalis:Run worker: <Oxalis(pid-101547)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101548)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101549)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101550)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101551)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101552)>...\nINFO:oxalis:Run worker: <Oxalis(pid-101554)>...\n```\n\nRun client(producer):\n```python\nimport asyncio\n\nasyncio.get_event_loop().run_until_complete(oxalis.connect())\nfor i in range(10):\n    asyncio.get_event_loop().run_until_complete(hello_task.delay())\n    asyncio.get_event_loop().run_until_complete(hello_task.delay(_delay=1))  # delay execution after 1s\n```\n\nRun cron beater:\n```python\nfrom oxalis.beater import Beater\n\nbeater = Beater(oxalis)\n\nbeater.register("*/1 * * * *", hello_task)\nbeater.run()\n```\n```shell\npython exb.py \nINFO:oxalis:Beat task: <Task(hello_task)> at <*/1 * * * *> ...\n```\n\n## TaskCodec\n\nThe `TaskCodec` will encode/decode task args, default codec will use `json`\n\nCustom task codec:\n```python\nfrom oxalis.base import TaskCodec\n\nclass MyTaskCodec(TaskCodec):\n    @classmethod\n    def encode(\n        cls,\n        task: Task,\n        task_args: tp.Sequence[tp.Any],\n        task_kwargs: tp.Dict[str, tp.Any],\n    ) -> bytes:\n        ...\n\n    @classmethod\n    def decode(cls, content: bytes) -> TaskCodec.MESSAGE_TYPE:\n        ...\n\n\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")), task_codec=MyTaskCodec())\n...\n```\n\n\n## Task pool\n\nOxalis use one coroutine pool with concurrency limit and timeout limit to run all task\n\nCustom pool:\n\n```python\nfrom redis.asyncio.client import Redis\nfrom oxalis.redis import Oxalis\nfrom oxalis.pool import Pool\n\noxalis = Oxalis(Redis(host=os.getenv("REDIS_HOST", "redis")), pool=Pool(concurrency=10, timeout=60))\n```\n\n* For Redis task, the `queue` will be blocked util `pool` is not fully loaded\n* For AMQP task, oxalis use AMQP\'s QOS to limit worker concurrency(`pool`\'s concurrency will be -1 which means the pool\'s concurrency will not be limited)\n* `asyncio.TimeoutError` will be raised if one task is timeout\n* Every worker process has owned limited pool\n\n\nSpecified one task timeout limit:\n```python\n@oxalis.register(queue=custom_queue, timeout=10)\ndef custom_task():\n    print("Hello oxalis")\n```\n\n## Custom hook\n\nOxalis defined some hook API for inherited subclass:\n```python\nclass MyOxalis(Oxalis):\n    def on_worker_init():\n        # will be called before worker started\n        pass\n\n    def on_worker_close():\n        # will be called after worker started\n        pass\n```\n\nSome API can be rewritten or inherited for custom usage, eg:\n```python\nimport sentry_sdk\n\nclass MyOxalis(Oxalis):\n    async def exec_task(self, task: Task, *task_args, **task_kwargs):\n        """\n        capture exception to sentry\n        """\n        try:\n            await super().exec_task(task, *task_args, **task_kwargs)\n        except Exception as e:\n            sentry_sdk.capture_exception(e)\n```\n\n\n## Redis Backend Detail\n\nOxalis use redis\'s `list` and `pubsub` structure as a message queue\n\n### Queue\n\nCustom queue:\n```python\nfrom oxalis.redis import Queue, PubsubQueue\n\ncustom_queue = Queue("custom")\nbus_queue = PubsubQueue("bus")\n```\n\nRegister task:\n```python\n@oxalis.register(queue=custom_queue)\ndef custom_task():\n    print("Hello oxalis")\n\n@oxalis.register(queue=bus_queue)\ndef bus_task():\n    print("Hello oxalis")\n```\n\n* For task producer, the task will send to specified queue when call `task.delay()`\n* For task consumer, oxalis will listen those queues and receive task from them\n\n### Concurrency limit\n\nOxalis using coroutine pool\'s concurrency limit way, we can set different concurrency limit with specified pool for one task:\n\n```python\n@oxalis.register(pool=Pool(concurrency=1))\ndef custom_task():\n    print("Hello oxalis")\n```\n\n### Delayed task\n\nSupport by redis [zset](https://redis.com/ebook/part-2-core-concepts/chapter-6-application-components-in-redis/6-4-task-queues/6-4-2-delayed-tasks/)\n\n##  AMQP Backend Detail\n\n\n### Custom Queue and Exchange\n\nOxalis using AMQP\'s way to define Exchange, Queue and their bindings\n\n```python\nimport asyncio\nimport logging\nimport time\n\nfrom aio_pika import RobustConnection\nfrom oxalis.amqp import Exchange, ExchangeType, Oxalis, Pool, Queue\n\ne = Exchange("test")\nq = Queue("test", durable=False)\ne2 = Exchange("testfanout", type=ExchangeType.FANOUT)\nq2 = Queue("testfanout", durable=False)\n\n\noxalis = Oxalis(RobustConnection("amqp://root:letmein@rabbitmq:5672/"))\noxalis.register_binding(q, e, "test")\noxalis.register_binding(q2, e2, "")\noxalis.register_queues([q, q2])\n\n\n@oxalis.register(exchange=e, routing_key="test")\nasync def task1():\n    await asyncio.sleep(1)\n    print("hello oxalis")\n\n\n@oxalis.register(exchange=e2)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n\n```\n\n* For producer, task `oxalis.register`  defined one task message will send to which exchange(by routing key)\n* For consumer, `register_queues` defined which queues oxalis will listened\n* Task routing defined by bindings\n\n### Concurrency limit\n\nOxalis use AMQP\'s QOS to limit worker concurrency(Task\'s `ack_later` should be true), so coroutine pool\'s concurrency should not be limited.\n\nCustom queue QOS:\n```python\noxalis = Oxalis(RobustConnection("amqp://root:letmein@rabbitmq:5672/"), default_queue=Queue("custom",consumer_prefetch_count=10))\n...\nfanout_queue = Queue("testfanout", durable=False, consumer_prefetch_count=3)\noxalis.register_queues([fanout_queue])\n...\n```\n\n### Custom task behavior\n\nDefine task how to perform `ack` and `reject` \n\n```python\n# always ack even task failed(raise exception)\n@oxalis.register(ack_always=True, reject=False)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n\n#  reject with requeue when task failed\n@oxalis.register(reject_requeue=True)\nasync def task2():\n    await asyncio.sleep(10)\n    print("hello oxalis")\n```\n\n### Delayed task\n\nSupport by RabbitMq\'s [plugin](https://blog.rabbitmq.com/posts/2015/04/scheduling-messages-with-rabbitmq)\n',
     'author': 'strongbugman',
     'author_email': 'strongbugman@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['oxalis']
 package_data = \ {'': ['*']} install_requires = \ ['aio-pika>=8.0.3',
 'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1'] setup_kwargs = { 'name':
-'oxalis', 'version': '0.5.3', 'description': 'Distributed async task/job
+'oxalis', 'version': '0.5.4', 'description': 'Distributed async task/job
 queue', 'long_description': '
 \n\n_[Package_version]\n\n
 \n\n# Oxalis \n\nDistributed async task/job queue, like Celery for `asyncio`
 world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout
 and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ)
 support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and
 time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis
```

### Comparing `oxalis-0.5.3/PKG-INFO` & `oxalis-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.5.3
+Version: 0.5.4
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

