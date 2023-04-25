# Comparing `tmp/questdb-connect-0.0.11.tar.gz` & `tmp/questdb-connect-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.11.tar", last modified: Mon Apr 24 17:52:49 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.12.tar", last modified: Tue Apr 25 10:30:36 2023, max compression
```

## Comparing `questdb-connect-0.0.11.tar` & `questdb-connect-0.0.12.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 17:52:49.078377 questdb-connect-0.0.11/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.11/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-24 17:52:49.078247 questdb-connect-0.0.11/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.11/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2339 2023-04-24 17:52:18.000000 questdb-connect-0.0.11/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-24 17:52:49.078414 questdb-connect-0.0.11/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 17:52:49.075178 questdb-connect-0.0.11/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 17:52:49.076726 questdb-connect-0.0.11/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.11/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    13289 2023-04-24 14:22:58.000000 questdb-connect-0.0.11/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     9943 2023-04-24 17:52:10.000000 questdb-connect-0.0.11/src/questdb_connect/superset.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 17:52:49.077768 questdb-connect-0.0.11/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-24 17:52:49.000000 questdb-connect-0.0.11/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      409 2023-04-24 17:52:49.000000 questdb-connect-0.0.11/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-24 17:52:49.000000 questdb-connect-0.0.11/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-24 17:52:49.000000 questdb-connect-0.0.11/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-24 17:52:49.000000 questdb-connect-0.0.11/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-24 17:52:49.000000 questdb-connect-0.0.11/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-24 17:52:49.077898 questdb-connect-0.0.11/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9795 2023-04-24 12:28:24.000000 questdb-connect-0.0.11/tests/test_dialect.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.727172 questdb-connect-0.0.12/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.12/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 10:30:36.727020 questdb-connect-0.0.12/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.12/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2372 2023-04-25 10:28:54.000000 questdb-connect-0.0.12/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-25 10:30:36.727206 questdb-connect-0.0.12/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.723523 questdb-connect-0.0.12/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.725044 questdb-connect-0.0.12/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1319 2023-04-24 12:28:52.000000 questdb-connect-0.0.12/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9957 2023-04-25 09:12:33.000000 questdb-connect-0.0.12/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6903 2023-04-25 10:28:54.000000 questdb-connect-0.0.12/src/questdb_connect/superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9914 2023-04-25 09:41:56.000000 questdb-connect-0.0.12/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.726246 questdb-connect-0.0.12/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      458 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      101 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-25 10:30:36.000000 questdb-connect-0.0.12/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-25 10:30:36.726712 questdb-connect-0.0.12/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9805 2023-04-25 10:23:19.000000 questdb-connect-0.0.12/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3253 2023-04-25 10:27:32.000000 questdb-connect-0.0.12/tests/test_types.py
```

### Comparing `questdb-connect-0.0.11/LICENSE` & `questdb-connect-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.11/PKG-INFO` & `questdb-connect-0.0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.11
+Version: 0.0.12
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.11/README.md` & `questdb-connect-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.11/pyproject.toml` & `questdb-connect-0.0.12/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.11"
+version = "0.0.12"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -72,7 +72,8 @@
 ]
 
 [tool.ruff.pylint]
 max-branches = 20
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
+"tests/test_types.py" = ["S101"]
```

### Comparing `questdb-connect-0.0.11/src/questdb_connect/__init__.py` & `questdb-connect-0.0.12/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.11/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.12/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.11
+Version: 0.0.12
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.11/tests/test_dialect.py` & `questdb-connect-0.0.12/tests/test_dialect.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import datetime
 
-import questdb_connect.dialect as qdbc
 import sqlalchemy as sqla
+from questdb_connect import types
 from sqlalchemy.orm import Session
 
 from tests.conftest import TEST_TABLE_NAME, collect_select_all, collect_select_all_raw_connection
 
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
@@ -109,29 +109,29 @@
     finally:
         if session:
             session.close()
     metadata = sqla.MetaData()
     table = sqla.Table(TEST_TABLE_NAME, metadata, autoload_with=test_engine)
     table_columns = str([(col.name, col.type, col.primary_key) for col in table.columns])
     assert table_columns == str([
-        ('col_boolean', qdbc.Boolean(), False),
-        ('col_byte', qdbc.Byte(), False),
-        ('col_short', qdbc.Short(), False),
-        ('col_int', qdbc.Int(), False),
-        ('col_long', qdbc.Long(), False),
-        ('col_float', qdbc.Float(), False),
-        ('col_double', qdbc.Double(), False),
-        ('col_symbol', qdbc.Symbol(), False),
-        ('col_string', qdbc.String(), False),
-        ('col_char', qdbc.Char(), False),
-        ('col_uuid', qdbc.UUID(), False),
-        ('col_date', qdbc.Date(), False),
-        ('col_ts', qdbc.Timestamp(), True),
-        ('col_geohash', qdbc.geohash_type(40)(), False),
-        ('col_long256', qdbc.Long256(), False)
+        ('col_boolean', types.Boolean(), False),
+        ('col_byte', types.Byte(), False),
+        ('col_short', types.Short(), False),
+        ('col_int', types.Int(), False),
+        ('col_long', types.Long(), False),
+        ('col_float', types.Float(), False),
+        ('col_double', types.Double(), False),
+        ('col_symbol', types.Symbol(), False),
+        ('col_string', types.String(), False),
+        ('col_char', types.Char(), False),
+        ('col_uuid', types.UUID(), False),
+        ('col_date', types.Date(), False),
+        ('col_ts', types.Timestamp(), True),
+        ('col_geohash', types.geohash_type(40)(), False),
+        ('col_long256', types.Long256(), False)
     ])
 
 
 def test_multiple_insert(test_engine, test_model):
     now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
     now_date = now.date()
     session = Session(test_engine)
```

