# Comparing `tmp/fern_metriport-0.0.3.tar.gz` & `tmp/fern_metriport-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_metriport-0.0.3.tar", max compression
+gzip compressed data, was "fern_metriport-0.0.4.tar", max compression
```

## Comparing `fern_metriport-0.0.3.tar` & `fern_metriport-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      420 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      529 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/__init__.py
--rw-r--r--   0        0        0      929 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/client.py
--rw-r--r--   0        0        0      348 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/__init__.py
--rw-r--r--   0        0        0      426 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-25 02:33:21.101051 fern_metriport-0.0.3/src/metriport/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      210 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/environment.py
--rw-r--r--   0        0        0        0 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/py.typed
--rw-r--r--   0        0        0      469 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/__init__.py
--rw-r--r--   0        0        0      427 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/__init__.py
--rw-r--r--   0        0        0     6077 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/client.py
--rw-r--r--   0        0        0      589 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/__init__.py
--rw-r--r--   0        0        0      844 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/codeable_concept.py
--rw-r--r--   0        0        0      826 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/coding.py
--rw-r--r--   0        0        0     1226 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/document.py
--rw-r--r--   0        0        0      759 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/download_document_response.py
--rw-r--r--   0        0        0      962 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/get_documents_response.py
--rw-r--r--   0        0        0      492 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/query_status.py
--rw-r--r--   0        0        0      903 2023-04-25 02:33:21.105051 fern_metriport-0.0.3/src/metriport/resources/document/types/trigger_documents_query_response.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 fern_metriport-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-04-25 02:42:43.312368 fern_metriport-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      529 2023-04-25 02:42:43.312368 fern_metriport-0.0.4/src/metriport/__init__.py
+-rw-r--r--   0        0        0      929 2023-04-25 02:42:43.312368 fern_metriport-0.0.4/src/metriport/client.py
+-rw-r--r--   0        0        0      348 2023-04-25 02:42:43.312368 fern_metriport-0.0.4/src/metriport/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-04-25 02:42:43.312368 fern_metriport-0.0.4/src/metriport/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-04-25 02:42:43.312368 fern_metriport-0.0.4/src/metriport/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      210 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/environment.py
+-rw-r--r--   0        0        0        0 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/py.typed
+-rw-r--r--   0        0        0      469 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/__init__.py
+-rw-r--r--   0        0        0     6077 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/client.py
+-rw-r--r--   0        0        0      589 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/codeable_concept.py
+-rw-r--r--   0        0        0      826 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/coding.py
+-rw-r--r--   0        0        0     1226 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/document.py
+-rw-r--r--   0        0        0      759 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/download_document_response.py
+-rw-r--r--   0        0        0      962 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/get_documents_response.py
+-rw-r--r--   0        0        0      492 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/query_status.py
+-rw-r--r--   0        0        0      903 2023-04-25 02:42:43.316368 fern_metriport-0.0.4/src/metriport/resources/document/types/trigger_documents_query_response.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 fern_metriport-0.0.4/PKG-INFO
```

### Comparing `fern_metriport-0.0.3/src/metriport/__init__.py` & `fern_metriport-0.0.4/src/metriport/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/client.py` & `fern_metriport-0.0.4/src/metriport/client.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/core/datetime_utils.py` & `fern_metriport-0.0.4/src/metriport/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/core/jsonable_encoder.py` & `fern_metriport-0.0.4/src/metriport/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/client.py` & `fern_metriport-0.0.4/src/metriport/resources/document/client.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/__init__.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/codeable_concept.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/codeable_concept.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/coding.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/coding.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/document.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/document.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/download_document_response.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/download_document_response.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/get_documents_response.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/get_documents_response.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/src/metriport/resources/document/types/trigger_documents_query_response.py` & `fern_metriport-0.0.4/src/metriport/resources/document/types/trigger_documents_query_response.py`

 * *Files identical despite different names*

### Comparing `fern_metriport-0.0.3/PKG-INFO` & `fern_metriport-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-metriport
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

