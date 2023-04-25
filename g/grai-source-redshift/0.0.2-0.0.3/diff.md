# Comparing `tmp/grai_source_redshift-0.0.2.tar.gz` & `tmp/grai_source_redshift-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.0.2.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.0.3.tar", max compression
```

## Comparing `grai_source_redshift-0.0.2.tar` & `grai_source_redshift-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      773 2023-04-24 23:04:02.946233 grai_source_redshift-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      145 2023-04-19 18:45:33.558481 grai_source_redshift-0.0.2/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     6562 2023-04-24 23:00:41.807746 grai_source_redshift-0.0.2/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1201 2023-04-24 15:52:37.165718 grai_source_redshift-0.0.2/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     7181 2023-04-24 21:21:28.175258 grai_source_redshift-0.0.2/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     4369 2023-04-24 21:21:13.073883 grai_source_redshift-0.0.2/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      186 2023-04-20 05:30:43.838248 grai_source_redshift-0.0.2/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.2/setup.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      775 2023-04-25 00:54:43.259686 grai_source_redshift-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-04-19 18:45:33.558481 grai_source_redshift-0.0.3/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     6562 2023-04-24 23:00:41.807746 grai_source_redshift-0.0.3/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1185 2023-04-25 00:59:25.399992 grai_source_redshift-0.0.3/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     7181 2023-04-25 00:57:39.596347 grai_source_redshift-0.0.3/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     4369 2023-04-24 21:21:13.073883 grai_source_redshift-0.0.3/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      186 2023-04-20 05:30:43.838248 grai_source_redshift-0.0.3/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.3/setup.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.3/PKG-INFO
```

### Comparing `grai_source_redshift-0.0.2/pyproject.toml` & `grai_source_redshift-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
  [tool.poetry]
 name = "grai_source_redshift"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 [tool.poetry.dependencies]
@@ -19,17 +19,17 @@
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 types-psycopg2 = "^2.9.18"
 pytest = "^7.2.0"
 
-  [tool.isort]
+   [tool.isort]
 profile = "black"
 known_first_party = "grai_source_redshift"
 
-  [tool.black]
+   [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grai_source_redshift-0.0.2/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.0.3/src/grai_source_redshift/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.2/src/grai_source_redshift/base.py` & `grai_source_redshift-0.0.3/src/grai_source_redshift/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,25 +16,26 @@
     nodes = adapt_to_client(nodes, version)
     edges = adapt_to_client(edges, version)
     return nodes, edges
 
 
 def update_server(
     client: BaseClient,
+    namespace: str,
     database: Optional[str] = None,
-    namespace: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     host: Optional[str] = None,
     port: Optional[str] = None,
 ):
     conn = RedshiftConnector(
         database=database,
         user=user,
         password=password,
         host=host,
         port=port,
         namespace=namespace,
     )
     nodes, edges = get_nodes_and_edges(conn, client.id)
+
     update(client, nodes)
     update(client, edges)
```

### Comparing `grai_source_redshift-0.0.2/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.0.3/src/grai_source_redshift/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.2/src/grai_source_redshift/models.py` & `grai_source_redshift-0.0.3/src/grai_source_redshift/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_redshift-0.0.2/setup.py` & `grai_source_redshift-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'grai-schemas>=0.1.5,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic[dotenv]>=1.10.7,<2.0.0',
  'redshift-connector>=2.0.910,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-redshift',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_redshift-0.0.2/PKG-INFO` & `grai_source_redshift-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

