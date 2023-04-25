# Comparing `tmp/pyecotrend-ista-2.0.7.tar.gz` & `tmp/pyecotrend-ista-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecotrend-ista-2.0.7.tar", last modified: Tue Apr 25 08:05:02 2023, max compression
+gzip compressed data, was "pyecotrend-ista-2.0.8.tar", last modified: Tue Apr 25 08:14:18 2023, max compression
```

## Comparing `pyecotrend-ista-2.0.7.tar` & `pyecotrend-ista-2.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:02.432847 pyecotrend-ista-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:05:02.428847 pyecotrend-ista-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:05:02.432847 pyecotrend-ista-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:02.428847 pyecotrend-ista-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:02.428847 pyecotrend-ista-2.0.7/src/pyecotrend_ista/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista/helper_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista/ista_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-04-25 08:04:50.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista/pyecotrend_ista.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:02.428847 pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:05:02.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 08:05:02.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:05:02.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 08:05:02.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 08:05:02.000000 pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.753484 pyecotrend-ista-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.753484 pyecotrend-ista-2.0.8/src/pyecotrend_ista/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/helper_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/ista_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/pyecotrend_ista.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/top_level.txt
```

### Comparing `pyecotrend-ista-2.0.7/LICENSE` & `pyecotrend-ista-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.7/PKG-INFO` & `pyecotrend-ista-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

### Comparing `pyecotrend-ista-2.0.7/README.md` & `pyecotrend-ista-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.7/setup.py` & `pyecotrend-ista-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import setuptools
 import configparser
 
+import setuptools
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("./src/pyecotrend_ista/const.py") as f:
     config_string = "[dummy_section]\n" + f.read()
     config = configparser.ConfigParser(allow_no_value=True)
     config.read_string(config_string)
```

### Comparing `pyecotrend-ista-2.0.7/src/pyecotrend_ista/helper_object.py` & `pyecotrend-ista-2.0.8/src/pyecotrend_ista/helper_object.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.7/src/pyecotrend_ista/ista_object.py` & `pyecotrend-ista-2.0.8/src/pyecotrend_ista/ista_object.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.7/src/pyecotrend_ista/pyecotrend_ista.py` & `pyecotrend-ista-2.0.8/src/pyecotrend_ista/pyecotrend_ista.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.7/src/pyecotrend_ista.egg-info/PKG-INFO` & `pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

