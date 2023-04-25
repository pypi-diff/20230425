# Comparing `tmp/NewCode-Utils-1.0.8.tar.gz` & `tmp/NewCode-Utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NewCode-Utils-1.0.8.tar", last modified: Tue Apr 25 02:21:32 2023, max compression
+gzip compressed data, was "dist/NewCode-Utils-1.0.9.tar", last modified: Tue Apr 25 02:22:45 2023, max compression
```

## Comparing `NewCode-Utils-1.0.8.tar` & `NewCode-Utils-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 NewCode-Utils-1.0.8/LICENSE
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 NewCode-Utils-1.0.8/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_Utils.egg-info/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2034 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_Utils.egg-info/PKG-INFO
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      561 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_Utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_Utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      123 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_Utils.egg-info/requires.txt
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_utils/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.8/NewCode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_utils/admins/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.8/NewCode_utils/admins/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.8/NewCode_utils/admins/audit_admin.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.8/NewCode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_utils/helpers/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.8/NewCode_utils/helpers/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.8/NewCode_utils/helpers/utils.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.8/NewCode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_utils/migrations/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.8/NewCode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/NewCode_utils/models/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.8/NewCode_utils/models/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.8/NewCode_utils/models/audit.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2034 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/PKG-INFO
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      785 2023-04-25 02:21:30.000000 NewCode-Utils-1.0.8/README.md
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1046 2023-04-25 02:21:32.000000 NewCode-Utils-1.0.8/setup.cfg
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 NewCode-Utils-1.0.8/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 NewCode-Utils-1.0.9/LICENSE
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 NewCode-Utils-1.0.9/MANIFEST.in
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_Utils.egg-info/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2083 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_Utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      561 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_Utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_Utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      123 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_Utils.egg-info/requires.txt
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_utils/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.9/NewCode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_utils/admins/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.9/NewCode_utils/admins/__init__.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.9/NewCode_utils/admins/audit_admin.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.9/NewCode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_utils/helpers/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.9/NewCode_utils/helpers/__init__.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.9/NewCode_utils/helpers/utils.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.9/NewCode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_utils/migrations/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.9/NewCode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/NewCode_utils/models/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.9/NewCode_utils/models/__init__.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.9/NewCode_utils/models/audit.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2083 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/PKG-INFO
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      785 2023-04-25 02:22:41.000000 NewCode-Utils-1.0.9/README.md
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1109 2023-04-25 02:22:45.000000 NewCode-Utils-1.0.9/setup.cfg
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 NewCode-Utils-1.0.9/setup.py
```

### Comparing `NewCode-Utils-1.0.8/LICENSE` & `NewCode-Utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.8/NewCode_Utils.egg-info/PKG-INFO` & `NewCode-Utils-1.0.9/NewCode_Utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Necessary elements for the development of apps.
-Home-page: UNKNOWN
+Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
@@ -55,15 +55,15 @@
         ```
         
         * update repository
         
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-1.0.8*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.9*
         ```
         
         
         
 Keywords: django Audit
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `NewCode-Utils-1.0.8/NewCode_Utils.egg-info/SOURCES.txt` & `NewCode-Utils-1.0.9/NewCode_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.8/NewCode_utils/admins/audit_admin.py` & `NewCode-Utils-1.0.9/NewCode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.8/NewCode_utils/helpers/utils.py` & `NewCode-Utils-1.0.9/NewCode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.8/NewCode_utils/helpers/utils_permission_rest.py` & `NewCode-Utils-1.0.9/NewCode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.8/NewCode_utils/models/audit.py` & `NewCode-Utils-1.0.9/NewCode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.8/PKG-INFO` & `NewCode-Utils-1.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: NewCode-Utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Necessary elements for the development of apps.
-Home-page: UNKNOWN
+Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 License: MIT
 Description: ### New Code Utils
         
@@ -55,15 +55,15 @@
         ```
         
         * update repository
         
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/NewCode-Utils-1.0.8*
+        twine upload --repository pypi dist/NewCode-Utils-1.0.9*
         ```
         
         
         
 Keywords: django Audit
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `NewCode-Utils-1.0.8/README.md` & `NewCode-Utils-1.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -45,11 +45,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/NewCode-Utils-1.0.8*
+twine upload --repository pypi dist/NewCode-Utils-1.0.9*
 ```
```

### Comparing `NewCode-Utils-1.0.8/setup.cfg` & `NewCode-Utils-1.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [metadata]
 name = NewCode-Utils
-version = 1.0.8
+version = 1.0.9
 author = NewCode_
 author_email = new.code.2523@gmail.com
 maintainer = NewCode_
 maintainer_email = new.code.2523@gmail.com
 description = Necessary elements for the development of apps.
 long_description = file:README.md
+url = https://github.com/New-Code-S-A-S/NewCode_Utils_packeges
 license = MIT
 keywords = django Audit
 long_description_content_type = text/markdown
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	License :: OSI Approved :: MIT License
```

