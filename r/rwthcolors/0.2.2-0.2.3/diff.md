# Comparing `tmp/rwthcolors-0.2.2.tar.gz` & `tmp/rwthcolors-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwthcolors-0.2.2.tar", max compression
+gzip compressed data, was "rwthcolors-0.2.3.tar", max compression
```

## Comparing `rwthcolors-0.2.2.tar` & `rwthcolors-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      735 2023-04-24 15:41:04.440123 rwthcolors-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.2/README.md
--rw-r--r--   0        0        0      933 2023-04-24 14:29:37.538409 rwthcolors-0.2.2/RWTHColors/__init__.py
--rw-r--r--   0        0        0     6381 2022-06-21 12:19:23.066702 rwthcolors-0.2.2/RWTHColors/cm.py
--rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.2/RWTHColors/colors/__init__.py
--rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.2/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.2/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
--rw-r--r--   0        0        0     5090 2022-02-01 15:18:59.876053 rwthcolors-0.2.2/RWTHColors/colors/colors.py
--rw-r--r--   0        0        0      535 2023-04-24 15:40:42.132533 rwthcolors-0.2.2/RWTHColors/mpl-styles/rwth-full.mplstyle
--rw-r--r--   0        0        0      137 2023-04-24 15:37:41.325630 rwthcolors-0.2.2/RWTHColors/mpl-styles/rwth.mplstyle
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 rwthcolors-0.2.2/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 rwthcolors-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      798 2023-04-25 12:44:19.094052 rwthcolors-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-01 16:21:46.097203 rwthcolors-0.2.3/README.md
+-rw-r--r--   0        0        0      933 2023-04-24 14:29:37.538409 rwthcolors-0.2.3/RWTHColors/__init__.py
+-rw-r--r--   0        0        0     7266 2023-04-25 07:43:47.734660 rwthcolors-0.2.3/RWTHColors/cm.py
+-rw-r--r--   0        0        0       21 2022-02-01 10:44:53.069840 rwthcolors-0.2.3/RWTHColors/colors/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-24 13:39:59.918195 rwthcolors-0.2.3/RWTHColors/colors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5526 2023-04-24 13:39:59.930905 rwthcolors-0.2.3/RWTHColors/colors/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0        0        0     5090 2022-02-01 15:18:59.876053 rwthcolors-0.2.3/RWTHColors/colors/colors.py
+-rw-r--r--   0        0        0      535 2023-04-24 15:40:42.132533 rwthcolors-0.2.3/RWTHColors/mpl-styles/rwth-full.mplstyle
+-rw-r--r--   0        0        0      137 2023-04-24 15:37:41.325630 rwthcolors-0.2.3/RWTHColors/mpl-styles/rwth.mplstyle
+-rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 rwthcolors-0.2.3/setup.py
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 rwthcolors-0.2.3/PKG-INFO
```

### Comparing `rwthcolors-0.2.2/pyproject.toml` & `rwthcolors-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "RWTHColors"
-version = "0.2.2"
+version = "0.2.3"
 description = "Simple library that makes it easier to use RWTH CI colors in python projects"
 authors = ["Philipp Simon Leibner <philipp.leibner@ifs.rwth-aachen.de>"]
 license = "Apache-2.0"
 readme = "README.md"
+repository = "https://github.com/ifs-rwth-aachen/RWTH-Colors"
 
 classifiers = [
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Intended Audience :: Science/Research"
 ]
 
 keywords = ["rwth", "aachen", "rwth aachen", "farbwelt"]
```

### Comparing `rwthcolors-0.2.2/RWTHColors/__init__.py` & `rwthcolors-0.2.3/RWTHColors/__init__.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.2/RWTHColors/colors/__pycache__/colors.cpython-39.pyc` & `rwthcolors-0.2.3/RWTHColors/colors/__pycache__/colors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.2/RWTHColors/colors/colors.py` & `rwthcolors-0.2.3/RWTHColors/colors/colors.py`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.2/RWTHColors/mpl-styles/rwth-full.mplstyle` & `rwthcolors-0.2.3/RWTHColors/mpl-styles/rwth-full.mplstyle`

 * *Files identical despite different names*

### Comparing `rwthcolors-0.2.2/setup.py` & `rwthcolors-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*'], 'rwthcolors': ['mpl-styles/*']}
 
 install_requires = \
 ['cycler>=0.11.0,<0.12.0', 'matplotlib>=3.5.2,<4.0.0', 'pytest>=7.1.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'rwthcolors',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Simple library that makes it easier to use RWTH CI colors in python projects',
     'long_description': '',
     'author': 'Philipp Simon Leibner',
     'author_email': 'philipp.leibner@ifs.rwth-aachen.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/ifs-rwth-aachen/RWTH-Colors',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `rwthcolors-0.2.2/PKG-INFO` & `rwthcolors-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: rwthcolors
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple library that makes it easier to use RWTH CI colors in python projects
+Home-page: https://github.com/ifs-rwth-aachen/RWTH-Colors
 License: Apache-2.0
 Keywords: rwth,aachen,rwth aachen,farbwelt
 Author: Philipp Simon Leibner
 Author-email: philipp.leibner@ifs.rwth-aachen.de
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,10 +16,11 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Dist: cycler (>=0.11.0,<0.12.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: pytest (>=7.1.1,<8.0.0)
+Project-URL: Repository, https://github.com/ifs-rwth-aachen/RWTH-Colors
 Description-Content-Type: text/markdown
```

