# Comparing `tmp/NewCode-Utils-1.0.1.tar.gz` & `tmp/NewCode-Utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NewCode-Utils-1.0.1.tar", last modified: Mon Apr 24 23:27:08 2023, max compression
+gzip compressed data, was "dist/NewCode-Utils-1.0.2.tar", last modified: Mon Apr 24 23:52:39 2023, max compression
```

## Comparing `NewCode-Utils-1.0.1.tar` & `NewCode-Utils-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      109 2023-04-24 18:06:31.000000 NewCode-Utils-1.0.1/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_Utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1292 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_Utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      262 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_Utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/NewCode_utils/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.1/NewCode_utils/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.1/NewCode_utils/apps.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1292 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      638 2023-04-24 23:26:38.000000 NewCode-Utils-1.0.1/README.md
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-24 23:27:08.000000 NewCode-Utils-1.0.1/setup.cfg
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-24 23:27:06.000000 NewCode-Utils-1.0.1/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      153 2023-04-24 23:49:01.000000 NewCode-Utils-1.0.2/MANIFEST.in
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_Utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      543 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_Utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_utils/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.2/NewCode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_utils/admins/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.2/NewCode_utils/admins/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.2/NewCode_utils/admins/audit_admin.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.2/NewCode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_utils/helpers/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.2/NewCode_utils/helpers/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.2/NewCode_utils/helpers/utils.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.2/NewCode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_utils/migrations/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.2/NewCode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/NewCode_utils/models/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.2/NewCode_utils/models/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.2/NewCode_utils/models/audit.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-24 23:52:04.000000 NewCode-Utils-1.0.2/README.md
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-24 23:52:39.000000 NewCode-Utils-1.0.2/setup.cfg
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-24 23:52:35.000000 NewCode-Utils-1.0.2/setup.py
```

### Comparing `NewCode-Utils-1.0.1/NewCode_Utils.egg-info/PKG-INFO` & `NewCode-Utils-1.0.2/NewCode_Utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
         Basic components for the development of NewCode_
         
         ### Requirements
+        
         1. Install pip
         
         ### Install
+        
         ``` bash
-        pip install NewCode-Utils==1.0.1
+        pip install NewCode-Utils==1.0.2
         ```
-        ### settings.py
+        
+        Quick start
+        -----------
         ``` bash
-        NewCode_utils
+        
+        1. Add "NewCode_utils" to your INSTALLED_APPS setting like this::
+        INSTALLED_APPS = [
+                ...
+                'NewCode_utils',
+            ]
         ```
+        
         ### Components
+        
         * Admin
-          * AuditAdmin
-          * AuditStackedInline
-          * AuditTabularInline
+            * AuditAdmin
+            * AuditStackedInline
+            * AuditTabularInline
         * Models
-          * Audit
+            * Audit
         * Helpers
-          * Utils
-            * File departments of columbia
-          * Utils permission rest
-        
+            * Utils
+                * File departments of columbia
+            * Utils permission rest
         
         ### Deploy pypi versions
-        * install requirements 
+        
+        * install requirements
+        
         ``` bash
         pip install -U twine wheel setuptools
         ```
+        
         * update repository
+        
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-1.0.1*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.2*
         ```
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-1.0.1/PKG-INFO` & `NewCode-Utils-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
         Basic components for the development of NewCode_
         
         ### Requirements
+        
         1. Install pip
         
         ### Install
+        
         ``` bash
-        pip install NewCode-Utils==1.0.1
+        pip install NewCode-Utils==1.0.2
         ```
-        ### settings.py
+        
+        Quick start
+        -----------
         ``` bash
-        NewCode_utils
+        
+        1. Add "NewCode_utils" to your INSTALLED_APPS setting like this::
+        INSTALLED_APPS = [
+                ...
+                'NewCode_utils',
+            ]
         ```
+        
         ### Components
+        
         * Admin
-          * AuditAdmin
-          * AuditStackedInline
-          * AuditTabularInline
+            * AuditAdmin
+            * AuditStackedInline
+            * AuditTabularInline
         * Models
-          * Audit
+            * Audit
         * Helpers
-          * Utils
-            * File departments of columbia
-          * Utils permission rest
-        
+            * Utils
+                * File departments of columbia
+            * Utils permission rest
         
         ### Deploy pypi versions
-        * install requirements 
+        
+        * install requirements
+        
         ``` bash
         pip install -U twine wheel setuptools
         ```
+        
         * update repository
+        
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-1.0.1*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.2*
         ```
         
         
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-1.0.1/setup.py` & `NewCode-Utils-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name='NewCode-Utils',
-    version='1.0.1',
+    version='1.0.2',
     packages=['NewCode_utils'],
     description='Necessary elements for the development of apps.',
     long_description=README,
     long_description_content_type="text/markdown",
     author='NewCode_',
     author_email='new.code.2523@gmail.com',
     url='https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git',
```

