# Comparing `tmp/newcode-utils-0.0.2.tar.gz` & `tmp/newcode-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newcode-utils-0.0.2.tar", last modified: Tue Apr 25 04:11:19 2023, max compression
+gzip compressed data, was "dist/newcode-utils-0.0.3.tar", last modified: Tue Apr 25 04:34:58 2023, max compression
```

## Comparing `newcode-utils-0.0.2.tar` & `newcode-utils-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode-utils-0.0.2/LICENSE
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 newcode-utils-0.0.2/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/NewCode_utils/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 newcode-utils-0.0.2/NewCode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/NewCode_utils/admins/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 newcode-utils-0.0.2/NewCode_utils/admins/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode-utils-0.0.2/NewCode_utils/admins/audit_admin.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 newcode-utils-0.0.2/NewCode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/NewCode_utils/helpers/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 newcode-utils-0.0.2/NewCode_utils/helpers/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode-utils-0.0.2/NewCode_utils/helpers/utils.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode-utils-0.0.2/NewCode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/NewCode_utils/migrations/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode-utils-0.0.2/NewCode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/NewCode_utils/models/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 newcode-utils-0.0.2/NewCode_utils/models/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode-utils-0.0.2/NewCode_utils/models/audit.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1982 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/PKG-INFO
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 04:11:16.000000 newcode-utils-0.0.2/README.md
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/newcode_utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1982 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/newcode_utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      561 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/newcode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/newcode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      123 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/newcode_utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/newcode_utils.egg-info/top_level.txt
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1109 2023-04-25 04:11:19.000000 newcode-utils-0.0.2/setup.cfg
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 newcode-utils-0.0.2/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode-utils-0.0.3/LICENSE
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 newcode-utils-0.0.3/MANIFEST.in
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1982 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/PKG-INFO
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 04:34:54.000000 newcode-utils-0.0.3/README.md
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-25 04:34:54.000000 newcode-utils-0.0.3/newcode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils/admins/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode-utils-0.0.3/newcode_utils/admins/__init__.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode-utils-0.0.3/newcode_utils/admins/audit_admin.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 04:31:55.000000 newcode-utils-0.0.3/newcode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils/helpers/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode-utils-0.0.3/newcode_utils/helpers/__init__.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode-utils-0.0.3/newcode_utils/helpers/utils.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode-utils-0.0.3/newcode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils/migrations/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode-utils-0.0.3/newcode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils/models/
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 04:34:54.000000 newcode-utils-0.0.3/newcode_utils/models/__init__.py
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode-utils-0.0.3/newcode_utils/models/audit.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1982 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      561 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      123 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/newcode_utils.egg-info/top_level.txt
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1109 2023-04-25 04:34:58.000000 newcode-utils-0.0.3/setup.cfg
+-rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 newcode-utils-0.0.3/setup.py
```

### Comparing `newcode-utils-0.0.2/LICENSE` & `newcode-utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.2/NewCode_utils/admins/audit_admin.py` & `newcode-utils-0.0.3/newcode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.2/NewCode_utils/helpers/utils.py` & `newcode-utils-0.0.3/newcode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.2/NewCode_utils/helpers/utils_permission_rest.py` & `newcode-utils-0.0.3/newcode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.2/NewCode_utils/models/audit.py` & `newcode-utils-0.0.3/newcode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.2/PKG-INFO` & `newcode-utils-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcode-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 License: MIT
@@ -49,15 +49,15 @@
         ```
         
         * update repository
         
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/newcode-utils-0.0.2*
+        twine upload --repository pypi dist/newcode-utils-0.0.3*
         ```
         
         
         
 Keywords: django Audit
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `newcode-utils-0.0.2/README.md` & `newcode-utils-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/newcode-utils-0.0.2*
+twine upload --repository pypi dist/newcode-utils-0.0.3*
 ```
```

### Comparing `newcode-utils-0.0.2/newcode_utils.egg-info/PKG-INFO` & `newcode-utils-0.0.3/newcode_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcode-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/NewCode_Utils_packeges
 Author: NewCode_
 Author-email: new.code.2523@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 License: MIT
@@ -49,15 +49,15 @@
         ```
         
         * update repository
         
         ``` bash
         python3.7 setup.py sdist bdist_wheel
         twine check dist/*
-        twine upload --repository pypi dist/newcode-utils-0.0.2*
+        twine upload --repository pypi dist/newcode-utils-0.0.3*
         ```
         
         
         
 Keywords: django Audit
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `newcode-utils-0.0.2/setup.cfg` & `newcode-utils-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = newcode-utils
-version = 0.0.2
+version = 0.0.3
 author = NewCode_
 author_email = new.code.2523@gmail.com
 maintainer = NewCode_
 maintainer_email = new.code.2523@gmail.com
 description = Necessary elements for the development of apps.
 long_description = file:README.md
 url = https://github.com/New-Code-S-A-S/NewCode_Utils_packeges
```

