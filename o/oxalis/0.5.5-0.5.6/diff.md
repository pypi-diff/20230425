# Comparing `tmp/oxalis-0.5.5.tar.gz` & `tmp/oxalis-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.5.5.tar", max compression
+gzip compressed data, was "oxalis-0.5.6.tar", max compression
```

## Comparing `oxalis-0.5.5.tar` & `oxalis-0.5.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.5/LICENSE
--rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.5.5/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.5/oxalis/__init__.py
--rw-r--r--   0        0        0    10989 2023-04-24 10:09:33.396921 oxalis-0.5.5/oxalis/amqp.py
--rw-r--r--   0        0        0     7362 2023-04-25 06:16:48.318116 oxalis-0.5.5/oxalis/base.py
--rw-r--r--   0        0        0     1976 2023-04-25 06:16:48.314116 oxalis-0.5.5/oxalis/beater.py
--rw-r--r--   0        0        0     3833 2023-04-24 10:09:33.396921 oxalis-0.5.5/oxalis/kafka.py
--rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.5.5/oxalis/pool.py
--rw-r--r--   0        0        0     6536 2023-04-24 10:09:33.396921 oxalis-0.5.5/oxalis/redis.py
--rw-r--r--   0        0        0      972 2023-04-25 06:18:08.264159 oxalis-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     7859 1970-01-01 00:00:00.000000 oxalis-0.5.5/setup.py
--rw-r--r--   0        0        0     8003 1970-01-01 00:00:00.000000 oxalis-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.5.6/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.5.6/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.5.6/oxalis/__init__.py
+-rw-r--r--   0        0        0    10989 2023-04-24 10:09:33.396921 oxalis-0.5.6/oxalis/amqp.py
+-rw-r--r--   0        0        0     7363 2023-04-25 08:52:26.060476 oxalis-0.5.6/oxalis/base.py
+-rw-r--r--   0        0        0     1976 2023-04-25 06:16:48.314116 oxalis-0.5.6/oxalis/beater.py
+-rw-r--r--   0        0        0     3833 2023-04-24 10:09:33.396921 oxalis-0.5.6/oxalis/kafka.py
+-rw-r--r--   0        0        0     3506 2023-04-20 05:15:02.508527 oxalis-0.5.6/oxalis/pool.py
+-rw-r--r--   0        0        0     6536 2023-04-24 10:09:33.396921 oxalis-0.5.6/oxalis/redis.py
+-rw-r--r--   0        0        0      972 2023-04-25 08:52:42.632074 oxalis-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     7859 1970-01-01 00:00:00.000000 oxalis-0.5.6/setup.py
+-rw-r--r--   0        0        0     8003 1970-01-01 00:00:00.000000 oxalis-0.5.6/PKG-INFO
```

### Comparing `oxalis-0.5.5/LICENSE` & `oxalis-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/README.md` & `oxalis-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/oxalis/amqp.py` & `oxalis-0.5.6/oxalis/amqp.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/oxalis/base.py` & `oxalis-0.5.6/oxalis/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     @classmethod
     def decode(cls, content: bytes) -> MESSAGE_TYPE:
         return json.loads(content)
 
 
 class Oxalis(abc.ABC, tp.Generic[TASK_TV]):
     READY_FILE_PATH: tp.ClassVar[str] = "/tmp/oxalis_ready"
-    HEATBEAT_FILE_PATH: tp.ClassVar[str] = "/tmp/oxalis_heatbeat"
+    HEATBEAT_FILE_PATH: tp.ClassVar[str] = "/tmp/oxalis_heartbeat"
 
     def __init__(
         self,
         task_cls: tp.Type[TASK_TV],
         task_codec: TaskCodec = TaskCodec(),
         pool: Pool = Pool(),
         timeout: float = 5.0,
```

### Comparing `oxalis-0.5.5/oxalis/beater.py` & `oxalis-0.5.6/oxalis/beater.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/oxalis/kafka.py` & `oxalis-0.5.6/oxalis/kafka.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/oxalis/pool.py` & `oxalis-0.5.6/oxalis/pool.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/oxalis/redis.py` & `oxalis-0.5.6/oxalis/redis.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.5.5/pyproject.toml` & `oxalis-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.5.5"
+version = "0.5.6"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.7",
```

### Comparing `oxalis-0.5.5/setup.py` & `oxalis-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aio-pika>=8.0.3', 'aiokafka>=0.8.0', 'croniter>=1.3.5', 'redis>=4.5.1']
 
 setup_kwargs = {
     'name': 'oxalis',
-    'version': '0.5.5',
+    'version': '0.5.6',
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
-'oxalis', 'version': '0.5.5', 'description': 'Distributed async task/job
+'oxalis', 'version': '0.5.6', 'description': 'Distributed async task/job
 queue', 'long_description': '
 \n\n_[Package_version]\n\n
 \n\n# Oxalis \n\nDistributed async task/job queue, like Celery for `asyncio`
 world\n\n## Feature\n\n* Redis and AMQP(RabbitMQ etc.) support\n* Task timeout
 and concurrency limit support\n* Delayed task(Both Redis and RabbitMQ)
 support\n* Cron task/job beater\n* Built-in coroutine pool with concurrency and
 time limit\n\n## Install\n\n```pip install oxalis```\n\n## Example with Redis
```

### Comparing `oxalis-0.5.5/PKG-INFO` & `oxalis-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.5.5
+Version: 0.5.6
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

