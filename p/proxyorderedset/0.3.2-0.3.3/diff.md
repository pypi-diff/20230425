# Comparing `tmp/proxyorderedset-0.3.2.tar.gz` & `tmp/proxyorderedset-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyorderedset-0.3.2.tar", last modified: Fri Apr 21 13:49:53 2023, max compression
+gzip compressed data, was "proxyorderedset-0.3.3.tar", last modified: Tue Apr 25 13:11:16 2023, max compression
```

## Comparing `proxyorderedset-0.3.2.tar` & `proxyorderedset-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.186386 proxyorderedset-0.3.2/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1211 2021-12-21 10:52:02.000000 proxyorderedset-0.3.2/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2023-04-21 13:49:53.186540 proxyorderedset-0.3.2/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      552 2022-08-03 14:10:17.000000 proxyorderedset-0.3.2/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      815 2023-04-21 13:48:32.000000 proxyorderedset-0.3.2/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1071 2023-04-21 13:49:53.186985 proxyorderedset-0.3.2/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:03:26.000000 proxyorderedset-0.3.2/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.181514 proxyorderedset-0.3.2/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.184102 proxyorderedset-0.3.2/src/orderedset/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      119 2023-04-21 13:48:36.000000 proxyorderedset-0.3.2/src/orderedset/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     9988 2023-04-21 13:48:24.000000 proxyorderedset-0.3.2/src/orderedset/orderedset.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.185740 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      346 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      191 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       11 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/top_level.txt
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.186022 proxyorderedset-0.3.2/tests/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     5172 2022-08-03 14:14:09.000000 proxyorderedset-0.3.2/tests/test_orderedset.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-25 13:11:16.517727 proxyorderedset-0.3.3/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1211 2021-12-21 10:52:02.000000 proxyorderedset-0.3.3/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2023-04-25 13:11:16.517950 proxyorderedset-0.3.3/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      552 2022-08-03 14:10:17.000000 proxyorderedset-0.3.3/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      815 2023-04-25 13:10:14.000000 proxyorderedset-0.3.3/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1071 2023-04-25 13:11:16.518736 proxyorderedset-0.3.3/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:03:26.000000 proxyorderedset-0.3.3/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-25 13:11:16.511429 proxyorderedset-0.3.3/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-25 13:11:16.514293 proxyorderedset-0.3.3/src/orderedset/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      119 2023-04-25 13:10:07.000000 proxyorderedset-0.3.3/src/orderedset/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     9996 2023-04-25 13:09:40.000000 proxyorderedset-0.3.3/src/orderedset/orderedset.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-25 13:11:16.516250 proxyorderedset-0.3.3/src/proxyorderedset.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2023-04-25 13:11:16.000000 proxyorderedset-0.3.3/src/proxyorderedset.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      346 2023-04-25 13:11:16.000000 proxyorderedset-0.3.3/src/proxyorderedset.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-25 13:11:16.000000 proxyorderedset-0.3.3/src/proxyorderedset.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      191 2023-04-25 13:11:16.000000 proxyorderedset-0.3.3/src/proxyorderedset.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       11 2023-04-25 13:11:16.000000 proxyorderedset-0.3.3/src/proxyorderedset.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-25 13:11:16.516760 proxyorderedset-0.3.3/tests/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     5172 2022-08-03 14:14:09.000000 proxyorderedset-0.3.3/tests/test_orderedset.py
```

### Comparing `proxyorderedset-0.3.2/LICENSE` & `proxyorderedset-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyorderedset-0.3.2/PKG-INFO` & `proxyorderedset-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyorderedset
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple implementation of ordered sets as a proxy to Python's standard dict class.
 Home-page: https://github.com/rindPHI/proxyorderedset
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `proxyorderedset-0.3.2/README.md` & `proxyorderedset-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `proxyorderedset-0.3.2/pyproject.toml` & `proxyorderedset-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxyorderedset"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "A simple implementation of ordered sets as a proxy to Python's standard dict class."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `proxyorderedset-0.3.2/setup.cfg` & `proxyorderedset-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `proxyorderedset-0.3.2/src/orderedset/orderedset.py` & `proxyorderedset-0.3.3/src/orderedset/orderedset.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                     return elem
 
                 idx += 1
 
             assert False
         else:
             start = item.start or 0
-            stop = item.stop or 0
+            stop = item.stop or len(self)
             step = item.step or 1
 
             return OrderedSet(itertools.islice(iter(self), start, stop, step))
 
     def add(self, element: T) -> None:
         self.the_dict = {**self.the_dict, **{element: None}}
```

### Comparing `proxyorderedset-0.3.2/src/proxyorderedset.egg-info/PKG-INFO` & `proxyorderedset-0.3.3/src/proxyorderedset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyorderedset
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple implementation of ordered sets as a proxy to Python's standard dict class.
 Home-page: https://github.com/rindPHI/proxyorderedset
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `proxyorderedset-0.3.2/tests/test_orderedset.py` & `proxyorderedset-0.3.3/tests/test_orderedset.py`

 * *Files identical despite different names*

