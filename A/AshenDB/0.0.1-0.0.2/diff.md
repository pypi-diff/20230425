# Comparing `tmp/AshenDB-0.0.1.tar.gz` & `tmp/AshenDB-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshenDB-0.0.1.tar", last modified: Sun Apr 23 07:23:49 2023, max compression
+gzip compressed data, was "AshenDB-0.0.2.tar", last modified: Tue Apr 25 04:03:28 2023, max compression
```

## Comparing `AshenDB-0.0.1.tar` & `AshenDB-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-23 07:23:49.121058 AshenDB-0.0.1/
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-23 07:23:49.120058 AshenDB-0.0.1/AshenDB.egg-info/
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-04-23 07:23:49.000000 AshenDB-0.0.1/AshenDB.egg-info/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-04-23 07:23:49.000000 AshenDB-0.0.1/AshenDB.egg-info/SOURCES.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-04-23 07:23:49.000000 AshenDB-0.0.1/AshenDB.egg-info/dependency_links.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-04-23 07:23:49.000000 AshenDB-0.0.1/AshenDB.egg-info/entry_points.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-04-23 07:23:49.000000 AshenDB-0.0.1/AshenDB.egg-info/requires.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-04-23 07:23:49.000000 AshenDB-0.0.1/AshenDB.egg-info/top_level.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.1/LICENSE
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-04-23 07:23:49.121058 AshenDB-0.0.1/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      300 2023-04-23 07:22:33.000000 AshenDB-0.0.1/README.rst
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-23 07:23:49.120058 AshenDB-0.0.1/ashendb/
--rw-r--r--   0 aurka     (1000) aurka     (1000)      518 2023-04-23 06:15:07.000000 AshenDB-0.0.1/ashendb/__init__.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2511 2023-04-23 06:15:07.000000 AshenDB-0.0.1/ashendb/client.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      881 2023-04-22 08:20:33.000000 AshenDB-0.0.1/ashendb/collection.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2302 2023-04-20 00:18:31.000000 AshenDB-0.0.1/ashendb/database.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      923 2023-04-22 08:20:09.000000 AshenDB-0.0.1/ashendb/document.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)       92 2023-04-23 05:42:40.000000 AshenDB-0.0.1/ashendb/exception.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     3439 2023-04-22 10:33:14.000000 AshenDB-0.0.1/ashendb/helper.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-04-23 07:16:23.000000 AshenDB-0.0.1/pyproject.toml
--rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-04-23 07:23:49.121058 AshenDB-0.0.1/setup.cfg
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-25 04:03:28.971755 AshenDB-0.0.2/
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-25 04:03:28.970755 AshenDB-0.0.2/AshenDB.egg-info/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-04-25 04:03:28.000000 AshenDB-0.0.2/AshenDB.egg-info/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-04-25 04:03:28.000000 AshenDB-0.0.2/AshenDB.egg-info/SOURCES.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-04-25 04:03:28.000000 AshenDB-0.0.2/AshenDB.egg-info/dependency_links.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-04-25 04:03:28.000000 AshenDB-0.0.2/AshenDB.egg-info/entry_points.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-04-25 04:03:28.000000 AshenDB-0.0.2/AshenDB.egg-info/requires.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-04-25 04:03:28.000000 AshenDB-0.0.2/AshenDB.egg-info/top_level.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.2/LICENSE
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-04-25 04:03:28.971755 AshenDB-0.0.2/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      300 2023-04-23 07:22:33.000000 AshenDB-0.0.2/README.rst
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-25 04:03:28.971755 AshenDB-0.0.2/ashendb/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      744 2023-04-25 03:52:03.000000 AshenDB-0.0.2/ashendb/__init__.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     6569 2023-04-25 03:31:02.000000 AshenDB-0.0.2/ashendb/client.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7588 2023-04-25 03:47:51.000000 AshenDB-0.0.2/ashendb/collection.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7416 2023-04-25 03:31:05.000000 AshenDB-0.0.2/ashendb/database.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      923 2023-04-22 08:20:09.000000 AshenDB-0.0.2/ashendb/document.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.2/ashendb/exception.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     3439 2023-04-22 10:33:14.000000 AshenDB-0.0.2/ashendb/helper.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-04-25 03:56:40.000000 AshenDB-0.0.2/pyproject.toml
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-04-25 04:03:28.971755 AshenDB-0.0.2/setup.cfg
```

### Comparing `AshenDB-0.0.1/AshenDB.egg-info/PKG-INFO` & `AshenDB-0.0.2/AshenDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.1
+Version: 0.0.2
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.1/LICENSE` & `AshenDB-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.1/PKG-INFO` & `AshenDB-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.1
+Version: 0.0.2
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.1/ashendb/document.py` & `AshenDB-0.0.2/ashendb/document.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.1/ashendb/helper.py` & `AshenDB-0.0.2/ashendb/helper.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.1/pyproject.toml` & `AshenDB-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AshenDB"
-version = "0.0.1"
+version = "0.0.2"
 description = "Another stupid library for using json as Database"
 readme = "README.rst"
 authors = [{name = "Abdullah Al Muaz", email = "abdullahalmuaz15@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
```

