# Comparing `tmp/osint-python-starter-service-2.0.7.tar.gz` & `tmp/osint-python-starter-service-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.7.tar", last modified: Fri Apr 14 16:06:04 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.8.tar", last modified: Tue Apr 25 07:18:30 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.7.tar` & `osint-python-starter-service-2.0.8.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.7/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.7/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-14 16:02:11.000000 osint-python-starter-service-2.0.7/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.7/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.7/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6865 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.7/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.7/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3061 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.7/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-13 20:22:15.000000 osint-python-starter-service-2.0.7/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.7/starter_service/examples/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/starter_service/examples/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 15:58:14.000000 osint-python-starter-service-2.0.7/starter_service/examples/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-14 16:03:53.000000 osint-python-starter-service-2.0.7/starter_service/examples/classes/article_raw_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-14 16:03:53.000000 osint-python-starter-service-2.0.7/starter_service/examples/classes/metadata_item_key_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.7/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.7/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.7/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1186 2023-04-14 16:04:08.000000 osint-python-starter-service-2.0.7/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.7/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.7/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6392 2023-04-14 16:04:58.000000 osint-python-starter-service-2.0.7/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.8/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1731 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.8/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2202 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      721 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-25 07:18:30.000000 osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.8/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.8/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.8/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6965 2023-04-25 05:49:53.000000 osint-python-starter-service-2.0.8/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-25 06:44:40.000000 osint-python-starter-service-2.0.8/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3401 2023-04-25 06:59:18.000000 osint-python-starter-service-2.0.8/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-24 18:58:31.000000 osint-python-starter-service-2.0.8/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-25 07:18:30.740267 osint-python-starter-service-2.0.8/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.8/starter_service/examples/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      593 2023-04-25 07:05:40.000000 osint-python-starter-service-2.0.8/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1287 2023-04-25 07:13:29.000000 osint-python-starter-service-2.0.8/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1223 2023-04-21 12:06:51.000000 osint-python-starter-service-2.0.8/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1155 2023-04-25 07:17:35.000000 osint-python-starter-service-2.0.8/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6236 2023-04-25 06:28:52.000000 osint-python-starter-service-2.0.8/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      985 2023-04-25 07:17:35.000000 osint-python-starter-service-2.0.8/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     7571 2023-04-25 06:06:55.000000 osint-python-starter-service-2.0.8/starter_service/schemas.py
```

### Comparing `osint-python-starter-service-2.0.7/LICENSE` & `osint-python-starter-service-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.7/PKG-INFO` & `osint-python-starter-service-2.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 First you need to provide ENV variables for the service to run.
 
 ### ENV variables
 
 Main ENV variables:
 
 - `CLIENT_ID` - client id of the service
-- `REST_API_ENABLED` - enable/disable REST API
+- `REST_API_ENABLED` - enable/disable REST API (default: `true`)
 
 ## Kafka
 
 - `CONSUME` - comma separated list of topics to consume
 - `PRODUCE` - comma separated list of topics to produce
 - `KAFKA_HOST` - kafka host
 - `SCHEMA_REGISTRY` - schema registry host
```

### Comparing `osint-python-starter-service-2.0.7/README.md` & `osint-python-starter-service-2.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 First you need to provide ENV variables for the service to run.
 
 ### ENV variables
 
 Main ENV variables:
 
 - `CLIENT_ID` - client id of the service
-- `REST_API_ENABLED` - enable/disable REST API
+- `REST_API_ENABLED` - enable/disable REST API (default: `true`)
 
 ## Kafka
 
 - `CONSUME` - comma separated list of topics to consume
 - `PRODUCE` - comma separated list of topics to produce
 - `KAFKA_HOST` - kafka host
 - `SCHEMA_REGISTRY` - schema registry host
```

### Comparing `osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 First you need to provide ENV variables for the service to run.
 
 ### ENV variables
 
 Main ENV variables:
 
 - `CLIENT_ID` - client id of the service
-- `REST_API_ENABLED` - enable/disable REST API
+- `REST_API_ENABLED` - enable/disable REST API (default: `true`)
 
 ## Kafka
 
 - `CONSUME` - comma separated list of topics to consume
 - `PRODUCE` - comma separated list of topics to produce
 - `KAFKA_HOST` - kafka host
 - `SCHEMA_REGISTRY` - schema registry host
```

### Comparing `osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.8/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,11 +15,8 @@
 starter_service/kafka_adapter.py
 starter_service/messages.py
 starter_service/schemas.py
 starter_service/examples/__init__.py
 starter_service/examples/error.py
 starter_service/examples/manual_kafka.py
 starter_service/examples/multi.py
-starter_service/examples/single.py
-starter_service/examples/classes/__init__.py
-starter_service/examples/classes/article_raw_en.py
-starter_service/examples/classes/metadata_item_key_en.py
+starter_service/examples/single.py
```

### Comparing `osint-python-starter-service-2.0.7/setup.py` & `osint-python-starter-service-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.7",
+    version="2.0.8",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/api.py` & `osint-python-starter-service-2.0.8/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.7/starter_service/api_server.py` & `osint-python-starter-service-2.0.8/starter_service/api_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 from starlette.status import HTTP_200_OK
 
 from starter_service.api import API
 from starter_service.env import ENV
 from starter_service.messages import MessageHistory
 from starter_service.schemas import SchemaRegistry
 
-_schema = SchemaRegistry()
-
 
 class APIServer:
 
     def __init__(self, name=None, ready: callable = None, health: callable = None, kafka_status: str = None,
-                 base_service=None, **kwargs):
+                 base_service=None, callback=None, **kwargs):
         self.name = name
         self._validated()
         self.app = FastAPI(title=self.name)
         self.router = APIRouter()
+        self.callback = callback
 
         @self.app.exception_handler(Exception)
         async def validation_exception_handler(request, err):
             base_error_message = f"Failed to execute: {request.method}: {request.url}"
             # Change here to LOGGER
             return JSONResponse(status_code=400, content={"message": f"{base_error_message}. Detail: {err}"})
 
@@ -75,15 +74,15 @@
                     "heartbeat_interval": ENV.HEARTBEAT_INTERVAL,
                     "offset_type": ENV.OFFSET_TYPE,
                     "topics": {
                         "consume": ENV.CONSUME,
                         "produce": ENV.PRODUCE
                     }
                 },
-                "schemas:": _schema.get_schemas_dict(),
+                "schemas:": SchemaRegistry.get_schemas_dict(),
                 "methods": API.functions
             }
 
         @self.router.get("/api/health", tags=["status"])
         def health(verbose: bool = False):
             """Return health status"""
             health = self._health()
@@ -107,14 +106,15 @@
     def start(self):
         """Start the server"""
         self._logger.info("Starting API server")
         self._uptime = datetime.datetime.now().isoformat()
         self._running = True
         self._thread = threading.Thread(target=self._run)
         self._thread.start()
+        self.callback()
 
     def stop(self):
         self._logger.info("Stopping API server")
         self._running = False
         self._thread.join()
 
     def _run(self):
@@ -130,17 +130,18 @@
         """Register routes that are dynamically added by the user"""
         self._logger.info("Registering dynamic routes")
         for consumer, producer, doc, func, _type in API.functions:
             self._register_route(consumer, producer, doc, func, _type)
 
     def _register_route(self, consumer, producer, doc, func, _type):
         """Register a route"""
-        self._logger.info(f"Registering route {consumer} -> {producer} ({doc})")
-        consumer_class = _schema.get_schema(consumer)
-        producer_class = _schema.get_schema(producer)
+        consumer_class = SchemaRegistry.get_schema(consumer)
+        producer_class = SchemaRegistry.get_schema(producer)
+
+        self._logger.info(f"Registering route {consumer}:{consumer_class} -> {producer}:{producer_class} ({doc})")
         func_wrapper = lambda message: func(self._base_service, message) \
             if isinstance(message, str) else func(self._base_service, jsonable_encoder(message))
         path = f"/api{f'/{consumer}' if consumer else ''}{f'/{producer}' if producer else ''}"
 
         func_wrapper.__annotations__ = {'message': consumer_class, 'return': producer_class}
         self.router.add_api_route(path, func_wrapper, methods=[_type], response_model=producer_class, tags=["topics"],
                                   summary=doc)
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.8/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.7/starter_service/base_service.py` & `osint-python-starter-service-2.0.8/starter_service/base_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import logging
 import traceback
 from abc import ABC, abstractmethod
 
 from starter_service.api_server import APIServer
 from starter_service.env import ENV
 from starter_service.kafka_adapter import KafkaAdapter
+from starter_service.schemas import SchemaRegistry
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
 
 class StarterService(ABC):
     """Base class for all services."""
     name = None  # Change this to the name of your service or use CLIENT_ID environment variable
+    path = None  # Path for local schemas, use SCHEMA_PATH environment variable
 
     def __init__(self):
         self.logger = logging.getLogger(__name__)
-        self._name = None
         self._kafka = None
         self._api = None
         self._schemas = None
         self._functions = None
         self._initialize()
+        self._schema_registry = None
 
     @abstractmethod
     def ready(self) -> bool:
         """Return True if service is ready to receive messages, False otherwise."""
         pass
 
     @abstractmethod
@@ -32,54 +34,60 @@
         """Return service health status."""
         pass
 
     def _initialize(self):
         """Initialize services"""
         self.name = ENV.CLIENT_ID = ENV.CLIENT_ID or self.name or self.__class__.__name__
 
-        def _schema_callback():
-            """Callback for Schema Registry, called when Schema Registry is ready or when an error occurs"""
-            self.logger.info("Schema callback")
-            self._register_api(_kafka_status)
+        """Initialize Schema Registry"""
+        SchemaRegistry.initialize(self.path)
+
+        def _api_callback():
+            """Callback for API Server, called when API Server is ready or when an error occurs"""
+            self.logger.info("API callback")
+            self.api_callback()
 
         def _kafka_callback():
             """Callback for Kafka Adapter, called when Kafka Adapter is ready or when an error occurs"""
             self.logger.info("Kafka callback")
-            self._register_schemas(_schema_callback)
+            self.kafka_callback()
+            self._register_api(_kafka_status, _api_callback)
 
         """Initialize services"""
         _kafka_status = "ok"
         self.logger.info("Initializing kafka")
         try:
             self._kafka = KafkaAdapter(callback=_kafka_callback, base_service=self)
             self._kafka.start()
             self.logger.info(f"Kafka initialized.")
         except Exception as e:
             _kafka_status = f"Error: {e}"
             _kafka_callback()
             self.logger.error(f'Error initializing kafka: {e}')
 
-    def _register_schemas(self, callback):
-        try:
-            callback()
-        except Exception as e:
-            self.logger.error(f'Error initializing schema registry: {e}')
-
-    def _register_api(self, _kafka_status):
+    def _register_api(self, _kafka_status, callback):
         try:
             self._api = APIServer(name=self.name, ready=self.ready, health=self.health, kafka_status=_kafka_status,
-                                  base_service=self)
+                                  base_service=self, callback=callback)
             self._api.start()
             self.logger.info(f"REST API initialized.")
         except Exception as e:
             self.logger.error(f'Error initializing api: {e}')
             traceback.print_exc()
 
         if self._kafka is None and self._api is None:
             self.logger.error('No services initialized. Shutting down.')
             exit(1)
 
-    def send_message(self, message, topic):
+    def send_message(self, message, topic, testing=True):
         """Send message to Kafka"""
         if self._kafka is None:
             raise Exception("Kafka is not initialized")
-        self._kafka.send_message(message, topics=topic, testing=True)
+        self._kafka.send_message(message, topics=topic, testing=testing)
+
+    def kafka_callback(self):
+        """Override this method to callback after service is initialized"""
+        pass
+
+    def api_callback(self):
+        """Override this method to callback after service is initialized"""
+        pass
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/env.py` & `osint-python-starter-service-2.0.8/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.7/starter_service/examples/error.py` & `osint-python-starter-service-2.0.8/starter_service/examples/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import os
-import sys
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 os.environ['CONSUME'] = 'article_raw_en'
 os.environ['PRODUCE'] = 'metadata_item_key_en'
-os.environ['REST_API_ENABLED'] = 'True'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class SingleRoute(StarterService):
     name = "single_error"
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.8/starter_service/examples/manual_kafka.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import os
-import sys
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 os.environ['CONSUME'] = 'article_raw_xx'
-os.environ['PRODUCE'] = 'article_raw_en,article_raw_lt'
-os.environ['REST_API_ENABLED'] = 'True'
+os.environ['PRODUCE'] = 'article_raw_en,article_raw_lt,metadata_item_update'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class ManualKafka(StarterService):
     name = "manual_kafka"
+    path = "app"
 
     def __init__(self):
         super().__init__()
 
     def health(self):
         return
 
     def ready(self):
         return True
 
+    def kafka_callback(self):
+        """Kafka callback"""
+        self.logger.info("Kafka callback")
+        # When testing is True, the message is not sent to Kafka, but is printed to the console
+        self.send_message({
+            "articleId": "string",
+            "origin": "string",
+            "data": []
+        }, 'metadata_item_update',
+            testing=True  # Default is False, when deploying to production, set to False
+        )
+
     @API.post(consumer="article_raw_xx", doc="Process article_raw_xx and send to article_raw_en, article_raw_lt")
     def handle_message(self, message: dict):
         message['language'] = 'en'
         self.send_message(message, 'article_raw_en')
+
         message['language'] = 'lt'
         self.send_message(message, 'article_raw_lt')
         return {}
 
 
 if __name__ == '__main__':
     ManualKafka()
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.8/starter_service/examples/multi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import os
-import sys
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 os.environ['CONSUME'] = 'article_raw_xx'
 os.environ['PRODUCE'] = 'article_raw_en,article_raw_lt,article_raw_nl'
 os.environ['REST_API_ENABLED'] = 'True'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.8/starter_service/kafka_adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 from starter_service.api import API
 from starter_service.env import ENV
 from starter_service.schemas import SchemaRegistry
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
-_schema = SchemaRegistry()
-
 
 class KafkaAdapter(Thread):
     """Kafka adapter"""
 
     def __init__(self, callback=None, base_service=None) -> None:
         super().__init__()
         self.daemon = True
@@ -54,15 +52,15 @@
             _consumer = ConsumerManager(
                 options=self._test_bed_options,
                 kafka_topic=topic,
                 handle_message=self._handle_message,
                 run=lambda: run
             )
             self.logger.info(f"Registering schema from kafka for {topic}")
-            _schema.register_schema(_consumer.schema_str, topic)
+            SchemaRegistry.register_schema(_consumer.schema_str, topic)
             self.logger.info(f"Initializing listener for topic {topic}")
             listener_threads.append(threading.Thread(
                 target=_consumer.listen)
             )
 
         # start all threads
         for thread in listener_threads:
@@ -90,37 +88,31 @@
         for thread in listener_threads:
             thread.join()
 
         raise Exception
 
     def send_message(self, message, topics=None, testing=False):
         """Send message to kafka topic"""
-        # _msg_uuid = kwargs.get('uuid')
         if testing:
             self.logger.info(f"Sending test message to {topics}\n{message}")
-            # MessageHistory.add_outgoing_message(_msg_uuid, message)
             return
 
         if topics:
             if isinstance(topics, str):
                 topics = [topic.strip() for topic in topics.split(',')]
             for topic in topics:
                 self.logger.info(f"Sending message to {topic}")
                 if topic in self._producers:
                     if ENV.DEBUG:
                         self.logger.info(f"Sending message to {topic}\n{message}")
-                    # if ENV.REST_API_ENABLED and ENV.REST_LOG_MESSAGES:
-                    #     MessageHistory.add_outgoing_message(_msg_uuid, message)
                     self._producers[topic].send_messages(messages=[message])
         else:
             for topic, producer in self._producers.items():
                 if ENV.DEBUG:
                     self.logger.info(f"Sending message to {topic}\n{message}")
-                # if ENV.REST_API_ENABLED and ENV.REST_LOG_MESSAGES:
-                #     MessageHistory.add_outgoing_message(_msg_uuid, message)
                 producer.send_messages(messages=[message])
 
     def _validate_params(self):
         """Validate that all required params are set"""
         if ENV.CLIENT_ID is None:
             raise ValueError("CLIENT_ID cannot be None. Please set it in the environment.")
         if not ENV.CONSUME and not ENV.PRODUCE:
@@ -131,15 +123,15 @@
         for topic in ENV.PRODUCE:
             self.logger.info(f"Initializing producer for topic {topic}")
             _producer = ProducerManager(
                 options=self._test_bed_options,
                 kafka_topic=topic
             )
             self._producers[topic] = _producer
-            _schema.register_schema(_producer.schema_str, topic)
+            SchemaRegistry.register_schema(_producer.schema_str, topic)
 
     def _init_options(self):
         _options = {
             "kafka_host": ENV.KAFKA_HOST,
             "schema_registry": ENV.SCHEMA_REGISTRY,
             "partitioner": ENV.PARTITIONER,
             "consumer_group": ENV.CLIENT_ID,
@@ -155,23 +147,19 @@
                          f" Consume{ENV.CONSUME}, Produce{ENV.PRODUCE}")
         self.logger.info(f"Connected to kafka: {_options}")
 
     def _handle_message(self, message, topic):
         self.logger.info(f"Received message for topic {topic}")
         if ENV.DEBUG:
             self.logger.info(f"Message {message}")
-        # message_uuid = uuid.uuid4().hex
-        # if ENV.REST_API_ENABLED and ENV.REST_LOG_MESSAGES:
-        # MessageHistory.add_incoming_message(message_uuid, message)
-        # methods = get_function_by_consummer(topic)
 
         funcs = API.get_func_by_consumer(topic)
         for consumer, producer, doc, func, _type in funcs:
             self.logger.info(f'Found function form {consumer}, to {producer}')
             try:
                 response = func(self._base_service, message)
                 if producer and response:
                     self.logger.info(f"Sending response: {producer}, {str(response)[:100]}")
                     self.send_message(response, topics=producer)
             except Exception as e:
                 traceback.print_exc()
-                self.logger.error(e)
+                self.logger.error(e)
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/messages.py` & `osint-python-starter-service-2.0.8/starter_service/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import collections
 
-from starter_service.schemas import SchemaRegistry
-
 _incoming_messages = collections.deque([], 20)
 _outgoing_messages = collections.deque([], 20)
-_schema = SchemaRegistry()
 
 # TODO: Add a message history class to store the last 20 messages
 class MessageHistory:
 
     @staticmethod
     def add_incoming_message(uuid, message):
         _incoming_messages.append((uuid, message))
```

### Comparing `osint-python-starter-service-2.0.7/starter_service/schemas.py` & `osint-python-starter-service-2.0.8/starter_service/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import logging
 from pathlib import Path
 from pydoc import locate
-from threading import Lock
 
 from starter_service.avro_parser import avsc_to_pydantic
 
-_pathlib_path = Path().absolute()
 _logger = logging.getLogger(__name__)
 
 
 class Schema:
 
     def __init__(self, topic=None, filename=None, class_name=None, class_obj=None, full_path=None):
         self.topic = topic
@@ -23,153 +21,181 @@
         return f"{self.class_name} from {self.filename}"
 
     def __repr__(self):
         return f"{self.class_name} from {self.filename}"
 
 
 class SchemaRegistry:
-    _lock = Lock()
-    _instance = None
     _logger = logging.getLogger(__name__)
-
+    _pathlib_path = None
     _schemas = {}
-    _classes = {}
-
-    def __new__(self):
-        with self._lock:
-            if self._instance is None:
-                self._instance = super().__new__(self)
-        return self._instance
-
-    def get_schemas(self):
-        return self._schemas
-
-    def get_schemas_dict(self):
-        return {schema.topic: schema.class_name for class_name, schema in self._schemas.items()}
 
-    def initialize(self):
+    @classmethod
+    def get_schemas(cls):
+        return cls._schemas
+
+    @classmethod
+    def get_schemas_dict(cls):
+        return {schema.topic: schema.class_name for class_name, schema in cls._schemas.items()}
+
+    @classmethod
+    def initialize(cls, path=None):
+        cls._pathlib_path = Path(path) if path else Path().absolute()
+        cls._logger.info(f"Initializing SchemaRegistry {cls._pathlib_path}")
         # create schema folder if not exists
-        self._init_dir()
+        cls._init_dir()
         # load schemas from folder
-        self._load_local_schemas()
+        cls._load_local_schemas()
         # load classes from folder
-        self._load_local_classes()
+        cls._load_local_classes()
 
-    def _load_local_schemas(self):
+    @classmethod
+    def _load_local_schemas(cls):
         # load avro schemas from local folder
         _schemas = []
-        schemas_dir = _pathlib_path / "schemas"
+        try:
+            if not cls._pathlib_path.exists():
+                cls._pathlib_path.mkdir()
+        except Exception as e:
+            cls._logger.error(f"Error creating schema folder: {e}")
+            return
+
+        schemas_dir = cls._pathlib_path / "schemas"
         for file in schemas_dir.iterdir():
             if file.suffix == ".avsc" or file.suffix == "-value.avsc" or file.suffix == "-key.avsc":
                 _schemas.append(file)
 
         if len(_schemas) == 0:
-            self._logger.warning(f"No schemas found in {_pathlib_path.absolute()}")
+            cls._logger.warning(f"No schemas found in {cls._pathlib_path.absolute()}")
             return
 
         for file in _schemas:
-            self._load_schema_from_file(file.name)
+            cls._load_schema_from_file(file.name)
 
-    def _load_local_classes(self):
-        classes_dir = _pathlib_path / "classes"
+    @classmethod
+    def _load_local_classes(cls):
+        classes_dir = cls._pathlib_path / "classes"
         for file in classes_dir.iterdir():
             if file.suffix == ".py" and file.name != "__init__.py":
                 topic = file.name.replace(".py", "")
-                if topic in self._schemas:
+                if topic in cls._schemas:
                     continue
-                self._logger.info(f"Loading class {topic} from file {file}")
-                main_class = self._read_main_class_from_file(file)
-                schema = Schema(topic, file, main_class, self._load_class_from_file(f'{topic}.py', main_class), file)
-                self._schemas[topic] = schema
+                cls._logger.info(f"Loading class {topic} from file {file}")
+                main_class = cls._read_main_class_from_file(file.name)
+                schema = Schema(topic, file, main_class, cls._load_class_from_file(f'{topic}.py', main_class), file)
+                cls._schemas[topic] = schema
 
-    def _read_main_class_from_file(self, file):
+    @classmethod
+    def _read_main_class_from_file(cls, file):
         main_class = None
-        file_path = _pathlib_path / "classes" / file
+        _logger.info(f"Reading main class from file {file}")
+        file_path = cls._pathlib_path / "classes" / file
+        if not file_path.exists():
+            _logger.error(f"File {file_path} does not exist")
+            return None
         with open(file_path, "r") as f:
             for line in f.readlines():
                 if line.startswith("main_class"):
                     main_class = line.split(" ")[2].strip()
+                    break
+            _logger.info(f"Main class is {main_class}")
         return main_class
 
-    def register_schema(self, schema: [str, dict], topic: str):
+    @classmethod
+    def register_schema(cls, schema: [str, dict], topic: str):
         """
         Register a schema from a string or dict
         :param schema: AVRO string schema
         :param topic: topic to register the schema for
         :param _type: SchemaType Enum (consume or produce)
         :return:
         """
-        self._logger.info(f"Registering schema for topic {topic}")
-        filename, main_class, python_classes = self._avro_to_file(schema)
+        cls._logger.info(f"Registering schema for topic {topic}")
+        filename, main_class, python_classes = cls._avro_to_file(schema)
 
-        full_path = _pathlib_path / "classes" / f'{topic}.py'
+        full_path = cls._pathlib_path / "classes" / f'{topic}.py'
+        cls._logger.info(f"Writing schema to file {full_path}, path {cls._pathlib_path}")
         with open(full_path, "w") as f:
             f.write(python_classes)
-        schema = Schema(topic, filename, main_class, self._load_class_from_file(f'{topic}.py', main_class), full_path)
-        self._schemas[topic] = schema
-
-    def _load_class_from_file(self, filename, class_name):
-        self._logger.info(f"Loading class from file {filename} with class {class_name}")
-        return locate(f"classes.{filename[:-3]}.{class_name}")
+        schema = Schema(topic, filename, main_class, cls._load_class_from_file(f'{topic}.py', main_class), full_path)
+        _logger.info(f"Registering schema {schema.__dict__} for topic {topic}")
+        cls._schemas[topic] = schema
+
+    @classmethod
+    def _load_class_from_file(cls, filename, class_name):
+        absolute = str(Path().absolute())
+        path = str(cls._pathlib_path).replace(absolute, "").replace("/", ".")
+        cls._logger.info(
+            f"Loading class from file {filename} with class {class_name}, path {path}.classes.{filename[:-3]}.{class_name}")
+        return locate(f"{path}.classes.{filename[:-3]}.{class_name}", True)
 
-    def _avro_to_file(self, schema: [str, dict]) -> [str, str, str]:
+    @classmethod
+    def _avro_to_file(cls, schema: [str, dict]) -> [str, str, str]:
         """
         :param schema: AVRO schema as string or dict
         :return: filename, main_class, python_classes
         """
         if isinstance(schema, str):
             schema = json.loads(schema)
         class_name = schema['name']
         if class_name is None:
             raise ValueError(f"Schema {schema[:20]} does not contain a name")
         python_classes, main_class = avsc_to_pydantic(schema)
         filename = f"{class_name.lower()}.py"
         return filename, main_class, python_classes
 
-    def _load_schema_from_file(self, filename):
+    @classmethod
+    def _load_schema_from_file(cls, filename):
         try:
-            self._logger.info(f"Loading schema {filename}")
-            filepath = _pathlib_path / "schemas" / filename
+            cls._logger.info(f"Loading schema {filename}")
+            filepath = cls._pathlib_path / "schemas" / filename
             with open(filepath, "r") as f:
-                self.register_schema(f.read(), self._filename_to_topic(filename))
+                cls.register_schema(f.read(), cls._filename_to_topic(filename))
         except Exception as e:
-            self._logger.error(f"Error loading schema {filename}: {e}")
+            cls._logger.error(f"Error loading schema {filename}: {e}")
 
-    def _filename_to_topic(self, filename):
+    @classmethod
+    def _filename_to_topic(cls, filename):
         if filename.endswith("-value.avsc"):
             return filename[:-11].lower()
         if filename.endswith("-key.avsc"):
             return filename[:-9].lower()
         if filename.endswith(".avsc"):
             return filename[:-5].lower()
 
-    def _init_dir(self):
-        classes_dir = _pathlib_path / "classes"
+    @classmethod
+    def _init_dir(cls):
+        try:
+            if not cls._pathlib_path.exists():
+                cls._pathlib_path.mkdir(parents=True, exist_ok=True)
+        except Exception as e:
+            cls._logger.error(f"Error creating schema folder: {e}")
+            return
+        classes_dir = cls._pathlib_path / "classes"
         if not classes_dir.exists():
             try:
                 classes_dir.mkdir()
                 init_file = classes_dir / "__init__.py"
                 init_file.touch()
                 readme_file = classes_dir / "readme.txt"
                 readme_file.write_text("This folder contains all the generated classes from the schemas")
             except Exception as e:
-                self._logger.error(f"Error creating classes folder {e}")
+                cls._logger.error(f"Error creating classes folder {e}")
                 raise e
 
-        schemas_dir = _pathlib_path / "schemas"
+        schemas_dir = cls._pathlib_path / "schemas"
         if not schemas_dir.exists():
             try:
                 schemas_dir.mkdir()
                 readme_file = schemas_dir / "readme.txt"
                 readme_file.write_text("Use this folder to provide AVRO schemas")
             except Exception as e:
-                self._logger.error(f"Error creating schema folder {e}")
+                cls._logger.error(f"Error creating schema folder {e}")
                 raise e
 
-    def get_schema(self, topic) -> object or dict:
-        with self._lock:
-            if not topic or topic not in self._schemas:
-                return dict
-            return self._schemas[topic].class_obj
-
-
-SchemaRegistry().initialize()
+    @classmethod
+    def get_schema(cls, topic) -> object or dict:
+        if not topic:
+            return dict
+        if topic not in cls._schemas.keys():
+            return dict
+        return cls._schemas[topic].class_obj
```

