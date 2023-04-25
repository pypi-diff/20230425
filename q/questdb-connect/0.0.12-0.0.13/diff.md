# Comparing `tmp/questdb-connect-0.0.12.tar.gz` & `tmp/questdb-connect-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.12.tar", last modified: Tue Apr 25 10:30:36 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.13.tar", last modified: Tue Apr 25 10:46:49 2023, max compression
```

## Comparing `questdb-connect-0.0.12.tar` & `questdb-connect-0.0.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.727172 questdb-connect-0.0.12/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.12/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 10:30:36.727020 questdb-connect-0.0.12/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.12/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2372 2023-04-25 10:28:54.000000 questdb-connect-0.0.12/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-25 10:30:36.727206 questdb-connect-0.0.12/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.723523 questdb-connect-0.0.12/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.725044 questdb-connect-0.0.12/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.12/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     9957 2023-04-25 09:12:33.000000 questdb-connect-0.0.12/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     6903 2023-04-25 10:28:54.000000 questdb-connect-0.0.12/src/questdb_connect/superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     9914 2023-04-25 09:41:56.000000 questdb-connect-0.0.12/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.726246 questdb-connect-0.0.12/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      458 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.726712 questdb-connect-0.0.12/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9805 2023-04-25 10:23:19.000000 questdb-connect-0.0.12/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3253 2023-04-25 10:27:32.000000 questdb-connect-0.0.12/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:46:49.490694 questdb-connect-0.0.13/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.13/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 10:46:49.490517 questdb-connect-0.0.13/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.13/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2372 2023-04-25 10:45:29.000000 questdb-connect-0.0.13/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-25 10:46:49.490745 questdb-connect-0.0.13/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:46:49.487123 questdb-connect-0.0.13/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:46:49.488801 questdb-connect-0.0.13/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.13/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9897 2023-04-25 10:45:04.000000 questdb-connect-0.0.13/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6903 2023-04-25 10:28:54.000000 questdb-connect-0.0.13/src/questdb_connect/superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9914 2023-04-25 09:41:56.000000 questdb-connect-0.0.13/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:46:49.489702 questdb-connect-0.0.13/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 10:46:49.000000 questdb-connect-0.0.13/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      458 2023-04-25 10:46:49.000000 questdb-connect-0.0.13/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-25 10:46:49.000000 questdb-connect-0.0.13/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-25 10:46:49.000000 questdb-connect-0.0.13/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-25 10:46:49.000000 questdb-connect-0.0.13/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-25 10:46:49.000000 questdb-connect-0.0.13/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:46:49.490160 questdb-connect-0.0.13/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9785 2023-04-25 10:45:04.000000 questdb-connect-0.0.13/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3253 2023-04-25 10:27:32.000000 questdb-connect-0.0.13/tests/test_types.py
```

### Comparing `questdb-connect-0.0.12/LICENSE` & `questdb-connect-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.12/PKG-INFO` & `questdb-connect-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.12
+Version: 0.0.13
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.12/README.md` & `questdb-connect-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.12/pyproject.toml` & `questdb-connect-0.0.13/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.12"
+version = "0.0.13"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.12/src/questdb_connect/__init__.py` & `questdb-connect-0.0.13/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.12/src/questdb_connect/dialect.py` & `questdb-connect-0.0.13/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,18 @@
 
     def _requires_quotes(self, _value):
         return True
 
 
 class QDBDDLCompiler(DDLCompiler):
     def visit_create_schema(self, create, **kw):
-        raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
+        raise Exception('QuestDB does not support SCHEMAS')
 
     def visit_drop_schema(self, drop, **kw):
-        raise Exception('QuestDB does not support SCHEMAS, there is only "public"')
+        raise Exception('QuestDB does not support SCHEMAS')
 
     def visit_create_table(self, create, **kw):
         table = create.element
         create_table = f"CREATE TABLE '{table.fullname}' ("
         create_table += ', '.join([self.get_column_specification(c.element) for c in create.columns])
         return create_table + ') ' + table.engine.get_table_suffix()
 
@@ -191,15 +191,15 @@
         } for row in result_set]
 
 
 # class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
 class QuestDBDialect(PGDialect_psycopg2, abc.ABC):
     name = 'questdb'
     psycopg2_version = (2, 9)
-    default_schema_name = 'public'
+    default_schema_name = None
     statement_compiler = QDBSQLCompiler
     ddl_compiler = QDBDDLCompiler
     type_compiler = GenericTypeCompiler
     inspector = QDBInspector
     preparer = QDBIdentifierPreparer
     supports_schemas = False
     supports_statement_cache = False
@@ -217,15 +217,15 @@
 
     @classmethod
     def dbapi(cls):
         import questdb_connect as dbapi
         return dbapi
 
     def get_schema_names(self, connection, **kw):
-        return ['public']
+        return []
 
     def get_table_names(self, connection, schema=None, **kw):
         return [row.table for row in connection.execute(sqla.text('SHOW TABLES'))]
 
     def get_pk_constraint(self, connection, table_name, schema=None, **kw):
         return []
```

### Comparing `questdb-connect-0.0.12/src/questdb_connect/superset.py` & `questdb-connect-0.0.13/src/questdb_connect/superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.12/src/questdb_connect/types.py` & `questdb-connect-0.0.13/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.12/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.13/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.12
+Version: 0.0.13
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.12/tests/test_dialect.py` & `questdb-connect-0.0.13/tests/test_dialect.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from sqlalchemy.orm import Session
 
 from tests.conftest import TEST_TABLE_NAME, collect_select_all, collect_select_all_raw_connection
 
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
-        assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME, 'public')
-        assert not test_engine.dialect.has_table(conn, 'scorchio', 'public')
+        assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME)
+        assert not test_engine.dialect.has_table(conn, 'scorchio')
         now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
         now_date = now.date()
         expected = ("(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                     "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                     "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj2v', "
                     "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
                     "(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
```

### Comparing `questdb-connect-0.0.12/tests/test_types.py` & `questdb-connect-0.0.13/tests/test_types.py`

 * *Files identical despite different names*

