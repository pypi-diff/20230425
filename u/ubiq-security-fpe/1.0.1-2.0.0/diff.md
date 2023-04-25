# Comparing `tmp/ubiq-security-fpe-1.0.1.tar.gz` & `tmp/ubiq-security-fpe-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubiq-security-fpe-1.0.1.tar", last modified: Tue Mar 21 07:05:14 2023, max compression
+gzip compressed data, was "ubiq-security-fpe-2.0.0.tar", last modified: Tue Apr 25 06:23:23 2023, max compression
```

## Comparing `ubiq-security-fpe-1.0.1.tar` & `ubiq-security-fpe-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 07:05:14.065474 ubiq-security-fpe-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1104 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5364 2023-03-21 07:05:14.065474 ubiq-security-fpe-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4381 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 07:05:14.065474 ubiq-security-fpe-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1599 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 07:05:14.065474 ubiq-security-fpe-1.0.1/ubiq_security_fpe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3081 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe/ff1.py
--rw-r--r--   0 root         (0) root         (0)     4437 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe/ff1_test.py
--rw-r--r--   0 root         (0) root         (0)     2437 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe/ffx.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-03-21 06:37:57.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe/ffx_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 07:05:14.065474 ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5364 2023-03-21 07:05:14.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      370 2023-03-21 07:05:14.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 07:05:14.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-21 07:05:14.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-21 07:05:14.000000 ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:23:23.765676 ubiq-security-fpe-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-04-25 06:23:23.765676 ubiq-security-fpe-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 06:23:23.765676 ubiq-security-fpe-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-24 23:10:27.000000 ubiq-security-fpe-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:23:23.765676 ubiq-security-fpe-2.0.0/ubiq_security_fpe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe/ff1.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe/ff1_test.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe/ffx.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-03-21 06:37:57.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe/ffx_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:23:23.765676 ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-04-25 06:23:23.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-25 06:23:23.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 06:23:23.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 06:23:23.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 06:23:23.000000 ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/top_level.txt
```

### Comparing `ubiq-security-fpe-1.0.1/LICENSE` & `ubiq-security-fpe-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubiq-security-fpe-1.0.1/PKG-INFO` & `ubiq-security-fpe-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security-fpe
-Version: 1.0.1
+Version: 2.0.0
 Summary: Python client library for format preserving encryption
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-fpe-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ubiq-security-fpe-1.0.1/README.md` & `ubiq-security-fpe-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ubiq-security-fpe-1.0.1/setup.py` & `ubiq-security-fpe-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 install_requires = []
 if os.path.isfile(requirementPath):
     with open(requirementPath, "r", encoding="utf-8") as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="ubiq-security-fpe",
-    version="1.0.1",
+    version="2.0.0",
     author="Ubiq Security, Inc.",
     author_email="support@ubiqsecurity.com",
     description="Python client library for format preserving encryption",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/ubiqsecurity/ubiq-fpe-python",
     packages=setuptools.find_packages(),
```

### Comparing `ubiq-security-fpe-1.0.1/ubiq_security_fpe/ff1.py` & `ubiq-security-fpe-2.0.0/ubiq_security_fpe/ff1.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-fpe-1.0.1/ubiq_security_fpe/ff1_test.py` & `ubiq-security-fpe-2.0.0/ubiq_security_fpe/ff1_test.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-fpe-1.0.1/ubiq_security_fpe/ffx.py` & `ubiq-security-fpe-2.0.0/ubiq_security_fpe/ffx.py`

 * *Files identical despite different names*

### Comparing `ubiq-security-fpe-1.0.1/ubiq_security_fpe.egg-info/PKG-INFO` & `ubiq-security-fpe-2.0.0/ubiq_security_fpe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubiq-security-fpe
-Version: 1.0.1
+Version: 2.0.0
 Summary: Python client library for format preserving encryption
 Home-page: https://gitlab.com/ubiqsecurity/ubiq-fpe-python
 Author: Ubiq Security, Inc.
 Author-email: support@ubiqsecurity.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

