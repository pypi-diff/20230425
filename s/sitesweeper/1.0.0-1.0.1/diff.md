# Comparing `tmp/sitesweeper-1.0.0.tar.gz` & `tmp/sitesweeper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesweeper-1.0.0.tar", last modified: Tue Apr 25 08:31:47 2023, max compression
+gzip compressed data, was "sitesweeper-1.0.1.tar", last modified: Tue Apr 25 08:42:08 2023, max compression
```

## Comparing `sitesweeper-1.0.0.tar` & `sitesweeper-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:31:47.498427 sitesweeper-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 08:31:47.498427 sitesweeper-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 08:31:33.000000 sitesweeper-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:31:47.502427 sitesweeper-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 08:31:33.000000 sitesweeper-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:31:47.498427 sitesweeper-1.0.0/sitesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:31:33.000000 sitesweeper-1.0.0/sitesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-25 08:31:33.000000 sitesweeper-1.0.0/sitesweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-25 08:31:33.000000 sitesweeper-1.0.0/sitesweeper/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:31:47.498427 sitesweeper-1.0.0/sitesweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 08:31:47.000000 sitesweeper-1.0.0/sitesweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:31:47.000000 sitesweeper-1.0.0/sitesweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:31:47.000000 sitesweeper-1.0.0/sitesweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:31:47.000000 sitesweeper-1.0.0/sitesweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:31:47.000000 sitesweeper-1.0.0/sitesweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:42:08.941511 sitesweeper-1.0.1/sitesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/sitesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/sitesweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-25 08:41:55.000000 sitesweeper-1.0.1/sitesweeper/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:42:08.945511 sitesweeper-1.0.1/sitesweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:42:08.000000 sitesweeper-1.0.1/sitesweeper.egg-info/top_level.txt
```

### Comparing `sitesweeper-1.0.0/PKG-INFO` & `sitesweeper-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesweeper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sitesweeper is a python package to help you automate your web scraping process, outputing pages to a file
 Home-page: https://github.com/radityaharya/sitesweeper
 Author: Raditya Harya
 Author-email: contact@radityaharya.com
 Description-Content-Type: text/markdown
```

### Comparing `sitesweeper-1.0.0/setup.py` & `sitesweeper-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         long_description = fh.read()
 else:
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 setup(
     name="sitesweeper",
-    version="1.0.0",
+    version="1.0.1",
     description="Sitesweeper is a python package to help you automate your web scraping process, outputing pages to a file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Raditya Harya",
     author_email="contact@radityaharya.com",
     url="https://github.com/radityaharya/sitesweeper",
     packages=find_packages(),
```

### Comparing `sitesweeper-1.0.0/sitesweeper/__main__.py` & `sitesweeper-1.0.1/sitesweeper/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import argparse
 import datetime
 import logging
 import os
 import sys
-import requests
-from rich.console import Console
-from rich.live import Live
 from rich.logging import RichHandler
-from rich.progress import BarColumn, Progress, TaskID, TextColumn
-from rich.table import Column
-from requests.adapters import HTTPAdapter
 
-from crawler import Crawler
+from .crawler import Crawler
 
 logger = logging.getLogger("website-crawler-to-pdf")
 logger.setLevel(logging.DEBUG)
 logger.addHandler(RichHandler())
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
```

### Comparing `sitesweeper-1.0.0/sitesweeper/crawler.py` & `sitesweeper-1.0.1/sitesweeper/crawler.py`

 * *Files identical despite different names*

### Comparing `sitesweeper-1.0.0/sitesweeper.egg-info/PKG-INFO` & `sitesweeper-1.0.1/sitesweeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesweeper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sitesweeper is a python package to help you automate your web scraping process, outputing pages to a file
 Home-page: https://github.com/radityaharya/sitesweeper
 Author: Raditya Harya
 Author-email: contact@radityaharya.com
 Description-Content-Type: text/markdown
```

