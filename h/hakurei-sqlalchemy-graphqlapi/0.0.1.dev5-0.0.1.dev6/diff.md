# Comparing `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev5.tar.gz` & `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev5.tar", last modified: Mon Apr 24 09:39:03 2023, max compression
+gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev6.tar", last modified: Tue Apr 25 00:45:45 2023, max compression
```

## Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5.tar` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:39:03.913124 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/
--rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/LICENSE
--rw-rw-rw-   0        0        0     3115 2023-04-24 09:39:03.913124 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:39:03.894175 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/__init__.py
--rw-rw-rw-   0        0        0    16743 2023-04-24 09:37:15.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/adapter.py
--rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/db_engine_specs.py
--rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/dialect.py
--rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/lib.py
--rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/types.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:39:03.912126 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-04-24 09:39:03.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-04-24 09:39:03.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:39:03.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-04-24 09:39:03.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-04-24 09:39:03.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 09:39:03.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 09:39:03.913124 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/setup.cfg
--rw-rw-rw-   0        0        0     4257 2023-04-24 09:39:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:45:45.557987 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/
+-rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/LICENSE
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:45:45.556990 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:45:45.540034 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/__init__.py
+-rw-rw-rw-   0        0        0    16803 2023-04-25 00:45:44.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/adapter.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/db_engine_specs.py
+-rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/dialect.py
+-rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/lib.py
+-rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:45:45.556990 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:45:45.557987 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/setup.cfg
+-rw-rw-rw-   0        0        0     4257 2023-04-25 00:45:44.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/setup.py
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/LICENSE` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei_sqlalchemy-graphqlapi
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/README.md` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/adapter.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import logging
 from collections import defaultdict
 from typing import (
     Any,
     Collection,
     Dict,
     Iterator,
     List,
@@ -457,14 +458,16 @@
                 include.extend(i.split(","))
 
         query_args = _parse_query_args(query_string)
 
         return (parsed.path, include, query_args, is_connection)
 
     def get_columns(self) -> Dict[str, Field]:
+
+        print("qqqqqqqqqqqqqqqqqqqqqqq")
         return self.columns
 
     def run_query(self, query: str) -> Dict[str, Any]:
         return run_query(self.graphql_api, query=query, bearer_token=self.bearer_token)
 
     def get_data_connection(
         self,
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/db_engine_specs.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/dialect.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/dialect.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/graphqldb/lib.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/lib.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei-sqlalchemy-graphqlapi
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev5/setup.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for GraphQL APIs."
-VERSION = "0.0.1.dev5"
+VERSION = "0.0.1.dev6"
 
 # -----------------------------------------------------------------------------
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type = "text/markdown; charset=UTF-8; variant=GFM"
```

