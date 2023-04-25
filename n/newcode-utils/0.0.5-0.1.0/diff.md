# Comparing `tmp/newcode_utils-0.0.5.tar.gz` & `tmp/newcode_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newcode_utils-0.0.5.tar", last modified: Tue Apr 25 05:23:02 2023, max compression
+gzip compressed data, was "dist/newcode_utils-0.1.0.tar", last modified: Tue Apr 25 05:37:42 2023, max compression
```

## Comparing `newcode_utils-0.0.5.tar` & `newcode_utils-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode_utils-0.0.5/LICENSE
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      228 2023-04-25 05:18:39.000000 newcode_utils-0.0.5/MANIFEST.in
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/PKG-INFO
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 05:22:08.000000 newcode_utils-0.0.5/README.md
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-25 04:34:54.000000 newcode_utils-0.0.5/newcode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/admins/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode_utils-0.0.5/newcode_utils/admins/__init__.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode_utils-0.0.5/newcode_utils/admins/audit_admin.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 04:31:55.000000 newcode_utils-0.0.5/newcode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/helpers/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode_utils-0.0.5/newcode_utils/helpers/__init__.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode_utils-0.0.5/newcode_utils/helpers/utils.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode_utils-0.0.5/newcode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/migrations/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode_utils-0.0.5/newcode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/models/
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 05:22:58.000000 newcode_utils-0.0.5/newcode_utils/models/__init__.py
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode_utils-0.0.5/newcode_utils/models/audit.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      578 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      286 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/top_level.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      285 2023-04-25 05:16:42.000000 newcode_utils-0.0.5/requirements.txt
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      117 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/setup.cfg
--rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1338 2023-04-25 05:20:10.000000 newcode_utils-0.0.5/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode_utils-0.1.0/LICENSE
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      228 2023-04-25 05:18:39.000000 newcode_utils-0.1.0/MANIFEST.in
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/PKG-INFO
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 05:31:24.000000 newcode_utils-0.1.0/README.md
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       61 2023-04-25 05:28:53.000000 newcode_utils-0.1.0/newcode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/admins/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode_utils-0.1.0/newcode_utils/admins/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode_utils-0.1.0/newcode_utils/admins/audit_admin.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 05:28:11.000000 newcode_utils-0.1.0/newcode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/helpers/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode_utils-0.1.0/newcode_utils/helpers/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode_utils-0.1.0/newcode_utils/helpers/utils.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode_utils-0.1.0/newcode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/migrations/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode_utils-0.1.0/newcode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/migrations/__pycache__/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 05:28:58.000000 newcode_utils-0.1.0/newcode_utils/migrations/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/models/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 05:22:58.000000 newcode_utils-0.1.0/newcode_utils/models/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils/models/__pycache__/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      246 2023-04-25 05:28:58.000000 newcode_utils-0.1.0/newcode_utils/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2328 2023-04-25 05:28:58.000000 newcode_utils-0.1.0/newcode_utils/models/__pycache__/audit.cpython-37.pyc
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode_utils-0.1.0/newcode_utils/models/audit.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      750 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      286 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/newcode_utils.egg-info/top_level.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      285 2023-04-25 05:16:42.000000 newcode_utils-0.1.0/requirements.txt
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      117 2023-04-25 05:37:42.000000 newcode_utils-0.1.0/setup.cfg
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1257 2023-04-25 05:30:41.000000 newcode_utils-0.1.0/setup.py
```

### Comparing `newcode_utils-0.0.5/LICENSE` & `newcode_utils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.0.5/PKG-INFO` & `newcode_utils-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcode_utils
-Version: 0.0.5
+Version: 0.1.0
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/newcode_utils
 Author: Camilo Suarez
 Author-email: juancamilosuarezquinones@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 Keywords: utils,newcode-utils,NewCode,Audit
@@ -60,11 +60,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/newcode_utils-0.0.4*
+twine upload --repository pypi dist/newcode-utils-0.1.0*
 ```
```

### Comparing `newcode_utils-0.0.5/README.md` & `newcode_utils-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/newcode_utils-0.0.4*
+twine upload --repository pypi dist/newcode-utils-0.1.0*
 ```
```

### Comparing `newcode_utils-0.0.5/newcode_utils/admins/audit_admin.py` & `newcode_utils-0.1.0/newcode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.0.5/newcode_utils/helpers/utils.py` & `newcode_utils-0.1.0/newcode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.0.5/newcode_utils/helpers/utils_permission_rest.py` & `newcode_utils-0.1.0/newcode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.0.5/newcode_utils/models/audit.py` & `newcode_utils-0.1.0/newcode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `newcode_utils-0.0.5/newcode_utils.egg-info/PKG-INFO` & `newcode_utils-0.1.0/newcode_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcode-utils
-Version: 0.0.5
+Version: 0.1.0
 Summary: Necessary elements for the development of apps.
 Home-page: https://github.com/New-Code-S-A-S/newcode_utils
 Author: Camilo Suarez
 Author-email: juancamilosuarezquinones@gmail.com
 Maintainer: NewCode_
 Maintainer-email: new.code.2523@gmail.com
 Keywords: utils,newcode-utils,NewCode,Audit
@@ -60,11 +60,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/newcode_utils-0.0.4*
+twine upload --repository pypi dist/newcode-utils-0.1.0*
 ```
```

### Comparing `newcode_utils-0.0.5/setup.py` & `newcode_utils-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='newcode_utils',
     packages=['newcode_utils'],  # this must be the same as the name above
-    version='0.0.5',
+    version='0.1.0',
     description='Necessary elements for the development of apps.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Camilo Suarez',
     author_email='juancamilosuarezquinones@gmail.com',
     maintainer='NewCode_',
     maintainer_email='new.code.2523@gmail.com',
     url='https://github.com/New-Code-S-A-S/newcode_utils',  # use the URL to the github repo
-    #download_url='https://github.com/UnTalDulcey/loducode_utils/tarball/1.5.2',
     keywords=['utils', 'newcode-utils', 'NewCode', 'Audit'],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

