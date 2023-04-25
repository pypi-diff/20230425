# Comparing `tmp/NewCode-Utils-1.0.5.tar.gz` & `tmp/NewCode-Utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NewCode-Utils-1.0.5.tar", last modified: Tue Apr 25 01:48:42 2023, max compression
+gzip compressed data, was "dist/NewCode-Utils-1.0.6.tar", last modified: Tue Apr 25 02:10:57 2023, max compression
```

## Comparing `NewCode-Utils-1.0.5.tar` & `NewCode-Utils-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 NewCode-Utils-1.0.5/LICENSE
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 NewCode-Utils-1.0.5/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1930 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      525 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.5/NewCode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/admins/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/admins/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/admins/audit_admin.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.5/NewCode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/utils.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/migrations/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.5/NewCode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/models/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/models/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/models/audit.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1930 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.5/README.md
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      755 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/setup.cfg
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 NewCode-Utils-1.0.5/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 NewCode-Utils-1.0.6/LICENSE
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 NewCode-Utils-1.0.6/MANIFEST.in
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_Utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2033 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      561 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      123 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_Utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_utils/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.6/NewCode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_utils/admins/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.6/NewCode_utils/admins/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.6/NewCode_utils/admins/audit_admin.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.6/NewCode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_utils/helpers/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.6/NewCode_utils/helpers/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.6/NewCode_utils/helpers/utils.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.6/NewCode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_utils/migrations/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.6/NewCode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/NewCode_utils/models/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.6/NewCode_utils/models/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.6/NewCode_utils/models/audit.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2033 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.6/README.md
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1050 2023-04-25 02:10:57.000000 NewCode-Utils-1.0.6/setup.cfg
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 NewCode-Utils-1.0.6/setup.py
```

### Comparing `NewCode-Utils-1.0.5/LICENSE` & `NewCode-Utils-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.5/NewCode_Utils.egg-info/PKG-INFO` & `NewCode-Utils-1.0.6/NewCode_Utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.5
+Version: 1.0.6
 Summary: Necessary elements for the development of apps.
-Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
+Home-page: UNKNOWN
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
@@ -67,9 +67,12 @@
 Keywords: django Audit
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-1.0.5/NewCode_utils/admins/audit_admin.py` & `NewCode-Utils-1.0.6/NewCode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.5/NewCode_utils/helpers/utils.py` & `NewCode-Utils-1.0.6/NewCode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.5/NewCode_utils/helpers/utils_permission_rest.py` & `NewCode-Utils-1.0.6/NewCode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.5/NewCode_utils/models/audit.py` & `NewCode-Utils-1.0.6/NewCode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.5/PKG-INFO` & `NewCode-Utils-1.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.5
+Version: 1.0.6
 Summary: Necessary elements for the development of apps.
-Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges.git
+Home-page: UNKNOWN
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
@@ -67,9 +67,12 @@
 Keywords: django Audit
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `NewCode-Utils-1.0.5/README.md` & `NewCode-Utils-1.0.6/README.md`

 * *Files identical despite different names*

