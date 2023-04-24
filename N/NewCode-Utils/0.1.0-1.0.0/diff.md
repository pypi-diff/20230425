# Comparing `tmp/NewCode-Utils-0.1.0.tar.gz` & `tmp/NewCode-Utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NewCode-Utils-0.1.0.tar", last modified: Mon Apr 24 21:07:06 2023, max compression
+gzip compressed data, was "dist/NewCode-Utils-1.0.0.tar", last modified: Mon Apr 24 21:52:29 2023, max compression
```

## Comparing `NewCode-Utils-0.1.0.tar` & `NewCode-Utils-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      109 2023-04-24 18:06:31.000000 NewCode-Utils-0.1.0/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_Utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1226 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_Utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      262 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_Utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/NewCode_utils/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 17:10:15.000000 NewCode-Utils-0.1.0/NewCode_utils/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 16:51:59.000000 NewCode-Utils-0.1.0/NewCode_utils/apps.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1226 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      596 2023-04-24 21:06:20.000000 NewCode-Utils-0.1.0/README.md
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-24 21:07:06.000000 NewCode-Utils-0.1.0/setup.cfg
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-24 21:07:04.000000 NewCode-Utils-0.1.0/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      109 2023-04-24 18:06:31.000000 NewCode-Utils-1.0.0/MANIFEST.in
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_Utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1226 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      262 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_Utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/NewCode_utils/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 17:10:15.000000 NewCode-Utils-1.0.0/NewCode_utils/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 16:51:59.000000 NewCode-Utils-1.0.0/NewCode_utils/apps.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1226 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      596 2023-04-24 21:09:01.000000 NewCode-Utils-1.0.0/README.md
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-24 21:52:29.000000 NewCode-Utils-1.0.0/setup.cfg
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-24 21:09:01.000000 NewCode-Utils-1.0.0/setup.py
```

### Comparing `NewCode-Utils-0.1.0/NewCode_Utils.egg-info/PKG-INFO` & `NewCode-Utils-1.0.0/NewCode_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 0.1.0
+Version: 1.0.0
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
         Basic components for the development of NewCode_
         
         ### Requirements
         1. Install pip
         
         ### Install
         ``` bash
-        pip install NewCode-Utils==0.0.1
+        pip install NewCode-Utils==1.0.0
         ```
         
         ### Components
         * Admin
           * AuditAdmin
           * AuditStackedInline
           * AuditTabularInline
@@ -36,14 +36,14 @@
         ``` bash
         pip install -U twine wheel setuptools
         ```
         * update repository
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-0.0.3*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.0*
         ```
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-0.1.0/PKG-INFO` & `NewCode-Utils-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 0.1.0
+Version: 1.0.0
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
         Basic components for the development of NewCode_
         
         ### Requirements
         1. Install pip
         
         ### Install
         ``` bash
-        pip install NewCode-Utils==0.0.1
+        pip install NewCode-Utils==1.0.0
         ```
         
         ### Components
         * Admin
           * AuditAdmin
           * AuditStackedInline
           * AuditTabularInline
@@ -36,14 +36,14 @@
         ``` bash
         pip install -U twine wheel setuptools
         ```
         * update repository
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-0.0.3*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.0*
         ```
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-0.1.0/README.md` & `NewCode-Utils-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Basic components for the development of NewCode_
 
 ### Requirements
 1. Install pip
 
 ### Install
 ``` bash
-pip install NewCode-Utils==0.0.1
+pip install NewCode-Utils==1.0.0
 ```
 
 ### Components
 * Admin
   * AuditAdmin
   * AuditStackedInline
   * AuditTabularInline
@@ -28,11 +28,11 @@
 ``` bash
 pip install -U twine wheel setuptools
 ```
 * update repository
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/NewCode-Utils-0.0.3*
+twine upload --repository pypi dist/NewCode-Utils-1.0.0*
 ```
```

### Comparing `NewCode-Utils-0.1.0/setup.py` & `NewCode-Utils-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name='NewCode-Utils',
-    version='0.1.0',
+    version='1.0.0',
     packages=['NewCode_utils'],
     description='Necessary elements for the development of apps.',
     long_description=README,
     long_description_content_type="text/markdown",
     author='NewCode_',
     author_email='new.code.2523@gmail.com',
     url='https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git',
```

