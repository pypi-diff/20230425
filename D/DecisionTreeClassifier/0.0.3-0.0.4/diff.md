# Comparing `tmp/DecisionTreeClassifier-0.0.3.tar.gz` & `tmp/DecisionTreeClassifier-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DecisionTreeClassifier-0.0.3.tar", last modified: Tue Apr 25 00:33:14 2023, max compression
+gzip compressed data, was "DecisionTreeClassifier-0.0.4.tar", last modified: Tue Apr 25 00:37:46 2023, max compression
```

## Comparing `DecisionTreeClassifier-0.0.3.tar` & `DecisionTreeClassifier-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:33:14.901548 DecisionTreeClassifier-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-25 00:33:14.892547 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/
-drwxrwxrwx   0        0        0        0 2023-04-25 00:33:14.898548 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/
--rw-rw-rw-   0        0        0      676 2023-04-25 00:33:14.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-25 00:33:14.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:33:14.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 00:33:14.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 00:33:14.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 00:33:14.900548 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/Testing/
--rw-rw-rw-   0        0        0     7652 2023-04-21 05:19:20.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/Testing/Testing.py
--rw-rw-rw-   0        0        0        0 2023-04-25 00:27:22.000000 DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/Testing/__init__.py
--rw-rw-rw-   0        0        0     1075 2023-04-21 04:53:44.000000 DecisionTreeClassifier-0.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0      676 2023-04-25 00:33:14.901548 DecisionTreeClassifier-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-25 00:33:14.901548 DecisionTreeClassifier-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-04-24 22:55:52.000000 DecisionTreeClassifier-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 00:37:46.495123 DecisionTreeClassifier-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-25 00:37:46.479505 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/
+drwxrwxrwx   0        0        0        0 2023-04-25 00:37:46.495123 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/
+-rw-rw-rw-   0        0        0      676 2023-04-25 00:37:46.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-25 00:37:46.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 00:37:46.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 00:37:46.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 00:37:46.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 00:37:46.495123 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/Testing/
+-rw-rw-rw-   0        0        0     7652 2023-04-21 05:19:20.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/Testing/Testing.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:27:22.000000 DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/Testing/__init__.py
+-rw-rw-rw-   0        0        0     1075 2023-04-21 04:53:44.000000 DecisionTreeClassifier-0.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0      676 2023-04-25 00:37:46.495123 DecisionTreeClassifier-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-25 00:37:46.495123 DecisionTreeClassifier-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-04-25 00:37:33.000000 DecisionTreeClassifier-0.0.4/setup.py
```

### Comparing `DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/PKG-INFO` & `DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/DecisionTreeClassifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DecisionTreeClassifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Decision Tree Classifier.
 Home-page: https://github.com/mlouii/Decision-Tree-Practicum
 Author: Mark Lou, Jobin Joyson
 Author-email: mlou@hawk.iit.edu, jjoyson1@hawk.iit.edu
 License: MIT
 Keywords: decision tree
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `DecisionTreeClassifier-0.0.3/DecisionTreeClassifier/Testing/Testing.py` & `DecisionTreeClassifier-0.0.4/DecisionTreeClassifier/Testing/Testing.py`

 * *Files identical despite different names*

### Comparing `DecisionTreeClassifier-0.0.3/LICENCE.txt` & `DecisionTreeClassifier-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `DecisionTreeClassifier-0.0.3/PKG-INFO` & `DecisionTreeClassifier-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DecisionTreeClassifier
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Decision Tree Classifier.
 Home-page: https://github.com/mlouii/Decision-Tree-Practicum
 Author: Mark Lou, Jobin Joyson
 Author-email: mlou@hawk.iit.edu, jjoyson1@hawk.iit.edu
 License: MIT
 Keywords: decision tree
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `DecisionTreeClassifier-0.0.3/setup.py` & `DecisionTreeClassifier-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 with open("DecisionTreeClassifier/README.txt", "r") as f:
     long_description = f.read()
  
 setup(
   name='DecisionTreeClassifier',
-  version='0.0.3',
+  version='0.0.4',
   description='A Decision Tree Classifier.',
   long_description=long_description,
   package_dir={"": "DecisionTreeClassifier"},
   packages=find_packages(where="DecisionTreeClassifier"),
   url='https://github.com/mlouii/Decision-Tree-Practicum',  
   author='Mark Lou, Jobin Joyson',
   author_email='mlou@hawk.iit.edu, jjoyson1@hawk.iit.edu',
```

