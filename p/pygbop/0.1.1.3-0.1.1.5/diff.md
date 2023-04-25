# Comparing `tmp/pygbop-0.1.1.3.tar.gz` & `tmp/pygbop-0.1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pygbop-0.1.1.3.tar", last modified: Wed Feb 15 06:20:36 2023, max compression
+gzip compressed data, was "dist\pygbop-0.1.1.5.tar", last modified: Tue Apr 25 09:46:41 2023, max compression
```

## Comparing `pygbop-0.1.1.3.tar` & `pygbop-0.1.1.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/
--rw-rw-rw-   0        0        0        2 2022-07-08 11:04:28.000000 pygbop-0.1.1.3/a.txt
--rw-rw-rw-   0        0        0      544 2022-07-08 06:25:59.000000 pygbop-0.1.1.3/main.py
--rw-rw-rw-   0        0        0      166 2022-07-08 07:20:39.000000 pygbop-0.1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1027 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop/
--rw-rw-rw-   0        0        0     3696 2023-02-15 06:09:05.000000 pygbop-0.1.1.3/pygbop/gbop.py
--rw-rw-rw-   0        0        0      359 2022-07-08 10:32:24.000000 pygbop-0.1.1.3/pygbop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop.egg-info/
--rw-rw-rw-   0        0        0        1 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1027 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop.egg-info/requires.txt
--rw-rw-rw-   0        0        0      266 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/pygbop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-02-15 06:20:25.000000 pygbop-0.1.1.3/README.rst
--rw-rw-rw-   0        0        0      801 2022-10-17 05:43:54.000000 pygbop-0.1.1.3/README.txt
--rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.1.1.3/requirements.txt
--rw-rw-rw-   0        0        0       64 2023-02-15 06:20:36.000000 pygbop-0.1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-02-15 06:09:16.000000 pygbop-0.1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/
+-rw-rw-rw-   0        0        0       40 2023-02-15 06:22:38.000000 pygbop-0.1.1.5/.gitignore
+-rw-rw-rw-   0        0        0        2 2022-07-08 11:04:28.000000 pygbop-0.1.1.5/a.txt
+-rw-rw-rw-   0        0        0      544 2022-07-08 06:25:59.000000 pygbop-0.1.1.5/main.py
+-rw-rw-rw-   0        0        0      166 2022-07-08 07:20:39.000000 pygbop-0.1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1108 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/pygbop/
+-rw-rw-rw-   0        0        0     3814 2023-04-25 09:46:16.000000 pygbop-0.1.1.5/pygbop/gbop.py
+-rw-rw-rw-   0        0        0      359 2022-07-08 10:32:24.000000 pygbop-0.1.1.5/pygbop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/pygbop.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1108 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      277 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 09:46:40.000000 pygbop-0.1.1.5/pygbop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-02-15 06:20:25.000000 pygbop-0.1.1.5/README.rst
+-rw-rw-rw-   0        0        0      801 2022-10-17 05:43:54.000000 pygbop-0.1.1.5/README.txt
+-rw-rw-rw-   0        0        0       16 2022-07-08 06:38:50.000000 pygbop-0.1.1.5/requirements.txt
+-rw-rw-rw-   0        0        0       64 2023-04-25 09:46:41.000000 pygbop-0.1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-04-25 09:43:09.000000 pygbop-0.1.1.5/setup.py
```

### Comparing `pygbop-0.1.1.3/main.py` & `pygbop-0.1.1.5/main.py`

 * *Files identical despite different names*

### Comparing `pygbop-0.1.1.3/PKG-INFO` & `pygbop-0.1.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: pygbop
-Version: 0.1.1.3
+Version: 0.1.1.5
 Summary: Geely GBOP Client
 Home-page: https://pypi.python.org/pypi/GbopApiClient
 Author: huang.xiaogang
 Author-email: huang.xiaogang@geely.com
 License: MIT
+Description: 常见问题
+        =========
+        
+        
+        Installation / 安装
+        --------------------------
+        
+        ::
+        
+            pip install pygbop
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
@@ -17,19 +27,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-
-常见问题
-=========
-
-
-Installation / 安装
---------------------------
-
-::
-
-    pip install pygbop
-
```

### Comparing `pygbop-0.1.1.3/pygbop/gbop.py` & `pygbop-0.1.1.5/pygbop/gbop.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,12 +88,15 @@
 
     def _get_url_str(self, path, params):
         query_str = self._get_query_str(params)
         format_string = f"{self.base_url}{path}?{query_str}" if query_str else f"{self.base_url}{path}"
         url = self.protocol + format_string
         return url
 
-    def execute(self, method=Method.GET, path='', params={}, data={}, is_beta_api=False):
+    def execute(self, method=Method.GET, path='', params={}, data={}, is_beta_api=False, is_have_status=False):
         url = self._get_url_str(path, params)
         headers = self._get_header(path, method.value, params, is_beta_api)
         res = requests.request(method.value, url, headers=headers, data=data)
-        return res.content
+        if is_have_status:
+            return res.status_code, res.content
+        else:
+            return res.content
```

### Comparing `pygbop-0.1.1.3/pygbop.egg-info/PKG-INFO` & `pygbop-0.1.1.5/pygbop.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: pygbop
-Version: 0.1.1.3
+Version: 0.1.1.5
 Summary: Geely GBOP Client
 Home-page: https://pypi.python.org/pypi/GbopApiClient
 Author: huang.xiaogang
 Author-email: huang.xiaogang@geely.com
 License: MIT
+Description: 常见问题
+        =========
+        
+        
+        Installation / 安装
+        --------------------------
+        
+        ::
+        
+            pip install pygbop
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Internet
@@ -17,19 +27,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-
-常见问题
-=========
-
-
-Installation / 安装
---------------------------
-
-::
-
-    pip install pygbop
-
```

### Comparing `pygbop-0.1.1.3/README.txt` & `pygbop-0.1.1.5/README.txt`

 * *Files identical despite different names*

### Comparing `pygbop-0.1.1.3/setup.py` & `pygbop-0.1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from __future__ import print_function
 from setuptools import setup, find_packages
 # from setuptools import find_package_data
 import sys
 
 setup(
     name="pygbop",
-    version="0.1.1.3",
+    version="0.1.1.5",
     author="huang.xiaogang",
     author_email="huang.xiaogang@geely.com",
     description="Geely GBOP Client",
-    long_description=open("README.rst").read(),
+    long_description=open("README.rst", encoding='utf-8').read(),
     license="MIT",
     url="https://pypi.python.org/pypi/GbopApiClient",
     packages=find_packages(exclude=["*.*"]),
     include_package_data=True,
     py_modules=[],
     install_requires=[
         "requests",
```

