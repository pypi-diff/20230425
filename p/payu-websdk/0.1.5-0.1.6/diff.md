# Comparing `tmp/payu_websdk-0.1.5.tar.gz` & `tmp/payu_websdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payu_websdk-0.1.5.tar", last modified: Tue Apr 25 09:45:56 2023, max compression
+gzip compressed data, was "payu_websdk-0.1.6.tar", last modified: Tue Apr 25 09:47:50 2023, max compression
```

## Comparing `payu_websdk-0.1.5.tar` & `payu_websdk-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 09:45:56.590032 payu_websdk-0.1.5/
--rw-rw-rw-   0        0        0     1063 2023-04-25 08:14:25.000000 payu_websdk-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1728 2023-04-25 09:45:56.588934 payu_websdk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2023-04-25 08:22:30.000000 payu_websdk-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 09:45:56.565922 payu_websdk-0.1.5/payu/
--rw-rw-rw-   0        0        0       60 2023-04-25 09:44:17.000000 payu_websdk-0.1.5/payu/__init__.py
--rw-rw-rw-   0        0        0     2845 2023-04-25 09:38:10.000000 payu_websdk-0.1.5/payu/payuClient.py
-drwxrwxrwx   0        0        0        0 2023-04-25 09:45:56.584871 payu_websdk-0.1.5/payu_websdk.egg-info/
--rw-rw-rw-   0        0        0     1728 2023-04-25 09:45:56.000000 payu_websdk-0.1.5/payu_websdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-25 09:45:56.000000 payu_websdk-0.1.5/payu_websdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 09:45:56.000000 payu_websdk-0.1.5/payu_websdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 09:45:56.000000 payu_websdk-0.1.5/payu_websdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 09:45:56.000000 payu_websdk-0.1.5/payu_websdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 09:45:56.590924 payu_websdk-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-04-25 09:45:37.000000 payu_websdk-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:47:50.065641 payu_websdk-0.1.6/
+-rw-rw-rw-   0        0        0     1063 2023-04-25 08:14:25.000000 payu_websdk-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1728 2023-04-25 09:47:50.063643 payu_websdk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-04-25 08:22:30.000000 payu_websdk-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 09:47:50.038180 payu_websdk-0.1.6/payu/
+-rw-rw-rw-   0        0        0       30 2023-04-25 09:47:28.000000 payu_websdk-0.1.6/payu/__init__.py
+-rw-rw-rw-   0        0        0     2845 2023-04-25 09:38:10.000000 payu_websdk-0.1.6/payu/payuClient.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:47:50.058654 payu_websdk-0.1.6/payu_websdk.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-04-25 09:47:49.000000 payu_websdk-0.1.6/payu_websdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-25 09:47:49.000000 payu_websdk-0.1.6/payu_websdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 09:47:49.000000 payu_websdk-0.1.6/payu_websdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 09:47:49.000000 payu_websdk-0.1.6/payu_websdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 09:47:49.000000 payu_websdk-0.1.6/payu_websdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 09:47:50.066646 payu_websdk-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-04-25 09:47:37.000000 payu_websdk-0.1.6/setup.py
```

### Comparing `payu_websdk-0.1.5/LICENSE` & `payu_websdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `payu_websdk-0.1.5/PKG-INFO` & `payu_websdk-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payu_websdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: PayU
 Home-page: https://github.com/payu-india/web-sdk-python
 Author: PayU Web SDK for Python
 Author-email: integration@payu.in
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `payu_websdk-0.1.5/README.md` & `payu_websdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `payu_websdk-0.1.5/payu/payuClient.py` & `payu_websdk-0.1.6/payu/payuClient.py`

 * *Files identical despite different names*

### Comparing `payu_websdk-0.1.5/payu_websdk.egg-info/PKG-INFO` & `payu_websdk-0.1.6/payu_websdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payu-websdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: PayU
 Home-page: https://github.com/payu-india/web-sdk-python
 Author: PayU Web SDK for Python
 Author-email: integration@payu.in
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `payu_websdk-0.1.5/setup.py` & `payu_websdk-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     readme_content = readme.read()
 
 setup(
     name='payu_websdk',
-    version='0.1.5',
+    version='0.1.6',
     description='PayU',
     author='PayU Web SDK for Python',
     author_email='integration@payu.in',
     url='https://github.com/payu-india/web-sdk-python',
     packages=find_packages(),
     package_dir={'payu_websdk':'payu'},
     long_description=readme_content,
```

