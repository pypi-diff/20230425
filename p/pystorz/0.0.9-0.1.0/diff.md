# Comparing `tmp/pystorz-0.0.9.tar.gz` & `tmp/pystorz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.0.9.tar", last modified: Tue Apr 25 03:55:43 2023, max compression
+gzip compressed data, was "dist/pystorz-0.1.0.tar", last modified: Tue Apr 25 04:15:02 2023, max compression
```

## Comparing `pystorz-0.0.9.tar` & `pystorz-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.601963 pystorz-0.0.9/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.0.9/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 03:55:43.601608 pystorz-0.0.9/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.0.9/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.591446 pystorz-0.0.9/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.0.9/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.594149 pystorz-0.0.9/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.0.9/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.0.9/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.596084 pystorz-0.0.9/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.0.9/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.0.9/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4132 2023-04-24 18:19:26.000000 pystorz-0.0.9/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.598370 pystorz-0.0.9/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.0.9/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.0.9/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)      616 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.0.9/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.598715 pystorz-0.0.9/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.0.9/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9486 2023-04-25 03:48:50.000000 pystorz-0.0.9/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.600427 pystorz-0.0.9/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.0.9/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2295 2023-04-25 03:51:35.000000 pystorz-0.0.9/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.0.9/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.0.9/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2368 2023-04-25 03:46:31.000000 pystorz-0.0.9/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 03:55:43.593500 pystorz-0.0.9/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 03:55:43.000000 pystorz-0.0.9/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-25 03:55:43.000000 pystorz-0.0.9/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-25 03:55:43.000000 pystorz-0.0.9/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-25 03:55:43.000000 pystorz-0.0.9/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-25 03:55:43.000000 pystorz-0.0.9/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-25 03:55:43.602048 pystorz-0.0.9/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-25 03:55:12.000000 pystorz-0.0.9/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.588432 pystorz-0.1.0/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.1.0/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 04:15:02.588205 pystorz-0.1.0/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1133 2023-04-24 16:29:08.000000 pystorz-0.1.0/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.581787 pystorz-0.1.0/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.1.0/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.582994 pystorz-0.1.0/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.1.0/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      279 2023-04-24 15:29:24.000000 pystorz-0.1.0/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.584460 pystorz-0.1.0/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.1.0/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.1.0/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4070 2023-04-25 04:09:44.000000 pystorz-0.1.0/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.586251 pystorz-0.1.0/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.1.0/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.1.0/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      846 2023-04-25 04:12:40.000000 pystorz-0.1.0/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1754 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.1.0/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.586549 pystorz-0.1.0/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.1.0/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9486 2023-04-25 03:48:50.000000 pystorz-0.1.0/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.587818 pystorz-0.1.0/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.1.0/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2295 2023-04-25 03:51:35.000000 pystorz-0.1.0/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4297 2023-04-24 14:15:03.000000 pystorz-0.1.0/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2947 2023-04-24 16:09:14.000000 pystorz-0.1.0/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2368 2023-04-25 03:46:31.000000 pystorz-0.1.0/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-04-25 04:15:02.582682 pystorz-0.1.0/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1491 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-04-25 04:15:02.000000 pystorz-0.1.0/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-04-25 04:15:02.588484 pystorz-0.1.0/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-04-25 04:14:50.000000 pystorz-0.1.0/setup.py
```

### Comparing `pystorz-0.0.9/LICENSE` & `pystorz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/PKG-INFO` & `pystorz-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.0.9/README.md` & `pystorz-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/mgen/builder.py` & `pystorz-0.1.0/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/mgen/loader.py` & `pystorz-0.1.0/pystorz/mgen/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 import yaml
 import logging
 
 from pystorz.mgen.utils import capitalize, decapitalize, yaml_files
 
 log = logging.getLogger(__name__)
-log.debug('loading loader.py...')
+log.debug("loading loader.py...")
 
 
 def jopp(obj):
     # json pretty print
-    jstring = '''JSON pretty print
-''' + json.dumps(obj, indent=4, sort_keys=True)
+    jstring = """JSON pretty print
+""" + json.dumps(
+        obj, indent=4, sort_keys=True
+    )
     return jstring
 
 
 class Model:
     def __init__(self, types=None):
         self.types = types or []
 
@@ -83,20 +85,16 @@
         # log.debug("model: {}".format(jopp(model)))
 
         for m in model["types"]:
             if m["kind"] == "Struct":
                 if m["name"] in struct_cache:
                     raise Exception("duplicate struct: {}".format(m["name"]))
                 struct_cache.add(m["name"])
-                
-                structs.append(Struct(
-                    m["name"],
-                    "",
-                    capitalize_props(m["properties"])
-                ))
+
+                structs.append(Struct(m["name"], "", capitalize_props(m["properties"])))
                 continue
             if m["kind"] == "Object":
                 if m["name"] in resource_cache:
                     raise Exception("duplicate object: {}".format(m["name"]))
                 resource_cache.add(m["name"])
 
                 pkey = "metadata.identity"
@@ -107,41 +105,39 @@
                 ext = None
                 if "external" in m:
                     ext = m["external"]
                 intr = None
                 if "internal" in m:
                     intr = m["internal"]
 
-                resources.append(Resource(
-                    m["name"],
-                    ext,
-                    intr,
-                    pkey))
+                resources.append(Resource(m["name"], ext, intr, pkey))
                 continue
 
     return structs, resources
 
 
 def read_model(path: str):
     log.debug(f"reading model from {path}")
-    
+
     with open(path, "r") as f:
         data = yaml.safe_load(f)
     return data
 
 
 def capitalize_props(l: list):
     res = []
     for p in l:
-        res.append(Prop(
-            capitalize(p['name']),
-            p['type'],
-            decapitalize(p['name']),
-            # p.default
-        ))
+        res.append(
+            Prop(
+                capitalize(p["name"]),
+                p["type"],
+                decapitalize(p["name"]),
+                # p.default
+            )
+        )
     return res
 
 
 def make_prop_caller_string(pkey: str):
     tok = pkey.split(".")
     cap = []
     for t in tok:
@@ -162,9 +158,11 @@
         return '""'
     if tp == "bool":
         return "False"
     if tp == "int":
         return "0"
     if tp == "float":
         return "0.0"
-    
+    if tp == "datetime":
+        return '"0001-01-01T00:00:00Z"'
+
     return f"{tp}Factory()"
```

### Comparing `pystorz-0.0.9/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.1.0/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/mgen/test.py` & `pystorz-0.1.0/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/mgen/utils.py` & `pystorz-0.1.0/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/sql/store.py` & `pystorz-0.1.0/pystorz/sql/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/store/meta.py` & `pystorz-0.1.0/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/store/options.py` & `pystorz-0.1.0/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/store/store.py` & `pystorz-0.1.0/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz/store/utils.py` & `pystorz-0.1.0/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/pystorz.egg-info/PKG-INFO` & `pystorz-0.1.0/pystorz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pystorz-0.0.9/pystorz.egg-info/SOURCES.txt` & `pystorz-0.1.0/pystorz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystorz-0.0.9/setup.py` & `pystorz-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.0.9',
+    version='0.1.0',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

