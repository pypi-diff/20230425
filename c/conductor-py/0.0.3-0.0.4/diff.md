# Comparing `tmp/conductor_py-0.0.3.tar.gz` & `tmp/conductor_py-0.0.4.tar.gz`

## Comparing `conductor_py-0.0.3.tar` & `conductor_py-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 conductor_py-0.0.3/operations.graphql
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 conductor_py-0.0.3/schema.graphql
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 conductor_py-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 conductor_py-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/__init__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/async_base_client.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/base_client.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/base_model.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/client.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/create_integration_connection.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/enums.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/exceptions.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/get_integration_connection.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/get_integration_connections.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/input_types.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/ping_integration_connection.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/scalars.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/graphql_client/send_integration_request.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/netsuite/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 conductor_py-0.0.3/conductor/netsuite/invoice.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 conductor_py-0.0.3/tests/test_package.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 conductor_py-0.0.3/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 conductor_py-0.0.3/LICENSE
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 conductor_py-0.0.3/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 conductor_py-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 conductor_py-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 conductor_py-0.0.4/operations.graphql
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 conductor_py-0.0.4/schema.graphql
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 conductor_py-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 conductor_py-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/base_client.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/base_model.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/client.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/create_integration_connection.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/enums.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/get_integration_connection.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/get_integration_connections.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/input_types.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/ping_integration_connection.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/scalars.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/graphql_client/send_integration_request.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/netsuite/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 conductor_py-0.0.4/conductor/netsuite/invoice.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 conductor_py-0.0.4/tests/test_package.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 conductor_py-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 conductor_py-0.0.4/LICENSE
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 conductor_py-0.0.4/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 conductor_py-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 conductor_py-0.0.4/PKG-INFO
```

### Comparing `conductor_py-0.0.3/operations.graphql` & `conductor_py-0.0.4/operations.graphql`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/schema.graphql` & `conductor_py-0.0.4/schema.graphql`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/.github/workflows/python-publish.yml` & `conductor_py-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/__init__.py` & `conductor_py-0.0.4/conductor/__init__.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/__init__.py` & `conductor_py-0.0.4/conductor/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/async_base_client.py` & `conductor_py-0.0.4/conductor/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/base_client.py` & `conductor_py-0.0.4/conductor/graphql_client/base_client.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/base_model.py` & `conductor_py-0.0.4/conductor/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/client.py` & `conductor_py-0.0.4/conductor/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/create_integration_connection.py` & `conductor_py-0.0.4/conductor/graphql_client/create_integration_connection.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/exceptions.py` & `conductor_py-0.0.4/conductor/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/get_integration_connection.py` & `conductor_py-0.0.4/conductor/graphql_client/get_integration_connection.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/get_integration_connections.py` & `conductor_py-0.0.4/conductor/graphql_client/get_integration_connections.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/input_types.py` & `conductor_py-0.0.4/conductor/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/ping_integration_connection.py` & `conductor_py-0.0.4/conductor/graphql_client/ping_integration_connection.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/graphql_client/send_integration_request.py` & `conductor_py-0.0.4/conductor/graphql_client/send_integration_request.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/conductor/netsuite/invoice.py` & `conductor_py-0.0.4/conductor/netsuite/invoice.py`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/.gitignore` & `conductor_py-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/LICENSE` & `conductor_py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `conductor_py-0.0.3/pyproject.toml` & `conductor_py-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "conductor-py"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Danny Nemer", email = "hi@dannynemer.com" }]
 description = "Python bindings for the Conductor API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["ariadne-codegen>=0.6"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
-[tool.setuptools]
-packages = ["conductor"]
+# [tool.setuptools]
+# packages = ["conductor"]
 
 [tool.ariadne-codegen]
 queries_path = "./operations.graphql"
 schema_path = "./schema.graphql"
 target_package_path = "./conductor_py/"
 async_client = false
```

### Comparing `conductor_py-0.0.3/PKG-INFO` & `conductor_py-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conductor-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python bindings for the Conductor API
 Author-email: Danny Nemer <hi@dannynemer.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

