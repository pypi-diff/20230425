# Comparing `tmp/dyn2py-0.4.0.tar.gz` & `tmp/dyn2py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyn2py-0.4.0.tar", last modified: Mon Apr 24 22:49:45 2023, max compression
+gzip compressed data, was "dyn2py-0.4.1.tar", last modified: Mon Apr 24 23:05:15 2023, max compression
```

## Comparing `dyn2py-0.4.0.tar` & `dyn2py-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.209891 dyn2py-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 22:49:34.000000 dyn2py-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48731 2023-04-24 22:49:45.209891 dyn2py-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-24 22:49:34.000000 dyn2py-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.205891 dyn2py-0.4.0/dyn2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26475 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.209891 dyn2py-0.4.0/dyn2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48731 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-24 22:49:34.000000 dyn2py-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:49:45.209891 dyn2py-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.209891 dyn2py-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_CommandLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_DynamoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_File.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_PythonFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_PythonNode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:15.190137 dyn2py-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 23:05:03.000000 dyn2py-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48731 2023-04-24 23:05:15.190137 dyn2py-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-24 23:05:03.000000 dyn2py-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:15.186137 dyn2py-0.4.1/dyn2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-24 23:05:03.000000 dyn2py-0.4.1/dyn2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 23:05:03.000000 dyn2py-0.4.1/dyn2py/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26475 2023-04-24 23:05:03.000000 dyn2py-0.4.1/dyn2py/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-24 23:05:03.000000 dyn2py-0.4.1/dyn2py/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:15.190137 dyn2py-0.4.1/dyn2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48731 2023-04-24 23:05:15.000000 dyn2py-0.4.1/dyn2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 23:05:15.000000 dyn2py-0.4.1/dyn2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:15.000000 dyn2py-0.4.1/dyn2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 23:05:15.000000 dyn2py-0.4.1/dyn2py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 23:05:15.000000 dyn2py-0.4.1/dyn2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 23:05:15.000000 dyn2py-0.4.1/dyn2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-24 23:05:03.000000 dyn2py-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:05:15.190137 dyn2py-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:15.190137 dyn2py-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-04-24 23:05:03.000000 dyn2py-0.4.1/tests/test_CommandLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-24 23:05:03.000000 dyn2py-0.4.1/tests/test_DynamoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 23:05:03.000000 dyn2py-0.4.1/tests/test_File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 23:05:03.000000 dyn2py-0.4.1/tests/test_PythonFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 23:05:03.000000 dyn2py-0.4.1/tests/test_PythonNode.py
```

### Comparing `dyn2py-0.4.0/LICENSE` & `dyn2py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/PKG-INFO` & `dyn2py-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyn2py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Extract python code from Dynamo graphs
 Author-email: infeeeee <gyetpet@mailbox.org>
 Maintainer-email: infeeeee <gyetpet@mailbox.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dyn2py-0.4.0/README.md` & `dyn2py-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/dyn2py/__init__.py` & `dyn2py-0.4.1/dyn2py/__init__.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/dyn2py/files.py` & `dyn2py-0.4.1/dyn2py/files.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/dyn2py/options.py` & `dyn2py-0.4.1/dyn2py/options.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/dyn2py.egg-info/PKG-INFO` & `dyn2py-0.4.1/dyn2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyn2py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Extract python code from Dynamo graphs
 Author-email: infeeeee <gyetpet@mailbox.org>
 Maintainer-email: infeeeee <gyetpet@mailbox.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dyn2py-0.4.0/pyproject.toml` & `dyn2py-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dyn2py"
-version = "0.4.0"
+version = "0.4.1"
 description = "Extract python code from Dynamo graphs"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["dynamo", "dyn", "visual programming"]
 license = { file = "LICENSE" }
```

### Comparing `dyn2py-0.4.0/tests/test_CommandLine.py` & `dyn2py-0.4.1/tests/test_CommandLine.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/tests/test_DynamoFile.py` & `dyn2py-0.4.1/tests/test_DynamoFile.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/tests/test_File.py` & `dyn2py-0.4.1/tests/test_File.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/tests/test_PythonFile.py` & `dyn2py-0.4.1/tests/test_PythonFile.py`

 * *Files identical despite different names*

### Comparing `dyn2py-0.4.0/tests/test_PythonNode.py` & `dyn2py-0.4.1/tests/test_PythonNode.py`

 * *Files identical despite different names*

