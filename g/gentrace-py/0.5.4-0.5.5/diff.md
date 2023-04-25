# Comparing `tmp/gentrace_py-0.5.4.tar.gz` & `tmp/gentrace_py-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.5.4.tar", max compression
+gzip compressed data, was "gentrace_py-0.5.5.tar", max compression
```

## Comparing `gentrace_py-0.5.4.tar` & `gentrace_py-0.5.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      968 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      787 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    25461 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6400 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      695 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12257 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-24 19:54:47.233528 gentrace_py-0.5.4/gentrace/schemas.py
--rw-r--r--   0        0        0     1571 2023-04-24 19:54:47.237527 gentrace_py-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      968 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-25 10:54:39.683107 gentrace_py-0.5.5/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5209 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4998 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    33338 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32730 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     1072 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    25461 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6400 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      695 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12257 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/gentrace/schemas.py
+-rw-r--r--   0        0        0     1571 2023-04-25 10:54:39.687107 gentrace_py-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 gentrace_py-0.5.5/PKG-INFO
```

### Comparing `gentrace_py-0.5.4/gentrace/__init__.py` & `gentrace_py-0.5.5/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/api_client.py` & `gentrace_py-0.5.5/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/configuration.py` & `gentrace_py-0.5.5/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/exceptions.py` & `gentrace_py-0.5.5/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/feedback_request.py` & `gentrace_py-0.5.5/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/feedback_request.pyi` & `gentrace_py-0.5.5/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/feedback_response.py` & `gentrace_py-0.5.5/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/feedback_response.pyi` & `gentrace_py-0.5.5/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.5.5/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.5.5/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.5.5/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.5.5/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/models/__init__.py` & `gentrace_py-0.5.5/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.5.5/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/providers/llms/openai.py` & `gentrace_py-0.5.5/gentrace/providers/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/providers/pipeline.py` & `gentrace_py-0.5.5/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/providers/pipeline_run.py` & `gentrace_py-0.5.5/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/providers/step_run.py` & `gentrace_py-0.5.5/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/providers/utils.py` & `gentrace_py-0.5.5/gentrace/providers/utils.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.5.5/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/rest.py` & `gentrace_py-0.5.5/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/gentrace/schemas.py` & `gentrace_py-0.5.5/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.5.4/pyproject.toml` & `gentrace_py-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.5.4"
+version = "0.5.5"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
```

### Comparing `gentrace_py-0.5.4/PKG-INFO` & `gentrace_py-0.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

