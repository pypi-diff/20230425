# Comparing `tmp/fern_metriport-0.0.2.tar.gz` & `tmp/fern_metriport-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_metriport-0.0.2.tar", max compression
+gzip compressed data, was "fern_metriport-0.0.3.tar", max compression
```

## Comparing `fern_metriport-0.0.2.tar` & `fern_metriport-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      420 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/__init__.py
--rw-r--r--   0        0        0      796 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/client.py
--rw-r--r--   0        0        0      348 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/core/__init__.py
--rw-r--r--   0        0        0      426 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/core/remove_none_from_headers.py
--rw-r--r--   0        0        0        0 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/py.typed
--rw-r--r--   0        0        0      469 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/__init__.py
--rw-r--r--   0        0        0      427 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/__init__.py
--rw-r--r--   0        0        0     5906 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/client.py
--rw-r--r--   0        0        0      589 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/__init__.py
--rw-r--r--   0        0        0      844 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/codeable_concept.py
--rw-r--r--   0        0        0      826 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/coding.py
--rw-r--r--   0        0        0     1226 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/document.py
--rw-r--r--   0        0        0      759 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/download_document_response.py
--rw-r--r--   0        0        0      962 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/get_documents_response.py
--rw-r--r--   0        0        0      492 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/query_status.py
--rw-r--r--   0        0        0      903 2023-04-25 02:32:05.933605 fern_metriport-0.0.2/src/metriport/resources/document/types/trigger_documents_query_response.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 fern_metriport-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/__init__.py
+-rw-r--r--   0        0        0      929 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/client.py
+-rw-r--r--   0        0        0      348 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      210 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/environment.py
+-rw-r--r--   0        0        0        0 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/py.typed
+-rw-r--r--   0        0        0      469 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/__init__.py
+-rw-r--r--   0        0        0     6077 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/client.py
+-rw-r--r--   0        0        0      589 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/codeable_concept.py
+-rw-r--r--   0        0        0      826 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/coding.py
+-rw-r--r--   0        0        0     1226 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/document.py
+-rw-r--r--   0        0        0      759 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/download_document_response.py
+-rw-r--r--   0        0        0      962 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/get_documents_response.py
+-rw-r--r--   0        0        0      492 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/query_status.py
+-rw-r--r--   0        0        0      903 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/trigger_documents_query_response.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 fern_metriport-0.0.3/PKG-INFO
```

### Comparing `fern_metriport-0.0.2/src/metriport/client.py` & `fern_metriport-0.0.3/src/metriport/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from backports.cached_property import cached_property
 
+from .environment import MercoaEnvironment
 from .resources.document.client import AsyncDocumentClient, DocumentClient
 
 
 class Mercoa:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     @cached_property
     def document(self) -> DocumentClient:
         return DocumentClient(environment=self._environment, api_key=self.api_key)
 
 
 class AsyncMercoa:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     @cached_property
     def document(self) -> AsyncDocumentClient:
         return AsyncDocumentClient(environment=self._environment, api_key=self.api_key)
```

### Comparing `fern_metriport-0.0.2/src/metriport/core/datetime_utils.py` & `fern_metriport-0.0.3/src/metriport/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/core/jsonable_encoder.py` & `fern_metriport-0.0.3/src/metriport/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/client.py` & `fern_metriport-0.0.3/src/metriport/resources/document/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,84 +5,85 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import MercoaEnvironment
 from .types.download_document_response import DownloadDocumentResponse
 from .types.get_documents_response import GetDocumentsResponse
 from .types.trigger_documents_query_response import TriggerDocumentsQueryResponse
 
 
 class DocumentClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     def get(
         self, *, patient_id: str, facility_id: str, force_query: typing.Optional[str] = None
     ) -> GetDocumentsResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "medical/v1/document"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "medical/v1/document"),
             params={"patientId": patient_id, "facilityId": facility_id, "forceQuery": force_query},
             headers=remove_none_from_headers({"X-API-Key": self.api_key}),
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetDocumentsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def trigger_query(self, *, patient_id: str, facility_id: str) -> TriggerDocumentsQueryResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "medical/v1/document/query"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "medical/v1/document/query"),
             params={"patientId": patient_id, "facilityId": facility_id},
             headers=remove_none_from_headers({"X-API-Key": self.api_key}),
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TriggerDocumentsQueryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def download(self, *, file_name: str) -> DownloadDocumentResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "medical/v1/document/downloadUrl"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "medical/v1/document/downloadUrl"),
             params={"fileName": file_name},
             headers=remove_none_from_headers({"X-API-Key": self.api_key}),
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DownloadDocumentResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncDocumentClient:
-    def __init__(self, *, environment: str, api_key: str):
+    def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
     async def get(
         self, *, patient_id: str, facility_id: str, force_query: typing.Optional[str] = None
     ) -> GetDocumentsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "medical/v1/document"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "medical/v1/document"),
                 params={"patientId": patient_id, "facilityId": facility_id, "forceQuery": force_query},
                 headers=remove_none_from_headers({"X-API-Key": self.api_key}),
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetDocumentsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -90,15 +91,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def trigger_query(self, *, patient_id: str, facility_id: str) -> TriggerDocumentsQueryResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "medical/v1/document/query"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "medical/v1/document/query"),
                 params={"patientId": patient_id, "facilityId": facility_id},
                 headers=remove_none_from_headers({"X-API-Key": self.api_key}),
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TriggerDocumentsQueryResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -106,15 +107,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def download(self, *, file_name: str) -> DownloadDocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "medical/v1/document/downloadUrl"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "medical/v1/document/downloadUrl"),
                 params={"fileName": file_name},
                 headers=remove_none_from_headers({"X-API-Key": self.api_key}),
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(DownloadDocumentResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
```

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/__init__.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/codeable_concept.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/codeable_concept.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/coding.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/coding.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/document.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/document.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/download_document_response.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/download_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/get_documents_response.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/get_documents_response.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/src/metriport/resources/document/types/trigger_documents_query_response.py` & `fern_metriport-0.0.3/src/metriport/resources/document/types/trigger_documents_query_response.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.2/PKG-INFO` & `fern_metriport-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-metriport
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

