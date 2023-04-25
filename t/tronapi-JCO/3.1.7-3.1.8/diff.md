# Comparing `tmp/tronapi-JCO-3.1.7.tar.gz` & `tmp/tronapi-JCO-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tronapi-JCO-3.1.7.tar", last modified: Tue Apr 25 09:48:53 2023, max compression
+gzip compressed data, was "tronapi-JCO-3.1.8.tar", last modified: Tue Apr 25 11:06:52 2023, max compression
```

## Comparing `tronapi-JCO-3.1.7.tar` & `tronapi-JCO-3.1.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 09:48:53.669415 tronapi-JCO-3.1.7/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1064 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/LICENSE
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 09:48:53.669245 tronapi-JCO-3.1.7/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4590 2023-04-21 10:07:20.000000 tronapi-JCO-3.1.7/README.rst
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       38 2023-04-25 09:48:53.669458 tronapi-JCO-3.1.7/setup.cfg
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3126 2023-04-25 09:48:51.000000 tronapi-JCO-3.1.7/setup.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 09:48:53.665567 tronapi-JCO-3.1.7/tronapi/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      716 2023-04-24 14:21:45.000000 tronapi-JCO-3.1.7/tronapi/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 09:48:53.667248 tronapi-JCO-3.1.7/tronapi/common/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    15063 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/abi.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3192 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/account.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1328 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/blocks.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4862 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/contracts.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     6408 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/datastructures.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1520 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/datatypes.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7948 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/encoding.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1781 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/formatters.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1820 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/normalizers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3280 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/threads.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 09:48:53.667384 tronapi-JCO-3.1.7/tronapi/common/toolz/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1013 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/toolz/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/transactions.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     6614 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/common/validation.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      582 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/constants.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    12561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/contract.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2329 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/exceptions.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    11311 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/main.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4231 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/manager.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1009 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/module.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 09:48:53.667761 tronapi-JCO-3.1.7/tronapi/providers/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/providers/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1382 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/providers/base.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4661 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.7/tronapi/providers/http.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    42814 2023-04-25 09:47:25.000000 tronapi-JCO-3.1.7/tronapi/transactionbuilder.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    33600 2023-04-25 09:47:56.000000 tronapi-JCO-3.1.7/tronapi/trx.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 09:48:53.669034 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 09:48:53.000000 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      892 2023-04-25 09:48:53.000000 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/SOURCES.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-25 09:48:53.000000 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/dependency_links.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/not-zip-safe
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      974 2023-04-25 09:48:53.000000 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/requires.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        8 2023-04-25 09:48:53.000000 tronapi-JCO-3.1.7/tronapi_JCO.egg-info/top_level.txt
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.881456 tronapi-JCO-3.1.8/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1064 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/LICENSE
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 11:06:52.881309 tronapi-JCO-3.1.8/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4590 2023-04-21 10:07:20.000000 tronapi-JCO-3.1.8/README.rst
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       38 2023-04-25 11:06:52.881494 tronapi-JCO-3.1.8/setup.cfg
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3126 2023-04-25 11:06:50.000000 tronapi-JCO-3.1.8/setup.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.875629 tronapi-JCO-3.1.8/tronapi/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      716 2023-04-24 14:21:45.000000 tronapi-JCO-3.1.8/tronapi/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.879514 tronapi-JCO-3.1.8/tronapi/common/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    15063 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/abi.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3192 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/account.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1328 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/blocks.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4862 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/contracts.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     6408 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/datastructures.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1520 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/datatypes.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     7948 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/encoding.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1781 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/formatters.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1820 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/normalizers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3280 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/threads.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.879727 tronapi-JCO-3.1.8/tronapi/common/toolz/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1013 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/toolz/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/transactions.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     6614 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/validation.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      582 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/constants.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    12561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/contract.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2329 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/exceptions.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    11311 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/main.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4231 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/manager.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1009 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/module.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.880192 tronapi-JCO-3.1.8/tronapi/providers/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/providers/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1382 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/providers/base.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4661 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/providers/http.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    43709 2023-04-25 11:06:34.000000 tronapi-JCO-3.1.8/tronapi/transactionbuilder.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    34240 2023-04-25 09:59:51.000000 tronapi-JCO-3.1.8/tronapi/trx.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.881133 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      892 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/SOURCES.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/dependency_links.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/not-zip-safe
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      974 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/requires.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        8 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/top_level.txt
```

### Comparing `tronapi-JCO-3.1.7/LICENSE` & `tronapi-JCO-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/PKG-INFO` & `tronapi-JCO-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tronapi-JCO
-Version: 3.1.7
+Version: 3.1.8
 Summary: A Python API for interacting with Tron (Forked from tronapi)
 Home-page: https://github.com/RastinS/tron-api-JCO
 Author: Rustin Soraki
 Author-email: rustin.souraki@gmail.com
 License: MIT License
 Keywords: tron tron-api tron-api-python iexbase
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tronapi-JCO-3.1.7/README.rst` & `tronapi-JCO-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/setup.py` & `tronapi-JCO-3.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import (
     find_packages,
     setup,
 )
 
 py_version = platform.python_version()
 
-PACKAGE_VERSION = "3.1.7"
+PACKAGE_VERSION = "3.1.8"
 
 EXTRAS_REQUIRE = {
     "tester": ["coverage", "pep8", "pyflakes", "pylint", "pytest-cov"],
     "docs": [
         "mock",
         "sphinx-better-theme>=0.1.4",
         "click>=5.1",
```

### Comparing `tronapi-JCO-3.1.7/tronapi/__init__.py` & `tronapi-JCO-3.1.8/tronapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/abi.py` & `tronapi-JCO-3.1.8/tronapi/common/abi.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/account.py` & `tronapi-JCO-3.1.8/tronapi/common/account.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/blocks.py` & `tronapi-JCO-3.1.8/tronapi/common/blocks.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/contracts.py` & `tronapi-JCO-3.1.8/tronapi/common/contracts.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/datastructures.py` & `tronapi-JCO-3.1.8/tronapi/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/datatypes.py` & `tronapi-JCO-3.1.8/tronapi/common/datatypes.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/encoding.py` & `tronapi-JCO-3.1.8/tronapi/common/encoding.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/formatters.py` & `tronapi-JCO-3.1.8/tronapi/common/formatters.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/normalizers.py` & `tronapi-JCO-3.1.8/tronapi/common/normalizers.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/threads.py` & `tronapi-JCO-3.1.8/tronapi/common/threads.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/toolz/__init__.py` & `tronapi-JCO-3.1.8/tronapi/common/toolz/__init__.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/transactions.py` & `tronapi-JCO-3.1.8/tronapi/common/transactions.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/common/validation.py` & `tronapi-JCO-3.1.8/tronapi/common/validation.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/constants.py` & `tronapi-JCO-3.1.8/tronapi/constants.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/contract.py` & `tronapi-JCO-3.1.8/tronapi/contract.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/exceptions.py` & `tronapi-JCO-3.1.8/tronapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/main.py` & `tronapi-JCO-3.1.8/tronapi/main.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/manager.py` & `tronapi-JCO-3.1.8/tronapi/manager.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/module.py` & `tronapi-JCO-3.1.8/tronapi/module.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/providers/base.py` & `tronapi-JCO-3.1.8/tronapi/providers/base.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/providers/http.py` & `tronapi-JCO-3.1.8/tronapi/providers/http.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi/transactionbuilder.py` & `tronapi-JCO-3.1.8/tronapi/transactionbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         # If the address of the sender is not specified, we prescribe the default
         if account is None:
             account = self.tron.default_address.hex
 
         if not self.tron.isAddress(to):
             raise InvalidTronError("Invalid recipient address provided")
 
-        if not isinstance(amount, float) or amount <= 0:
+        if not isinstance(amount, float) or not isinstance(amount, int) or amount <= 0:
             raise InvalidTronError("Invalid amount provided")
 
         _to = self.tron.address.to_hex(to)
         _from = self.tron.address.to_hex(account)
 
         if _to == _from:
             raise TronError("Cannot transfer TRX to the same account")
@@ -194,14 +194,42 @@
             },
         )
 
         if "Error" in response:
             raise ValueError(response["Error"])
 
         return response
+
+    def withdraw_expire_unfreeze(self, account=None):
+        """
+        Withdraw unfrozen balance in Stake2.0.
+        the user can call this API to get back their funds.
+        After executing /wallet/unfreezebalancev2 transaction and waiting N days, N is a network parameter
+
+        Args:
+            account (str): address that owns the staked trx
+
+        """
+        if account is None:
+            account = self.tron.default_address.hex
+
+        if not self.tron.isAddress(account):
+            raise InvalidTronError("Invalid address provided")
+
+        response = self.tron.manager.request(
+            "/wallet/withdrawexpireunfreeze",
+            {
+                "owner_address": self.tron.address.to_hex(account),
+            },
+        )
+
+        if "Error" in response:
+            raise ValueError(response["Error"])
+
+        return response
 
     def delegate_resource(
         self, amount=0, resource="BANDWIDTH", receiver=None, lock=False, account=None
     ):
         """
         Delegate resource to another account.
         Will give bandwidth OR Energy and TRON Power(voting rights)
```

### Comparing `tronapi-JCO-3.1.7/tronapi/trx.py` & `tronapi-JCO-3.1.8/tronapi/trx.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,34 @@
             amount, resource, account
         )
         sign = self.sign(transaction)
         response = self.broadcast(sign)
 
         return response
 
+    def withdraw_expire_unfreeze(self, account=None):
+        """
+        Withdraw unfrozen balance in Stake2.0.
+        the user can call this API to get back their funds.
+        After executing /wallet/unfreezebalancev2 transaction and waiting N days, N is a network parameter
+
+        Args:
+            account (str): address that owns the staked trx
+
+        """
+
+        if account is None:
+            account = self.tron.default_address.hex
+
+        transaction = self.tron.transaction_builder.withdraw_expire_unfreeze(account)
+        sign = self.sign(transaction)
+        response = self.broadcast(sign)
+
+        return response
+
     def delegate_resource(
         self, amount=0, resource="BANDWIDTH", receiver=None, lock=False, account=None
     ):
         """
         Delegate resource to another account.
         Will give bandwidth OR Energy and TRON Power(voting rights)
         to the receiver of the frozen tokens.
```

### Comparing `tronapi-JCO-3.1.7/tronapi_JCO.egg-info/PKG-INFO` & `tronapi-JCO-3.1.8/tronapi_JCO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tronapi-JCO
-Version: 3.1.7
+Version: 3.1.8
 Summary: A Python API for interacting with Tron (Forked from tronapi)
 Home-page: https://github.com/RastinS/tron-api-JCO
 Author: Rustin Soraki
 Author-email: rustin.souraki@gmail.com
 License: MIT License
 Keywords: tron tron-api tron-api-python iexbase
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tronapi-JCO-3.1.7/tronapi_JCO.egg-info/SOURCES.txt` & `tronapi-JCO-3.1.8/tronapi_JCO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.7/tronapi_JCO.egg-info/requires.txt` & `tronapi-JCO-3.1.8/tronapi_JCO.egg-info/requires.txt`

 * *Files identical despite different names*

