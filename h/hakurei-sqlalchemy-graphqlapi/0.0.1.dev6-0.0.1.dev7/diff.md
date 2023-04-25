# Comparing `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev6.tar.gz` & `tmp/hakurei_sqlalchemy-graphqlapi-0.0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev6.tar", last modified: Tue Apr 25 00:45:45 2023, max compression
+gzip compressed data, was "hakurei_sqlalchemy-graphqlapi-0.0.1.dev7.tar", last modified: Tue Apr 25 00:51:07 2023, max compression
```

## Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6.tar` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:45:45.557987 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/
--rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/LICENSE
--rw-rw-rw-   0        0        0     3115 2023-04-25 00:45:45.556990 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/PKG-INFO
--rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:45:45.540034 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/__init__.py
--rw-rw-rw-   0        0        0    16803 2023-04-25 00:45:44.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/adapter.py
--rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/db_engine_specs.py
--rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/dialect.py
--rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/lib.py
--rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/types.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:45:45.556990 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 00:45:45.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 00:45:45.557987 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/setup.cfg
--rw-rw-rw-   0        0        0     4257 2023-04-25 00:45:44.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:51:07.312396 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/
+-rw-rw-rw-   0        0        0     1091 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/LICENSE
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:51:07.312396 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/PKG-INFO
+-rw-rw-rw-   0        0        0     2298 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:51:07.297184 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/__init__.py
+-rw-rw-rw-   0        0        0    16933 2023-04-25 00:51:06.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/adapter.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/db_engine_specs.py
+-rw-rw-rw-   0        0        0     2954 2023-04-24 08:52:02.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/dialect.py
+-rw-rw-rw-   0        0        0     1758 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/lib.py
+-rw-rw-rw-   0        0        0      166 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/types.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:51:07.311399 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/
+-rw-rw-rw-   0        0        0     3115 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 00:51:07.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      143 2023-04-24 06:09:10.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:51:07.312396 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/setup.cfg
+-rw-rw-rw-   0        0        0     4257 2023-04-25 00:51:06.000000 hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/setup.py
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/LICENSE` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei_sqlalchemy-graphqlapi
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/README.md` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/adapter.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     String,
 )
 from shillelagh.typing import RequestedOrder
 
 from .lib import get_last_query, run_query
 from .types import TypedDict
 
+
 # -----------------------------------------------------------------------------
 
 
 class MaybeNamed(TypedDict):
     name: Optional[str]
 
 
@@ -53,14 +54,15 @@
 
 class TypeInfoWithFields(TypeInfo):
     fields: Optional[List[FieldInfo]]
 
 
 QueryArg = Union[str, int]
 
+
 # -----------------------------------------------------------------------------
 
 
 def parse_gql_type(type_info: TypeInfo) -> Field:
     # TODO(cancan101): do we want to handle Nones here?
     name: Optional[str] = type_info["name"]
     if name == "String":
@@ -87,19 +89,19 @@
         return ISOTime()
     else:
         # TODO(cancan101): how do we want to handle other scalars?
         raise ValueError(f"Unknown type: {name}")
 
 
 def get_type_entries(
-    field_obj: FieldInfo,
-    *,
-    data_types: Dict[str, TypeInfoWithFields],
-    include: Collection[str],
-    path: Optional[List[str]] = None,
+        field_obj: FieldInfo,
+        *,
+        data_types: Dict[str, TypeInfoWithFields],
+        include: Collection[str],
+        path: Optional[List[str]] = None,
 ) -> Dict[str, Field]:
     path = path or []
 
     field_name = field_obj["name"]
     new_path = path + [field_name]
 
     field_obj_type = field_obj["type"]
@@ -261,22 +263,22 @@
 # -----------------------------------------------------------------------------
 
 
 class GraphQLAdapter(Adapter):
     safe = True
 
     def __init__(
-        self,
-        table: str,
-        include: Collection[str],
-        query_args: Dict[str, QueryArg],
-        is_connection: bool,
-        graphql_api: str,
-        bearer_token: Optional[str] = None,
-        pagination_relay: Optional[bool] = None,
+            self,
+            table: str,
+            include: Collection[str],
+            query_args: Dict[str, QueryArg],
+            is_connection: bool,
+            graphql_api: str,
+            bearer_token: Optional[str] = None,
+            pagination_relay: Optional[bool] = None,
     ):
         super().__init__()
 
         # The query field name
         self.table = table
         print("初始化了我哈哈哈哈")
 
@@ -458,26 +460,26 @@
                 include.extend(i.split(","))
 
         query_args = _parse_query_args(query_string)
 
         return (parsed.path, include, query_args, is_connection)
 
     def get_columns(self) -> Dict[str, Field]:
-
-        print("qqqqqqqqqqqqqqqqqqqqqqq")
+        logging.log(0, "hhhh-hh")
+        logging.log(5, "hhhh-hh")
         return self.columns
 
     def run_query(self, query: str) -> Dict[str, Any]:
         return run_query(self.graphql_api, query=query, bearer_token=self.bearer_token)
 
     def get_data_connection(
-        self,
-        bounds: Dict[str, Filter],
-        order: List[Tuple[str, RequestedOrder]],
-        **kwargs: Any,
+            self,
+            bounds: Dict[str, Filter],
+            order: List[Tuple[str, RequestedOrder]],
+            **kwargs: Any,
     ) -> Iterator[Dict[str, Any]]:
         fields_str = get_gql_fields(list(self.columns.keys()))
         query_args_user = dict(self.query_args)
 
         after = query_args_user.pop("after", None)
 
         # We loop for each page in the pagination
@@ -523,18 +525,18 @@
                     break
                 after = page_info["endCursor"]
             else:
                 # If there is no pagination being used, break immediately
                 break
 
     def get_data_list(
-        self,
-        bounds: Dict[str, Filter],
-        order: List[Tuple[str, RequestedOrder]],
-        **kwargs: Any,
+            self,
+            bounds: Dict[str, Filter],
+            order: List[Tuple[str, RequestedOrder]],
+            **kwargs: Any,
     ) -> Iterator[Dict[str, Any]]:
         fields_str = get_gql_fields(list(self.columns.keys()))
 
         if self.query_args:
             variable_str = f"({_get_variable_argument_str(self.query_args)})"
         else:
             # Don't generate the () for empty list of query_args
@@ -548,16 +550,16 @@
         query_data = self.run_query(query=query)
         nodes: List[Dict[str, Any]] = query_data[self.table]
 
         for node in nodes:
             yield {c: extract_flattened_value(node, c) for c in self.columns.keys()}
 
     def get_data(
-        self,
-        bounds: Dict[str, Filter],
-        order: List[Tuple[str, RequestedOrder]],
-        **kwargs: Any,
+            self,
+            bounds: Dict[str, Filter],
+            order: List[Tuple[str, RequestedOrder]],
+            **kwargs: Any,
     ) -> Iterator[Dict[str, Any]]:
         if self.is_connection:
             return self.get_data_connection(bounds=bounds, order=order, **kwargs)
         else:
             return self.get_data_list(bounds=bounds, order=order, **kwargs)
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/db_engine_specs.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/dialect.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/dialect.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/graphqldb/lib.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/graphqldb/lib.py`

 * *Files identical despite different names*

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/hakurei_sqlalchemy_graphqlapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hakurei-sqlalchemy-graphqlapi
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: Python DB-API and SQLAlchemy interface for GraphQL APIs.
 Home-page: https://github.com/cancan101/graphql-db-api
 Author: Alex Rothberg
 Author-email: agrothberg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hakurei_sqlalchemy-graphqlapi-0.0.1.dev6/setup.py` & `hakurei_sqlalchemy-graphqlapi-0.0.1.dev7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Tuple
 
 from setuptools import Command, find_packages, setup
 
 # -----------------------------------------------------------------------------
 
 DESCRIPTION = "Python DB-API and SQLAlchemy interface for GraphQL APIs."
-VERSION = "0.0.1.dev6"
+VERSION = "0.0.1.dev7"
 
 # -----------------------------------------------------------------------------
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 long_description_content_type = "text/markdown; charset=UTF-8; variant=GFM"
```

