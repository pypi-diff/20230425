# Comparing `tmp/quickmacapp-2023.3.3.tar.gz` & `tmp/quickmacapp-2023.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickmacapp-2023.3.3.tar", last modified: Fri Mar  3 23:05:43 2023, max compression
+gzip compressed data, was "quickmacapp-2023.4.24.tar", last modified: Tue Apr 25 04:17:31 2023, max compression
```

## Comparing `quickmacapp-2023.3.3.tar` & `quickmacapp-2023.4.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-03-03 23:05:43.588878 quickmacapp-2023.3.3/
--rw-r--r--   0 glyph      (501) staff       (20)     1091 2023-02-25 20:48:24.000000 quickmacapp-2023.3.3/LICENSE
--rw-r--r--   0 glyph      (501) staff       (20)     1116 2023-03-03 23:05:43.588772 quickmacapp-2023.3.3/PKG-INFO
--rw-r--r--   0 glyph      (501) staff       (20)      946 2023-03-03 22:58:15.000000 quickmacapp-2023.3.3/README.rst
--rw-r--r--   0 glyph      (501) staff       (20)      436 2023-03-03 22:52:37.000000 quickmacapp-2023.3.3/pyproject.toml
--rw-r--r--   0 glyph      (501) staff       (20)       38 2023-03-03 23:05:43.588908 quickmacapp-2023.3.3/setup.cfg
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-03-03 23:05:43.587339 quickmacapp-2023.3.3/src/
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-03-03 23:05:43.588126 quickmacapp-2023.3.3/src/quickmacapp/
--rw-r--r--   0 glyph      (501) staff       (20)      239 2023-03-03 22:37:22.000000 quickmacapp-2023.3.3/src/quickmacapp/__init__.py
--rw-r--r--   0 glyph      (501) staff       (20)     2772 2023-03-03 22:47:00.000000 quickmacapp-2023.3.3/src/quickmacapp/_interactions.py
--rw-r--r--   0 glyph      (501) staff       (20)     7295 2023-02-21 18:03:27.000000 quickmacapp-2023.3.3/src/quickmacapp/_quickapp.py
--rw-r--r--   0 glyph      (501) staff       (20)        0 2023-02-17 22:57:07.000000 quickmacapp-2023.3.3/src/quickmacapp/py.typed
-drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-03-03 23:05:43.588638 quickmacapp-2023.3.3/src/quickmacapp.egg-info/
--rw-r--r--   0 glyph      (501) staff       (20)     1116 2023-03-03 23:05:43.000000 quickmacapp-2023.3.3/src/quickmacapp.egg-info/PKG-INFO
--rw-r--r--   0 glyph      (501) staff       (20)      342 2023-03-03 23:05:43.000000 quickmacapp-2023.3.3/src/quickmacapp.egg-info/SOURCES.txt
--rw-r--r--   0 glyph      (501) staff       (20)        1 2023-03-03 23:05:43.000000 quickmacapp-2023.3.3/src/quickmacapp.egg-info/dependency_links.txt
--rw-r--r--   0 glyph      (501) staff       (20)      121 2023-03-03 23:05:43.000000 quickmacapp-2023.3.3/src/quickmacapp.egg-info/requires.txt
--rw-r--r--   0 glyph      (501) staff       (20)       12 2023-03-03 23:05:43.000000 quickmacapp-2023.3.3/src/quickmacapp.egg-info/top_level.txt
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-25 04:17:31.791349 quickmacapp-2023.4.24/
+-rw-r--r--   0 glyph      (501) staff       (20)     1091 2023-02-25 20:48:24.000000 quickmacapp-2023.4.24/LICENSE
+-rw-r--r--   0 glyph      (501) staff       (20)     1117 2023-04-25 04:17:31.791246 quickmacapp-2023.4.24/PKG-INFO
+-rw-r--r--   0 glyph      (501) staff       (20)      946 2023-03-03 22:58:15.000000 quickmacapp-2023.4.24/README.rst
+-rw-r--r--   0 glyph      (501) staff       (20)      436 2023-04-25 04:15:57.000000 quickmacapp-2023.4.24/pyproject.toml
+-rw-r--r--   0 glyph      (501) staff       (20)       38 2023-04-25 04:17:31.791379 quickmacapp-2023.4.24/setup.cfg
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-25 04:17:31.789788 quickmacapp-2023.4.24/src/
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-25 04:17:31.790594 quickmacapp-2023.4.24/src/quickmacapp/
+-rw-r--r--   0 glyph      (501) staff       (20)      239 2023-03-03 22:37:22.000000 quickmacapp-2023.4.24/src/quickmacapp/__init__.py
+-rw-r--r--   0 glyph      (501) staff       (20)     2772 2023-03-03 22:47:00.000000 quickmacapp-2023.4.24/src/quickmacapp/_interactions.py
+-rw-r--r--   0 glyph      (501) staff       (20)     7302 2023-04-25 04:14:08.000000 quickmacapp-2023.4.24/src/quickmacapp/_quickapp.py
+-rw-r--r--   0 glyph      (501) staff       (20)        0 2023-02-17 22:57:07.000000 quickmacapp-2023.4.24/src/quickmacapp/py.typed
+drwxr-xr-x   0 glyph      (501) staff       (20)        0 2023-04-25 04:17:31.791108 quickmacapp-2023.4.24/src/quickmacapp.egg-info/
+-rw-r--r--   0 glyph      (501) staff       (20)     1117 2023-04-25 04:17:31.000000 quickmacapp-2023.4.24/src/quickmacapp.egg-info/PKG-INFO
+-rw-r--r--   0 glyph      (501) staff       (20)      342 2023-04-25 04:17:31.000000 quickmacapp-2023.4.24/src/quickmacapp.egg-info/SOURCES.txt
+-rw-r--r--   0 glyph      (501) staff       (20)        1 2023-04-25 04:17:31.000000 quickmacapp-2023.4.24/src/quickmacapp.egg-info/dependency_links.txt
+-rw-r--r--   0 glyph      (501) staff       (20)      121 2023-04-25 04:17:31.000000 quickmacapp-2023.4.24/src/quickmacapp.egg-info/requires.txt
+-rw-r--r--   0 glyph      (501) staff       (20)       12 2023-04-25 04:17:31.000000 quickmacapp-2023.4.24/src/quickmacapp.egg-info/top_level.txt
```

### Comparing `quickmacapp-2023.3.3/LICENSE` & `quickmacapp-2023.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmacapp-2023.3.3/PKG-INFO` & `quickmacapp-2023.4.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickmacapp
-Version: 2023.3.3
+Version: 2023.4.24
 Summary: Make it easier to write Mac apps in Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 QuickMacApp
 ==============================
```

### Comparing `quickmacapp-2023.3.3/README.rst` & `quickmacapp-2023.4.24/README.rst`

 * *Files identical despite different names*

### Comparing `quickmacapp-2023.3.3/src/quickmacapp/_interactions.py` & `quickmacapp-2023.4.24/src/quickmacapp/_interactions.py`

 * *Files identical despite different names*

### Comparing `quickmacapp-2023.3.3/src/quickmacapp/_quickapp.py` & `quickmacapp-2023.4.24/src/quickmacapp/_quickapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import os
 import sys
 import traceback
 from typing import Callable, Protocol, Any
 
-from objc import ivar, IBAction
+from objc import ivar, IBAction, super
 
 from Foundation import (
     NSObject,
     NSException,
 )
 
 from AppKit import (
```

### Comparing `quickmacapp-2023.3.3/src/quickmacapp.egg-info/PKG-INFO` & `quickmacapp-2023.4.24/src/quickmacapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickmacapp
-Version: 2023.3.3
+Version: 2023.4.24
 Summary: Make it easier to write Mac apps in Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 QuickMacApp
 ==============================
```

