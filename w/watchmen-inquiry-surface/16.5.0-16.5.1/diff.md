# Comparing `tmp/watchmen_inquiry_surface-16.5.0.tar.gz` & `tmp/watchmen_inquiry_surface-16.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_surface-16.5.0.tar", max compression
+gzip compressed data, was "watchmen_inquiry_surface-16.5.1.tar", max compression
```

## Comparing `watchmen_inquiry_surface-16.5.0.tar` & `watchmen_inquiry_surface-16.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/LICENSE
--rw-r--r--   0        0        0     1304 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/src/watchmen_inquiry_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/src/watchmen_inquiry_surface/data/__init__.py
--rw-r--r--   0        0        0     9852 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/src/watchmen_inquiry_surface/data/data_router.py
--rw-r--r--   0        0        0      176 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/src/watchmen_inquiry_surface/main.py
--rw-r--r--   0        0        0      476 2023-04-06 09:13:10.392011 watchmen_inquiry_surface-16.5.0/src/watchmen_inquiry_surface/settings.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/LICENSE
+-rw-r--r--   0        0        0     1304 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/data/__init__.py
+-rw-r--r--   0        0        0     9852 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/data/data_router.py
+-rw-r--r--   0        0        0      176 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/main.py
+-rw-r--r--   0        0        0      476 2023-04-25 10:52:45.984220 watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/settings.py
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.1/PKG-INFO
```

### Comparing `watchmen_inquiry_surface-16.5.0/LICENSE` & `watchmen_inquiry_surface-16.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.5.0/pyproject.toml` & `watchmen_inquiry_surface-16.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-surface"
-version = "16.5.0"
+version = "16.5.1"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.0"
-watchmen-rest = "16.5.0"
-watchmen-inquiry-trino = { version = "16.5.0", optional = true }
-watchmen-storage-mysql = { version = "16.5.0", optional = true }
-watchmen-storage-oracle = { version = "16.5.0", optional = true }
-watchmen-storage-mongodb = { version = "16.5.0", optional = true }
-watchmen-storage-mssql = { version = "16.5.0", optional = true }
-watchmen-storage-postgresql = { version = "16.5.0", optional = true }
-watchmen-storage-oss = { version = "16.5.0", optional = true }
-watchmen-storage-s3 = { version = "16.5.0", optional = true }
+watchmen-inquiry-kernel = "16.5.1"
+watchmen-rest = "16.5.1"
+watchmen-inquiry-trino = { version = "16.5.1", optional = true }
+watchmen-storage-mysql = { version = "16.5.1", optional = true }
+watchmen-storage-oracle = { version = "16.5.1", optional = true }
+watchmen-storage-mongodb = { version = "16.5.1", optional = true }
+watchmen-storage-mssql = { version = "16.5.1", optional = true }
+watchmen-storage-postgresql = { version = "16.5.1", optional = true }
+watchmen-storage-oss = { version = "16.5.1", optional = true }
+watchmen-storage-s3 = { version = "16.5.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 trino = ["watchmen-inquiry-trino"]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_surface-16.5.0/src/watchmen_inquiry_surface/data/data_router.py` & `watchmen_inquiry_surface-16.5.1/src/watchmen_inquiry_surface/data/data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.5.0/PKG-INFO` & `watchmen_inquiry_surface-16.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-surface
-Version: 16.5.0
+Version: 16.5.1
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.0)
-Requires-Dist: watchmen-inquiry-trino (==16.5.0) ; extra == "trino"
-Requires-Dist: watchmen-rest (==16.5.0)
-Requires-Dist: watchmen-storage-mongodb (==16.5.0) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.0) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.0) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.0) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.0) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.0) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.0) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.1)
+Requires-Dist: watchmen-inquiry-trino (==16.5.1) ; extra == "trino"
+Requires-Dist: watchmen-rest (==16.5.1)
+Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
```

