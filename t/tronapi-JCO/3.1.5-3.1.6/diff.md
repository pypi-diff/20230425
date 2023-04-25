# Comparing `tmp/tronapi-JCO-3.1.5.tar.gz` & `tmp/tronapi-JCO-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tronapi-JCO-3.1.5.tar", last modified: Fri Apr 21 10:05:40 2023, max compression
+gzip compressed data, was "tronapi-JCO-3.1.6.tar", last modified: Mon Apr 24 14:22:10 2023, max compression
```

## Comparing `tronapi-JCO-3.1.5.tar` & `tronapi-JCO-3.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-21 10:05:40.026771 tronapi-JCO-3.1.5/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1064 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/LICENSE
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5369 2023-04-21 10:05:40.026610 tronapi-JCO-3.1.5/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4586 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/README.rst
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       38 2023-04-21 10:05:40.026819 tronapi-JCO-3.1.5/setup.cfg
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3126 2023-04-21 10:05:26.000000 tronapi-JCO-3.1.5/setup.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-21 10:05:40.022233 tronapi-JCO-3.1.5/tronapi/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      712 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-21 10:05:40.024834 tronapi-JCO-3.1.5/tronapi/common/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    15063 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/abi.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3192 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/account.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1328 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/blocks.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4862 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/contracts.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     6408 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/datastructures.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1520 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/datatypes.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7948 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/encoding.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1781 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/formatters.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1820 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/normalizers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3280 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/threads.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-21 10:05:40.025027 tronapi-JCO-3.1.5/tronapi/common/toolz/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1013 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/toolz/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/transactions.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     6614 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/common/validation.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      582 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/constants.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    12561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/contract.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2329 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/exceptions.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    11311 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/main.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4231 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/manager.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1009 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/module.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-21 10:05:40.025533 tronapi-JCO-3.1.5/tronapi/providers/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/providers/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1382 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/providers/base.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4661 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.5/tronapi/providers/http.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    41363 2023-04-21 10:00:43.000000 tronapi-JCO-3.1.5/tronapi/transactionbuilder.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    32719 2023-04-21 10:01:26.000000 tronapi-JCO-3.1.5/tronapi/trx.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-21 10:05:40.026391 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5369 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      892 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/SOURCES.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/dependency_links.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/not-zip-safe
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      974 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/requires.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        8 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.5/tronapi_JCO.egg-info/top_level.txt
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-24 14:22:10.853388 tronapi-JCO-3.1.6/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1064 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/LICENSE
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-24 14:22:10.853205 tronapi-JCO-3.1.6/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4590 2023-04-21 10:07:20.000000 tronapi-JCO-3.1.6/README.rst
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       38 2023-04-24 14:22:10.853442 tronapi-JCO-3.1.6/setup.cfg
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3126 2023-04-24 14:21:56.000000 tronapi-JCO-3.1.6/setup.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-24 14:22:10.847814 tronapi-JCO-3.1.6/tronapi/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      716 2023-04-24 14:21:45.000000 tronapi-JCO-3.1.6/tronapi/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-24 14:22:10.850601 tronapi-JCO-3.1.6/tronapi/common/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    15063 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/abi.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3192 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/account.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1328 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/blocks.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4862 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/contracts.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     6408 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/datastructures.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1520 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/datatypes.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     7948 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/encoding.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1781 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/formatters.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1820 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/normalizers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3280 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/threads.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-24 14:22:10.850819 tronapi-JCO-3.1.6/tronapi/common/toolz/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1013 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/toolz/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/transactions.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     6614 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/common/validation.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      582 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/constants.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    12561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/contract.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2329 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/exceptions.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    11311 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/main.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4231 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/manager.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1009 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/module.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-24 14:22:10.851552 tronapi-JCO-3.1.6/tronapi/providers/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/providers/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1382 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/providers/base.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4661 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.6/tronapi/providers/http.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    41363 2023-04-21 10:00:43.000000 tronapi-JCO-3.1.6/tronapi/transactionbuilder.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    32719 2023-04-21 10:01:26.000000 tronapi-JCO-3.1.6/tronapi/trx.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-24 14:22:10.852911 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-24 14:22:10.000000 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      892 2023-04-24 14:22:10.000000 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/SOURCES.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-24 14:22:10.000000 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/dependency_links.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/not-zip-safe
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      974 2023-04-24 14:22:10.000000 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/requires.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        8 2023-04-24 14:22:10.000000 tronapi-JCO-3.1.6/tronapi_JCO.egg-info/top_level.txt
```

### Comparing `tronapi-JCO-3.1.5/LICENSE` & `tronapi-JCO-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/PKG-INFO` & `tronapi-JCO-3.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tronapi-JCO
-Version: 3.1.5
+Version: 3.1.6
 Summary: A Python API for interacting with Tron (Forked from tronapi)
 Home-page: https://github.com/RastinS/tron-api-JCO
 Author: Rustin Soraki
 Author-email: rustin.souraki@gmail.com
 License: MIT License
 Keywords: tron tron-api tron-api-python iexbase
 Classifier: Development Status :: 3 - Alpha
@@ -51,15 +51,15 @@
 
 **A Command-Line Interface framework**
 
 You can install it in a system-wide location via pip:
 
 .. code-block:: bash
 
-    sudo pip3 install tronapi
+    sudo pip3 install tronapi-JCO
 
 Or install it locally using `virtualenv <https://github.com/pypa/virtualenv>`__:
 
 .. code-block:: bash
 
     virtualenv -p /usr/bin/python3 ~/tronapi
     source ~/tronapi/bin/activate
```

### Comparing `tronapi-JCO-3.1.5/README.rst` & `tronapi-JCO-3.1.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 **A Command-Line Interface framework**
 
 You can install it in a system-wide location via pip:
 
 .. code-block:: bash
 
-    sudo pip3 install tronapi
+    sudo pip3 install tronapi-JCO
 
 Or install it locally using `virtualenv <https://github.com/pypa/virtualenv>`__:
 
 .. code-block:: bash
 
     virtualenv -p /usr/bin/python3 ~/tronapi
     source ~/tronapi/bin/activate
```

### Comparing `tronapi-JCO-3.1.5/setup.py` & `tronapi-JCO-3.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import (
     find_packages,
     setup,
 )
 
 py_version = platform.python_version()
 
-PACKAGE_VERSION = "3.1.5"
+PACKAGE_VERSION = "3.1.6"
 
 EXTRAS_REQUIRE = {
     "tester": ["coverage", "pep8", "pyflakes", "pylint", "pytest-cov"],
     "docs": [
         "mock",
         "sphinx-better-theme>=0.1.4",
         "click>=5.1",
```

### Comparing `tronapi-JCO-3.1.5/tronapi/__init__.py` & `tronapi-JCO-3.1.6/tronapi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tronapi.providers.http import HttpProvider  # noqa: E402
 from tronapi.main import Tron  # noqa: E402
 
 if sys.version_info < (3, 5):
     raise EnvironmentError("Python 3.5 or above is required")
 
 
-__version__ = pkg_resources.get_distribution("tronapi").version
+__version__ = pkg_resources.get_distribution("tronapi-JCO").version
 
 __all__ = [
-    '__version__',
-    'HttpProvider',
-    'Account',
-    'Tron',
+    "__version__",
+    "HttpProvider",
+    "Account",
+    "Tron",
 ]
```

### Comparing `tronapi-JCO-3.1.5/tronapi/common/abi.py` & `tronapi-JCO-3.1.6/tronapi/common/abi.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/account.py` & `tronapi-JCO-3.1.6/tronapi/common/account.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/blocks.py` & `tronapi-JCO-3.1.6/tronapi/common/blocks.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/contracts.py` & `tronapi-JCO-3.1.6/tronapi/common/contracts.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/datastructures.py` & `tronapi-JCO-3.1.6/tronapi/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/datatypes.py` & `tronapi-JCO-3.1.6/tronapi/common/datatypes.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/encoding.py` & `tronapi-JCO-3.1.6/tronapi/common/encoding.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/formatters.py` & `tronapi-JCO-3.1.6/tronapi/common/formatters.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/normalizers.py` & `tronapi-JCO-3.1.6/tronapi/common/normalizers.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/threads.py` & `tronapi-JCO-3.1.6/tronapi/common/threads.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/toolz/__init__.py` & `tronapi-JCO-3.1.6/tronapi/common/toolz/__init__.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/transactions.py` & `tronapi-JCO-3.1.6/tronapi/common/transactions.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/common/validation.py` & `tronapi-JCO-3.1.6/tronapi/common/validation.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/constants.py` & `tronapi-JCO-3.1.6/tronapi/constants.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/contract.py` & `tronapi-JCO-3.1.6/tronapi/contract.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/exceptions.py` & `tronapi-JCO-3.1.6/tronapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/main.py` & `tronapi-JCO-3.1.6/tronapi/main.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/manager.py` & `tronapi-JCO-3.1.6/tronapi/manager.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/module.py` & `tronapi-JCO-3.1.6/tronapi/module.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/providers/base.py` & `tronapi-JCO-3.1.6/tronapi/providers/base.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/providers/http.py` & `tronapi-JCO-3.1.6/tronapi/providers/http.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/transactionbuilder.py` & `tronapi-JCO-3.1.6/tronapi/transactionbuilder.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi/trx.py` & `tronapi-JCO-3.1.6/tronapi/trx.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi_JCO.egg-info/PKG-INFO` & `tronapi-JCO-3.1.6/tronapi_JCO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tronapi-JCO
-Version: 3.1.5
+Version: 3.1.6
 Summary: A Python API for interacting with Tron (Forked from tronapi)
 Home-page: https://github.com/RastinS/tron-api-JCO
 Author: Rustin Soraki
 Author-email: rustin.souraki@gmail.com
 License: MIT License
 Keywords: tron tron-api tron-api-python iexbase
 Classifier: Development Status :: 3 - Alpha
@@ -51,15 +51,15 @@
 
 **A Command-Line Interface framework**
 
 You can install it in a system-wide location via pip:
 
 .. code-block:: bash
 
-    sudo pip3 install tronapi
+    sudo pip3 install tronapi-JCO
 
 Or install it locally using `virtualenv <https://github.com/pypa/virtualenv>`__:
 
 .. code-block:: bash
 
     virtualenv -p /usr/bin/python3 ~/tronapi
     source ~/tronapi/bin/activate
```

### Comparing `tronapi-JCO-3.1.5/tronapi_JCO.egg-info/SOURCES.txt` & `tronapi-JCO-3.1.6/tronapi_JCO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.5/tronapi_JCO.egg-info/requires.txt` & `tronapi-JCO-3.1.6/tronapi_JCO.egg-info/requires.txt`

 * *Files identical despite different names*

