# Comparing `tmp/NewCode-Utils-1.0.3.tar.gz` & `tmp/NewCode-Utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NewCode-Utils-1.0.3.tar", last modified: Tue Apr 25 00:43:50 2023, max compression
+gzip compressed data, was "dist/NewCode-Utils-1.0.4.tar", last modified: Tue Apr 25 01:01:52 2023, max compression
```

## Comparing `NewCode-Utils-1.0.3.tar` & `NewCode-Utils-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      321 2023-04-25 00:43:13.000000 NewCode-Utils-1.0.3/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_Utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_Utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      543 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_Utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_utils/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.3/NewCode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_utils/admins/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.3/NewCode_utils/admins/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.3/NewCode_utils/admins/audit_admin.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.3/NewCode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_utils/helpers/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.3/NewCode_utils/helpers/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.3/NewCode_utils/helpers/utils.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.3/NewCode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_utils/migrations/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.3/NewCode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/NewCode_utils/models/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.3/NewCode_utils/models/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.3/NewCode_utils/models/audit.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-25 00:43:37.000000 NewCode-Utils-1.0.3/README.md
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 00:43:50.000000 NewCode-Utils-1.0.3/setup.cfg
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-25 00:43:37.000000 NewCode-Utils-1.0.3/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      271 2023-04-25 01:01:42.000000 NewCode-Utils-1.0.4/MANIFEST.in
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      543 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.4/NewCode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/admins/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/admins/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/admins/audit_admin.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.4/NewCode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/utils.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/migrations/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.4/NewCode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/models/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/models/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/models/audit.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.4/README.md
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/setup.cfg
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.4/setup.py
```

### Comparing `NewCode-Utils-1.0.3/NewCode_Utils.egg-info/PKG-INFO` & `NewCode-Utils-1.0.4/NewCode_Utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
@@ -13,15 +13,15 @@
         ### Requirements
         
         1. Install pip
         
         ### Install
         
         ``` bash
-        pip install NewCode-Utils==1.0.3
+        pip install NewCode-Utils==1.0.4
         ```
         
         Quick start
         -----------
         ``` bash
         
         1. Add "NewCode_utils" to your INSTALLED_APPS setting like this::
@@ -53,14 +53,14 @@
         ```
         
         * update repository
         
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-1.0.3*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.4*
         ```
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-1.0.3/NewCode_Utils.egg-info/SOURCES.txt` & `NewCode-Utils-1.0.4/NewCode_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.3/NewCode_utils/admins/audit_admin.py` & `NewCode-Utils-1.0.4/NewCode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.3/NewCode_utils/helpers/utils.py` & `NewCode-Utils-1.0.4/NewCode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.3/NewCode_utils/helpers/utils_permission_rest.py` & `NewCode-Utils-1.0.4/NewCode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.3/NewCode_utils/models/audit.py` & `NewCode-Utils-1.0.4/NewCode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.3/PKG-INFO` & `NewCode-Utils-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
@@ -13,15 +13,15 @@
         ### Requirements
         
         1. Install pip
         
         ### Install
         
         ``` bash
-        pip install NewCode-Utils==1.0.3
+        pip install NewCode-Utils==1.0.4
         ```
         
         Quick start
         -----------
         ``` bash
         
         1. Add "NewCode_utils" to your INSTALLED_APPS setting like this::
@@ -53,14 +53,14 @@
         ```
         
         * update repository
         
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-1.0.3*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.4*
         ```
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-1.0.3/README.md` & `NewCode-Utils-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ### Requirements
 
 1. Install pip
 
 ### Install
 
 ``` bash
-pip install NewCode-Utils==1.0.3
+pip install NewCode-Utils==1.0.4
 ```
 
 Quick start
 -----------
 ``` bash
 
 1. Add "NewCode_utils" to your INSTALLED_APPS setting like this::
@@ -45,11 +45,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/NewCode-Utils-1.0.3*
+twine upload --repository pypi dist/NewCode-Utils-1.0.4*
 ```
```

### Comparing `NewCode-Utils-1.0.3/setup.py` & `NewCode-Utils-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name='NewCode-Utils',
-    version='1.0.3',
+    version='1.0.4',
     packages=['NewCode_utils'],
     description='Necessary elements for the development of apps.',
     long_description=README,
     long_description_content_type="text/markdown",
     author='NewCode_',
     author_email='new.code.2523@gmail.com',
     url='https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git',
```

