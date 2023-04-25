# Comparing `tmp/hydrogibs-0.0.5.tar.gz` & `tmp/hydrogibs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.5.tar", last modified: Tue Apr 25 01:07:55 2023, max compression
+gzip compressed data, was "hydrogibs-0.0.6.tar", last modified: Tue Apr 25 01:10:29 2023, max compression
```

## Comparing `hydrogibs-0.0.5.tar` & `hydrogibs-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:07:55.173559 hydrogibs-0.0.5/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.5/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:07:55.173559 hydrogibs-0.0.5/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.5/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:07:55.169559 hydrogibs-0.0.5/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)    17759 2023-04-25 01:07:03.000000 hydrogibs-0.0.5/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       56 2023-04-24 23:46:38.000000 hydrogibs-0.0.5/hydrogibs/__init_.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.5/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:07:55.169559 hydrogibs-0.0.5/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:07:55.000000 hydrogibs-0.0.5/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 01:07:55.000000 hydrogibs-0.0.5/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 01:07:55.000000 hydrogibs-0.0.5/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 01:07:55.000000 hydrogibs-0.0.5/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 01:07:41.000000 hydrogibs-0.0.5/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 01:07:55.173559 hydrogibs-0.0.5/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:10:29.102588 hydrogibs-0.0.6/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.6/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:10:29.102588 hydrogibs-0.0.6/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.6/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:10:29.098588 hydrogibs-0.0.6/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    17759 2023-04-25 01:07:03.000000 hydrogibs-0.0.6/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       44 2023-04-25 01:09:50.000000 hydrogibs-0.0.6/hydrogibs/__init_.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.6/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 01:10:29.102588 hydrogibs-0.0.6/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 01:10:29.000000 hydrogibs-0.0.6/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 01:10:29.000000 hydrogibs-0.0.6/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 01:10:29.000000 hydrogibs-0.0.6/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 01:10:29.000000 hydrogibs-0.0.6/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 01:10:08.000000 hydrogibs-0.0.6/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 01:10:29.102588 hydrogibs-0.0.6/setup.cfg
```

### Comparing `hydrogibs-0.0.5/LICENSE` & `hydrogibs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.5/PKG-INFO` & `hydrogibs-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.0.5/hydrogibs/GR4.py` & `hydrogibs-0.0.6/hydrogibs/GR4.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.5/hydrogibs/misc.py` & `hydrogibs-0.0.6/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.5/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.0.6/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

