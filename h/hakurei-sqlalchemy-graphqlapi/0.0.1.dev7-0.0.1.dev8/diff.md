# Comparing `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev7.tar.gz` & `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev7.tar", last modified: Tue Apr 25 00:51:07 2023, max compression
+gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev8.tar", last modified: Tue Apr 25 00:54:12 2023, max compression
```

## Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7.tar` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:51:07.312396 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/
--rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/LICENSE
--rw-rw-rw-   0        0        0     3115 2023-04-25 00:51:07.312396 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/PKG-INFO
--rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:51:07.297184 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/__init__.py
--rw-rw-rw-   0        0        0    16933 2023-04-25 00:51:06.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/adapter.py
--rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/db_engine_specs.py
--rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/dialect.py
--rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/lib.py
--rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/types.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:51:07.311399 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 00:51:07.312396 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/setup.cfg
--rw-rw-rw-   0        0        0     4257 2023-04-25 00:51:06.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:54:12.466536 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/
+-rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/LICENSE
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:54:12.466536 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/PKG-INFO
+-rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:54:12.445459 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/__init__.py
+-rw-rw-rw-   0        0        0    16998 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/adapter.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/db_engine_specs.py
+-rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/dialect.py
+-rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/lib.py
+-rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:54:12.465539 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:54:12.466536 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/setup.cfg
+-rw-rw-rw-   0        0        0     4257 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/setup.py
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/LICENSE` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei_sqlalchemy-graphqlapi
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/README.md` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/adapter.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import logging
+from shillelagh.fields import DateTime, Field, Float, Order, Integer
 from collections import defaultdict
 from typing import (
     Any,
     Collection,
     Dict,
     Iterator,
     List,
@@ -426,21 +426,23 @@
             if node_type_name is None:
                 raise ValueError("Unable to resolve node_type_name")
 
         node_fields = data_types[node_type_name]["fields"]
         if node_fields is None:
             raise ValueError("No fields found on node")
 
-        self.columns: Dict[str, Field] = {}
-        for node_field in node_fields:
-            self.columns.update(
-                get_type_entries(
-                    node_field, data_types=data_types, include=self.include
-                )
-            )
+        self._set_columns()
+
+    def _set_columns(self) -> None:
+        self.columns: Dict[str, Field] = {
+            "timestamp": DateTime(filters=None, order=Order.ASCENDING, exact=False),
+            "value": Integer(filters=None,
+                             order=Order.NONE,
+                             exact=False, )
+        }
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         # TODO the slow path here could connect to the GQL Server
         return True
 
     @staticmethod
@@ -460,16 +462,14 @@
                 include.extend(i.split(","))
 
         query_args = _parse_query_args(query_string)
 
         return (parsed.path, include, query_args, is_connection)
 
     def get_columns(self) -> Dict[str, Field]:
-        logging.log(0, "hhhh-hh")
-        logging.log(5, "hhhh-hh")
         return self.columns
 
     def run_query(self, query: str) -> Dict[str, Any]:
         return run_query(self.graphql_api, query=query, bearer_token=self.bearer_token)
 
     def get_data_connection(
             self,
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/db_engine_specs.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/dialect.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/dialect.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/lib.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/lib.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei-sqlalchemy-graphqlapi
-Version: 0.0.1.dev7
+Version: 0.0.1.dev8
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/setup.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for GraphQL APIs."
-VERSION = "0.0.1.dev7"
+VERSION = "0.0.1.dev8"
 
 # -----------------------------------------------------------------------------
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type = "text/markdown; charset=UTF-8; variant=GFM"
```

