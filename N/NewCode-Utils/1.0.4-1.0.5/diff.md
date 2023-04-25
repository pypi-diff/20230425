# Comparing `tmp/NewCode-Utils-1.0.4.tar.gz` & `tmp/NewCode-Utils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NewCode-Utils-1.0.4.tar", last modified: Tue Apr 25 01:01:52 2023, max compression
+gzip compressed data, was "dist/NewCode-Utils-1.0.5.tar", last modified: Tue Apr 25 01:48:42 2023, max compression
```

## Comparing `NewCode-Utils-1.0.4.tar` & `NewCode-Utils-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      271 2023-04-25 01:01:42.000000 NewCode-Utils-1.0.4/MANIFEST.in
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      543 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       12 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/requires.txt
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_Utils.egg-info/top_level.txt
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.4/NewCode_utils/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/admins/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/admins/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/admins/audit_admin.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.4/NewCode_utils/apps.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/utils.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.4/NewCode_utils/helpers/utils_permission_rest.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/migrations/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.4/NewCode_utils/migrations/__init__.py
-drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/NewCode_utils/models/
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/models/__init__.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.4/NewCode_utils/models/audit.py
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1550 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/PKG-INFO
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.4/README.md
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:01:52.000000 NewCode-Utils-1.0.4/setup.cfg
--rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      590 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.4/setup.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1105 2023-04-24 17:29:43.000000 NewCode-Utils-1.0.5/LICENSE
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      203 2023-04-25 01:43:19.000000 NewCode-Utils-1.0.5/MANIFEST.in
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1930 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      525 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        1 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       14 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_Utils.egg-info/top_level.txt
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       60 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.5/NewCode_utils/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/admins/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      185 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/admins/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/admins/audit_admin.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      194 2023-04-24 23:25:02.000000 NewCode-Utils-1.0.5/NewCode_utils/apps.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      193 2023-04-24 17:11:39.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1220 2023-04-24 17:15:05.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/utils.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1251 2023-04-24 17:10:47.000000 NewCode-Utils-1.0.5/NewCode_utils/helpers/utils_permission_rest.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/migrations/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-24 16:33:29.000000 NewCode-Utils-1.0.5/NewCode_utils/migrations/__init__.py
+drwxr-xr-x   0 camilo-suarez  (1000) camilo-suarez  (1000)        0 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/NewCode_utils/models/
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       45 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/models/__init__.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     2139 2023-04-24 17:02:01.000000 NewCode-Utils-1.0.5/NewCode_utils/models/audit.py
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)     1930 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/PKG-INFO
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      784 2023-04-25 00:58:06.000000 NewCode-Utils-1.0.5/README.md
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)      755 2023-04-25 01:48:42.000000 NewCode-Utils-1.0.5/setup.cfg
+-rw-r--r--   0 camilo-suarez  (1000) camilo-suarez  (1000)       38 2023-04-25 01:44:42.000000 NewCode-Utils-1.0.5/setup.py
```

### Comparing `NewCode-Utils-1.0.4/NewCode_utils/admins/audit_admin.py` & `NewCode-Utils-1.0.5/NewCode_utils/admins/audit_admin.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.4/NewCode_utils/helpers/utils.py` & `NewCode-Utils-1.0.5/NewCode_utils/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.4/NewCode_utils/helpers/utils_permission_rest.py` & `NewCode-Utils-1.0.5/NewCode_utils/helpers/utils_permission_rest.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.4/NewCode_utils/models/audit.py` & `NewCode-Utils-1.0.5/NewCode_utils/models/audit.py`

 * *Files identical despite different names*

### Comparing `NewCode-Utils-1.0.4/README.md` & `NewCode-Utils-1.0.5/README.md`

 * *Files identical despite different names*

