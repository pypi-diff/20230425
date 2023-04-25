# Comparing `tmp/indexed_pq-0.1.4.tar.gz` & `tmp/indexed_pq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexed_pq-0.1.4.tar", last modified: Sun Mar 26 14:11:54 2023, max compression
+gzip compressed data, was "indexed_pq-0.1.5.tar", last modified: Tue Apr 25 11:06:49 2023, max compression
```

## Comparing `indexed_pq-0.1.4.tar` & `indexed_pq-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 14:11:53.996605 indexed_pq-0.1.4/
--rw-rw-rw-   0        0        0     3449 2023-03-26 14:11:53.995606 indexed_pq-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3071 2023-03-26 07:39:56.000000 indexed_pq-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 14:11:53.975959 indexed_pq-0.1.4/indexed_pq/
--rw-rw-rw-   0        0        0       48 2023-03-26 14:11:08.000000 indexed_pq-0.1.4/indexed_pq/__init__.py
--rw-rw-rw-   0        0        0    10512 2023-03-26 07:30:52.000000 indexed_pq-0.1.4/indexed_pq/ipq.py
-drwxrwxrwx   0        0        0        0 2023-03-26 14:11:53.993605 indexed_pq-0.1.4/indexed_pq.egg-info/
--rw-rw-rw-   0        0        0     3449 2023-03-26 14:11:53.000000 indexed_pq-0.1.4/indexed_pq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-03-26 14:11:53.000000 indexed_pq-0.1.4/indexed_pq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 14:11:53.000000 indexed_pq-0.1.4/indexed_pq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-26 14:11:53.000000 indexed_pq-0.1.4/indexed_pq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 14:11:53.997605 indexed_pq-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-03-26 14:11:45.000000 indexed_pq-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 11:06:49.427264 indexed_pq-0.1.5/
+-rw-rw-rw-   0        0        0     3494 2023-04-25 11:06:49.426264 indexed_pq-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3071 2023-03-26 07:39:56.000000 indexed_pq-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 11:06:49.403986 indexed_pq-0.1.5/indexed_pq/
+-rw-rw-rw-   0        0        0       48 2023-03-26 14:11:08.000000 indexed_pq-0.1.5/indexed_pq/__init__.py
+-rw-rw-rw-   0        0        0    10512 2023-03-26 07:30:52.000000 indexed_pq-0.1.5/indexed_pq/ipq.py
+drwxrwxrwx   0        0        0        0 2023-04-25 11:06:49.423261 indexed_pq-0.1.5/indexed_pq.egg-info/
+-rw-rw-rw-   0        0        0     3494 2023-04-25 11:06:49.000000 indexed_pq-0.1.5/indexed_pq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-04-25 11:06:49.000000 indexed_pq-0.1.5/indexed_pq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 11:06:49.000000 indexed_pq-0.1.5/indexed_pq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 11:06:49.000000 indexed_pq-0.1.5/indexed_pq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 11:06:49.427264 indexed_pq-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-04-25 11:06:38.000000 indexed_pq-0.1.5/setup.py
```

### Comparing `indexed_pq-0.1.4/PKG-INFO` & `indexed_pq-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: indexed_pq
-Version: 0.1.4
-Summary: UNKNOWN
+Version: 0.1.5
+Summary: max and min Indexed priority queue with median heap 
 Home-page: UNKNOWN
 Author: humblemat
 Author-email: humblemat@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `indexed_pq-0.1.4/README.md` & `indexed_pq-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `indexed_pq-0.1.4/indexed_pq/ipq.py` & `indexed_pq-0.1.5/indexed_pq/ipq.py`

 * *Files identical despite different names*

### Comparing `indexed_pq-0.1.4/indexed_pq.egg-info/PKG-INFO` & `indexed_pq-0.1.5/indexed_pq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: indexed-pq
-Version: 0.1.4
-Summary: UNKNOWN
+Version: 0.1.5
+Summary: max and min Indexed priority queue with median heap 
 Home-page: UNKNOWN
 Author: humblemat
 Author-email: humblemat@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `indexed_pq-0.1.4/setup.py` & `indexed_pq-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="indexed_pq",
     # version of the module
-    version="0.1.4",
+    version="0.1.5",
  
     # Name of Author
     author="humblemat",
  
     # your Email address
     author_email="humblemat@gmail.com",
- 
+    description='max and min Indexed priority queue with median heap ',
     # Specifying that we are using markdown file for description
     long_description=long_description,
     long_description_content_type="text/markdown",
  
     # Any link to reach this module, ***if*** you have any webpage or github profile
     # url="https://github.com/username/",
     packages=setuptools.find_packages(),
```

