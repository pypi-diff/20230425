# Comparing `tmp/swiftshadow-0.1.0.tar.gz` & `tmp/swiftshadow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.1.0.tar", last modified: Tue Apr 25 07:08:06 2023, max compression
+gzip compressed data, was "swiftshadow-0.1.1.tar", last modified: Tue Apr 25 10:43:40 2023, max compression
```

## Comparing `swiftshadow-0.1.0.tar` & `swiftshadow-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-25 07:07:53.000000 swiftshadow-0.1.0/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:08:06.281445 swiftshadow-0.1.0/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 07:08:06.000000 swiftshadow-0.1.0/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.1.0/LICENSE` & `swiftshadow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.0/PKG-INFO` & `swiftshadow-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.1.0
+Version: 0.1.1
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,15 @@
 ```
 
 ## One class rules all
 Everything in swiftshadow is under one class for ease of use and minimal code.
 
 Get a proxy using just 3 lines of code!
 ``` py
-from swiftshadow import Proxy
+from swiftshadow.swiftshadow import Proxy
 
 swift = Proxy()
 print(swift.proxy())
 ```
 That was easy. 
 
 Head to [Documentation](https://sachin-sankar.github.io/swiftshadow/) to get started.
```

### Comparing `swiftshadow-0.1.0/README.md` & `swiftshadow-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 
 ## One class rules all
 Everything in swiftshadow is under one class for ease of use and minimal code.
 
 Get a proxy using just 3 lines of code!
 ``` py
-from swiftshadow import Proxy
+from swiftshadow.swiftshadow import Proxy
 
 swift = Proxy()
 print(swift.proxy())
 ```
 That was easy. 
 
 Head to [Documentation](https://sachin-sankar.github.io/swiftshadow/) to get started.
```

### Comparing `swiftshadow-0.1.0/setup.py` & `swiftshadow-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
     url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=VERSION.get("__version__", "0.1.0"),
+    version=VERSION.get("__version__", "0.1.1"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.1.0/swiftshadow/classes.py` & `swiftshadow-0.1.1/swiftshadow/classes.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.0/swiftshadow/constants.py` & `swiftshadow-0.1.1/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.0/swiftshadow/helpers.py` & `swiftshadow-0.1.1/swiftshadow/helpers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.0/swiftshadow/providers.py` & `swiftshadow-0.1.1/swiftshadow/providers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.0/swiftshadow/swiftshadow.py` & `swiftshadow-0.1.1/swiftshadow/swiftshadow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from requests import get
 from random import choice
 from datetime import datetime, timezone, timedelta
 from pickle import dump, load
-from helpers import log
-from providers import Proxyscrape, Scrapingant
+from swiftshadow.helpers import log
+from swiftshadow.providers import Proxyscrape, Scrapingant
 
 
 class Proxy:
     def __init__(
         self,
         countries: list = [],
         protocol: str = "http",
@@ -28,15 +28,15 @@
                 cachePeriod: Time to cache proxies in minutes.
 
         Returns:
                 proxyClass (swiftshadow.Proxy): `swiftshadow.Proxy` class instance
 
         Examples:
                 Simplest way to get a proxy
-                >>> from swiftshadow import Proxy
+                >>> from swiftshadow.swiftshadow import Proxy
                 >>> swift = Proxy()
                 >>> print(swift.proxy())
                 {'http':'192.0.0.1:8080'}
         Note:
                 Proxies are sourced from **Proxyscrape** and **Scrapingant** websites which are freely available and validated locally.
         """
         self.countries = [i.upper() for i in countries]
```

### Comparing `swiftshadow-0.1.0/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-0.1.1/swiftshadow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.1.0
+Version: 0.1.1
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,15 @@
 ```
 
 ## One class rules all
 Everything in swiftshadow is under one class for ease of use and minimal code.
 
 Get a proxy using just 3 lines of code!
 ``` py
-from swiftshadow import Proxy
+from swiftshadow.swiftshadow import Proxy
 
 swift = Proxy()
 print(swift.proxy())
 ```
 That was easy. 
 
 Head to [Documentation](https://sachin-sankar.github.io/swiftshadow/) to get started.
```

