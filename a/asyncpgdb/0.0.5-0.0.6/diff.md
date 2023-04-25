# Comparing `tmp/asyncpgdb-0.0.5.tar.gz` & `tmp/asyncpgdb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpgdb-0.0.5.tar", max compression
+gzip compressed data, was "asyncpgdb-0.0.6.tar", max compression
```

## Comparing `asyncpgdb-0.0.5.tar` & `asyncpgdb-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2023-01-25 13:04:40.809165 asyncpgdb-0.0.5/README.md
--rw-r--r--   0        0        0      894 2023-04-24 17:21:33.756204 asyncpgdb-0.0.5/asyncpgdb/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 13:45:42.124801 asyncpgdb-0.0.5/asyncpgdb/types/__init__.py
--rw-r--r--   0        0        0      172 2023-04-24 13:55:34.429438 asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6185 2023-04-24 17:21:37.382326 asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc
--rw-r--r--   0        0        0     1074 2023-04-24 16:29:11.125800 asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc
--rw-r--r--   0        0        0     4740 2023-04-24 14:06:39.702336 asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc
--rw-r--r--   0        0        0     6757 2023-04-24 17:22:11.748892 asyncpgdb-0.0.5/asyncpgdb/types/connectionpool.py
--rw-r--r--   0        0        0     1072 2023-04-24 15:46:54.657895 asyncpgdb-0.0.5/asyncpgdb/types/dsn.py
--rw-r--r--   0        0        0     1995 2023-04-24 17:21:31.315636 asyncpgdb-0.0.5/asyncpgdb/types/maps/__init__.py
--rw-r--r--   0        0        0     3147 2023-04-24 17:21:37.259989 asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      427 2023-04-24 15:40:06.471910 asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     2256 2023-04-24 17:16:47.189170 asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc
--rw-r--r--   0        0        0     5910 2023-04-24 17:16:47.187943 asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0      281 2023-04-24 15:32:16.634327 asyncpgdb-0.0.5/asyncpgdb/types/maps/base.py
--rw-r--r--   0        0        0     1430 2023-04-24 17:00:44.146569 asyncpgdb-0.0.5/asyncpgdb/types/maps/jsonifier.py
--rw-r--r--   0        0        0     6109 2023-04-24 17:00:15.902858 asyncpgdb-0.0.5/asyncpgdb/types/maps/util.py
--rw-r--r--   0        0        0        0 2023-04-24 14:10:13.542655 asyncpgdb-0.0.5/asyncpgdb/types/sql/__init__.py
--rw-r--r--   0        0        0      176 2023-04-24 14:16:23.734081 asyncpgdb-0.0.5/asyncpgdb/types/sql/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3160 2023-04-24 17:16:47.196672 asyncpgdb-0.0.5/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc
--rw-r--r--   0        0        0     4773 2023-04-24 17:16:47.194774 asyncpgdb-0.0.5/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc
--rw-r--r--   0        0        0     2375 2023-04-24 17:46:00.907302 asyncpgdb-0.0.5/asyncpgdb/types/sql/metadata.py
--rw-r--r--   0        0        0     4293 2023-04-24 17:22:11.716892 asyncpgdb-0.0.5/asyncpgdb/types/sql/stmt.py
--rw-r--r--   0        0        0      474 2023-04-24 17:46:06.806410 asyncpgdb-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 asyncpgdb-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-25 13:04:40.809165 asyncpgdb-0.0.6/README.md
+-rw-r--r--   0        0        0      894 2023-04-24 17:21:33.756204 asyncpgdb-0.0.6/asyncpgdb/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 13:45:42.124801 asyncpgdb-0.0.6/asyncpgdb/types/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-24 13:55:34.429438 asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6185 2023-04-24 17:21:37.382326 asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc
+-rw-r--r--   0        0        0     1074 2023-04-24 16:29:11.125800 asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc
+-rw-r--r--   0        0        0     4740 2023-04-24 14:06:39.702336 asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc
+-rw-r--r--   0        0        0     6844 2023-04-25 00:08:25.692681 asyncpgdb-0.0.6/asyncpgdb/types/connectionpool.py
+-rw-r--r--   0        0        0     1072 2023-04-24 15:46:54.657895 asyncpgdb-0.0.6/asyncpgdb/types/dsn.py
+-rw-r--r--   0        0        0     1995 2023-04-24 17:21:31.315636 asyncpgdb-0.0.6/asyncpgdb/types/maps/__init__.py
+-rw-r--r--   0        0        0     3147 2023-04-24 17:21:37.259989 asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      427 2023-04-24 15:40:06.471910 asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2256 2023-04-24 17:16:47.189170 asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc
+-rw-r--r--   0        0        0     5910 2023-04-24 17:16:47.187943 asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0      281 2023-04-24 15:32:16.634327 asyncpgdb-0.0.6/asyncpgdb/types/maps/base.py
+-rw-r--r--   0        0        0     1430 2023-04-24 17:00:44.146569 asyncpgdb-0.0.6/asyncpgdb/types/maps/jsonifier.py
+-rw-r--r--   0        0        0     6109 2023-04-24 17:00:15.902858 asyncpgdb-0.0.6/asyncpgdb/types/maps/util.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:10:13.542655 asyncpgdb-0.0.6/asyncpgdb/types/sql/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-24 14:16:23.734081 asyncpgdb-0.0.6/asyncpgdb/types/sql/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3160 2023-04-24 17:16:47.196672 asyncpgdb-0.0.6/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc
+-rw-r--r--   0        0        0     4773 2023-04-24 17:16:47.194774 asyncpgdb-0.0.6/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc
+-rw-r--r--   0        0        0     2375 2023-04-24 17:46:00.907302 asyncpgdb-0.0.6/asyncpgdb/types/sql/metadata.py
+-rw-r--r--   0        0        0     4293 2023-04-24 17:22:11.716892 asyncpgdb-0.0.6/asyncpgdb/types/sql/stmt.py
+-rw-r--r--   0        0        0      474 2023-04-25 00:08:41.305220 asyncpgdb-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 asyncpgdb-0.0.6/PKG-INFO
```

### Comparing `asyncpgdb-0.0.5/asyncpgdb/__init__.py` & `asyncpgdb-0.0.6/asyncpgdb/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/connectionpool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/dsn.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/__pycache__/stmt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/connectionpool.py` & `asyncpgdb-0.0.6/asyncpgdb/types/connectionpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
         await self.connect()
         try:
             if vars:
                 result = await self.connection.execute(query, *vars, timeout=timeout)
             else:
                 result = await self.connection.execute(query, timeout=timeout)
-        except:
-            result = "error"
+        except BaseException as error:
+            result = f"error: {str(error)}"
         finally:
             await self.close()
         return result
 
     async def executemany_raw(
         self,
         stmt: str,
@@ -102,15 +102,15 @@
             if vars:
                 result = await self.connection.executemany(
                     query, args=vars, timeout=timeout
                 )
             else:
                 result = await self.connection.executemany(query, timeout=timeout)
         except BaseException as error:
-            result = f"execute_raw.error:\n\n{str(error)}\n\n"
+            result = f"executemany_raw.error:\n\n{str(error)}\n\n"
         finally:
             await self.close()
         return result
 
     async def execute_raw(
         self,
         stmt: str,
@@ -193,16 +193,16 @@
             try:
 
                 result = await self.connection.executemany(
                     query, args=vars, timeout=timeout
                 )
                 result = "success"
 
-            except:
-                result = "error"
+            except BaseException as error:
+                result = f"upsert.error: {str(error)}"
             finally:
                 await self.close()
         else:
             result = "error: no vars to upsert"
         return result
 
     async def insert(
```

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/dsn.py` & `asyncpgdb-0.0.6/asyncpgdb/types/dsn.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/maps/__init__.py` & `asyncpgdb-0.0.6/asyncpgdb/types/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/jsonifier.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/maps/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/maps/jsonifier.py` & `asyncpgdb-0.0.6/asyncpgdb/types/maps/jsonifier.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/maps/util.py` & `asyncpgdb-0.0.6/asyncpgdb/types/maps/util.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/sql/__pycache__/metadata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc` & `asyncpgdb-0.0.6/asyncpgdb/types/sql/__pycache__/stmt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/sql/metadata.py` & `asyncpgdb-0.0.6/asyncpgdb/types/sql/metadata.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/asyncpgdb/types/sql/stmt.py` & `asyncpgdb-0.0.6/asyncpgdb/types/sql/stmt.py`

 * *Files identical despite different names*

### Comparing `asyncpgdb-0.0.5/PKG-INFO` & `asyncpgdb-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpgdb
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 License: MIT
 Author: wayfaring-stranger
 Author-email: zw6p226m@duck.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

