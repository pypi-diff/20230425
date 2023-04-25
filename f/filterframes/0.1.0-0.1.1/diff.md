# Comparing `tmp/filterframes-0.1.0.tar.gz` & `tmp/filterframes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filterframes-0.1.0.tar", last modified: Tue Apr 25 00:23:28 2023, max compression
+gzip compressed data, was "filterframes-0.1.1.tar", last modified: Tue Apr 25 00:38:59 2023, max compression
```

## Comparing `filterframes-0.1.0.tar` & `filterframes-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:23:28.192624 filterframes-0.1.0/
--rw-rw-rw-   0        0        0     2437 2023-04-25 00:23:28.192624 filterframes-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-04-24 23:05:38.000000 filterframes-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 00:23:28.166093 filterframes-0.1.0/filterframes/
--rw-rw-rw-   0        0        0       70 2023-04-25 00:22:58.000000 filterframes-0.1.0/filterframes/__init__.py
--rw-rw-rw-   0        0        0    10483 2023-04-25 00:04:18.000000 filterframes-0.1.0/filterframes/filterframes.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:23:28.189499 filterframes-0.1.0/filterframes.egg-info/
--rw-rw-rw-   0        0        0     2437 2023-04-25 00:23:28.000000 filterframes-0.1.0/filterframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-25 00:23:28.000000 filterframes-0.1.0/filterframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:23:28.000000 filterframes-0.1.0/filterframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 00:23:28.000000 filterframes-0.1.0/filterframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 00:23:28.000000 filterframes-0.1.0/filterframes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 00:23:28.193470 filterframes-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-04-25 00:21:33.000000 filterframes-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:23:28.190632 filterframes-0.1.0/test/
--rw-rw-rw-   0        0        0     2174 2023-04-25 00:05:20.000000 filterframes-0.1.0/test/test_filterframes.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.837158 filterframes-0.1.1/
+-rw-rw-rw-   0        0        0     2437 2023-04-25 00:38:59.836062 filterframes-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-04-24 23:05:38.000000 filterframes-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.815257 filterframes-0.1.1/filterframes/
+-rw-rw-rw-   0        0        0       70 2023-04-25 00:22:58.000000 filterframes-0.1.1/filterframes/__init__.py
+-rw-rw-rw-   0        0        0    10483 2023-04-25 00:04:18.000000 filterframes-0.1.1/filterframes/filterframes.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.834059 filterframes-0.1.1/filterframes.egg-info/
+-rw-rw-rw-   0        0        0     2437 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 00:38:59.000000 filterframes-0.1.1/filterframes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:38:59.837158 filterframes-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-04-25 00:38:00.000000 filterframes-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:38:59.835061 filterframes-0.1.1/test/
+-rw-rw-rw-   0        0        0     2174 2023-04-25 00:05:20.000000 filterframes-0.1.1/test/test_filterframes.py
```

### Comparing `filterframes-0.1.0/PKG-INFO` & `filterframes-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filterframes
-Version: 0.1.0
+Version: 0.1.1
 Summary: A very simple DTASelect-Filter.txt parser.
 Home-page: 
 Author: Patrick Garrett
 Author-email: pgarrett@scripps.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `filterframes-0.1.0/README.md` & `filterframes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `filterframes-0.1.0/filterframes/filterframes.py` & `filterframes-0.1.1/filterframes/filterframes.py`

 * *Files identical despite different names*

### Comparing `filterframes-0.1.0/filterframes.egg-info/PKG-INFO` & `filterframes-0.1.1/filterframes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filterframes
-Version: 0.1.0
+Version: 0.1.1
 Summary: A very simple DTASelect-Filter.txt parser.
 Home-page: 
 Author: Patrick Garrett
 Author-email: pgarrett@scripps.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `filterframes-0.1.0/setup.py` & `filterframes-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='filterframes',
-    version='0.1.0',
+    version='0.1.1',
     packages=['filterframes'],
     url='',
     license='',
-    install_requires=['pandas==2.0.1',],
+    install_requires=['pandas==1.5.3',],
     author='Patrick Garrett',
     author_email='pgarrett@scripps.edu',
     description='A very simple DTASelect-Filter.txt parser.',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `filterframes-0.1.0/test/test_filterframes.py` & `filterframes-0.1.1/test/test_filterframes.py`

 * *Files identical despite different names*

