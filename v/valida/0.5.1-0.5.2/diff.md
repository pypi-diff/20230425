# Comparing `tmp/valida-0.5.1.tar.gz` & `tmp/valida-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valida-0.5.1.tar", max compression
+gzip compressed data, was "valida-0.5.2.tar", max compression
```

## Comparing `valida-0.5.1.tar` & `valida-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-04-05 12:03:58.510097 valida-0.5.1/LICENSE
--rw-r--r--   0        0        0     1439 2023-04-05 12:03:58.510097 valida-0.5.1/README.md
--rw-r--r--   0        0        0      720 2023-04-05 12:03:58.510097 valida-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      200 2023-04-05 12:03:58.510097 valida-0.5.1/valida/__init__.py
--rw-r--r--   0        0        0     2903 2023-04-05 12:03:58.510097 valida-0.5.1/valida/callables.py
--rw-r--r--   0        0        0      353 2023-04-05 12:03:58.510097 valida-0.5.1/valida/casting.py
--rw-r--r--   0        0        0    27446 2023-04-05 12:03:58.510097 valida-0.5.1/valida/conditions.py
--rw-r--r--   0        0        0    10524 2023-04-05 12:03:58.510097 valida-0.5.1/valida/data.py
--rw-r--r--   0        0        0    27821 2023-04-05 12:03:58.510097 valida-0.5.1/valida/datapath.py
--rw-r--r--   0        0        0      485 2023-04-05 12:03:58.510097 valida-0.5.1/valida/errors.py
--rw-r--r--   0        0        0     6560 2023-04-05 12:03:58.510097 valida-0.5.1/valida/rules.py
--rw-r--r--   0        0        0     3885 2023-04-05 12:03:58.510097 valida-0.5.1/valida/schema.py
--rw-r--r--   0        0        0      869 2023-04-05 12:03:58.510097 valida-0.5.1/valida/utils.py
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-25 11:25:07.571026 valida-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1439 2023-04-25 11:25:07.571026 valida-0.5.2/README.md
+-rw-r--r--   0        0        0      720 2023-04-25 11:25:07.575026 valida-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-04-25 11:25:07.575026 valida-0.5.2/valida/__init__.py
+-rw-r--r--   0        0        0     2903 2023-04-25 11:25:07.575026 valida-0.5.2/valida/callables.py
+-rw-r--r--   0        0        0      353 2023-04-25 11:25:07.575026 valida-0.5.2/valida/casting.py
+-rw-r--r--   0        0        0    27447 2023-04-25 11:25:07.575026 valida-0.5.2/valida/conditions.py
+-rw-r--r--   0        0        0    10524 2023-04-25 11:25:07.575026 valida-0.5.2/valida/data.py
+-rw-r--r--   0        0        0    27707 2023-04-25 11:25:07.575026 valida-0.5.2/valida/datapath.py
+-rw-r--r--   0        0        0      485 2023-04-25 11:25:07.575026 valida-0.5.2/valida/errors.py
+-rw-r--r--   0        0        0     6560 2023-04-25 11:25:07.575026 valida-0.5.2/valida/rules.py
+-rw-r--r--   0        0        0     3885 2023-04-25 11:25:07.575026 valida-0.5.2/valida/schema.py
+-rw-r--r--   0        0        0      869 2023-04-25 11:25:07.575026 valida-0.5.2/valida/utils.py
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 valida-0.5.2/PKG-INFO
```

### Comparing `valida-0.5.1/LICENSE` & `valida-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/README.md` & `valida-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/pyproject.toml` & `valida-0.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "valida"
-version = "0.5.1"
+version = "0.5.2"
 description = "Comprehensive validation library for nested data structures."
 authors = ["Adam J. Plowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -16,15 +16,15 @@
 pytest = "^6.2.5"
 commitizen = "^2.20.3"
 pre-commit = "^2.16.0"
 black = "^21.12b0"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.1"
+version = "0.5.2"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "valida/__init__.py"
 ]
 
 [build-system]
```

### Comparing `valida-0.5.1/valida/callables.py` & `valida-0.5.2/valida/callables.py`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/valida/conditions.py` & `valida-0.5.2/valida/conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,14 +526,15 @@
 
         return condition_like
 
     @classmethod
     def from_json_like(cls, json_like, *args, **kwargs):
         return cls.from_spec(json_like)
 
+
 class Condition(ConditionLike):
 
     PRE_PROCESSOR = None
 
     def __init__(self, callable, *args, **kwargs):
         """
         Parameters
```

### Comparing `valida-0.5.1/valida/data.py` & `valida-0.5.2/valida/data.py`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/valida/datapath.py` & `valida-0.5.2/valida/datapath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import copy
 import enum
-from multiprocessing.dummy import Value
-from os import path
-from tkinter import E
 
 import valida.data
 import valida.conditions as cnds
 from valida.errors import (
     DuplicateRule,
     IncompatibleRules,
-    MalformedContainerItemSpec,
     MalformedDataPathSpec,
 )
 
 
 def get_container_value_condition(
     condition,
     datum_condition,
```

### Comparing `valida-0.5.1/valida/rules.py` & `valida-0.5.2/valida/rules.py`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/valida/schema.py` & `valida-0.5.2/valida/schema.py`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/valida/utils.py` & `valida-0.5.2/valida/utils.py`

 * *Files identical despite different names*

### Comparing `valida-0.5.1/PKG-INFO` & `valida-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valida
-Version: 0.5.1
+Version: 0.5.2
 Summary: Comprehensive validation library for nested data structures.
 License: MIT
 Author: Adam J. Plowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

