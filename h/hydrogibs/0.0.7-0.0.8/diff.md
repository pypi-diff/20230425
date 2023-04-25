# Comparing `tmp/hydrogibs-0.0.7.tar.gz` & `tmp/hydrogibs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.7.tar", last modified: Tue Apr 25 01:47:01 2023, max compression
+gzip compressed data, was "hydrogibs-0.0.8.tar", last modified: Tue Apr 25 01:48:01 2023, max compression
```

## Comparing `hydrogibs-0.0.7.tar` & `hydrogibs-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:47:01.497836 hydrogibs-0.0.7/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.7/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:47:01.493836 hydrogibs-0.0.7/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.7/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:47:01.493836 hydrogibs-0.0.7/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)    20256 2023-04-25 01:45:58.000000 hydrogibs-0.0.7/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      163 2023-04-25 01:34:02.000000 hydrogibs-0.0.7/hydrogibs/__init_.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.7/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:47:01.493836 hydrogibs-0.0.7/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:47:01.000000 hydrogibs-0.0.7/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 01:47:01.000000 hydrogibs-0.0.7/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 01:47:01.000000 hydrogibs-0.0.7/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 01:47:01.000000 hydrogibs-0.0.7/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 01:46:41.000000 hydrogibs-0.0.7/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 01:47:01.497836 hydrogibs-0.0.7/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.8/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.8/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:48:01.393835 hydrogibs-0.0.8/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    20256 2023-04-25 01:45:58.000000 hydrogibs-0.0.8/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      120 2023-04-25 01:47:38.000000 hydrogibs-0.0.8/hydrogibs/__init_.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.8/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 01:48:01.000000 hydrogibs-0.0.8/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 01:47:43.000000 hydrogibs-0.0.8/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 01:48:01.397836 hydrogibs-0.0.8/setup.cfg
```

### Comparing `hydrogibs-0.0.7/LICENSE` & `hydrogibs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.7/PKG-INFO` & `hydrogibs-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.0.7/hydrogibs/GR4.py` & `hydrogibs-0.0.8/hydrogibs/GR4.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.7/hydrogibs/misc.py` & `hydrogibs-0.0.8/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.7/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.0.8/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

