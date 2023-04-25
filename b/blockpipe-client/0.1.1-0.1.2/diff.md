# Comparing `tmp/blockpipe-client-0.1.1.tar.gz` & `tmp/blockpipe-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe-client-0.1.1.tar", last modified: Tue Apr 25 11:14:33 2023, max compression
+gzip compressed data, was "blockpipe-client-0.1.2.tar", last modified: Tue Apr 25 11:20:50 2023, max compression
```

## Comparing `blockpipe-client-0.1.1.tar` & `blockpipe-client-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-25 11:14:33.498366 blockpipe-client-0.1.1/
--rw-r--r--   0 paul       (501) staff       (20)    10936 2023-04-25 10:23:33.000000 blockpipe-client-0.1.1/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)     2393 2023-04-25 11:14:33.498213 blockpipe-client-0.1.1/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     1688 2023-04-25 11:14:24.000000 blockpipe-client-0.1.1/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-25 11:14:33.497962 blockpipe-client-0.1.1/blockpipe_client.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     2393 2023-04-25 11:14:33.000000 blockpipe-client-0.1.1/blockpipe_client.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      225 2023-04-25 11:14:33.000000 blockpipe-client-0.1.1/blockpipe_client.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-04-25 11:14:33.000000 blockpipe-client-0.1.1/blockpipe_client.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        9 2023-04-25 11:14:33.000000 blockpipe-client-0.1.1/blockpipe_client.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-04-25 11:14:33.000000 blockpipe-client-0.1.1/blockpipe_client.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-04-25 11:14:33.498409 blockpipe-client-0.1.1/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)      937 2023-04-25 11:13:13.000000 blockpipe-client-0.1.1/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-25 11:20:50.390137 blockpipe-client-0.1.2/
+-rw-r--r--   0 paul       (501) staff       (20)    10936 2023-04-25 10:23:33.000000 blockpipe-client-0.1.2/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)     2393 2023-04-25 11:20:50.390029 blockpipe-client-0.1.2/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1688 2023-04-25 11:14:24.000000 blockpipe-client-0.1.2/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-04-25 11:20:50.389883 blockpipe-client-0.1.2/blockpipe_client.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     2393 2023-04-25 11:20:50.000000 blockpipe-client-0.1.2/blockpipe_client.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      225 2023-04-25 11:20:50.000000 blockpipe-client-0.1.2/blockpipe_client.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-04-25 11:20:50.000000 blockpipe-client-0.1.2/blockpipe_client.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        9 2023-04-25 11:20:50.000000 blockpipe-client-0.1.2/blockpipe_client.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-04-25 11:20:50.000000 blockpipe-client-0.1.2/blockpipe_client.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-04-25 11:20:50.390170 blockpipe-client-0.1.2/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)      937 2023-04-25 11:20:47.000000 blockpipe-client-0.1.2/setup.py
```

### Comparing `blockpipe-client-0.1.1/LICENSE` & `blockpipe-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blockpipe-client-0.1.1/PKG-INFO` & `blockpipe-client-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for interacting with Blockpipe Endpoint API
 Home-page: https://github.com/blockpipe/python
 Author: blockpipe.io
 Author-email: support@blockpipe.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `blockpipe-client-0.1.1/README.md` & `blockpipe-client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blockpipe-client-0.1.1/blockpipe_client.egg-info/PKG-INFO` & `blockpipe-client-0.1.2/blockpipe_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for interacting with Blockpipe Endpoint API
 Home-page: https://github.com/blockpipe/python
 Author: blockpipe.io
 Author-email: support@blockpipe.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `blockpipe-client-0.1.1/setup.py` & `blockpipe-client-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="blockpipe-client",
-    version="0.1.1",
+    version="0.1.2",
     author="blockpipe.io",
     author_email="support@blockpipe.io",
     description="A Python library for interacting with Blockpipe Endpoint API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blockpipe/python",
     packages=find_packages(),
```

