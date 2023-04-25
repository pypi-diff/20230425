# Comparing `tmp/pyrepresent-0.0.7.tar.gz` & `tmp/pyrepresent-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.0.7.tar", last modified: Sun Apr 16 14:51:53 2023, max compression
+gzip compressed data, was "pyrepresent-0.0.8.tar", last modified: Tue Apr 25 10:08:36 2023, max compression
```

## Comparing `pyrepresent-0.0.7.tar` & `pyrepresent-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:51:53.114583 pyrepresent-0.0.7/
--rw-rw-rw-   0        0        0      115 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-04-16 14:51:53.114583 pyrepresent-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.7/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.7/build.py
--rw-rw-rw-   0        0        0      715 2023-04-16 14:51:48.000000 pyrepresent-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-16 14:51:53.088067 pyrepresent-0.0.7/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-16 14:51:53.000000 pyrepresent-0.0.7/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 14:51:53.113581 pyrepresent-0.0.7/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.7/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.7/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.7/represent/document.py
--rw-rw-rw-   0        0        0     2121 2023-04-05 09:22:18.000000 pyrepresent-0.0.7/represent/indentation.py
--rw-rw-rw-   0        0        0    11534 2023-04-16 14:51:13.000000 pyrepresent-0.0.7/represent/object.py
--rw-rw-rw-   0        0        0    19611 2023-04-09 18:51:47.000000 pyrepresent-0.0.7/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.7/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:51:53.114583 pyrepresent-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-16 14:51:47.000000 pyrepresent-0.0.7/setup.py
--rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.7/test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:08:36.494293 pyrepresent-0.0.8/
+-rw-rw-rw-   0        0        0      115 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-04-25 10:08:36.493294 pyrepresent-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.8/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.8/build.py
+-rw-rw-rw-   0        0        0      715 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 10:08:36.470324 pyrepresent-0.0.8/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-25 10:08:36.000000 pyrepresent-0.0.8/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:08:36.492295 pyrepresent-0.0.8/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.8/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.8/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.8/represent/document.py
+-rw-rw-rw-   0        0        0     2121 2023-04-05 09:22:18.000000 pyrepresent-0.0.8/represent/indentation.py
+-rw-rw-rw-   0        0        0    11534 2023-04-16 14:51:13.000000 pyrepresent-0.0.8/represent/object.py
+-rw-rw-rw-   0        0        0    19724 2023-04-25 10:08:07.000000 pyrepresent-0.0.8/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.8/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:08:36.494293 pyrepresent-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-25 10:08:31.000000 pyrepresent-0.0.8/setup.py
+-rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.8/test.py
```

### Comparing `pyrepresent-0.0.7/PKG-INFO` & `pyrepresent-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.7
+Version: 0.0.8
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.7/README.md` & `pyrepresent-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.7/build.py` & `pyrepresent-0.0.8/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.7/pyproject.toml` & `pyrepresent-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.0.7'
+version = '0.0.8'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.0.7/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.0.8/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.7
+Version: 0.0.8
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.7/represent/base.py` & `pyrepresent-0.0.8/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.7/represent/indentation.py` & `pyrepresent-0.0.8/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.7/represent/object.py` & `pyrepresent-0.0.8/represent/object.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.7/represent/structures.py` & `pyrepresent-0.0.8/represent/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,21 @@
 class DataStructure(metaclass=DataStructureMeta):
     """A class to represent a structure."""
 
     __type__ = None
     __value__ = None
     __class__ = False
 
-    color = is_proxy_process()
+    # noinspection PyBroadException
+    try:
+        color = is_proxy_process()
+
+    except Exception:
+        color = True
+    # end try
 
     def __repr__(self) -> str:
         """
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
```

### Comparing `pyrepresent-0.0.7/setup.py` & `pyrepresent-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.0.7',
+        version='0.0.8',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.0.7/test.py` & `pyrepresent-0.0.8/test.py`

 * *Files identical despite different names*

