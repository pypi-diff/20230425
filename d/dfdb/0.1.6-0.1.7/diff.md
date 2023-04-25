# Comparing `tmp/dfdb-0.1.6.tar.gz` & `tmp/dfdb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfdb-0.1.6.tar", last modified: Fri Mar 31 03:14:18 2023, max compression
+gzip compressed data, was "dfdb-0.1.7.tar", last modified: Tue Apr 25 00:35:48 2023, max compression
```

## Comparing `dfdb-0.1.6.tar` & `dfdb-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-31 03:14:18.340772 dfdb-0.1.6/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2023-03-25 18:57:15.000000 dfdb-0.1.6/LICENSE
--rw-r--r--   0 hoyinchau   (501) staff       (20)       28 2023-03-30 21:11:25.000000 dfdb-0.1.6/MANIFEST.in
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1766 2023-03-31 03:14:18.340641 dfdb-0.1.6/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)       60 2023-03-25 18:57:15.000000 dfdb-0.1.6/README.md
--rw-r--r--   0 hoyinchau   (501) staff       (20)      713 2023-03-31 03:14:12.000000 dfdb-0.1.6/pyproject.toml
--rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-03-31 03:14:18.340805 dfdb-0.1.6/setup.cfg
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-31 03:14:18.337586 dfdb-0.1.6/src/
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-31 03:14:18.339706 dfdb-0.1.6/src/dfdb/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       94 2023-03-26 21:37:06.000000 dfdb-0.1.6/src/dfdb/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      514 2023-03-30 22:10:58.000000 dfdb-0.1.6/src/dfdb/abc.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      108 2023-03-27 05:07:02.000000 dfdb-0.1.6/src/dfdb/config.toml
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2729 2023-03-30 22:17:28.000000 dfdb-0.1.6/src/dfdb/database.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    16028 2023-03-31 03:06:08.000000 dfdb-0.1.6/src/dfdb/dataframe.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3300 2023-03-29 06:04:05.000000 dfdb-0.1.6/src/dfdb/parsing.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-31 03:14:18.340484 dfdb-0.1.6/src/dfdb.egg-info/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1766 2023-03-31 03:14:18.000000 dfdb-0.1.6/src/dfdb.egg-info/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)      324 2023-03-31 03:14:18.000000 dfdb-0.1.6/src/dfdb.egg-info/SOURCES.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-03-31 03:14:18.000000 dfdb-0.1.6/src/dfdb.egg-info/dependency_links.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)       39 2023-03-31 03:14:18.000000 dfdb-0.1.6/src/dfdb.egg-info/requires.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        5 2023-03-31 03:14:18.000000 dfdb-0.1.6/src/dfdb.egg-info/top_level.txt
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 00:35:48.314623 dfdb-0.1.7/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2023-03-25 18:57:15.000000 dfdb-0.1.7/LICENSE
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       28 2023-03-30 21:11:25.000000 dfdb-0.1.7/MANIFEST.in
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1766 2023-04-25 00:35:48.314452 dfdb-0.1.7/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       60 2023-03-25 18:57:15.000000 dfdb-0.1.7/README.md
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      772 2023-04-16 02:44:58.000000 dfdb-0.1.7/pyproject.toml
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-04-25 00:35:48.314670 dfdb-0.1.7/setup.cfg
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 00:35:48.309939 dfdb-0.1.7/src/
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 00:35:48.313004 dfdb-0.1.7/src/dfdb/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      243 2023-04-16 02:48:50.000000 dfdb-0.1.7/src/dfdb/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2554 2023-04-25 00:33:03.000000 dfdb-0.1.7/src/dfdb/abc.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2337 2023-04-23 19:21:24.000000 dfdb-0.1.7/src/dfdb/alter.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      239 2023-04-25 00:20:09.000000 dfdb-0.1.7/src/dfdb/config.toml
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     8528 2023-04-22 20:25:34.000000 dfdb-0.1.7/src/dfdb/database.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    53962 2023-04-24 23:52:39.000000 dfdb-0.1.7/src/dfdb/dataframe.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1454 2023-04-23 19:35:06.000000 dfdb-0.1.7/src/dfdb/defs.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3300 2023-03-29 06:04:05.000000 dfdb-0.1.7/src/dfdb/parsing.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     6093 2023-04-16 03:58:20.000000 dfdb-0.1.7/src/dfdb/triggers.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7579 2023-04-25 00:19:29.000000 dfdb-0.1.7/src/dfdb/types.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 00:35:48.314068 dfdb-0.1.7/src/dfdb.egg-info/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1766 2023-04-25 00:35:48.000000 dfdb-0.1.7/src/dfdb.egg-info/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      421 2023-04-25 00:35:48.000000 dfdb-0.1.7/src/dfdb.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-04-25 00:35:48.000000 dfdb-0.1.7/src/dfdb.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       60 2023-04-25 00:35:48.000000 dfdb-0.1.7/src/dfdb.egg-info/requires.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        5 2023-04-25 00:35:48.000000 dfdb-0.1.7/src/dfdb.egg-info/top_level.txt
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 00:35:48.314212 dfdb-0.1.7/test/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    25156 2023-04-25 00:33:45.000000 dfdb-0.1.7/test/test_dataframe.py
```

### Comparing `dfdb-0.1.6/LICENSE` & `dfdb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.6/PKG-INFO` & `dfdb-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdb
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pandas-like interface for manipulating SQL databases.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dfdb-0.1.6/pyproject.toml` & `dfdb-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfdb"
-version = "0.1.6"
+version = "0.1.7"
 description = "Pandas-like interface for manipulating SQL databases."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
@@ -16,14 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     'numpy',
-    'pandas',
-    'SQLAlchemy',
-    'hyclib>=0.1.11',
+    'pandas>=2.0.0',
+    'SQLAlchemy>=2.0.0',
+    'hyclib>=0.1.13',
+    'addict', # attribute access for options
 ]
 
 [project.urls]
 repository = "https://github.com/hchau630/dfdb"
```

### Comparing `dfdb-0.1.6/src/dfdb/parsing.py` & `dfdb-0.1.7/src/dfdb/parsing.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.6/src/dfdb.egg-info/PKG-INFO` & `dfdb-0.1.7/src/dfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdb
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pandas-like interface for manipulating SQL databases.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

