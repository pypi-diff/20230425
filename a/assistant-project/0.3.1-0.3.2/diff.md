# Comparing `tmp/assistant_project-0.3.1.tar.gz` & `tmp/assistant_project-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant_project-0.3.1.tar", last modified: Mon Apr 24 14:20:26 2023, max compression
+gzip compressed data, was "assistant_project-0.3.2.tar", last modified: Tue Apr 25 10:12:41 2023, max compression
```

## Comparing `assistant_project-0.3.1.tar` & `assistant_project-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.237404 assistant_project-0.3.1/
--rw-rw-rw-   0        0        0     1091 2023-03-10 10:20:05.000000 assistant_project-0.3.1/LICENCE
--rw-rw-rw-   0        0        0     3031 2023-04-24 14:20:26.233577 assistant_project-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-04-24 14:19:19.000000 assistant_project-0.3.1/README.md
--rw-rw-rw-   0        0        0      725 2023-04-24 14:19:19.000000 assistant_project-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 14:20:26.238436 assistant_project-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.089631 assistant_project-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.117215 assistant_project-0.3.1/src/assistant_project/
--rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.152029 assistant_project-0.3.1/src/assistant_project/dict_wrapper/
--rw-rw-rw-   0        0        0       27 2023-04-24 14:12:52.000000 assistant_project-0.3.1/src/assistant_project/dict_wrapper/__init__.py
--rw-rw-rw-   0        0        0     1987 2023-04-24 14:18:14.000000 assistant_project-0.3.1/src/assistant_project/dict_wrapper/dict_wrapper.py
--rw-rw-rw-   0        0        0      262 2023-04-23 08:12:23.000000 assistant_project-0.3.1/src/assistant_project/dict_wrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.177170 assistant_project-0.3.1/src/assistant_project/graphdb/
--rw-rw-rw-   0        0        0       68 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/graphdb/__init__.py
--rw-rw-rw-   0        0        0     2553 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/graphdb/graph_db.py
--rw-rw-rw-   0        0        0     4408 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/graphdb/onto_refine.py
--rw-rw-rw-   0        0        0     1066 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/graphdb/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.224886 assistant_project-0.3.1/src/assistant_project/production_system/
--rw-rw-rw-   0        0        0       86 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/__init__.py
--rw-rw-rw-   0        0        0       29 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/file_reader.py
--rw-rw-rw-   0        0        0      776 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/opg_list.py
--rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/osg_list.py
--rw-rw-rw-   0        0        0      512 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/production_system.py
--rw-rw-rw-   0        0        0      800 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/resource_list.py
--rw-rw-rw-   0        0        0      137 2023-03-10 10:20:05.000000 assistant_project-0.3.1/src/assistant_project/production_system/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:20:26.134153 assistant_project-0.3.1/src/assistant_project.egg-info/
--rw-rw-rw-   0        0        0     3031 2023-04-24 14:20:26.000000 assistant_project-0.3.1/src/assistant_project.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-04-24 14:20:26.000000 assistant_project-0.3.1/src/assistant_project.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:20:26.000000 assistant_project-0.3.1/src/assistant_project.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-24 14:20:26.000000 assistant_project-0.3.1/src/assistant_project.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.647680 assistant_project-0.3.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-10 10:20:05.000000 assistant_project-0.3.2/LICENCE
+-rw-rw-rw-   0        0        0     3181 2023-04-25 10:12:41.644956 assistant_project-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1398 2023-04-25 10:11:42.000000 assistant_project-0.3.2/README.md
+-rw-rw-rw-   0        0        0      740 2023-04-25 10:11:49.000000 assistant_project-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:12:41.648193 assistant_project-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.560900 assistant_project-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.575183 assistant_project-0.3.2/src/assistant_project/
+-rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.598328 assistant_project-0.3.2/src/assistant_project/dict_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-04-24 15:06:40.000000 assistant_project-0.3.2/src/assistant_project/dict_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-04-25 10:10:58.000000 assistant_project-0.3.2/src/assistant_project/dict_wrapper/dict_wrapper.py
+-rw-rw-rw-   0        0        0      262 2023-04-23 08:12:23.000000 assistant_project-0.3.2/src/assistant_project/dict_wrapper/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.614231 assistant_project-0.3.2/src/assistant_project/graphdb/
+-rw-rw-rw-   0        0        0       68 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/graphdb/__init__.py
+-rw-rw-rw-   0        0        0     2553 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/graphdb/graph_db.py
+-rw-rw-rw-   0        0        0     4408 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/graphdb/onto_refine.py
+-rw-rw-rw-   0        0        0     1066 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/graphdb/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.640531 assistant_project-0.3.2/src/assistant_project/production_system/
+-rw-rw-rw-   0        0        0       86 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/file_reader.py
+-rw-rw-rw-   0        0        0      776 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/opg_list.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/osg_list.py
+-rw-rw-rw-   0        0        0      512 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/production_system.py
+-rw-rw-rw-   0        0        0      800 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/resource_list.py
+-rw-rw-rw-   0        0        0      137 2023-03-10 10:20:05.000000 assistant_project-0.3.2/src/assistant_project/production_system/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:12:41.587608 assistant_project-0.3.2/src/assistant_project.egg-info/
+-rw-rw-rw-   0        0        0     3181 2023-04-25 10:12:41.000000 assistant_project-0.3.2/src/assistant_project.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-04-25 10:12:41.000000 assistant_project-0.3.2/src/assistant_project.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:12:41.000000 assistant_project-0.3.2/src/assistant_project.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 10:12:41.000000 assistant_project-0.3.2/src/assistant_project.egg-info/top_level.txt
```

### Comparing `assistant_project-0.3.1/LICENCE` & `assistant_project-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/PKG-INFO` & `assistant_project-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant_project
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Library for the EU ASSISTANT-Project
 Author-email: Nikolas Laudenbach <nikolas.laudenbach@tum.de>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -57,14 +57,18 @@
 ### Dict Wrapper
 
 Allows to read every key-value pair and return list/dict based on custom config.
 
 ---
 ## Change History
 
+**0.3.2**:
+- FIX: relative import of *json_wapper*
+- Add condition to return correct value if two keys are identical in different subdirectories
+
 **0.3.1**:
 - Add method to get identifier from cfg_file based on name for *json_wrapper*
 
 **0.3**:
 - Create new sublibrary *json_wrapper*
 
 **0.2**:
```

### Comparing `assistant_project-0.3.1/README.md` & `assistant_project-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 ### Dict Wrapper
 
 Allows to read every key-value pair and return list/dict based on custom config.
 
 ---
 ## Change History
 
+**0.3.2**:
+- FIX: relative import of *json_wapper*
+- Add condition to return correct value if two keys are identical in different subdirectories
+
 **0.3.1**:
 - Add method to get identifier from cfg_file based on name for *json_wrapper*
 
 **0.3**:
 - Create new sublibrary *json_wrapper*
 
 **0.2**:
```

### Comparing `assistant_project-0.3.1/pyproject.toml` & `assistant_project-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "requests~=2.28"]
+requires = ["setuptools>=61.0", "requests~=2.28", "PyYAML>=6.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "assistant_project"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Nikolas Laudenbach", email="nikolas.laudenbach@tum.de" },
 ]
 description = "Python Library for the EU ASSISTANT-Project"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `assistant_project-0.3.1/src/assistant_project/dict_wrapper/dict_wrapper.py` & `assistant_project-0.3.2/src/assistant_project/dict_wrapper/dict_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import json
-from utils import import_yaml_cfg
+from .utils import import_yaml_cfg
 
 
 class DictReader:
     def __init__(self, data_cfg):
         self.config = import_yaml_cfg(data_cfg)
         print(self.config)
 
     def get_cfg_from_name(self, file_name):
         return self.config["FILES"][file_name]
 
-    def iterate_dict(self, obj, cfg, return_list=False):
+    def iterate_dict(self, obj, cfg, return_list=False, prekey=""):
         new_dict = {}
         """Walk through a dictionary of dicts and lists and return list of relevant items."""
         if type(obj) is dict:
             for key, value in obj.items():
                 if type(value) in [dict, list]:
-                    if key == cfg['LIST'] and return_list:
+                    if (prekey+'.' + key).__contains__(cfg['LIST']) and return_list:
                         return value
-                    self.iterate_dict(value, cfg, return_list)
+                    self.iterate_dict(value, cfg, return_list, prekey=(prekey + '.' + key))
                 elif not return_list:
-                    if key in cfg["ATTRIBUTES"].values():
-                        new_dict_key = [i for i in cfg["ATTRIBUTES"] if cfg["ATTRIBUTES"][i] == key][0]
+                    contained = [x for x in cfg["ATTRIBUTES"].values() if (prekey+'.' + key).__contains__(x)]
+                    if contained:
+                        new_dict_key = list(cfg["ATTRIBUTES"].keys())[list(cfg["ATTRIBUTES"].values()).index(contained[0])]
                         new_dict[new_dict_key] = value
         return new_dict
         # elif type(obj) is list:
         #     for i, element in enumerate(obj):
         #         if type(element) in [dict, list]:
         #             self.iterate_dict(element, cfg, return_list)
         # else:
```

### Comparing `assistant_project-0.3.1/src/assistant_project/graphdb/graph_db.py` & `assistant_project-0.3.2/src/assistant_project/graphdb/graph_db.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/src/assistant_project/graphdb/onto_refine.py` & `assistant_project-0.3.2/src/assistant_project/graphdb/onto_refine.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/src/assistant_project/graphdb/utils.py` & `assistant_project-0.3.2/src/assistant_project/graphdb/utils.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/src/assistant_project/production_system/opg_list.py` & `assistant_project-0.3.2/src/assistant_project/production_system/opg_list.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/src/assistant_project/production_system/production_system.py` & `assistant_project-0.3.2/src/assistant_project/production_system/production_system.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/src/assistant_project/production_system/resource_list.py` & `assistant_project-0.3.2/src/assistant_project/production_system/resource_list.py`

 * *Files identical despite different names*

### Comparing `assistant_project-0.3.1/src/assistant_project.egg-info/PKG-INFO` & `assistant_project-0.3.2/src/assistant_project.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant-project
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Library for the EU ASSISTANT-Project
 Author-email: Nikolas Laudenbach <nikolas.laudenbach@tum.de>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -57,14 +57,18 @@
 ### Dict Wrapper
 
 Allows to read every key-value pair and return list/dict based on custom config.
 
 ---
 ## Change History
 
+**0.3.2**:
+- FIX: relative import of *json_wapper*
+- Add condition to return correct value if two keys are identical in different subdirectories
+
 **0.3.1**:
 - Add method to get identifier from cfg_file based on name for *json_wrapper*
 
 **0.3**:
 - Create new sublibrary *json_wrapper*
 
 **0.2**:
```

### Comparing `assistant_project-0.3.1/src/assistant_project.egg-info/SOURCES.txt` & `assistant_project-0.3.2/src/assistant_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

