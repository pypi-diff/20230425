# Comparing `tmp/cutepy-0.0.1.tar.gz` & `tmp/cutepy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutepy-0.0.1.tar", last modified: Tue Apr 25 12:54:36 2023, max compression
+gzip compressed data, was "cutepy-0.0.2.tar", last modified: Tue Apr 25 13:13:34 2023, max compression
```

## Comparing `cutepy-0.0.1.tar` & `cutepy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 12:54:36.546708 cutepy-0.0.1/
--rw-rw-r--   0 gast      (1000) gast      (1000)      447 2023-04-25 12:54:36.546708 cutepy-0.0.1/PKG-INFO
-drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 12:54:36.546708 cutepy-0.0.1/cutepy/
--rw-rw-r--   0 gast      (1000) gast      (1000)        0 2023-04-25 12:52:17.000000 cutepy-0.0.1/cutepy/__init__.py
--rw-rw-r--   0 gast      (1000) gast      (1000)     4182 2023-04-25 12:34:12.000000 cutepy-0.0.1/cutepy/cutepy.py
-drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 12:54:36.546708 cutepy-0.0.1/cutepy.egg-info/
--rw-rw-r--   0 gast      (1000) gast      (1000)      447 2023-04-25 12:54:36.000000 cutepy-0.0.1/cutepy.egg-info/PKG-INFO
--rw-rw-r--   0 gast      (1000) gast      (1000)      164 2023-04-25 12:54:36.000000 cutepy-0.0.1/cutepy.egg-info/SOURCES.txt
--rw-rw-r--   0 gast      (1000) gast      (1000)        1 2023-04-25 12:54:36.000000 cutepy-0.0.1/cutepy.egg-info/dependency_links.txt
--rw-rw-r--   0 gast      (1000) gast      (1000)        7 2023-04-25 12:54:36.000000 cutepy-0.0.1/cutepy.egg-info/top_level.txt
--rw-rw-r--   0 gast      (1000) gast      (1000)       38 2023-04-25 12:54:36.546708 cutepy-0.0.1/setup.cfg
--rw-rw-r--   0 gast      (1000) gast      (1000)      753 2023-04-25 12:53:04.000000 cutepy-0.0.1/setup.py
+drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:13:34.148921 cutepy-0.0.2/
+-rw-rw-r--   0 gast      (1000) gast      (1000)     1996 2023-04-25 13:13:34.148921 cutepy-0.0.2/PKG-INFO
+-rw-rw-r--   0 gast      (1000) gast      (1000)     1629 2023-04-25 13:08:42.000000 cutepy-0.0.2/README.md
+drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:13:34.148921 cutepy-0.0.2/cutepy/
+-rw-rw-r--   0 gast      (1000) gast      (1000)        0 2023-04-25 12:52:17.000000 cutepy-0.0.2/cutepy/__init__.py
+-rw-rw-r--   0 gast      (1000) gast      (1000)     4193 2023-04-25 13:06:52.000000 cutepy-0.0.2/cutepy/cutepy.py
+drwxrwxr-x   0 gast      (1000) gast      (1000)        0 2023-04-25 13:13:34.148921 cutepy-0.0.2/cutepy.egg-info/
+-rw-rw-r--   0 gast      (1000) gast      (1000)     1996 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/PKG-INFO
+-rw-rw-r--   0 gast      (1000) gast      (1000)      174 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gast      (1000) gast      (1000)        1 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gast      (1000) gast      (1000)        7 2023-04-25 13:13:34.000000 cutepy-0.0.2/cutepy.egg-info/top_level.txt
+-rw-rw-r--   0 gast      (1000) gast      (1000)       38 2023-04-25 13:13:34.148921 cutepy-0.0.2/setup.cfg
+-rw-rw-r--   0 gast      (1000) gast      (1000)      761 2023-04-25 13:13:32.000000 cutepy-0.0.2/setup.py
```

### Comparing `cutepy-0.0.1/cutepy/cutepy.py` & `cutepy-0.0.2/cutepy/cutepy.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,27 +140,27 @@
 
 
 # Loading
 # spinners = ["|", "/", "-", "\\"]
 # Loader.spinner("Loading", 4, spinners)
 
 # RGB printing
-# x = RGB.print(252, 145, 83)
-# print(f"Hello {x}RGB{RGB.reset} test {x}aa")
+# x = RGB.print(103, 252, 125)
+# print(f"Hello {x}RGB{RGB.reset} test {x}aa{RGB.reset}"))
 
 # HEX printing
-# x = HEX.print("fc9153")
+# x = HEX.print("6771fc")
 # print(f"Hello {x}RGB{RGB.reset} test {x}aa{RGB.reset}")
 
 # System detection
 # x = System.detect()
 # print(x)
 
 # Terminal clearance
 # Clear.sys()
 
 # Hash identifier
 # x = Identify.hash("a875e3b9476d5d976160b308ace6b62e")
 # print(x)
 
 # Color palette
-# Color.palette()
+Color.palette()
```

### Comparing `cutepy-0.0.1/setup.py` & `cutepy-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A helpfull python package!'
-LONG_DESCRIPTION = 'A package that allows you to have simplicity and effectiveness in your projects!'
-
+this_directory = Path(__file__).parent
+LONG_DES = (this_directory / "README.md").read_text()
 # Setting up
 setup(
     name="cutepy",
     version=VERSION,
     author="Birdlinux (G. P.)",
     author_email="<prepakis.geo@gmail.com>",
     description=DESCRIPTION,
+    long_description= LONG_DES,
     long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'python system Detection', 'python hex', 'python rgb', 'python hex', 'python loader', 'rich python', 'python rich', 'cutepy'],
     classifiers=[]
 )
```

