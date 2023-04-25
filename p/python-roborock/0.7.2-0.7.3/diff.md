# Comparing `tmp/python_roborock-0.7.2.tar.gz` & `tmp/python_roborock-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.7.2.tar", max compression
+gzip compressed data, was "python_roborock-0.7.3.tar", max compression
```

## Comparing `python_roborock-0.7.2.tar` & `python_roborock-0.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-25 11:57:05.494174 python_roborock-0.7.2/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-25 11:57:05.494174 python_roborock-0.7.2/README.md
--rw-r--r--   0        0        0     1370 2023-04-25 11:57:06.242186 python_roborock-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-25 11:57:05.494174 python_roborock-0.7.2/roborock/__init__.py
--rw-r--r--   0        0        0    19300 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/cloud_api.py
--rw-r--r--   0        0        0     4283 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/code_mappings.py
--rw-r--r--   0        0        0     9872 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/exceptions.py
--rw-r--r--   0        0        0     6178 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/roborock_message.py
--rw-r--r--   0        0        0    12103 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/typing.py
--rw-r--r--   0        0        0      754 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-25 12:21:43.377767 python_roborock-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-25 12:21:43.377767 python_roborock-0.7.3/README.md
+-rw-r--r--   0        0        0     1370 2023-04-25 12:21:44.101740 python_roborock-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/__init__.py
+-rw-r--r--   0        0        0    19300 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/cli.py
+-rw-r--r--   0        0        0     8241 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4383 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9872 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/exceptions.py
+-rw-r--r--   0        0        0     6178 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12103 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/typing.py
+-rw-r--r--   0        0        0      754 2023-04-25 12:21:43.377767 python_roborock-0.7.3/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.3/PKG-INFO
```

### Comparing `python_roborock-0.7.2/LICENSE` & `python_roborock-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/README.md` & `python_roborock-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/pyproject.toml` & `python_roborock-0.7.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.7.2"
+version = "0.7.3"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.7.2/roborock/api.py` & `python_roborock-0.7.3/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/cli.py` & `python_roborock-0.7.3/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/cloud_api.py` & `python_roborock-0.7.3/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/code_mappings.py` & `python_roborock-0.7.3/roborock/code_mappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,15 +150,19 @@
     },
 )
 
 RoborockDockTypeCode = create_code_enum(
     "RoborockDockTypeCode",
     {
         0: "no_dock",
+        1: "unknown",
+        2: "unknown",
         3: "empty_wash_fill_dock",
+        4: "unknown",
+        5: "auto_empty_dock_pure"
     },
 )
 
 RoborockDockDustCollectionModeCode = create_code_enum(
     "RoborockDockDustCollectionModeCode",
     {
         0: "smart",
```

### Comparing `python_roborock-0.7.2/roborock/containers.py` & `python_roborock-0.7.3/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/exceptions.py` & `python_roborock-0.7.3/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/local_api.py` & `python_roborock-0.7.3/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/roborock_future.py` & `python_roborock-0.7.3/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/roborock_message.py` & `python_roborock-0.7.3/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/typing.py` & `python_roborock-0.7.3/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/roborock/util.py` & `python_roborock-0.7.3/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.2/PKG-INFO` & `python_roborock-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.7.2
+Version: 0.7.3
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.7.2 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.7.3 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

