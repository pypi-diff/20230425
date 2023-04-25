# Comparing `tmp/newcode_utils-0.1.1.tar.gz` & `tmp/newcode_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newcode_utils-0.1.1.tar", last modified: Tue Apr 25 05:43:27 2023, max compression
+gzip compressed data, was "dist/newcode_utils-0.1.2.tar", last modified: Tue Apr 25 06:00:34 2023, max compression
```

## Comparing `newcode_utils-0.1.1.tar` & `newcode_utils-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode_utils-0.1.1/LICENSE
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      228 2023-04-25 05:18:39.000000 newcode_utils-0.1.1/MANIFEST.in
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/PKG-INFO
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 05:43:21.000000 newcode_utils-0.1.1/README.md
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       61 2023-04-25 05:28:53.000000 newcode_utils-0.1.1/newcode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/admins/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode_utils-0.1.1/newcode_utils/admins/__init__.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode_utils-0.1.1/newcode_utils/admins/audit_admin.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 05:28:11.000000 newcode_utils-0.1.1/newcode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/helpers/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode_utils-0.1.1/newcode_utils/helpers/__init__.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode_utils-0.1.1/newcode_utils/helpers/utils.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode_utils-0.1.1/newcode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/migrations/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode_utils-0.1.1/newcode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/migrations/__pycache__/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 05:28:58.000000 newcode_utils-0.1.1/newcode_utils/migrations/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/models/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 05:22:58.000000 newcode_utils-0.1.1/newcode_utils/models/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils/models/__pycache__/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      246 2023-04-25 05:28:58.000000 newcode_utils-0.1.1/newcode_utils/models/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2328 2023-04-25 05:28:58.000000 newcode_utils-0.1.1/newcode_utils/models/__pycache__/audit.cpython-37.pyc
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode_utils-0.1.1/newcode_utils/models/audit.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:43:26.000000 newcode_utils-0.1.1/newcode_utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      750 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/newcode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 05:43:26.000000 newcode_utils-0.1.1/newcode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      217 2023-04-25 05:43:26.000000 newcode_utils-0.1.1/newcode_utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 05:43:26.000000 newcode_utils-0.1.1/newcode_utils.egg-info/top_level.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      216 2023-04-25 05:42:29.000000 newcode_utils-0.1.1/requirements.txt
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      117 2023-04-25 05:43:27.000000 newcode_utils-0.1.1/setup.cfg
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1257 2023-04-25 05:43:21.000000 newcode_utils-0.1.1/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode_utils-0.1.2/LICENSE
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      228 2023-04-25 05:18:39.000000 newcode_utils-0.1.2/MANIFEST.in
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/PKG-INFO
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 05:43:21.000000 newcode_utils-0.1.2/README.md
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       61 2023-04-25 05:28:53.000000 newcode_utils-0.1.2/newcode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/admins/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode_utils-0.1.2/newcode_utils/admins/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode_utils-0.1.2/newcode_utils/admins/audit_admin.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 05:28:11.000000 newcode_utils-0.1.2/newcode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/helpers/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode_utils-0.1.2/newcode_utils/helpers/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode_utils-0.1.2/newcode_utils/helpers/utils.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode_utils-0.1.2/newcode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/migrations/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode_utils-0.1.2/newcode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/migrations/__pycache__/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 05:28:58.000000 newcode_utils-0.1.2/newcode_utils/migrations/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/models/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 05:22:58.000000 newcode_utils-0.1.2/newcode_utils/models/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils/models/__pycache__/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      246 2023-04-25 05:28:58.000000 newcode_utils-0.1.2/newcode_utils/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2328 2023-04-25 05:28:58.000000 newcode_utils-0.1.2/newcode_utils/models/__pycache__/audit.cpython-37.pyc
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode_utils-0.1.2/newcode_utils/models/audit.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      750 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      217 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/newcode_utils.egg-info/top_level.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      216 2023-04-25 05:46:45.000000 newcode_utils-0.1.2/requirements.txt
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      117 2023-04-25 06:00:34.000000 newcode_utils-0.1.2/setup.cfg
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1257 2023-04-25 05:58:23.000000 newcode_utils-0.1.2/setup.py
```

### Comparing `newcode_utils-0.1.1/LICENSE` & `newcode_utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/PKG-INFO` & `newcode_utils-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcode_utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/newcode_utils
 Author: Camilo Suarez
 Author-email: juancamilosuarezquinones@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 Keywords: utils,newcode-utils,NewCode,Audit
```

### Comparing `newcode_utils-0.1.1/README.md` & `newcode_utils-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/newcode_utils/admins/audit_admin.py` & `newcode_utils-0.1.2/newcode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/newcode_utils/helpers/utils.py` & `newcode_utils-0.1.2/newcode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/newcode_utils/helpers/utils_permission_rest.py` & `newcode_utils-0.1.2/newcode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/newcode_utils/models/__pycache__/audit.cpython-37.pyc` & `newcode_utils-0.1.2/newcode_utils/models/__pycache__/audit.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/newcode_utils/models/audit.py` & `newcode_utils-0.1.2/newcode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/newcode_utils.egg-info/PKG-INFO` & `newcode_utils-0.1.2/newcode_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcode-utils
-Version: 0.1.1
+Version: 0.1.2
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/newcode_utils
 Author: Camilo Suarez
 Author-email: juancamilosuarezquinones@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 Keywords: utils,newcode-utils,NewCode,Audit
```

### Comparing `newcode_utils-0.1.1/newcode_utils.egg-info/SOURCES.txt` & `newcode_utils-0.1.2/newcode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.1.1/setup.py` & `newcode_utils-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='newcode_utils',
     packages=['newcode_utils'],  # this must be the same as the name above
-    version='0.1.1',
+    version='0.1.2',
     description='Necessary elements for the development of apps.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Camilo Suarez',
     author_email='juancamilosuarezquinones@gmail.com',
     maintainer='NewCode_',
     maintainer_email='new.code.2523@gmail.com',
```

