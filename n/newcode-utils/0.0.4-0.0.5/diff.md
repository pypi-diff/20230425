# Comparing `tmp/newcode-utils-0.0.4.tar.gz` & `tmp/newcode_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newcode-utils-0.0.4.tar", last modified: Tue Apr 25 04:42:58 2023, max compression
+gzip compressed data, was "dist/newcode_utils-0.0.5.tar", last modified: Tue Apr 25 05:23:02 2023, max compression
```

## Comparing `newcode-utils-0.0.4.tar` & `newcode_utils-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode-utils-0.0.4/LICENSE
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 newcode-utils-0.0.4/MANIFEST.in
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1982 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/PKG-INFO
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 04:42:57.000000 newcode-utils-0.0.4/README.md
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-25 04:34:54.000000 newcode-utils-0.0.4/newcode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils/admins/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode-utils-0.0.4/newcode_utils/admins/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode-utils-0.0.4/newcode_utils/admins/audit_admin.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 04:31:55.000000 newcode-utils-0.0.4/newcode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils/helpers/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode-utils-0.0.4/newcode_utils/helpers/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode-utils-0.0.4/newcode_utils/helpers/utils.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode-utils-0.0.4/newcode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils/migrations/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode-utils-0.0.4/newcode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils/models/
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 04:34:54.000000 newcode-utils-0.0.4/newcode_utils/models/__init__.py
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode-utils-0.0.4/newcode_utils/models/audit.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1982 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      561 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      123 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/newcode_utils.egg-info/top_level.txt
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)     1134 2023-04-25 04:42:58.000000 newcode-utils-0.0.4/setup.cfg
--rwxrwxrwx   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 newcode-utils-0.0.4/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 newcode_utils-0.0.5/LICENSE
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      228 2023-04-25 05:18:39.000000 newcode_utils-0.0.5/MANIFEST.in
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/PKG-INFO
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      732 2023-04-25 05:22:08.000000 newcode_utils-0.0.5/README.md
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-25 04:34:54.000000 newcode_utils-0.0.5/newcode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/admins/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      184 2023-04-25 04:34:54.000000 newcode_utils-0.0.5/newcode_utils/admins/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 newcode_utils-0.0.5/newcode_utils/admins/audit_admin.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-25 04:31:55.000000 newcode_utils-0.0.5/newcode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/helpers/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-25 04:34:54.000000 newcode_utils-0.0.5/newcode_utils/helpers/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 newcode_utils-0.0.5/newcode_utils/helpers/utils.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 newcode_utils-0.0.5/newcode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/migrations/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 newcode_utils-0.0.5/newcode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils/models/
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-25 05:22:58.000000 newcode_utils-0.0.5/newcode_utils/models/__init__.py
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 newcode_utils-0.0.5/newcode_utils/models/audit.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1546 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      578 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      286 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/requires.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/newcode_utils.egg-info/top_level.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      285 2023-04-25 05:16:42.000000 newcode_utils-0.0.5/requirements.txt
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)      117 2023-04-25 05:23:02.000000 newcode_utils-0.0.5/setup.cfg
+-rwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)     1338 2023-04-25 05:20:10.000000 newcode_utils-0.0.5/setup.py
```

### Comparing `newcode-utils-0.0.4/LICENSE` & `newcode_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.4/README.md` & `newcode_utils-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 ```
 
 * update repository
 
 ``` bash
 python3.7 setup.py sdist bdist_wheel
 twine check dist/*
-twine upload --repository pypi dist/newcode-utils-0.0.4*
+twine upload --repository pypi dist/newcode_utils-0.0.4*
 ```
```

### Comparing `newcode-utils-0.0.4/newcode_utils/admins/audit_admin.py` & `newcode_utils-0.0.5/newcode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.4/newcode_utils/helpers/utils.py` & `newcode_utils-0.0.5/newcode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.4/newcode_utils/helpers/utils_permission_rest.py` & `newcode_utils-0.0.5/newcode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.4/newcode_utils/models/audit.py` & `newcode_utils-0.0.5/newcode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `newcode-utils-0.0.4/newcode_utils.egg-info/SOURCES.txt` & `newcode_utils-0.0.5/newcode_utils.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 newcode_utils/__init__.py
 newcode_utils/apps.py
 newcode_utils.egg-info/PKG-INFO
 newcode_utils.egg-info/SOURCES.txt
 newcode_utils.egg-info/dependency_links.txt
```

