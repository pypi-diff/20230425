# Comparing `tmp/payu_websdk-0.1.3.tar.gz` & `tmp/payu_websdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payu_websdk-0.1.3.tar", last modified: Tue Apr 25 09:19:59 2023, max compression
+gzip compressed data, was "payu_websdk-0.1.4.tar", last modified: Tue Apr 25 09:26:42 2023, max compression
```

## Comparing `payu_websdk-0.1.3.tar` & `payu_websdk-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 09:19:59.027936 payu_websdk-0.1.3/
--rw-rw-rw-   0        0        0     1063 2023-04-25 08:14:25.000000 payu_websdk-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1728 2023-04-25 09:19:59.027123 payu_websdk-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2023-04-25 08:22:30.000000 payu_websdk-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 09:19:59.019011 payu_websdk-0.1.3/payu_websdk.egg-info/
--rw-rw-rw-   0        0        0     1728 2023-04-25 09:19:58.000000 payu_websdk-0.1.3/payu_websdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-25 09:19:58.000000 payu_websdk-0.1.3/payu_websdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 09:19:58.000000 payu_websdk-0.1.3/payu_websdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 09:19:58.000000 payu_websdk-0.1.3/payu_websdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 09:19:58.000000 payu_websdk-0.1.3/payu_websdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 09:19:59.022907 payu_websdk-0.1.3/resources/
--rw-rw-rw-   0        0        0     2642 2023-04-25 07:07:22.000000 payu_websdk-0.1.3/resources/hasher.py
--rw-rw-rw-   0        0        0       42 2023-04-25 09:19:59.028903 payu_websdk-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-04-25 09:18:19.000000 payu_websdk-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:26:42.801188 payu_websdk-0.1.4/
+-rw-rw-rw-   0        0        0     1063 2023-04-25 08:14:25.000000 payu_websdk-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1728 2023-04-25 09:26:42.799166 payu_websdk-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-04-25 08:22:30.000000 payu_websdk-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 09:26:42.775300 payu_websdk-0.1.4/payu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 09:11:40.000000 payu_websdk-0.1.4/payu/__init__.py
+-rw-rw-rw-   0        0        0     2849 2023-04-25 05:21:08.000000 payu_websdk-0.1.4/payu/payuClient.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:26:42.795157 payu_websdk-0.1.4/payu_websdk.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-04-25 09:26:42.000000 payu_websdk-0.1.4/payu_websdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-25 09:26:42.000000 payu_websdk-0.1.4/payu_websdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 09:26:42.000000 payu_websdk-0.1.4/payu_websdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 09:26:42.000000 payu_websdk-0.1.4/payu_websdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 09:26:42.000000 payu_websdk-0.1.4/payu_websdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 09:26:42.802140 payu_websdk-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-04-25 09:26:35.000000 payu_websdk-0.1.4/setup.py
```

### Comparing `payu_websdk-0.1.3/LICENSE` & `payu_websdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `payu_websdk-0.1.3/PKG-INFO` & `payu_websdk-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payu_websdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: PayU
 Home-page: https://github.com/payu-india/web-sdk-python
 Author: PayU Web SDK for Python
 Author-email: integration@payu.in
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `payu_websdk-0.1.3/README.md` & `payu_websdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `payu_websdk-0.1.3/payu_websdk.egg-info/PKG-INFO` & `payu_websdk-0.1.4/payu_websdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payu-websdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: PayU
 Home-page: https://github.com/payu-india/web-sdk-python
 Author: PayU Web SDK for Python
 Author-email: integration@payu.in
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `payu_websdk-0.1.3/setup.py` & `payu_websdk-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     readme_content = readme.read()
 
 setup(
     name='payu_websdk',
-    version='0.1.3',
+    version='0.1.4',
     description='PayU',
     author='PayU Web SDK for Python',
     author_email='integration@payu.in',
     url='https://github.com/payu-india/web-sdk-python',
     packages=find_packages(),
     long_description=readme_content,
     long_description_content_type='text/markdown',
```

