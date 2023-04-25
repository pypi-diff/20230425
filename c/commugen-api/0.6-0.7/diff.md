# Comparing `tmp/commugen_api-0.6.tar.gz` & `tmp/commugen_api-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commugen_api-0.6.tar", last modified: Tue Apr 11 08:45:10 2023, max compression
+gzip compressed data, was "commugen_api-0.7.tar", last modified: Tue Apr 25 08:26:40 2023, max compression
```

## Comparing `commugen_api-0.6.tar` & `commugen_api-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:45:10.353068 commugen_api-0.6/
--rw-rw-rw-   0        0        0      516 2023-04-11 08:45:10.353068 commugen_api-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      191 2022-10-18 06:07:28.000000 commugen_api-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 08:45:10.325873 commugen_api-0.6/commugen_api/
--rw-rw-rw-   0        0        0       39 2022-10-11 09:14:21.000000 commugen_api-0.6/commugen_api/__init__.py
--rw-rw-rw-   0        0        0     8728 2023-04-11 08:43:06.000000 commugen_api-0.6/commugen_api/commugen_api.py
--rw-rw-rw-   0        0        0     7522 2022-10-27 12:56:36.000000 commugen_api-0.6/commugen_api/response_objects.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:45:10.351423 commugen_api-0.6/commugen_api.egg-info/
--rw-rw-rw-   0        0        0      516 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 08:45:10.000000 commugen_api-0.6/commugen_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 08:45:10.353068 commugen_api-0.6/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-04-11 08:43:06.000000 commugen_api-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:26:40.403801 commugen_api-0.7/
+-rw-rw-rw-   0        0        0      598 2023-04-25 08:26:40.403801 commugen_api-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-13 09:32:27.000000 commugen_api-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 08:26:40.388058 commugen_api-0.7/commugen_api/
+-rw-rw-rw-   0        0        0       39 2022-10-11 09:14:21.000000 commugen_api-0.7/commugen_api/__init__.py
+-rw-rw-rw-   0        0        0     8726 2023-04-25 08:21:38.000000 commugen_api-0.7/commugen_api/commugen_api.py
+-rw-rw-rw-   0        0        0     7522 2022-10-27 12:56:36.000000 commugen_api-0.7/commugen_api/response_objects.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:26:40.403801 commugen_api-0.7/commugen_api.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-04-25 08:26:40.000000 commugen_api-0.7/commugen_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-25 08:26:40.000000 commugen_api-0.7/commugen_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:26:40.000000 commugen_api-0.7/commugen_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-25 08:26:40.000000 commugen_api-0.7/commugen_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 08:26:40.000000 commugen_api-0.7/commugen_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:26:40.403801 commugen_api-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-04-25 08:23:47.000000 commugen_api-0.7/setup.py
```

### Comparing `commugen_api-0.6/PKG-INFO` & `commugen_api-0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commugen_api
-Version: 0.6
+Version: 0.7
 Summary: Python wrapper for commugen api
 Home-page: https://bitbucket.org/kobi_commugen/commugen_api/
 Author: kobi kolodner
 Author-email: kobi@commugen.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
@@ -13,8 +13,8 @@
 ============
 
 This is a simple python wrapper for commugen api
 
 API documentation
 -----------------
 the oficial api documentation can be found here:
-[api documentation]()
+[api documentation](https://drive.google.com/file/d/1NTgP7V_3DfyaFxFOhXWmN7vmvnmvqHf4/view?ts=640f20ca)
```

### Comparing `commugen_api-0.6/commugen_api/commugen_api.py` & `commugen_api-0.7/commugen_api/commugen_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 
 import requests
 from curlify import to_curl
 from keyring import get_password, set_password
-from stdiomask import getpass
+from getpass import getpass
 
 from commugen_api.response_objects import CommugenModel, CommugenDomains, CommugenTables, CommugenSingleRecord, \
     CommugenOptions
 
 MAX_COUNT = 100
```

### Comparing `commugen_api-0.6/commugen_api/response_objects.py` & `commugen_api-0.7/commugen_api/response_objects.py`

 * *Files identical despite different names*

### Comparing `commugen_api-0.6/commugen_api.egg-info/PKG-INFO` & `commugen_api-0.7/commugen_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commugen-api
-Version: 0.6
+Version: 0.7
 Summary: Python wrapper for commugen api
 Home-page: https://bitbucket.org/kobi_commugen/commugen_api/
 Author: kobi kolodner
 Author-email: kobi@commugen.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
@@ -13,8 +13,8 @@
 ============
 
 This is a simple python wrapper for commugen api
 
 API documentation
 -----------------
 the oficial api documentation can be found here:
-[api documentation]()
+[api documentation](https://drive.google.com/file/d/1NTgP7V_3DfyaFxFOhXWmN7vmvnmvqHf4/view?ts=640f20ca)
```

### Comparing `commugen_api-0.6/setup.py` & `commugen_api-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from setuptools import setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(name='commugen_api',
-      version='0.6',
+      version='0.7',
       description='Python wrapper for commugen api',
       url='https://bitbucket.org/kobi_commugen/commugen_api/',
       author='kobi kolodner',
       author_email='kobi@commugen.com',
       license='MIT',
       packages=['commugen_api'],
       install_requires=[
             'requests',
             'tablib',
             'curlify',
             'keyring',
-            'stdiomask'
       ],
       classifiers=[
             'Development Status :: 2 - Pre-Alpha'
       ],
       long_description=long_description,  # Optional
       long_description_content_type="text/markdown",  # Optional (see note above)
```

