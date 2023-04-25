# Comparing `tmp/pystorz-0.0.7.tar.gz` & `tmp/pystorz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.0.7.tar", last modified: Mon Apr 24 18:12:55 2023, max compression
+gzip compressed data, was "dist/pystorz-0.0.8.tar", last modified: Tue Apr 25 03:29:20 2023, max compression
```

## Comparing `pystorz-0.0.7.tar` & `pystorz-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.989273 pystorz-0.0.7/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.7/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 18:12:55.989030 pystorz-0.0.7/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.0.7/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.977862 pystorz-0.0.7/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.7/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.978946 pystorz-0.0.7/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.7/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.7/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.981140 pystorz-0.0.7/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.7/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.0.7/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4159 2023-04-24 14:46:41.000000 pystorz-0.0.7/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.986550 pystorz-0.0.7/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.7/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.7/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.7/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.987101 pystorz-0.0.7/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.7/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9558 2023-04-24 18:11:22.000000 pystorz-0.0.7/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.988532 pystorz-0.0.7/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.7/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2270 2023-04-24 16:09:40.000000 pystorz-0.0.7/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.7/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.7/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2073 2023-04-24 15:41:15.000000 pystorz-0.0.7/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-24 18:12:55.978671 pystorz-0.0.7/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-24 18:12:55.000000 pystorz-0.0.7/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-24 18:12:55.989332 pystorz-0.0.7/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-24 18:11:55.000000 pystorz-0.0.7/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.834741 pystorz-0.0.8/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.8/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 03:29:20.834490 pystorz-0.0.8/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.0.8/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.827554 pystorz-0.0.8/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.8/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.828605 pystorz-0.0.8/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.8/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.8/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.830160 pystorz-0.0.8/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.8/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.0.8/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4132 2023-04-24 18:19:26.000000 pystorz-0.0.8/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.832195 pystorz-0.0.8/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.8/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.8/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.8/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.832587 pystorz-0.0.8/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.8/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9506 2023-04-25 03:25:40.000000 pystorz-0.0.8/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.833931 pystorz-0.0.8/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.8/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2270 2023-04-24 16:09:40.000000 pystorz-0.0.8/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.8/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.8/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2296 2023-04-25 03:26:29.000000 pystorz-0.0.8/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:29:20.828330 pystorz-0.0.8/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 03:29:20.000000 pystorz-0.0.8/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-25 03:29:20.000000 pystorz-0.0.8/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-25 03:29:20.000000 pystorz-0.0.8/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-25 03:29:20.000000 pystorz-0.0.8/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-25 03:29:20.000000 pystorz-0.0.8/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-25 03:29:20.834818 pystorz-0.0.8/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-25 03:29:18.000000 pystorz-0.0.8/setup.py
```

### Comparing `pystorz-0.0.7/LICENSE` & `pystorz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/PKG-INFO` & `pystorz-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.0.7/README.md` & `pystorz-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/mgen/builder.py` & `pystorz-0.0.8/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/mgen/loader.py` & `pystorz-0.0.8/pystorz/mgen/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,17 +96,16 @@
                 continue
             if m["kind"] == "Object":
                 if m["name"] in resource_cache:
                     raise Exception("duplicate object: {}".format(m["name"]))
                 resource_cache.add(m["name"])
 
                 pkey = "metadata.identity"
-                mpkey = m["primarykey"]
-                if len(mpkey) > 0:
-                    pkey = mpkey
+                if "primarykey" in m:
+                    pkey = m["primarykey"]
                 pkey = make_prop_caller_string(pkey)
 
                 ext = None
                 if "external" in m:
                     ext = m["external"]
                 intr = None
                 if "internal" in m:
```

### Comparing `pystorz-0.0.7/pystorz/mgen/templates/structure.py` & `pystorz-0.0.8/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.0.8/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/mgen/test.py` & `pystorz-0.0.8/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/mgen/utils.py` & `pystorz-0.0.8/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/sql/store.py` & `pystorz-0.0.8/pystorz/sql/store.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         except Exception as e:
             pass
         if existing is not None:
             raise Exception(constants.ErrObjectExists)
 
         self.TestConnection()
 
-        obj.Metadata().SetCreated(datetime.now().strftime(constants.DATETIME_FORMAT))
+        obj.Metadata().SetCreated(utils.datetime_current())
         obj.Metadata().SetUpdated(obj.Metadata().Created())
 
         self._setIdentity(
             obj.Metadata().Identity().Path(),
             obj.PrimaryKey(),
             obj.Metadata().Kind())
 
@@ -93,15 +93,15 @@
         self._setIdentity(obj.Metadata().Identity().Path(),
                           obj.PrimaryKey(), obj.Metadata().Kind())
 
         self._removeObject(existing.PrimaryKey(),
                            existing.Metadata().Kind())
 
         obj.Metadata().SetCreated(existing.Metadata().Created())
-        obj.Metadata().SetUpdated(datetime.now().strftime(constants.DATETIME_FORMAT))
+        obj.Metadata().SetUpdated(utils.datetime_current())
 
         self._setObject(obj.PrimaryKey(), obj.Metadata().Kind(), obj)
 
         return obj.Clone()
 
     def Delete(self, identity, *opt):
         log.info("delete {}".format(identity.Path()))
```

### Comparing `pystorz-0.0.7/pystorz/store/meta.py` & `pystorz-0.0.8/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/store/options.py` & `pystorz-0.0.8/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/store/store.py` & `pystorz-0.0.8/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/pystorz/store/utils.py` & `pystorz-0.0.8/pystorz/store/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 import time
 import logging
 import pathlib
 from jsonpath import JSONPath
+from datetime import datetime
 
 log = logging.getLogger(__name__)
 
 # import gabs
 
 from pystorz.internal import constants
 from pystorz.store import store
@@ -78,7 +79,14 @@
     with open(target_file, 'w') as f:
         f.write(content)
 
 
 def runtime_dir() -> str:
     rd = pathlib.Path(__file__).parent.parent.absolute()
     return rd
+
+
+def datetime_current() -> str:
+    return datetime.now().strftime(constants.DATETIME_FORMAT)
+
+def datetime_parse(dtstr) -> str:
+    return datetime.strptime(dtstr, constants.DATETIME_FORMAT)
```

### Comparing `pystorz-0.0.7/pystorz.egg-info/PKG-INFO` & `pystorz-0.0.8/pystorz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.0.7/pystorz.egg-info/SOURCES.txt` & `pystorz-0.0.8/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.7/setup.py` & `pystorz-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.0.7',
+    version='0.0.8',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

