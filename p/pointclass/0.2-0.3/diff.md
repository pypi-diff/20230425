# Comparing `tmp/pointclass-0.2.tar.gz` & `tmp/pointclass-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-0.2.tar", last modified: Tue Apr 25 10:52:19 2023, max compression
+gzip compressed data, was "pointclass-0.3.tar", last modified: Tue Apr 25 10:59:33 2023, max compression
```

## Comparing `pointclass-0.2.tar` & `pointclass-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 10:52:19.708685 pointclass-0.2/
--rw-rw-rw-   0        0        0      177 2023-04-25 10:52:19.656356 pointclass-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.2/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 10:52:19.627074 pointclass-0.2/pointclass/
--rw-rw-rw-   0        0        0      550 2023-04-25 10:51:58.000000 pointclass-0.2/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 10:52:19.653428 pointclass-0.2/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-04-25 10:52:19.000000 pointclass-0.2/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-04-25 10:52:19.000000 pointclass-0.2/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 10:52:19.000000 pointclass-0.2/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 10:52:19.000000 pointclass-0.2/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 10:52:19.709662 pointclass-0.2/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-04-25 10:52:08.000000 pointclass-0.2/setup1.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:59:33.008828 pointclass-0.3/
+-rw-rw-rw-   0        0        0      177 2023-04-25 10:59:33.007841 pointclass-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.3/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 10:59:32.985395 pointclass-0.3/pointclass/
+-rw-rw-rw-   0        0        0      563 2023-04-25 10:59:19.000000 pointclass-0.3/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 10:59:33.005889 pointclass-0.3/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-04-25 10:59:32.000000 pointclass-0.3/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-04-25 10:59:32.000000 pointclass-0.3/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 10:59:32.000000 pointclass-0.3/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 10:59:32.000000 pointclass-0.3/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 10:59:33.008828 pointclass-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-04-25 10:59:26.000000 pointclass-0.3/setup1.py
```

### Comparing `pointclass-0.2/pointclass/__init__.py` & `pointclass-0.3/pointclass/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 class point:
     def __init__(self,x=0,y=0):
         self.x=x
         self.y=y
     def show(self):
         return self.x
         return self.y
```

