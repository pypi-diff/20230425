# Comparing `tmp/tomplotlib-1.2.1.tar.gz` & `tmp/tomplotlib-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomplotlib-1.2.1.tar", last modified: Wed Apr 12 14:02:42 2023, max compression
+gzip compressed data, was "tomplotlib-1.2.2.tar", last modified: Tue Apr 25 10:21:20 2023, max compression
```

## Comparing `tomplotlib-1.2.1.tar` & `tomplotlib-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 14:02:42.578047 tomplotlib-1.2.1/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-12 14:02:42.577866 tomplotlib-1.2.1/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2436 2023-04-12 13:44:36.000000 tomplotlib-1.2.1/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       38 2023-04-12 14:02:42.578101 tomplotlib-1.2.1/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)      757 2023-04-12 14:02:39.000000 tomplotlib-1.2.1/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 14:02:42.576787 tomplotlib-1.2.1/tomplotlib/
--rw-r--r--   0 tomgeorge   (501) staff       (20)       43 2023-04-12 14:02:30.000000 tomplotlib-1.2.1/tomplotlib/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7854 2023-04-12 14:02:34.000000 tomplotlib-1.2.1/tomplotlib/tpl.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-12 14:02:42.577542 tomplotlib-1.2.1/tomplotlib.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      228 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       17 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       11 2023-04-12 14:02:42.000000 tomplotlib-1.2.1/tomplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 10:21:20.584765 tomplotlib-1.2.2/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-25 10:21:20.584638 tomplotlib-1.2.2/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2436 2023-04-12 13:44:36.000000 tomplotlib-1.2.2/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       38 2023-04-25 10:21:20.584800 tomplotlib-1.2.2/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      757 2023-04-25 10:21:02.000000 tomplotlib-1.2.2/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 10:21:20.583723 tomplotlib-1.2.2/tomplotlib/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       43 2023-04-12 14:02:30.000000 tomplotlib-1.2.2/tomplotlib/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7854 2023-04-12 14:02:34.000000 tomplotlib-1.2.2/tomplotlib/tpl.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-25 10:21:20.584447 tomplotlib-1.2.2/tomplotlib.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2880 2023-04-25 10:21:20.000000 tomplotlib-1.2.2/tomplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      228 2023-04-25 10:21:20.000000 tomplotlib-1.2.2/tomplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-25 10:21:20.000000 tomplotlib-1.2.2/tomplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       17 2023-04-25 10:21:20.000000 tomplotlib-1.2.2/tomplotlib.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       11 2023-04-25 10:21:20.000000 tomplotlib-1.2.2/tomplotlib.egg-info/top_level.txt
```

### Comparing `tomplotlib-1.2.1/PKG-INFO` & `tomplotlib-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomplotlib
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package which formats matplotlib plots and contains some other useful functions
 Home-page: https://github.com/TomGeorge1234/tomplotlib
 Author: Tom George
 Author-email: tom.george.20@ucl.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tomplotlib-1.2.1/README.md` & `tomplotlib-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tomplotlib-1.2.1/setup.py` & `tomplotlib-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tomplotlib",
-    version="1.2.1",
+    version="1.2.2",
     scripts=["tomplotlib/tpl.py"],
     author="Tom George",
     author_email="tom.george.20@ucl.ac.uk",
     description="A package which formats matplotlib plots and contains some other useful functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TomGeorge1234/tomplotlib",
```

### Comparing `tomplotlib-1.2.1/tomplotlib/tpl.py` & `tomplotlib-1.2.2/tomplotlib/tpl.py`

 * *Files identical despite different names*

### Comparing `tomplotlib-1.2.1/tomplotlib.egg-info/PKG-INFO` & `tomplotlib-1.2.2/tomplotlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomplotlib
-Version: 1.2.1
+Version: 1.2.2
 Summary: A package which formats matplotlib plots and contains some other useful functions
 Home-page: https://github.com/TomGeorge1234/tomplotlib
 Author: Tom George
 Author-email: tom.george.20@ucl.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

