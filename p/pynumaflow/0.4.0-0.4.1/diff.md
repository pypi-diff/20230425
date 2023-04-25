# Comparing `tmp/pynumaflow-0.4.0.tar.gz` & `tmp/pynumaflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumaflow-0.4.0.tar", max compression
+gzip compressed data, was "pynumaflow-0.4.1.tar", max compression
```

## Comparing `pynumaflow-0.4.0.tar` & `pynumaflow-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0    11357 2023-04-14 17:52:54.631606 pynumaflow-0.4.0/LICENSE
--rw-r--r--   0        0        0     3506 2023-04-14 17:52:54.631606 pynumaflow-0.4.0/README.md
--rw-r--r--   0        0        0      985 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/__init__.py
--rw-r--r--   0        0        0      511 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/_constants.py
--rw-r--r--   0        0        0      248 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/exceptions.py
--rw-r--r--   0        0        0      521 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/__init__.py
--rw-r--r--   0        0        0     9146 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/_dtypes.py
--rw-r--r--   0        0        0     1779 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/_udfunction_pb2.pyi
--rw-r--r--   0        0        0    11695 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/async_server.py
--rw-r--r--   0        0        0      512 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/asynciter.py
--rw-r--r--   0        0        0    10262 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/multiproc_server.py
--rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/__init__.py
--rw-r--r--   0        0        0     2029 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/udfunction.proto
--rw-r--r--   0        0        0     3137 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2.py
--rw-r--r--   0        0        0     7522 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2_grpc.py
--rw-r--r--   0        0        0     8370 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/server.py
--rw-r--r--   0        0        0      219 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/__init__.py
--rw-r--r--   0        0        0     3290 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/_dtypes.py
--rw-r--r--   0        0        0     2257 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/_udfunction_pb2.pyi
--rw-r--r--   0        0        0     5429 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/async_sink.py
--rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/__init__.py
--rw-r--r--   0        0        0     1716 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/udsink.proto
--rw-r--r--   0        0        0     2512 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2.py
--rw-r--r--   0        0        0     4105 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2_grpc.py
--rw-r--r--   0        0        0     4696 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/server.py
--rw-r--r--   0        0        0       79 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/__init__.py
--rw-r--r--   0        0        0     2037 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/server_utils.py
--rw-r--r--   0        0        0    10505 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_async_server.py
--rw-r--r--   0        0        0     4678 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_async_server_err.py
--rw-r--r--   0        0        0     6720 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_datatypes.py
--rw-r--r--   0        0        0     3889 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_messages.py
--rw-r--r--   0        0        0     3663 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_messagets.py
--rw-r--r--   0        0        0     9632 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_multiproc.py
--rw-r--r--   0        0        0     8131 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_sync_server.py
--rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/__init__.py
--rw-r--r--   0        0        0     5153 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_async_sink.py
--rw-r--r--   0        0        0     3327 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_datatypes.py
--rw-r--r--   0        0        0     1305 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_responses.py
--rw-r--r--   0        0        0     5937 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_server.py
--rw-r--r--   0        0        0      170 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/types.py
--rw-r--r--   0        0        0     1358 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 pynumaflow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 00:58:49.725827 pynumaflow-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3506 2023-04-25 00:58:49.725827 pynumaflow-0.4.1/README.md
+-rw-r--r--   0        0        0      985 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/__init__.py
+-rw-r--r--   0        0        0      511 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/_constants.py
+-rw-r--r--   0        0        0      248 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/exceptions.py
+-rw-r--r--   0        0        0      521 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/__init__.py
+-rw-r--r--   0        0        0     9146 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/_dtypes.py
+-rw-r--r--   0        0        0     1779 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/_udfunction_pb2.pyi
+-rw-r--r--   0        0        0    13045 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/async_server.py
+-rw-r--r--   0        0        0      512 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/asynciter.py
+-rw-r--r--   0        0        0    11555 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/multiproc_server.py
+-rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/__init__.py
+-rw-r--r--   0        0        0     2029 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/udfunction.proto
+-rw-r--r--   0        0        0     3138 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2.py
+-rw-r--r--   0        0        0     7523 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2_grpc.py
+-rw-r--r--   0        0        0     9546 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/function/server.py
+-rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/info/__init__.py
+-rw-r--r--   0        0        0     1594 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/info/server.py
+-rw-r--r--   0        0        0     1249 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/info/types.py
+-rw-r--r--   0        0        0      219 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/__init__.py
+-rw-r--r--   0        0        0     3290 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/_dtypes.py
+-rw-r--r--   0        0        0     2257 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/_udfunction_pb2.pyi
+-rw-r--r--   0        0        0     5832 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/async_sink.py
+-rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/udsink.proto
+-rw-r--r--   0        0        0     2513 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2.py
+-rw-r--r--   0        0        0     4106 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2_grpc.py
+-rw-r--r--   0        0        0     5100 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/sink/server.py
+-rw-r--r--   0        0        0       79 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/__init__.py
+-rw-r--r--   0        0        0    13402 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_async_server.py
+-rw-r--r--   0        0        0     4741 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_async_server_err.py
+-rw-r--r--   0        0        0     6720 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_datatypes.py
+-rw-r--r--   0        0        0     1940 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_info_server.py
+-rw-r--r--   0        0        0     3889 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_messages.py
+-rw-r--r--   0        0        0     3663 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_messagets.py
+-rw-r--r--   0        0        0    10620 2023-04-25 00:58:49.733827 pynumaflow-0.4.1/pynumaflow/tests/function/test_multiproc.py
+-rw-r--r--   0        0        0    10117 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/function/test_sync_server.py
+-rw-r--r--   0        0        0     2800 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/function/testing_utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/__init__.py
+-rw-r--r--   0        0        0     5153 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_async_sink.py
+-rw-r--r--   0        0        0     3327 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_datatypes.py
+-rw-r--r--   0        0        0     1305 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_responses.py
+-rw-r--r--   0        0        0     5937 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/tests/sink/test_server.py
+-rw-r--r--   0        0        0      170 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pynumaflow/types.py
+-rw-r--r--   0        0        0     1358 2023-04-25 00:58:49.737828 pynumaflow-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 pynumaflow-0.4.1/PKG-INFO
```

### Comparing `pynumaflow-0.4.0/LICENSE` & `pynumaflow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/README.md` & `pynumaflow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/__init__.py` & `pynumaflow-0.4.1/pynumaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/function/__init__.py` & `pynumaflow-0.4.1/pynumaflow/function/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/function/_dtypes.py` & `pynumaflow-0.4.1/pynumaflow/function/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/function/_udfunction_pb2.pyi` & `pynumaflow-0.4.1/pynumaflow/function/_udfunction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/function/async_server.py` & `pynumaflow-0.4.1/pynumaflow/function/async_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 )
 from pynumaflow.function import Messages, MessageTs, Datum, IntervalWindow, Metadata
 from pynumaflow.function._dtypes import ReduceResult, DatumMetadata
 from pynumaflow.function.asynciter import NonBlockingIterator
 from pynumaflow.function.proto import udfunction_pb2
 from pynumaflow.function.proto import udfunction_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
+from pynumaflow.info.server import get_sdk_version, write as info_server_write
+from pynumaflow.info.types import ServerInfo, Protocol, Language, SERVER_INFO_FILE_PATH
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
 UDFMapCallable = Callable[[List[str], Datum], Messages]
 UDFMapTCallable = Callable[[List[str], Datum], MessageTs]
@@ -134,29 +136,42 @@
     ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a function to each datum element.
         The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
         """
         # proto repeated field(keys) is of type google._upb._message.RepeatedScalarContainer
         # we need to explicitly convert it to list
-        res = await self.__invoke_map(
-            list(request.keys),
-            Datum(
-                keys=list(request.keys),
-                value=request.value,
-                event_time=request.event_time.event_time.ToDatetime(),
-                watermark=request.watermark.watermark.ToDatetime(),
-                metadata=DatumMetadata(
-                    msg_id=request.metadata.id,
-                    num_delivered=request.metadata.num_delivered,
+        try:
+            res = await self.__invoke_map(
+                list(request.keys),
+                Datum(
+                    keys=list(request.keys),
+                    value=request.value,
+                    event_time=request.event_time.event_time.ToDatetime(),
+                    watermark=request.watermark.watermark.ToDatetime(),
+                    metadata=DatumMetadata(
+                        msg_id=request.metadata.id,
+                        num_delivered=request.metadata.num_delivered,
+                    ),
                 ),
-            ),
-        )
+            )
+        except Exception as e:
+            context.set_code(grpc.StatusCode.UNKNOWN)
+            context.set_details(str(e))
+            return udfunction_pb2.DatumResponseList(elements=[])
+
         return udfunction_pb2.DatumResponseList(elements=res)
 
+    async def MapTFn(
+        self, request: udfunction_pb2.DatumRequest, context: NumaflowServicerContext
+    ) -> udfunction_pb2.DatumResponseList:
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        return udfunction_pb2.DatumResponseList(elements=[])
+
     async def __invoke_map(self, keys: List[str], req: Datum):
         try:
             msgs = await self.__map_handler(keys, req)
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
             raise err
         datums = []
@@ -180,18 +195,21 @@
         start, end = None, None
         for metadata_key, metadata_value in context.invocation_metadata():
             if metadata_key == WIN_START_TIME:
                 start = metadata_value
             elif metadata_key == WIN_END_TIME:
                 end = metadata_value
         if not (start or end):
-            raise ValueError(
+            context.set_code(grpc.StatusCode.INVALID_ARGUMENT)
+            context.set_details(
                 f"Expected to have all key/window_start_time/window_end_time; "
                 f"got start: {start}, end: {end}."
             )
+            yield udfunction_pb2.DatumResponseList(elements=[])
+            return
 
         start_dt = datetime.fromtimestamp(int(start) / 1e3, timezone.utc)
         end_dt = datetime.fromtimestamp(int(end) / 1e3, timezone.utc)
         interval_window = IntervalWindow(start=start_dt, end=end_dt)
 
         datum_iterator = datum_generator(request_iterator=request_iterator)
 
@@ -203,17 +221,22 @@
         # task disappearing mid-execution.
         self.background_tasks.add(response_task)
         response_task.add_done_callback(lambda t: self.background_tasks.remove(t))
 
         await response_task
         results_futures = response_task.result()
 
-        for fut in results_futures:
-            await fut
-            yield udfunction_pb2.DatumResponseList(elements=fut.result())
+        try:
+            for fut in results_futures:
+                await fut
+                yield udfunction_pb2.DatumResponseList(elements=fut.result())
+        except Exception as e:
+            context.set_code(grpc.StatusCode.UNKNOWN)
+            context.set_details(e.__str__())
+            yield udfunction_pb2.DatumResponseList(elements=[])
 
     async def __async_reduce_handler(self, interval_window, datum_iterator: AsyncIterable[Datum]):
         callable_dict = {}
         # iterate through all the values
         async for d in datum_iterator:
             keys = d.keys()
             unified_key = DELIMITER.join(keys)
@@ -281,14 +304,20 @@
                 reduce_handler=self.__reduce_handler,
             ),
             server,
         )
         server.add_insecure_port(self.sock_path)
         _LOGGER.info("GRPC Async Server listening on: %s", self.sock_path)
         await server.start()
+        serv_info = ServerInfo(
+            protocol=Protocol.UDS,
+            language=Language.PYTHON,
+            version=get_sdk_version(),
+        )
+        info_server_write(server_info=serv_info, info_file=SERVER_INFO_FILE_PATH)
 
         async def server_graceful_shutdown():
             """
             Shuts down the server with 5 seconds of grace period. During the
             grace period, the server won't accept new connections and allow
             existing RPCs to continue within the grace period.
             """
```

### Comparing `pynumaflow-0.4.0/pynumaflow/function/asynciter.py` & `pynumaflow-0.4.1/pynumaflow/function/asynciter.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/function/multiproc_server.py` & `pynumaflow-0.4.1/pynumaflow/function/multiproc_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,24 +17,34 @@
 from pynumaflow._constants import MULTIPROC_FUNCTION_SOCK_PORT, MULTIPROC_FUNCTION_SOCK_ADDR
 from pynumaflow.exceptions import SocketError
 from pynumaflow.function import Messages, MessageTs, Datum, Metadata
 from pynumaflow.function._dtypes import DatumMetadata
 from pynumaflow.function.proto import udfunction_pb2
 from pynumaflow.function.proto import udfunction_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
+from pynumaflow.info.server import (
+    get_sdk_version,
+    write as info_server_write,
+    get_metadata_env,
+)
+from pynumaflow.info.types import (
+    ServerInfo,
+    Protocol,
+    Language,
+    SERVER_INFO_FILE_PATH,
+    METADATA_ENVS,
+)
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
 UDFMapCallable = Callable[[List[str], Datum], Messages]
 UDFMapTCallable = Callable[[List[str], Datum], MessageTs]
 UDFReduceCallable = Callable[[List[str], AsyncIterable[Datum], Metadata], Messages]
-_PROCESS_COUNT = int(os.getenv("NUM_CPU_MULTIPROC", multiprocessing.cpu_count()))
-MAX_THREADS = int(os.getenv("MAX_THREADS", 0)) or (_PROCESS_COUNT * 4)
 
 
 class MultiProcServer(udfunction_pb2_grpc.UserDefinedFunctionServicer):
     """
     Provides an interface to write a User Defined Function (UDFunction)
     which will be exposed over gRPC.
 
@@ -80,39 +90,39 @@
     def __init__(
         self,
         map_handler: UDFMapCallable = None,
         mapt_handler: UDFMapTCallable = None,
         reduce_handler: UDFReduceCallable = None,
         sock_path=MULTIPROC_FUNCTION_SOCK_PORT,
         max_message_size=MAX_MESSAGE_SIZE,
-        max_threads=MAX_THREADS,
     ):
         if not (map_handler or mapt_handler or reduce_handler):
             raise ValueError("Require a valid map/mapt handler and/or a valid reduce handler.")
 
         self.__map_handler: UDFMapCallable = map_handler
         self.__mapt_handler: UDFMapTCallable = mapt_handler
         self.__reduce_handler: UDFReduceCallable = reduce_handler
         self._max_message_size = max_message_size
-        self._max_threads = max_threads
         self.cleanup_coroutines = []
         # Collection for storing strong references to all running tasks.
         # Event loop only keeps a weak reference, which can cause it to
         # get lost during execution.
         self.background_tasks = set()
 
         self._server_options = [
             ("grpc.max_send_message_length", self._max_message_size),
             ("grpc.max_receive_message_length", self._max_message_size),
             ("grpc.so_reuseport", 1),
             ("grpc.so_reuseaddr", 1),
         ]
         self._sock_path = sock_path
-        self._process_count = int(os.getenv("NUM_CPU_MULTIPROC", multiprocessing.cpu_count()))
-        self._thread_concurrency = MAX_THREADS
+        self._process_count = int(
+            os.getenv("NUM_CPU_MULTIPROC") or os.getenv("NUMAFLOW_CPU_LIMIT", 1)
+        )
+        self._thread_concurrency = int(os.getenv("MAX_THREADS", 0)) or (self._process_count * 4)
 
     def MapFn(
         self, request: udfunction_pb2.DatumRequest, context: NumaflowServicerContext
     ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a function to each datum element.
         The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
@@ -131,15 +141,17 @@
                         msg_id=request.metadata.id,
                         num_delivered=request.metadata.num_delivered,
                     ),
                 ),
             )
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
-            raise err
+            context.set_code(grpc.StatusCode.UNKNOWN)
+            context.set_details(str(err))
+            return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
 
         for msg in msgs.items():
             datums.append(
                 udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
@@ -168,15 +180,17 @@
                         msg_id=request.metadata.id,
                         num_delivered=request.metadata.num_delivered,
                     ),
                 ),
             )
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
-            raise err
+            context.set_code(grpc.StatusCode.UNKNOWN)
+            context.set_details(str(err))
+            return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
         for msgt in msgts.items():
             event_time_timestamp = _timestamp_pb2.Timestamp()
             event_time_timestamp.FromDatetime(dt=msgt.event_time)
             watermark_timestamp = _timestamp_pb2.Timestamp()
             watermark_timestamp.FromDatetime(dt=request.watermark.watermark.ToDatetime())
@@ -187,14 +201,27 @@
                     tags=msgt.tags,
                     event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
                     watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
                 )
             )
         return udfunction_pb2.DatumResponseList(elements=datums)
 
+    def ReduceFn(
+        self,
+        request_iterator: AsyncIterable[udfunction_pb2.DatumRequest],
+        context: NumaflowServicerContext,
+    ) -> udfunction_pb2.DatumResponseList:
+        """
+        This method is not implemented because we multiplex different keys
+        on to a single stream and reduce requires a persistent connection.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        yield from ()
+
     def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> udfunction_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
         """
@@ -208,14 +235,24 @@
                 max_workers=self._thread_concurrency,
             ),
             options=self._server_options,
         )
         udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(self, server)
         server.add_insecure_port(bind_address)
         server.start()
+        serv_info = ServerInfo(
+            protocol=Protocol.TCP,
+            language=Language.PYTHON,
+            version=get_sdk_version(),
+            metadata=get_metadata_env(envs=METADATA_ENVS),
+        )
+        # Overwrite the CPU_LIMIT metadata using user input
+        serv_info.metadata["CPU_LIMIT"] = str(self._process_count)
+        info_server_write(server_info=serv_info, info_file=SERVER_INFO_FILE_PATH)
+
         _LOGGER.info("GRPC Multi-Processor Server listening on: %s %d", bind_address, os.getpid())
         server.wait_for_termination()
 
     @contextlib.contextmanager
     def _reserve_port(self) -> int:
         """Find and reserve a port for all subprocesses to use."""
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
```

### Comparing `pynumaflow-0.4.0/pynumaflow/function/proto/udfunction.proto` & `pynumaflow-0.4.1/pynumaflow/function/proto/udfunction.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2.py` & `pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x10udfunction.proto\x12\x0b\x66unction.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto";\n\tEventTime\x12.\n\nevent_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp":\n\tWatermark\x12-\n\twatermark\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"-\n\x08Metadata\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rnum_delivered\x18\x02 \x01(\x04"\xab\x01\n\x0c\x44\x61tumRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12*\n\nevent_time\x18\x03 \x01(\x0b\x32\x16.function.v1.EventTime\x12)\n\twatermark\x18\x04 \x01(\x0b\x32\x16.function.v1.Watermark\x12\'\n\x08metadata\x18\x05 \x01(\x0b\x32\x15.function.v1.Metadata"\x91\x01\n\rDatumResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12*\n\nevent_time\x18\x03 \x01(\x0b\x32\x16.function.v1.EventTime\x12)\n\twatermark\x18\x04 \x01(\x0b\x32\x16.function.v1.Watermark\x12\x0c\n\x04tags\x18\x05 \x03(\t"A\n\x11\x44\x61tumResponseList\x12,\n\x08\x65lements\x18\x01 \x03(\x0b\x32\x1a.function.v1.DatumResponse"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\x32\xa8\x02\n\x13UserDefinedFunction\x12\x42\n\x05MapFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList\x12\x43\n\x06MapTFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList\x12I\n\x08ReduceFn\x12\x19.function.v1.DatumRequest\x1a\x1e.function.v1.DatumResponseList(\x01\x30\x01\x12=\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x1a.function.v1.ReadyResponseb\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "udfunction_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
+
     DESCRIPTOR._options = None
     _EVENTTIME._serialized_start = 95
     _EVENTTIME._serialized_end = 154
     _WATERMARK._serialized_start = 156
     _WATERMARK._serialized_end = 214
     _METADATA._serialized_start = 216
     _METADATA._serialized_end = 261
```

### Comparing `pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2_grpc.py` & `pynumaflow-0.4.1/pynumaflow/function/proto/udfunction_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class UserDefinedFunctionStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
+
         Args:
             channel: A grpc.Channel.
         """
         self.MapFn = channel.unary_unary(
             "/function.v1.UserDefinedFunction/MapFn",
             request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
             response_deserializer=udfunction__pb2.DatumResponseList.FromString,
```

### Comparing `pynumaflow-0.4.0/pynumaflow/function/server.py` & `pynumaflow-0.4.1/pynumaflow/function/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 from concurrent.futures import ThreadPoolExecutor
 from typing import Callable, AsyncIterable, List
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from pynumaflow.info.server import get_sdk_version, write as info_server_write
+from pynumaflow.info.types import ServerInfo, Protocol, Language, SERVER_INFO_FILE_PATH
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     FUNCTION_SOCK_PATH,
     MAX_MESSAGE_SIZE,
 )
 from pynumaflow.function import Messages, MessageTs, Datum, Metadata
@@ -123,15 +125,17 @@
                         msg_id=request.metadata.id,
                         num_delivered=request.metadata.num_delivered,
                     ),
                 ),
             )
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
-            raise err
+            context.set_code(grpc.StatusCode.UNKNOWN)
+            context.set_details(str(err))
+            return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
 
         for msg in msgs.items():
             datums.append(
                 udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
@@ -160,15 +164,17 @@
                         msg_id=request.metadata.id,
                         num_delivered=request.metadata.num_delivered,
                     ),
                 ),
             )
         except Exception as err:
             _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
-            raise err
+            context.set_code(grpc.StatusCode.UNKNOWN)
+            context.set_details(str(err))
+            return udfunction_pb2.DatumResponseList(elements=[])
 
         datums = []
         for msgt in msgts.items():
             event_time_timestamp = _timestamp_pb2.Timestamp()
             event_time_timestamp.FromDatetime(dt=msgt.event_time)
             watermark_timestamp = _timestamp_pb2.Timestamp()
             watermark_timestamp.FromDatetime(dt=request.watermark.watermark.ToDatetime())
@@ -179,14 +185,27 @@
                     tags=msgt.tags,
                     event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
                     watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
                 )
             )
         return udfunction_pb2.DatumResponseList(elements=datums)
 
+    def ReduceFn(
+        self,
+        request_iterator: AsyncIterable[udfunction_pb2.DatumRequest],
+        context: NumaflowServicerContext,
+    ) -> udfunction_pb2.DatumResponseList:
+        """
+        This method is not implemented because we multiplex different keys
+        on to a single stream and reduce requires a persistent connection.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        yield from ()
+
     def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> udfunction_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
         """
@@ -198,11 +217,17 @@
         """
         server = grpc.server(
             ThreadPoolExecutor(max_workers=self._max_threads), options=self._server_options
         )
         udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(self, server)
         server.add_insecure_port(self.sock_path)
         server.start()
+        serv_info = ServerInfo(
+            protocol=Protocol.UDS,
+            language=Language.PYTHON,
+            version=get_sdk_version(),
+        )
+        info_server_write(server_info=serv_info, info_file=SERVER_INFO_FILE_PATH)
         _LOGGER.info(
             "GRPC Server listening on: %s with max threads: %s", self.sock_path, self._max_threads
         )
         server.wait_for_termination()
```

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/_dtypes.py` & `pynumaflow-0.4.1/pynumaflow/sink/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/_udfunction_pb2.pyi` & `pynumaflow-0.4.1/pynumaflow/sink/_udfunction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/async_sink.py` & `pynumaflow-0.4.1/pynumaflow/sink/async_sink.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     SINK_SOCK_PATH,
     MAX_MESSAGE_SIZE,
 )
+from pynumaflow.info.server import get_sdk_version, write as info_server_write
+from pynumaflow.info.types import ServerInfo, Protocol, Language, SERVER_INFO_FILE_PATH
 from pynumaflow.sink import Responses, Datum, Response
 from pynumaflow.sink.proto import udsink_pb2_grpc, udsink_pb2
 from pynumaflow.types import NumaflowServicerContext
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
@@ -124,14 +126,20 @@
     async def __serve_async(self, server) -> None:
         udsink_pb2_grpc.add_UserDefinedSinkServicer_to_server(
             AsyncSink(self.__sink_handler), server
         )
         server.add_insecure_port(self.sock_path)
         _LOGGER.info("GRPC Async Server listening on: %s", self.sock_path)
         await server.start()
+        serv_info = ServerInfo(
+            protocol=Protocol.UDS,
+            language=Language.PYTHON,
+            version=get_sdk_version(),
+        )
+        info_server_write(server_info=serv_info, info_file=SERVER_INFO_FILE_PATH)
 
         async def server_graceful_shutdown():
             _LOGGER.info("Starting graceful shutdown...")
             """
             Shuts down the server with 5 seconds of grace period. During the
             grace period, the server won't accept new connections and allow
             existing RPCs to continue within the grace period.
```

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/proto/udsink.proto` & `pynumaflow-0.4.1/pynumaflow/sink/proto/udsink.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2.py` & `pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
     b'\n\x0cudsink.proto\x12\x07sink.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto";\n\tEventTime\x12.\n\nevent_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp":\n\tWatermark\x12-\n\twatermark\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\x86\x01\n\x0c\x44\x61tumRequest\x12\x0c\n\x04keys\x18\x01 \x03(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\x12&\n\nevent_time\x18\x03 \x01(\x0b\x32\x12.sink.v1.EventTime\x12%\n\twatermark\x18\x04 \x01(\x0b\x32\x12.sink.v1.Watermark\x12\n\n\x02id\x18\x05 \x01(\t"\x1e\n\rReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08"8\n\x08Response\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x0f\n\x07\x65rr_msg\x18\x03 \x01(\t"4\n\x0cResponseList\x12$\n\tresponses\x18\x01 \x03(\x0b\x32\x11.sink.v1.Response2\x86\x01\n\x0fUserDefinedSink\x12\x38\n\x06SinkFn\x12\x15.sink.v1.DatumRequest\x1a\x15.sink.v1.ResponseList(\x01\x12\x39\n\x07IsReady\x12\x16.google.protobuf.Empty\x1a\x16.sink.v1.ReadyResponseb\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "udsink_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
+
     DESCRIPTOR._options = None
     _EVENTTIME._serialized_start = 87
     _EVENTTIME._serialized_end = 146
     _WATERMARK._serialized_start = 148
     _WATERMARK._serialized_end = 206
     _DATUMREQUEST._serialized_start = 209
     _DATUMREQUEST._serialized_end = 343
```

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2_grpc.py` & `pynumaflow-0.4.1/pynumaflow/sink/proto/udsink_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class UserDefinedSinkStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
+
         Args:
             channel: A grpc.Channel.
         """
         self.SinkFn = channel.stream_unary(
             "/sink.v1.UserDefinedSink/SinkFn",
             request_serializer=udsink__pb2.DatumRequest.SerializeToString,
             response_deserializer=udsink__pb2.ResponseList.FromString,
```

### Comparing `pynumaflow-0.4.0/pynumaflow/sink/server.py` & `pynumaflow-0.4.1/pynumaflow/sink/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     SINK_SOCK_PATH,
     MAX_MESSAGE_SIZE,
 )
+from pynumaflow.info.server import get_sdk_version, write as info_server_write
+from pynumaflow.info.types import ServerInfo, Protocol, Language, SERVER_INFO_FILE_PATH
 from pynumaflow.sink import Responses, Datum, Response
 from pynumaflow.sink.proto import udsink_pb2_grpc, udsink_pb2
 from pynumaflow.types import NumaflowServicerContext
 
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
@@ -120,11 +122,18 @@
         """
         server = grpc.server(
             ThreadPoolExecutor(max_workers=self._max_threads), options=self._server_options
         )
         udsink_pb2_grpc.add_UserDefinedSinkServicer_to_server(Sink(self.__sink_handler), server)
         server.add_insecure_port(self.sock_path)
         server.start()
+        serv_info = ServerInfo(
+            protocol=Protocol.UDS,
+            language=Language.PYTHON,
+            version=get_sdk_version(),
+        )
+        info_server_write(server_info=serv_info, info_file=SERVER_INFO_FILE_PATH)
+
         _LOGGER.info(
             "GRPC Server listening on: %s with max threads: %s", self.sock_path, self._max_threads
         )
         server.wait_for_termination()
```

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/server_utils.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/testing_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import json
 from datetime import datetime, timezone
 from typing import Iterator, List
 
 from pynumaflow.function import (
     Message,
     Messages,
     MessageT,
     MessageTs,
     Datum,
     Metadata,
 )
+from pynumaflow.info.types import EOF
 
 
 def map_handler(keys: List[str], datum: Datum) -> Messages:
     val = datum.value
     msg = "payload:%s event_time:%s watermark:%s" % (
         val.decode("utf-8"),
         datum.event_time,
@@ -79,7 +81,35 @@
 
 def mock_interval_window_start():
     return 1662998400000
 
 
 def mock_interval_window_end():
     return 1662998460000
+
+
+def read_info_server(info_file: str):
+    f = open(info_file, "r")
+    retry = 10
+    res = f.read()
+    a, b = info_serv_is_ready(info_serv_data=res)
+    while (a is not True) and retry > 0:
+        a, b = info_serv_is_ready(info_serv_data=res)
+
+    a, b = info_serv_is_ready(info_serv_data=res)
+    if a:
+        res = json.loads(b)
+        return res
+
+    else:
+        return None
+
+
+def info_serv_is_ready(info_serv_data: str, eof: str = EOF):
+    if len(info_serv_data) < len(eof):
+        return False
+    len_diff = len(info_serv_data) - len(eof)
+    last_char = info_serv_data[len_diff:]
+    if last_char == EOF:
+        data = info_serv_data[:len_diff]
+        return True, data
+    return False, None
```

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_async_server.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_async_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,39 +17,48 @@
     Datum,
     AsyncServer,
     MessageTs,
     MessageT,
     Metadata,
 )
 from pynumaflow.function.proto import udfunction_pb2, udfunction_pb2_grpc
-from pynumaflow.tests.function.server_utils import (
+from pynumaflow.tests.function.testing_utils import (
     mock_event_time,
     mock_watermark,
     mock_message,
     mock_interval_window_start,
     mock_interval_window_end,
     mock_new_event_time,
 )
 
 LOGGER = setup_logging(__name__)
 
+# if set to true, map handler will raise a `ValueError` exception.
+raise_error_from_map = False
+
 
 async def async_map_handler(keys: List[str], datum: Datum) -> Messages:
+    if raise_error_from_map:
+        raise ValueError("Exception thrown from map")
     val = datum.value
     msg = "payload:%s event_time:%s watermark:%s" % (
         val.decode("utf-8"),
         datum.event_time,
         datum.watermark,
     )
     val = bytes(msg, encoding="utf-8")
     messages = Messages()
     messages.append(Message(str.encode(msg), keys=keys))
     return messages
 
 
+async def async_map_error_fn(keys: List[str], datum: Datum) -> Messages:
+    raise ValueError("error invoking map")
+
+
 async def async_mapt_handler(keys: List[str], datum: Datum) -> MessageTs:
     val = datum.value
     msg = "payload:%s event_time:%s watermark:%s" % (
         val.decode("utf-8"),
         datum.event_time,
         datum.watermark,
     )
@@ -106,21 +115,30 @@
 
 
 def startup_callable(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
 
-async def start_server():
-    server = grpc.aio.server()
+def NewAsyncServer(
+    map_handler=async_map_handler,
+    mapt_handler=async_mapt_handler,
+    reduce_handler=async_reduce_handler,
+):
     udfs = AsyncServer(
-        reduce_handler=async_reduce_handler,
-        map_handler=async_map_handler,
-        mapt_handler=async_mapt_handler,
+        reduce_handler=reduce_handler,
+        map_handler=map_handler,
+        mapt_handler=mapt_handler,
     )
+
+    return udfs
+
+
+async def start_server(udfs: AsyncServer):
+    server = grpc.aio.server()
     udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(udfs, server)
     listen_addr = "[::]:50051"
     server.add_insecure_port(listen_addr)
     logging.info("Starting server on %s", listen_addr)
     global _s
     _s = server
     await server.start()
@@ -131,15 +149,16 @@
     @classmethod
     def setUpClass(cls) -> None:
         global _loop
         loop = asyncio.new_event_loop()
         _loop = loop
         _thread = threading.Thread(target=startup_callable, args=(loop,), daemon=True)
         _thread.start()
-        asyncio.run_coroutine_threadsafe(start_server(), loop=loop)
+        udfs = NewAsyncServer()
+        asyncio.run_coroutine_threadsafe(start_server(udfs), loop=loop)
         while True:
             try:
                 with grpc.insecure_channel("localhost:50051") as channel:
                     f = grpc.channel_ready_future(channel)
                     f.result(timeout=10)
                     if f.done():
                         break
@@ -218,32 +237,93 @@
                 "payload:test_mock_message "
                 "event_time:2022-09-12 16:00:00 watermark:2022-09-12 16:01:00",
                 encoding="utf-8",
             ),
             response.elements[0].value,
         )
 
+    def test_map_grpc_error(self) -> None:
+        stub = udfunction_pb2_grpc.UserDefinedFunctionStub(_channel)
+        event_time_timestamp = _timestamp_pb2.Timestamp()
+        event_time_timestamp.FromDatetime(dt=mock_event_time())
+        watermark_timestamp = _timestamp_pb2.Timestamp()
+        watermark_timestamp.FromDatetime(dt=mock_watermark())
+
+        request = udfunction_pb2.DatumRequest(
+            keys=["test"],
+            value=mock_message(),
+            event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
+            watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
+        )
+
+        metadata = (("this_metadata_will_be_skipped", "test_ignore"),)
+
+        grpcException = None
+
+        try:
+            global raise_error_from_map
+            raise_error_from_map = True
+            _ = stub.MapFn(request=request, metadata=metadata)
+        except grpc.RpcError as e:
+            grpcException = e
+            self.assertEqual(grpc.StatusCode.UNKNOWN, e.code())
+            print(e.details())
+
+        finally:
+            raise_error_from_map = False
+
+        self.assertIsNotNone(grpcException)
+
+    def test_unimplemented_mapt(self) -> None:
+        stub = udfunction_pb2_grpc.UserDefinedFunctionStub(_channel)
+        event_time_timestamp = _timestamp_pb2.Timestamp()
+        event_time_timestamp.FromDatetime(dt=mock_event_time())
+        watermark_timestamp = _timestamp_pb2.Timestamp()
+        watermark_timestamp.FromDatetime(dt=mock_watermark())
+
+        request = udfunction_pb2.DatumRequest(
+            keys=["test"],
+            value=mock_message(),
+            event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
+            watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
+        )
+
+        metadata = (("this_metadata_will_be_skipped", "test_ignore"),)
+        grpcException = None
+        try:
+            _ = stub.MapTFn(request=request, metadata=metadata)
+        except grpc.RpcError as e:
+            grpcException = e
+            self.assertEqual(grpc.StatusCode.UNIMPLEMENTED, e.code())
+            self.assertEqual("Method not implemented!", e.details())
+
+        self.assertIsNotNone(grpcException)
+
     def test_reduce_invalid_metadata(self) -> None:
         stub = self.__stub()
         request, metadata = start_reduce_streaming_request()
         invalid_metadata = {}
         try:
             generator_response = stub.ReduceFn(
                 request_iterator=request_generator(count=10, request=request),
                 metadata=invalid_metadata,
             )
             count = 0
             for _ in generator_response:
                 count += 1
-        except Exception as err:
-            self.assertTrue(
-                "Expected to have all key/window_start_time/window_end_time" in err.__str__()
+        except grpc.RpcError as e:
+            self.assertEqual(grpc.StatusCode.INVALID_ARGUMENT, e.code())
+            self.assertEqual(
+                "Expected to have all key/window_start_time/window_end_time;"
+                " got start: None, end: None.",
+                e.details(),
             )
-            return
-        self.fail("Expected an exception.")
+        except Exception as err:
+            self.fail("Expected an exception.")
+            logging.error(err)
 
     def test_reduce(self) -> None:
         stub = self.__stub()
         request, metadata = start_reduce_streaming_request()
         generator_response = None
         try:
             generator_response = stub.ReduceFn(
```

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_async_server_err.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_async_server_err.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from grpc.aio._server import Server
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import WIN_START_TIME, WIN_END_TIME
 from pynumaflow.function import Messages, Message, Datum, Metadata, AsyncServer
 from pynumaflow.function.proto import udfunction_pb2, udfunction_pb2_grpc
-from pynumaflow.tests.function.server_utils import (
+from pynumaflow.tests.function.testing_utils import (
     mapt_handler,
     map_handler,
     mock_event_time,
     mock_watermark,
     mock_message,
     mock_interval_window_start,
     mock_interval_window_end,
@@ -29,15 +29,15 @@
 async def err_async_reduce_handler(
     key: str, datums: AsyncIterable[Datum], md: Metadata
 ) -> Messages:
     interval_window = md.interval_window
     counter = 0
     async for _ in datums:
         counter += 1
-        raise RuntimeError("Got a runtime error from reduce handler.")
+        raise ValueError("Got a runtime error from reduce handler.")
 
     msg = (
         f"counter:{counter} interval_window_start:{interval_window.start} "
         f"interval_window_end:{interval_window.end}"
     )
 
     return Messages(Message.to_vtx(key, str.encode(msg)))
@@ -130,17 +130,19 @@
         try:
             generator_response = stub.ReduceFn(
                 request_iterator=request_generator(count=10, request=request), metadata=metadata
             )
             count = 0
             for _ in generator_response:
                 count += 1
-        except Exception as err:
-            self.assertTrue("Got a runtime error from reduce handler." in err.__str__())
+        except grpc.RpcError as e:
+            self.assertEqual(e.code(), grpc.StatusCode.UNKNOWN)
+            self.assertEqual(e.details(), "Got a runtime error from reduce handler.")
             return
+
         self.fail("Expected an exception.")
 
     def __stub(self):
         return udfunction_pb2_grpc.UserDefinedFunctionStub(_channel)
 
     def test_invalid_input(self):
         with self.assertRaises(ValueError):
```

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_datatypes.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_messages.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_messages.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_messagets.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_messagets.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_multiproc.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_multiproc.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from grpc import StatusCode
 from grpc_testing import server_from_dictionary, strict_real_time
 
 from pynumaflow.function.multiproc_server import MultiProcServer
 from pynumaflow.function.proto import udfunction_pb2_grpc, udfunction_pb2
-from pynumaflow.tests.function.server_utils import (
+from pynumaflow.tests.function.testing_utils import (
     mapt_handler,
     map_handler,
     err_map_handler,
     mock_event_time,
     mock_watermark,
     mock_message,
     mock_new_event_time,
@@ -39,14 +39,22 @@
     def test_multiproc_init(self) -> None:
         server = MultiProcServer(
             reduce_handler=async_reduce_handler, map_handler=map_handler, mapt_handler=mapt_handler
         )
         self.assertEqual(server._sock_path, 55551)
         self.assertEqual(server._process_count, 3)
 
+    @mockenv(NUMAFLOW_CPU_LIMIT="4")
+    def test_multiproc_process_count(self) -> None:
+        server = MultiProcServer(
+            reduce_handler=async_reduce_handler, map_handler=map_handler, mapt_handler=mapt_handler
+        )
+        self.assertEqual(server._sock_path, 55551)
+        self.assertEqual(server._process_count, 4)
+
     # To test the reuse property for the grpc servers which allow multiple
     # bindings to the same server
     def test_reuse_port(self):
         serv_options = [("grpc.so_reuseport", 1), ("grpc.so_reuseaddr", 1)]
 
         server = MultiProcServer(
             reduce_handler=async_reduce_handler, map_handler=map_handler, mapt_handler=mapt_handler
@@ -94,15 +102,15 @@
             invocation_metadata={
                 ("this_metadata_will_be_skipped", "test_ignore"),
             },
             request=request,
             timeout=1,
         )
         response, metadata, code, details = method.termination()
-        self.assertEqual(None, response)
+        self.assertEqual(grpc.StatusCode.UNKNOWN, code)
 
     def test_udf_mapt_err(self):
         my_servicer = MultiProcServer(mapt_handler=err_mapt_handler)
         services = {udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"]: my_servicer}
         self.test_server = server_from_dictionary(services, strict_real_time())
 
         event_time_timestamp = _timestamp_pb2.Timestamp()
@@ -125,15 +133,15 @@
             invocation_metadata={
                 ("this_metadata_will_be_skipped", "test_ignore"),
             },
             request=request,
             timeout=1,
         )
         response, metadata, code, details = method.termination()
-        self.assertEqual(None, response)
+        self.assertEqual(grpc.StatusCode.UNKNOWN, code)
 
     def test_is_ready(self):
         method = self.test_server.invoke_unary_unary(
             method_descriptor=(
                 udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
                     "IsReady"
                 ]
@@ -236,10 +244,28 @@
         )
         self.assertEqual(code, StatusCode.OK)
 
     def test_invalid_input(self):
         with self.assertRaises(ValueError):
             MultiProcServer()
 
+    def test_unimplemented_reduce(self):
+        method = self.test_server.invoke_stream_stream(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "ReduceFn"
+                ]
+            ),
+            invocation_metadata={
+                ("this_metadata_will_be_skipped", "test_ignore"),
+            },
+            timeout=1,
+        )
+
+        metadata, code, details = method.termination()
+
+        self.assertEqual(grpc.StatusCode.UNIMPLEMENTED, code)
+        self.assertEqual("Method not implemented!", details)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/function/test_sync_server.py` & `pynumaflow-0.4.1/pynumaflow/tests/function/test_sync_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import unittest
 
+import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from grpc import StatusCode
 from grpc_testing import server_from_dictionary, strict_real_time
 
 from pynumaflow.function import Server
 from pynumaflow.function.proto import udfunction_pb2
-from pynumaflow.tests.function.server_utils import (
+from pynumaflow.tests.function.testing_utils import (
     mapt_handler,
     map_handler,
     reduce_handler,
     err_map_handler,
     mock_event_time,
     mock_watermark,
     mock_message,
@@ -64,15 +65,46 @@
             invocation_metadata={
                 ("this_metadata_will_be_skipped", "test_ignore"),
             },
             request=request,
             timeout=1,
         )
         response, metadata, code, details = method.termination()
-        self.assertEqual(None, response)
+        self.assertEqual(grpc.StatusCode.UNKNOWN, code)
+
+    def test_udf_map_error_response(self):
+        my_servicer = Server(map_handler=err_map_handler)
+        services = {udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"]: my_servicer}
+        self.test_server = server_from_dictionary(services, strict_real_time())
+
+        event_time_timestamp = _timestamp_pb2.Timestamp()
+        event_time_timestamp.FromDatetime(dt=mock_event_time())
+        watermark_timestamp = _timestamp_pb2.Timestamp()
+        watermark_timestamp.FromDatetime(dt=mock_watermark())
+
+        request = udfunction_pb2.DatumRequest(
+            value=mock_message(),
+            event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
+            watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
+        )
+
+        method = self.test_server.invoke_unary_unary(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "MapFn"
+                ]
+            ),
+            invocation_metadata={
+                ("this_metadata_will_be_skipped", "test_ignore"),
+            },
+            request=request,
+            timeout=1,
+        )
+        response, metadata, code, details = method.termination()
+        self.assertEqual(grpc.StatusCode.UNKNOWN, code)
 
     def test_udf_mapt_err(self):
         my_servicer = Server(mapt_handler=err_mapt_handler)
         services = {udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"]: my_servicer}
         self.test_server = server_from_dictionary(services, strict_real_time())
 
         event_time_timestamp = _timestamp_pb2.Timestamp()
@@ -95,15 +127,33 @@
             invocation_metadata={
                 ("this_metadata_will_be_skipped", "test_ignore"),
             },
             request=request,
             timeout=1,
         )
         response, metadata, code, details = method.termination()
-        self.assertEqual(None, response)
+        self.assertEqual(grpc.StatusCode.UNKNOWN, code)
+
+    def test_unimplemented_reduce(self):
+        method = self.test_server.invoke_stream_stream(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "ReduceFn"
+                ]
+            ),
+            invocation_metadata={
+                ("this_metadata_will_be_skipped", "test_ignore"),
+            },
+            timeout=1,
+        )
+
+        metadata, code, details = method.termination()
+
+        self.assertEqual(grpc.StatusCode.UNIMPLEMENTED, code)
+        self.assertEqual("Method not implemented!", details)
 
     def test_is_ready(self):
         method = self.test_server.invoke_unary_unary(
             method_descriptor=(
                 udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
                     "IsReady"
                 ]
```

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/sink/test_async_sink.py` & `pynumaflow-0.4.1/pynumaflow/tests/sink/test_async_sink.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/sink/test_datatypes.py` & `pynumaflow-0.4.1/pynumaflow/tests/sink/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/sink/test_responses.py` & `pynumaflow-0.4.1/pynumaflow/tests/sink/test_responses.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pynumaflow/tests/sink/test_server.py` & `pynumaflow-0.4.1/pynumaflow/tests/sink/test_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.4.0/pyproject.toml` & `pynumaflow-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynumaflow"
-version = "0.4.0"
+version = "0.4.1"
 description = "Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow."
 authors = ["NumaFlow Developers"]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Vigith Maurice <vigith@gmail.com>",
```

### Comparing `pynumaflow-0.4.0/PKG-INFO` & `pynumaflow-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumaflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow.
 Home-page: https://github.com/numaproj/numaflow-python
 License: Apache-2.0
 Author: NumaFlow Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

