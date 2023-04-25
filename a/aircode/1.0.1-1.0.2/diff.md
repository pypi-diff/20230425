# Comparing `tmp/aircode-1.0.1.tar.gz` & `tmp/aircode-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aircode-1.0.1.tar", last modified: Tue Apr 25 12:00:34 2023, max compression
+gzip compressed data, was "aircode-1.0.2.tar", last modified: Tue Apr 25 12:05:17 2023, max compression
```

## Comparing `aircode-1.0.1.tar` & `aircode-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 diu       (1000) diu       (1000)        0 2023-04-25 12:00:34.275786 aircode-1.0.1/
--rw-rw-r--   0 diu       (1000) diu       (1000)      513 2023-04-25 12:00:34.275786 aircode-1.0.1/PKG-INFO
-drwxrwxr-x   0 diu       (1000) diu       (1000)        0 2023-04-25 12:00:34.275786 aircode-1.0.1/aircode.egg-info/
--rw-rw-r--   0 diu       (1000) diu       (1000)      513 2023-04-25 12:00:34.000000 aircode-1.0.1/aircode.egg-info/PKG-INFO
--rw-rw-r--   0 diu       (1000) diu       (1000)      177 2023-04-25 12:00:34.000000 aircode-1.0.1/aircode.egg-info/SOURCES.txt
--rw-rw-r--   0 diu       (1000) diu       (1000)        1 2023-04-25 12:00:34.000000 aircode-1.0.1/aircode.egg-info/dependency_links.txt
--rw-rw-r--   0 diu       (1000) diu       (1000)       42 2023-04-25 12:00:34.000000 aircode-1.0.1/aircode.egg-info/entry_points.txt
--rw-rw-r--   0 diu       (1000) diu       (1000)        8 2023-04-25 12:00:34.000000 aircode-1.0.1/aircode.egg-info/top_level.txt
--rw-rw-r--   0 diu       (1000) diu       (1000)      113 2023-04-25 11:53:49.000000 aircode-1.0.1/aircode.py
--rw-rw-r--   0 diu       (1000) diu       (1000)       38 2023-04-25 12:00:34.275786 aircode-1.0.1/setup.cfg
--rw-rw-r--   0 diu       (1000) diu       (1000)      691 2023-04-25 12:00:24.000000 aircode-1.0.1/setup.py
+drwxrwxr-x   0 diu       (1000) diu       (1000)        0 2023-04-25 12:05:17.513105 aircode-1.0.2/
+-rw-rw-r--   0 diu       (1000) diu       (1000)      513 2023-04-25 12:05:17.513105 aircode-1.0.2/PKG-INFO
+drwxrwxr-x   0 diu       (1000) diu       (1000)        0 2023-04-25 12:05:17.513105 aircode-1.0.2/aircode.egg-info/
+-rw-rw-r--   0 diu       (1000) diu       (1000)      513 2023-04-25 12:05:17.000000 aircode-1.0.2/aircode.egg-info/PKG-INFO
+-rw-rw-r--   0 diu       (1000) diu       (1000)      177 2023-04-25 12:05:17.000000 aircode-1.0.2/aircode.egg-info/SOURCES.txt
+-rw-rw-r--   0 diu       (1000) diu       (1000)        1 2023-04-25 12:05:17.000000 aircode-1.0.2/aircode.egg-info/dependency_links.txt
+-rw-rw-r--   0 diu       (1000) diu       (1000)       42 2023-04-25 12:05:17.000000 aircode-1.0.2/aircode.egg-info/entry_points.txt
+-rw-rw-r--   0 diu       (1000) diu       (1000)        8 2023-04-25 12:05:17.000000 aircode-1.0.2/aircode.egg-info/top_level.txt
+-rw-rw-r--   0 diu       (1000) diu       (1000)      544 2023-04-25 12:05:00.000000 aircode-1.0.2/aircode.py
+-rw-rw-r--   0 diu       (1000) diu       (1000)       38 2023-04-25 12:05:17.513105 aircode-1.0.2/setup.cfg
+-rw-rw-r--   0 diu       (1000) diu       (1000)      691 2023-04-25 12:05:07.000000 aircode-1.0.2/setup.py
```

### Comparing `aircode-1.0.1/PKG-INFO` & `aircode-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aircode
-Version: 1.0.1
+Version: 1.0.2
 Summary: Enjoy!
 Home-page: https://github.com/H454NSec/aircode
 Author: H454NSec
 Author-email: mrhasan660066@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aircode-1.0.1/aircode.egg-info/PKG-INFO` & `aircode-1.0.2/aircode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aircode
-Version: 1.0.1
+Version: 1.0.2
 Summary: Enjoy!
 Home-page: https://github.com/H454NSec/aircode
 Author: H454NSec
 Author-email: mrhasan660066@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aircode-1.0.1/setup.py` & `aircode-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='aircode',
-    version='1.0.1',
+    version='1.0.2',
     py_modules=['aircode'],
     entry_points={
         'console_scripts': [
             'aircode=aircode:main'
         ]
     },
     install_requires=[],
```

