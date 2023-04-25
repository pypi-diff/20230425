# Comparing `tmp/yawaei-0.0.7.tar.gz` & `tmp/yawaei-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yawaei-0.0.7.tar", last modified: Tue Apr 25 11:36:55 2023, max compression
+gzip compressed data, was "yawaei-0.0.8.tar", last modified: Tue Apr 25 12:47:14 2023, max compression
```

## Comparing `yawaei-0.0.7.tar` & `yawaei-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.887306 yawaei-0.0.7/
--rw-r--r--   0 julien    (1000) julien    (1000)     1073 2022-08-18 21:23:40.000000 yawaei-0.0.7/LICENSE
--rw-r--r--   0 julien    (1000) julien    (1000)     2571 2023-04-25 11:36:55.887306 yawaei-0.0.7/PKG-INFO
--rw-r--r--   0 julien    (1000) julien    (1000)      779 2022-09-29 09:20:08.000000 yawaei-0.0.7/README.md
--rw-r--r--   0 julien    (1000) julien    (1000)      682 2023-04-25 11:36:18.000000 yawaei-0.0.7/pyproject.toml
--rw-r--r--   0 julien    (1000) julien    (1000)       38 2023-04-25 11:36:55.890639 yawaei-0.0.7/setup.cfg
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.883972 yawaei-0.0.7/src/
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.887306 yawaei-0.0.7/src/Yawaei/
--rw-r--r--   0 julien    (1000) julien    (1000)       71 2022-09-14 13:32:53.000000 yawaei-0.0.7/src/Yawaei/__init__.py
--rw-r--r--   0 julien    (1000) julien    (1000)     3404 2022-10-06 12:02:29.000000 yawaei-0.0.7/src/Yawaei/abc.py
--rw-r--r--   0 julien    (1000) julien    (1000)     1243 2022-08-29 14:05:21.000000 yawaei-0.0.7/src/Yawaei/checkers.py
--rw-r--r--   0 julien    (1000) julien    (1000)      334 2022-09-14 12:57:27.000000 yawaei-0.0.7/src/Yawaei/constants.py
--rw-r--r--   0 julien    (1000) julien    (1000)     5027 2022-10-06 12:33:45.000000 yawaei-0.0.7/src/Yawaei/intranet.py
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.887306 yawaei-0.0.7/src/yawaei.egg-info/
--rw-r--r--   0 julien    (1000) julien    (1000)     2571 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/PKG-INFO
--rw-r--r--   0 julien    (1000) julien    (1000)      279 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/SOURCES.txt
--rw-r--r--   0 julien    (1000) julien    (1000)        1 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/dependency_links.txt
--rw-r--r--   0 julien    (1000) julien    (1000)        7 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/top_level.txt
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 12:47:14.639193 yawaei-0.0.8/
+-rw-r--r--   0 julien    (1000) julien    (1000)     1073 2022-08-18 21:23:40.000000 yawaei-0.0.8/LICENSE
+-rw-r--r--   0 julien    (1000) julien    (1000)     2571 2023-04-25 12:47:14.639193 yawaei-0.0.8/PKG-INFO
+-rw-r--r--   0 julien    (1000) julien    (1000)      779 2022-09-29 09:20:08.000000 yawaei-0.0.8/README.md
+-rw-r--r--   0 julien    (1000) julien    (1000)      682 2023-04-25 12:44:56.000000 yawaei-0.0.8/pyproject.toml
+-rw-r--r--   0 julien    (1000) julien    (1000)       38 2023-04-25 12:47:14.639193 yawaei-0.0.8/setup.cfg
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 12:47:14.635860 yawaei-0.0.8/src/
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 12:47:14.639193 yawaei-0.0.8/src/yawaei/
+-rw-r--r--   0 julien    (1000) julien    (1000)       71 2022-09-14 13:32:53.000000 yawaei-0.0.8/src/yawaei/__init__.py
+-rw-r--r--   0 julien    (1000) julien    (1000)     3404 2022-10-06 12:02:29.000000 yawaei-0.0.8/src/yawaei/abc.py
+-rw-r--r--   0 julien    (1000) julien    (1000)     1243 2022-08-29 14:05:21.000000 yawaei-0.0.8/src/yawaei/checkers.py
+-rw-r--r--   0 julien    (1000) julien    (1000)      334 2022-09-14 12:57:27.000000 yawaei-0.0.8/src/yawaei/constants.py
+-rw-r--r--   0 julien    (1000) julien    (1000)     5027 2022-10-06 12:33:45.000000 yawaei-0.0.8/src/yawaei/intranet.py
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 12:47:14.639193 yawaei-0.0.8/src/yawaei.egg-info/
+-rw-r--r--   0 julien    (1000) julien    (1000)     2571 2023-04-25 12:47:14.000000 yawaei-0.0.8/src/yawaei.egg-info/PKG-INFO
+-rw-r--r--   0 julien    (1000) julien    (1000)      279 2023-04-25 12:47:14.000000 yawaei-0.0.8/src/yawaei.egg-info/SOURCES.txt
+-rw-r--r--   0 julien    (1000) julien    (1000)        1 2023-04-25 12:47:14.000000 yawaei-0.0.8/src/yawaei.egg-info/dependency_links.txt
+-rw-r--r--   0 julien    (1000) julien    (1000)        7 2023-04-25 12:47:14.000000 yawaei-0.0.8/src/yawaei.egg-info/top_level.txt
```

### Comparing `yawaei-0.0.7/LICENSE` & `yawaei-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yawaei-0.0.7/PKG-INFO` & `yawaei-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yawaei
-Version: 0.0.7
+Version: 0.0.8
 Summary: Yet Another Wrapper Around Epitech Intranet
 Author-email: Aldon Julien <julien.aldon@epitech.eu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `yawaei-0.0.7/README.md` & `yawaei-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `yawaei-0.0.7/pyproject.toml` & `yawaei-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests==2.28.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yawaei"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Aldon Julien", email="julien.aldon@epitech.eu" },
 ]
 description = "Yet Another Wrapper Around Epitech Intranet"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `yawaei-0.0.7/src/Yawaei/abc.py` & `yawaei-0.0.8/src/yawaei/abc.py`

 * *Files identical despite different names*

### Comparing `yawaei-0.0.7/src/Yawaei/checkers.py` & `yawaei-0.0.8/src/yawaei/checkers.py`

 * *Files identical despite different names*

### Comparing `yawaei-0.0.7/src/Yawaei/intranet.py` & `yawaei-0.0.8/src/yawaei/intranet.py`

 * *Files identical despite different names*

### Comparing `yawaei-0.0.7/src/yawaei.egg-info/PKG-INFO` & `yawaei-0.0.8/src/yawaei.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yawaei
-Version: 0.0.7
+Version: 0.0.8
 Summary: Yet Another Wrapper Around Epitech Intranet
 Author-email: Aldon Julien <julien.aldon@epitech.eu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

