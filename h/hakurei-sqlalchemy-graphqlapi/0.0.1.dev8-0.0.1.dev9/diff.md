# Comparing `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev8.tar.gz` & `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev8.tar", last modified: Tue Apr 25 00:54:12 2023, max compression
+gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev9.tar", last modified: Tue Apr 25 00:56:15 2023, max compression
```

## Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8.tar` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:54:12.466536 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/
--rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/LICENSE
--rw-rw-rw-   0        0        0     3115 2023-04-25 00:54:12.466536 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/PKG-INFO
--rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:54:12.445459 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/__init__.py
--rw-rw-rw-   0        0        0    16998 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/adapter.py
--rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/db_engine_specs.py
--rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/dialect.py
--rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/lib.py
--rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/types.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:54:12.465539 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 00:54:12.466536 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/setup.cfg
--rw-rw-rw-   0        0        0     4257 2023-04-25 00:54:12.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:56:15.479495 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/
+-rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/LICENSE
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:56:15.478497 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/PKG-INFO
+-rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:56:15.467527 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/__init__.py
+-rw-rw-rw-   0        0        0    16483 2023-04-25 00:55:48.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/adapter.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/db_engine_specs.py
+-rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/dialect.py
+-rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/lib.py
+-rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:56:15.478497 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:56:15.479495 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/setup.cfg
+-rw-rw-rw-   0        0        0     4257 2023-04-25 00:56:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/setup.py
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/LICENSE` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei_sqlalchemy-graphqlapi
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/README.md` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/adapter.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -442,32 +442,19 @@
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
         # TODO the slow path here could connect to the GQL Server
         return True
 
     @staticmethod
-    def parse_uri(table: str) -> Tuple[str, List[str], Dict[str, QueryArg], bool]:
+    def parse_uri(table: str) -> str:
         """
         This will pass in the first n args of __init__ for the Adapter
         """
-        parsed = urlparse(table)
-        query_string = parse_qs(parsed.query)
-
-        include_entry = query_string.get("include")
-        is_connection = get_last_query(query_string.get("is_connection", "1")) != "0"
-
-        include: List[str] = []
-        if include_entry:
-            for i in include_entry:
-                include.extend(i.split(","))
-
-        query_args = _parse_query_args(query_string)
-
-        return (parsed.path, include, query_args, is_connection)
+        return table
 
     def get_columns(self) -> Dict[str, Field]:
         return self.columns
 
     def run_query(self, query: str) -> Dict[str, Any]:
         return run_query(self.graphql_api, query=query, bearer_token=self.bearer_token)
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/db_engine_specs.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/dialect.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/dialect.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/graphqldb/lib.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/graphqldb/lib.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei-sqlalchemy-graphqlapi
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev8/setup.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for GraphQL APIs."
-VERSION = "0.0.1.dev8"
+VERSION = "0.0.1.dev9"
 
 # -----------------------------------------------------------------------------
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type = "text/markdown; charset=UTF-8; variant=GFM"
```

