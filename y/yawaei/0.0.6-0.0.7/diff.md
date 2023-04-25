# Comparing `tmp/Yawaei-0.0.6.tar.gz` & `tmp/yawaei-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Yawaei-0.0.6.tar", last modified: Thu Oct  6 12:36:26 2022, max compression
+gzip compressed data, was "yawaei-0.0.7.tar", last modified: Tue Apr 25 11:36:55 2023, max compression
```

## Comparing `Yawaei-0.0.6.tar` & `yawaei-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2022-10-06 12:36:26.338217 Yawaei-0.0.6/
--rw-r--r--   0 julien    (1000) julien    (1000)     1073 2022-08-18 21:23:40.000000 Yawaei-0.0.6/LICENSE
--rw-r--r--   0 julien    (1000) julien    (1000)     2571 2022-10-06 12:36:26.338217 Yawaei-0.0.6/PKG-INFO
--rw-r--r--   0 julien    (1000) julien    (1000)      779 2022-09-29 09:20:08.000000 Yawaei-0.0.6/README.md
--rw-r--r--   0 julien    (1000) julien    (1000)      682 2022-10-06 12:34:57.000000 Yawaei-0.0.6/pyproject.toml
--rw-r--r--   0 julien    (1000) julien    (1000)       38 2022-10-06 12:36:26.338217 Yawaei-0.0.6/setup.cfg
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2022-10-06 12:36:26.334884 Yawaei-0.0.6/src/
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2022-10-06 12:36:26.334884 Yawaei-0.0.6/src/Yawaei/
--rw-r--r--   0 julien    (1000) julien    (1000)       71 2022-09-14 13:32:53.000000 Yawaei-0.0.6/src/Yawaei/__init__.py
--rw-r--r--   0 julien    (1000) julien    (1000)     3404 2022-10-06 12:02:29.000000 Yawaei-0.0.6/src/Yawaei/abc.py
--rw-r--r--   0 julien    (1000) julien    (1000)     1243 2022-08-29 14:05:21.000000 Yawaei-0.0.6/src/Yawaei/checkers.py
--rw-r--r--   0 julien    (1000) julien    (1000)      334 2022-09-14 12:57:27.000000 Yawaei-0.0.6/src/Yawaei/constants.py
--rw-r--r--   0 julien    (1000) julien    (1000)     5027 2022-10-06 12:33:45.000000 Yawaei-0.0.6/src/Yawaei/intranet.py
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2022-10-06 12:36:26.334884 Yawaei-0.0.6/src/Yawaei.egg-info/
--rw-r--r--   0 julien    (1000) julien    (1000)     2571 2022-10-06 12:36:26.000000 Yawaei-0.0.6/src/Yawaei.egg-info/PKG-INFO
--rw-r--r--   0 julien    (1000) julien    (1000)      279 2022-10-06 12:36:26.000000 Yawaei-0.0.6/src/Yawaei.egg-info/SOURCES.txt
--rw-r--r--   0 julien    (1000) julien    (1000)        1 2022-10-06 12:36:26.000000 Yawaei-0.0.6/src/Yawaei.egg-info/dependency_links.txt
--rw-r--r--   0 julien    (1000) julien    (1000)        7 2022-10-06 12:36:26.000000 Yawaei-0.0.6/src/Yawaei.egg-info/top_level.txt
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.887306 yawaei-0.0.7/
+-rw-r--r--   0 julien    (1000) julien    (1000)     1073 2022-08-18 21:23:40.000000 yawaei-0.0.7/LICENSE
+-rw-r--r--   0 julien    (1000) julien    (1000)     2571 2023-04-25 11:36:55.887306 yawaei-0.0.7/PKG-INFO
+-rw-r--r--   0 julien    (1000) julien    (1000)      779 2022-09-29 09:20:08.000000 yawaei-0.0.7/README.md
+-rw-r--r--   0 julien    (1000) julien    (1000)      682 2023-04-25 11:36:18.000000 yawaei-0.0.7/pyproject.toml
+-rw-r--r--   0 julien    (1000) julien    (1000)       38 2023-04-25 11:36:55.890639 yawaei-0.0.7/setup.cfg
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.883972 yawaei-0.0.7/src/
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.887306 yawaei-0.0.7/src/Yawaei/
+-rw-r--r--   0 julien    (1000) julien    (1000)       71 2022-09-14 13:32:53.000000 yawaei-0.0.7/src/Yawaei/__init__.py
+-rw-r--r--   0 julien    (1000) julien    (1000)     3404 2022-10-06 12:02:29.000000 yawaei-0.0.7/src/Yawaei/abc.py
+-rw-r--r--   0 julien    (1000) julien    (1000)     1243 2022-08-29 14:05:21.000000 yawaei-0.0.7/src/Yawaei/checkers.py
+-rw-r--r--   0 julien    (1000) julien    (1000)      334 2022-09-14 12:57:27.000000 yawaei-0.0.7/src/Yawaei/constants.py
+-rw-r--r--   0 julien    (1000) julien    (1000)     5027 2022-10-06 12:33:45.000000 yawaei-0.0.7/src/Yawaei/intranet.py
+drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-04-25 11:36:55.887306 yawaei-0.0.7/src/yawaei.egg-info/
+-rw-r--r--   0 julien    (1000) julien    (1000)     2571 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/PKG-INFO
+-rw-r--r--   0 julien    (1000) julien    (1000)      279 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/SOURCES.txt
+-rw-r--r--   0 julien    (1000) julien    (1000)        1 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/dependency_links.txt
+-rw-r--r--   0 julien    (1000) julien    (1000)        7 2023-04-25 11:36:55.000000 yawaei-0.0.7/src/yawaei.egg-info/top_level.txt
```

### Comparing `Yawaei-0.0.6/LICENSE` & `yawaei-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Yawaei-0.0.6/PKG-INFO` & `yawaei-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: Yawaei
-Version: 0.0.6
-Summary: Yet Another Wrapper Arount Epitech Intranet
+Name: yawaei
+Version: 0.0.7
+Summary: Yet Another Wrapper Around Epitech Intranet
 Author-email: Aldon Julien <julien.aldon@epitech.eu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `Yawaei-0.0.6/README.md` & `yawaei-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Yawaei-0.0.6/pyproject.toml` & `yawaei-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests==2.28.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "Yawaei"
-version = "0.0.6"
+name = "yawaei"
+version = "0.0.7"
 authors = [
   { name="Aldon Julien", email="julien.aldon@epitech.eu" },
 ]
-description = "Yet Another Wrapper Arount Epitech Intranet"
+description = "Yet Another Wrapper Around Epitech Intranet"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `Yawaei-0.0.6/src/Yawaei/abc.py` & `yawaei-0.0.7/src/Yawaei/abc.py`

 * *Files identical despite different names*

### Comparing `Yawaei-0.0.6/src/Yawaei/checkers.py` & `yawaei-0.0.7/src/Yawaei/checkers.py`

 * *Files identical despite different names*

### Comparing `Yawaei-0.0.6/src/Yawaei/intranet.py` & `yawaei-0.0.7/src/Yawaei/intranet.py`

 * *Files identical despite different names*

### Comparing `Yawaei-0.0.6/src/Yawaei.egg-info/PKG-INFO` & `yawaei-0.0.7/src/yawaei.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: Yawaei
-Version: 0.0.6
-Summary: Yet Another Wrapper Arount Epitech Intranet
+Name: yawaei
+Version: 0.0.7
+Summary: Yet Another Wrapper Around Epitech Intranet
 Author-email: Aldon Julien <julien.aldon@epitech.eu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

