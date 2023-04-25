# Comparing `tmp/belt_logging-0.0.1.tar.gz` & `tmp/belt_logging-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belt_logging-0.0.1.tar", max compression
+gzip compressed data, was "belt_logging-0.0.2a0.tar", max compression
```

## Comparing `belt_logging-0.0.1.tar` & `belt_logging-0.0.2a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-24 09:00:38.701303 belt_logging-0.0.1/LICENSE
--rw-r--r--   0        0        0     1440 2023-04-24 09:00:38.701303 belt_logging-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-24 09:00:38.701303 belt_logging-0.0.1/belt_logging/__init__.py
--rw-r--r--   0        0        0      267 2023-04-24 09:00:38.701303 belt_logging-0.0.1/belt_logging/foo.py
--rw-r--r--   0        0        0     1834 2023-04-24 09:00:38.701303 belt_logging-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 belt_logging-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-25 09:46:48.608612 belt_logging-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0     1440 2023-04-25 09:46:48.608612 belt_logging-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 09:46:48.608612 belt_logging-0.0.2a0/belt_logging/__init__.py
+-rw-r--r--   0        0        0      267 2023-04-25 09:46:48.608612 belt_logging-0.0.2a0/belt_logging/foo.py
+-rw-r--r--   0        0        0     1837 2023-04-25 09:47:11.672900 belt_logging-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 belt_logging-0.0.2a0/PKG-INFO
```

### Comparing `belt_logging-0.0.1/README.md` & `belt_logging-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `belt_logging-0.0.1/pyproject.toml` & `belt_logging-0.0.2a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "belt_logging"
-version = "0.0.1"
+version = "0.0.2a0"
 description = "Belt python logging library"
 authors = ["Belt Software <frishi.mishra@belt.io>"]
 repository = "https://github.com/BeltSoftware/belt-plogging"
 documentation = "https://BeltSoftware.github.io/belt-plogging/"
 readme = "README.md"
 packages = [
   {include = "belt_logging"}
@@ -88,14 +88,14 @@
     "E731",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S101"]
 
 [tool.coverage.report]
-skip_empty = true
+skip_empty = false
 
 [tool.coverage.run]
 branch = true
 source = ["belt_logging"]
```

### Comparing `belt_logging-0.0.1/PKG-INFO` & `belt_logging-0.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belt-logging
-Version: 0.0.1
+Version: 0.0.2a0
 Summary: Belt python logging library
 Home-page: https://github.com/BeltSoftware/belt-plogging
 Author: Belt Software
 Author-email: frishi.mishra@belt.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

