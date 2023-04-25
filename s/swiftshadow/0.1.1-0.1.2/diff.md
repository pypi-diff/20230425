# Comparing `tmp/swiftshadow-0.1.1.tar.gz` & `tmp/swiftshadow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.1.1.tar", last modified: Tue Apr 25 10:43:40 2023, max compression
+gzip compressed data, was "swiftshadow-0.1.2.tar", last modified: Tue Apr 25 10:50:21 2023, max compression
```

## Comparing `swiftshadow-0.1.1.tar` & `swiftshadow-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-25 10:43:29.000000 swiftshadow-0.1.1/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:43:40.466202 swiftshadow-0.1.1/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:43:40.000000 swiftshadow-0.1.1/swiftshadow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/swiftshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-25 10:50:07.000000 swiftshadow-0.1.2/swiftshadow/swiftshadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:50:21.380784 swiftshadow-0.1.2/swiftshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:50:21.000000 swiftshadow-0.1.2/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.1.1/LICENSE` & `swiftshadow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.1/PKG-INFO` & `swiftshadow-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.1.1
+Version: 0.1.2
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `swiftshadow-0.1.1/README.md` & `swiftshadow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.1/setup.py` & `swiftshadow-0.1.2/setup.py`

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
-    version=VERSION.get("__version__", "0.1.1"),
+    version=VERSION.get("__version__", "0.1.2"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.1.1/swiftshadow/classes.py` & `swiftshadow-0.1.2/swiftshadow/classes.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.1/swiftshadow/constants.py` & `swiftshadow-0.1.2/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.1/swiftshadow/helpers.py` & `swiftshadow-0.1.2/swiftshadow/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from constants import CountryCodes
+from swiftshadow.constants import CountryCodes
 from requests import get
 
 
 def getCountryCode(countryName):
     try:
         return CountryCodes[countryName]
     except KeyError:
```

### Comparing `swiftshadow-0.1.1/swiftshadow/providers.py` & `swiftshadow-0.1.2/swiftshadow/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from requests import get
-from helpers import getCountryCode, checkProxy, log
+from swiftshadow.helpers import getCountryCode, checkProxy, log
 
 
 def Scrapingant(max, countries=[], protocol="http"):
     result = []
     count = 0
     raw = get("https://scrapingant.com/proxies").text
     log("info", "Updating proxies from ScrapingAnt")
```

### Comparing `swiftshadow-0.1.1/swiftshadow/swiftshadow.py` & `swiftshadow-0.1.2/swiftshadow/swiftshadow.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.1.1/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-0.1.2/swiftshadow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.1.1
+Version: 0.1.2
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

