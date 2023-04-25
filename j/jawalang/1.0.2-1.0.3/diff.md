# Comparing `tmp/jawalang-1.0.2.tar.gz` & `tmp/jawalang-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jawalang-1.0.2.tar", last modified: Tue Apr 25 00:30:09 2023, max compression
+gzip compressed data, was "jawalang-1.0.3.tar", last modified: Tue Apr 25 00:31:44 2023, max compression
```

## Comparing `jawalang-1.0.2.tar` & `jawalang-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:30:09.185038 jawalang-1.0.2/
--rw-rw-rw-   0        0        0     1085 2023-04-23 23:08:13.000000 jawalang-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1151 2023-04-25 00:30:09.184042 jawalang-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      816 2023-04-25 00:07:04.000000 jawalang-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:30:09.170125 jawalang-1.0.2/jawalang/
--rw-rw-rw-   0        0        0        4 2023-04-25 00:26:59.000000 jawalang-1.0.2/jawalang/__init__.py
--rw-rw-rw-   0        0        0     2990 2023-04-25 00:29:50.000000 jawalang-1.0.2/jawalang/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:30:09.183030 jawalang-1.0.2/jawalang.egg-info/
--rw-rw-rw-   0        0        0     1151 2023-04-25 00:30:09.000000 jawalang-1.0.2/jawalang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-04-25 00:30:09.000000 jawalang-1.0.2/jawalang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:30:09.000000 jawalang-1.0.2/jawalang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-25 00:30:09.000000 jawalang-1.0.2/jawalang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 00:30:09.000000 jawalang-1.0.2/jawalang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 00:30:09.185038 jawalang-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-04-25 00:29:55.000000 jawalang-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:31:44.705488 jawalang-1.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-04-23 23:08:13.000000 jawalang-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1151 2023-04-25 00:31:44.704494 jawalang-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-04-25 00:07:04.000000 jawalang-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:31:44.686870 jawalang-1.0.3/jawalang/
+-rw-rw-rw-   0        0        0        4 2023-04-25 00:26:59.000000 jawalang-1.0.3/jawalang/__init__.py
+-rw-rw-rw-   0        0        0     3008 2023-04-25 00:31:35.000000 jawalang-1.0.3/jawalang/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:31:44.703218 jawalang-1.0.3/jawalang.egg-info/
+-rw-rw-rw-   0        0        0     1151 2023-04-25 00:31:44.000000 jawalang-1.0.3/jawalang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-25 00:31:44.000000 jawalang-1.0.3/jawalang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:31:44.000000 jawalang-1.0.3/jawalang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-25 00:31:44.000000 jawalang-1.0.3/jawalang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 00:31:44.000000 jawalang-1.0.3/jawalang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:31:44.705488 jawalang-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-04-25 00:31:03.000000 jawalang-1.0.3/setup.py
```

### Comparing `jawalang-1.0.2/LICENSE` & `jawalang-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jawalang-1.0.2/PKG-INFO` & `jawalang-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jawalang
-Version: 1.0.2
+Version: 1.0.3
 Summary: Javanese programming language base on python
 Home-page: https://github.com/Arsybai/jawa-language
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: programming languages,languages
 Description-Content-Type: text/markdown
```

### Comparing `jawalang-1.0.2/README.md` & `jawalang-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jawalang-1.0.2/jawalang/__main__.py` & `jawalang-1.0.3/jawalang/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys, re, os, traceback
-from logic.transform import transform
-from logic.errorHandle import error
+from jawalang.logic.transform import transform
+from jawalang.logic.errorHandle import error
 
 def pars(script):
     scriptL = script.split("\n")
     final = ""
     for s in scriptL:
         def replace(match):
             keyword = match.group(1)
```

### Comparing `jawalang-1.0.2/jawalang.egg-info/PKG-INFO` & `jawalang-1.0.3/jawalang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jawalang
-Version: 1.0.2
+Version: 1.0.3
 Summary: Javanese programming language base on python
 Home-page: https://github.com/Arsybai/jawa-language
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: programming languages,languages
 Description-Content-Type: text/markdown
```

### Comparing `jawalang-1.0.2/setup.py` & `jawalang-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="jawalang",
-    version="1.0.2",
+    version="1.0.3",
     author="Arsybai",
     description="Javanese programming language base on python",
     packages=["jawalang"],
     license="MIT",
     author_email="me@arsybai.com",
     url="https://github.com/Arsybai/jawa-language",
     keywords=[
```

