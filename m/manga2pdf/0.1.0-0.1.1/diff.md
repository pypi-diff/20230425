# Comparing `tmp/manga2pdf-0.1.0.tar.gz` & `tmp/manga2pdf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga2pdf-0.1.0.tar", last modified: Sun Apr 16 05:49:21 2023, max compression
+gzip compressed data, was "manga2pdf-0.1.1.tar", last modified: Tue Apr 25 05:46:46 2023, max compression
```

## Comparing `manga2pdf-0.1.0.tar` & `manga2pdf-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-16 05:49:21.417041 manga2pdf-0.1.0/
--rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.0/LICENSE
--rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-16 05:49:21.416910 manga2pdf-0.1.0/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)     5369 2023-04-15 20:09:50.000000 manga2pdf-0.1.0/README.md
--rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-16 05:49:21.417106 manga2pdf-0.1.0/setup.cfg
--rw-r--r--   0 shun       (501) staff       (20)     1052 2023-04-16 05:42:55.000000 manga2pdf-0.1.0/setup.py
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-16 05:49:21.415760 manga2pdf-0.1.0/src/
-drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-16 05:49:21.416721 manga2pdf-0.1.0/src/manga2pdf.egg-info/
--rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/PKG-INFO
--rw-r--r--   0 shun       (501) staff       (20)      288 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/entry_points.txt
--rw-r--r--   0 shun       (501) staff       (20)       46 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/requires.txt
--rw-r--r--   0 shun       (501) staff       (20)       24 2023-04-16 05:49:21.000000 manga2pdf-0.1.0/src/manga2pdf.egg-info/top_level.txt
--rw-r--r--   0 shun       (501) staff       (20)    17683 2023-04-15 20:21:17.000000 manga2pdf-0.1.0/src/manga2pdf.py
--rw-r--r--   0 shun       (501) staff       (20)    18189 2023-04-15 20:21:57.000000 manga2pdf-0.1.0/src/manga2pdf_gui.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-25 05:46:46.726258 manga2pdf-0.1.1/
+-rw-r--r--   0 shun       (501) staff       (20)     1063 2023-03-12 05:13:58.000000 manga2pdf-0.1.1/LICENSE
+-rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-25 05:46:46.726152 manga2pdf-0.1.1/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)     5369 2023-04-15 20:09:50.000000 manga2pdf-0.1.1/README.md
+-rw-r--r--   0 shun       (501) staff       (20)       38 2023-04-25 05:46:46.726286 manga2pdf-0.1.1/setup.cfg
+-rw-r--r--   0 shun       (501) staff       (20)     1065 2023-04-22 06:44:25.000000 manga2pdf-0.1.1/setup.py
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-25 05:46:46.725430 manga2pdf-0.1.1/src/
+drwxr-xr-x   0 shun       (501) staff       (20)        0 2023-04-25 05:46:46.726022 manga2pdf-0.1.1/src/manga2pdf.egg-info/
+-rw-r--r--   0 shun       (501) staff       (20)     5913 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/PKG-INFO
+-rw-r--r--   0 shun       (501) staff       (20)      288 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 shun       (501) staff       (20)        1 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 shun       (501) staff       (20)       45 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/entry_points.txt
+-rw-r--r--   0 shun       (501) staff       (20)       52 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/requires.txt
+-rw-r--r--   0 shun       (501) staff       (20)       24 2023-04-25 05:46:46.000000 manga2pdf-0.1.1/src/manga2pdf.egg-info/top_level.txt
+-rw-r--r--   0 shun       (501) staff       (20)    17683 2023-04-15 20:21:17.000000 manga2pdf-0.1.1/src/manga2pdf.py
+-rw-r--r--   0 shun       (501) staff       (20)    18189 2023-04-15 20:21:57.000000 manga2pdf-0.1.1/src/manga2pdf_gui.py
```

### Comparing `manga2pdf-0.1.0/LICENSE` & `manga2pdf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.0/PKG-INFO` & `manga2pdf-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `manga2pdf-0.1.0/README.md` & `manga2pdf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.0/setup.py` & `manga2pdf-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 INSTALL_REQUIRES = (
+    "numpy",
     "img2pdf",
     "Pillow",
     "pikepdf",
     "rarfile",
     "beautifulsoup4"
 )
 CLASSIFIERS=[
```

### Comparing `manga2pdf-0.1.0/src/manga2pdf.egg-info/PKG-INFO` & `manga2pdf-0.1.1/src/manga2pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga2pdf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convert manga/comic files(zip, epub, etc.) or directory containing image files (jpg, png, etc.) to PDF.
 Home-page: https://github.com/mashu3/manga2pdf
 Author: mashu3
 License: MIT
 Keywords: manga comic pdf converter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `manga2pdf-0.1.0/src/manga2pdf.py` & `manga2pdf-0.1.1/src/manga2pdf.py`

 * *Files identical despite different names*

### Comparing `manga2pdf-0.1.0/src/manga2pdf_gui.py` & `manga2pdf-0.1.1/src/manga2pdf_gui.py`

 * *Files identical despite different names*

