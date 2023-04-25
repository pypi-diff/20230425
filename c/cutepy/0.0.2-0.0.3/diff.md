# Comparing `tmp/cutepy-0.0.2.tar.gz` & `tmp/cutepy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutepy-0.0.2.tar", last modified: Tue Apr 25 13:13:34 2023, max compression
+gzip compressed data, was "cutepy-0.0.3.tar", last modified: Tue Apr 25 13:22:55 2023, max compression
```

## Comparing `cutepy-0.0.2.tar` & `cutepy-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:13:34.148921 cutepy-0.0.2/
--rw-rw-r--   0 gast      (1000) gast      (1000)     1996 2023-04-25 13:13:34.148921 cutepy-0.0.2/PKG-INFO
--rw-rw-r--   0 gast      (1000) gast      (1000)     1629 2023-04-25 13:08:42.000000 cutepy-0.0.2/README.md
-drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:13:34.148921 cutepy-0.0.2/cutepy/
--rw-rw-r--   0 gast      (1000) gast      (1000)        0 2023-04-25 12:52:17.000000 cutepy-0.0.2/cutepy/__init__.py
--rw-rw-r--   0 gast      (1000) gast      (1000)     4193 2023-04-25 13:06:52.000000 cutepy-0.0.2/cutepy/cutepy.py
-drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:13:34.148921 cutepy-0.0.2/cutepy.egg-info/
--rw-rw-r--   0 gast      (1000) gast      (1000)     1996 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/PKG-INFO
--rw-rw-r--   0 gast      (1000) gast      (1000)      174 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/SOURCES.txt
--rw-rw-r--   0 gast      (1000) gast      (1000)        1 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/dependency_links.txt
--rw-rw-r--   0 gast      (1000) gast      (1000)        7 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/top_level.txt
--rw-rw-r--   0 gast      (1000) gast      (1000)       38 2023-04-25 13:13:34.148921 cutepy-0.0.2/setup.cfg
--rw-rw-r--   0 gast      (1000) gast      (1000)      761 2023-04-25 13:13:32.000000 cutepy-0.0.2/setup.py
+drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:22:55.034098 cutepy-0.0.3/
+-rw-rw-r--   0 gast      (1000) gast      (1000)     1996 2023-04-25 13:22:55.034098 cutepy-0.0.3/PKG-INFO
+-rw-rw-r--   0 gast      (1000) gast      (1000)     1629 2023-04-25 13:08:42.000000 cutepy-0.0.3/README.md
+drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:22:55.034098 cutepy-0.0.3/cutepy/
+-rw-rw-r--   0 gast      (1000) gast      (1000)     4193 2023-04-25 13:22:04.000000 cutepy-0.0.3/cutepy/__init__.py
+-rw-rw-r--   0 gast      (1000) gast      (1000)     4193 2023-04-25 13:06:52.000000 cutepy-0.0.3/cutepy/cutepy.py
+drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:22:55.034098 cutepy-0.0.3/cutepy.egg-info/
+-rw-rw-r--   0 gast      (1000) gast      (1000)     1996 2023-04-25 13:22:55.000000 cutepy-0.0.3/cutepy.egg-info/PKG-INFO
+-rw-rw-r--   0 gast      (1000) gast      (1000)      174 2023-04-25 13:22:55.000000 cutepy-0.0.3/cutepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gast      (1000) gast      (1000)        1 2023-04-25 13:22:55.000000 cutepy-0.0.3/cutepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gast      (1000) gast      (1000)        7 2023-04-25 13:22:55.000000 cutepy-0.0.3/cutepy.egg-info/top_level.txt
+-rw-rw-r--   0 gast      (1000) gast      (1000)       38 2023-04-25 13:22:55.034098 cutepy-0.0.3/setup.cfg
+-rw-rw-r--   0 gast      (1000) gast      (1000)      761 2023-04-25 13:22:25.000000 cutepy-0.0.3/setup.py
```

### Comparing `cutepy-0.0.2/PKG-INFO` & `cutepy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutepy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A helpfull python package!
 Home-page: UNKNOWN
 Author: Birdlinux (G. P.)
 Author-email: <prepakis.geo@gmail.com>
 License: UNKNOWN
 Keywords: python,python system Detection,python hex,python rgb,python hex,python loader,rich python,python rich,cutepy
 Platform: UNKNOWN
```

### Comparing `cutepy-0.0.2/README.md` & `cutepy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cutepy-0.0.2/cutepy/cutepy.py` & `cutepy-0.0.3/cutepy/__init__.py`

 * *Files identical despite different names*

### Comparing `cutepy-0.0.2/cutepy.egg-info/PKG-INFO` & `cutepy-0.0.3/cutepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutepy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A helpfull python package!
 Home-page: UNKNOWN
 Author: Birdlinux (G. P.)
 Author-email: <prepakis.geo@gmail.com>
 License: UNKNOWN
 Keywords: python,python system Detection,python hex,python rgb,python hex,python loader,rich python,python rich,cutepy
 Platform: UNKNOWN
```

### Comparing `cutepy-0.0.2/setup.py` & `cutepy-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A helpfull python package!'
 this_directory = Path(__file__).parent
 LONG_DES = (this_directory / "README.md").read_text()
 # Setting up
 setup(
     name="cutepy",
     version=VERSION,
```

