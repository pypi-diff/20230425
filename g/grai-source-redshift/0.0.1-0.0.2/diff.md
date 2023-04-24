# Comparing `tmp/grai_source_redshift-0.0.1.tar.gz` & `tmp/grai_source_redshift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_redshift-0.0.1.tar", max compression
+gzip compressed data, was "grai_source_redshift-0.0.2.tar", max compression
```

## Comparing `grai_source_redshift-0.0.1.tar` & `grai_source_redshift-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      734 2023-04-19 18:51:24.789557 grai_source_redshift-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      145 2023-04-19 18:45:33.558481 grai_source_redshift-0.0.1/src/grai_source_redshift/__init__.py
--rw-r--r--   0        0        0     6326 2023-04-19 18:45:33.563285 grai_source_redshift-0.0.1/src/grai_source_redshift/adapters.py
--rw-r--r--   0        0        0     1195 2023-04-20 05:03:13.848847 grai_source_redshift-0.0.1/src/grai_source_redshift/base.py
--rw-r--r--   0        0        0     7305 2023-04-20 23:08:26.515358 grai_source_redshift-0.0.1/src/grai_source_redshift/loader.py
--rw-r--r--   0        0        0     4361 2023-04-20 22:59:02.272825 grai_source_redshift-0.0.1/src/grai_source_redshift/models.py
--rw-r--r--   0        0        0      186 2023-04-20 05:30:43.838248 grai_source_redshift-0.0.1/src/grai_source_redshift/package_definitions.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.1/setup.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      773 2023-04-24 23:04:02.946233 grai_source_redshift-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-04-19 18:45:33.558481 grai_source_redshift-0.0.2/src/grai_source_redshift/__init__.py
+-rw-r--r--   0        0        0     6562 2023-04-24 23:00:41.807746 grai_source_redshift-0.0.2/src/grai_source_redshift/adapters.py
+-rw-r--r--   0        0        0     1201 2023-04-24 15:52:37.165718 grai_source_redshift-0.0.2/src/grai_source_redshift/base.py
+-rw-r--r--   0        0        0     7181 2023-04-24 21:21:28.175258 grai_source_redshift-0.0.2/src/grai_source_redshift/loader.py
+-rw-r--r--   0        0        0     4369 2023-04-24 21:21:13.073883 grai_source_redshift-0.0.2/src/grai_source_redshift/models.py
+-rw-r--r--   0        0        0      186 2023-04-20 05:30:43.838248 grai_source_redshift-0.0.2/src/grai_source_redshift/package_definitions.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.2/setup.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 grai_source_redshift-0.0.2/PKG-INFO
```

### Comparing `grai_source_redshift-0.0.1/pyproject.toml` & `grai_source_redshift-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[tool.poetry]
+ [tool.poetry]
 name = "grai_source_redshift"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_redshift", from = "src" },
 ]
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^1.9.1"
 grai-client = "^0.2.4"
 multimethod = "^1.8"
 grai-schemas = "^0.1.5"
 redshift-connector = "^2.0.910"
+pydantic = {extras = ["dotenv"], version = "^1.10.7"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.10.1"
 types-PyYAML = "^6.0.11"
 types-psycopg2 = "^2.9.18"
 pytest = "^7.2.0"
 
-[tool.isort]
+  [tool.isort]
 profile = "black"
 known_first_party = "grai_source_redshift"
 
-[tool.black]
+  [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grai_source_redshift-0.0.1/src/grai_source_redshift/adapters.py` & `grai_source_redshift-0.0.2/src/grai_source_redshift/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,20 @@
         elif isinstance(current.destination, TableID):
             data["edge_type"] = EdgeTypeLabels.table_to_table.value
             return TableToTableMetadata(**data)
     elif isinstance(current.source, ColumnID):
         if isinstance(current.destination, ColumnID):
             data["edge_type"] = EdgeTypeLabels.column_to_column.value
             return ColumnToColumnMetadata(**data)
+    else:
+        message = (
+            "No edge metadata implementation for edge with source type "
+            f"{type(current.source)} and destination type {type(current.destination)}"
+        )
+        raise NotImplementedError()
 
 
 @multimethod
 def build_app_metadata(current: Any, desired: Any) -> None:
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
```

### Comparing `grai_source_redshift-0.0.1/src/grai_source_redshift/base.py` & `grai_source_redshift-0.0.2/src/grai_source_redshift/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     nodes = adapt_to_client(nodes, version)
     edges = adapt_to_client(edges, version)
     return nodes, edges
 
 
 def update_server(
     client: BaseClient,
-    dbname: Optional[str] = None,
+    database: Optional[str] = None,
     namespace: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     host: Optional[str] = None,
     port: Optional[str] = None,
 ):
     conn = RedshiftConnector(
-        dbname=dbname,
+        database=database,
         user=user,
         password=password,
         host=host,
         port=port,
         namespace=namespace,
     )
     nodes, edges = get_nodes_and_edges(conn, client.id)
```

### Comparing `grai_source_redshift-0.0.1/src/grai_source_redshift/loader.py` & `grai_source_redshift-0.0.2/src/grai_source_redshift/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 
 class RedshiftConfig(BaseSettings):
     user: Optional[str] = None
     password: Optional[SecretStr] = None
     database: Optional[str] = None
     host: Optional[str] = None
-    port: Optional[int] = 5439
-    namespace: Optional[str] = None
+    port: Optional[int] = None
 
     class Config:
         env_prefix = "grai_redshift_"
         env_file = ".env"
 
 
 class RedshiftConnector:
@@ -35,24 +34,22 @@
         self,
         namespace: str,
         user: Optional[str] = None,
         password: Optional[str] = None,
         database: Optional[str] = None,
         host: Optional[str] = None,
         port: Optional[Union[str, int]] = None,
-        redshift_namespace: Optional[str] = None,
         **kwargs,
     ):
         passthrough_kwargs = {
             "user": user,
             "password": password,
             "database": database,
             "host": host,
             "port": port,
-            "namespace": redshift_namespace,
         }
 
         self.namespace = namespace
         self.config = RedshiftConfig(**{k: v for k, v in passthrough_kwargs.items() if v is not None})
         self.redshift_params: [Dict[str, Any]] = kwargs
         self._connection: Optional[Connection] = None
         self._is_connected: Optional[bool] = None
@@ -118,15 +115,15 @@
     def columns(self) -> List[Column]:
         """
         Creates and returns a list of dictionaries for the specified
         schema.table in the database connected to.
         """
         query = f"""
             SELECT table_catalog,
-                   table_schema AS schema,
+                   table_schema AS column_schema,
                    table_name,
                    column_name,
                    column_default,
                    is_nullable,
                    data_type,
                    character_maximum_length,
                    numeric_precision
```

### Comparing `grai_source_redshift-0.0.1/src/grai_source_redshift/models.py` & `grai_source_redshift-0.0.2/src/grai_source_redshift/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     class Config:
         allow_population_by_field_name = True
 
     @validator("full_name", always=True)
     def make_full_name(cls, full_name, values):
         if full_name is not None:
             return full_name
-        result = f"{values['table']}.{values['table']}.{values['name']}"
+        result = f"{values['column_schema']}.{values['table']}.{values['name']}"
         return result
 
 
 class Constraint(str, Enum):
     foreign_key = "FOREIGN KEY"
     primary_key = "PRIMARY KEY"
     belongs_to = "bt"
```

### Comparing `grai_source_redshift-0.0.1/setup.py` & `grai_source_redshift-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['grai-client>=0.2.4,<0.3.0',
  'grai-schemas>=0.1.5,<0.2.0',
  'multimethod>=1.8,<2.0',
- 'pydantic>=1.9.1,<2.0.0',
+ 'pydantic[dotenv]>=1.10.7,<2.0.0',
  'redshift-connector>=2.0.910,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-redshift',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_redshift-0.0.1/PKG-INFO` & `grai_source_redshift-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: grai-source-redshift
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grai-client (>=0.2.4,<0.3.0)
 Requires-Dist: grai-schemas (>=0.1.5,<0.2.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: redshift-connector (>=2.0.910,<3.0.0)
```

