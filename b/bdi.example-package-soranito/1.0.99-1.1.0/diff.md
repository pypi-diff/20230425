# Comparing `tmp/bdi.example_package_soranito-1.0.99.tar.gz` & `tmp/bdi.example_package_soranito-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdi.example_package_soranito-1.0.99.tar", last modified: Mon Apr 24 11:30:26 2023, max compression
+gzip compressed data, was "bdi.example_package_soranito-1.1.0.tar", last modified: Tue Apr 25 08:13:33 2023, max compression
```

## Comparing `bdi.example_package_soranito-1.0.99.tar` & `bdi.example_package_soranito-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 11:30:26.854859 bdi.example_package_soranito-1.0.99/
--rw-rw-rw-   0        0        0     1091 2023-04-04 22:01:40.000000 bdi.example_package_soranito-1.0.99/LICENSE
--rw-rw-rw-   0        0        0      710 2023-04-24 11:30:26.852856 bdi.example_package_soranito-1.0.99/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-04 22:04:03.000000 bdi.example_package_soranito-1.0.99/README.md
--rw-rw-rw-   0        0        0      614 2023-04-24 11:29:57.000000 bdi.example_package_soranito-1.0.99/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 11:30:26.854859 bdi.example_package_soranito-1.0.99/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 11:30:26.827860 bdi.example_package_soranito-1.0.99/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 11:30:26.846859 bdi.example_package_soranito-1.0.99/src/bdi.example_package_soranito.egg-info/
--rw-rw-rw-   0        0        0      710 2023-04-24 11:30:26.000000 bdi.example_package_soranito-1.0.99/src/bdi.example_package_soranito.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-04-24 11:30:26.000000 bdi.example_package_soranito-1.0.99/src/bdi.example_package_soranito.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 11:30:26.000000 bdi.example_package_soranito-1.0.99/src/bdi.example_package_soranito.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-24 11:30:26.000000 bdi.example_package_soranito-1.0.99/src/bdi.example_package_soranito.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 11:30:26.850863 bdi.example_package_soranito-1.0.99/src/example_package_soranito/
--rw-rw-rw-   0        0        0        0 2023-04-04 22:00:47.000000 bdi.example_package_soranito-1.0.99/src/example_package_soranito/__init__.py
--rw-rw-rw-   0        0        0       93 2023-04-24 11:29:57.000000 bdi.example_package_soranito-1.0.99/src/example_package_soranito/example.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:13:33.367016 bdi.example_package_soranito-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-04 22:01:40.000000 bdi.example_package_soranito-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      709 2023-04-25 08:13:33.365015 bdi.example_package_soranito-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-04 22:04:03.000000 bdi.example_package_soranito-1.1.0/README.md
+-rw-rw-rw-   0        0        0      613 2023-04-25 08:13:04.000000 bdi.example_package_soranito-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:13:33.368016 bdi.example_package_soranito-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 08:13:33.320017 bdi.example_package_soranito-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:13:33.349017 bdi.example_package_soranito-1.1.0/src/bdi.example_package_soranito.egg-info/
+-rw-rw-rw-   0        0        0      709 2023-04-25 08:13:33.000000 bdi.example_package_soranito-1.1.0/src/bdi.example_package_soranito.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-04-25 08:13:33.000000 bdi.example_package_soranito-1.1.0/src/bdi.example_package_soranito.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:13:33.000000 bdi.example_package_soranito-1.1.0/src/bdi.example_package_soranito.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-25 08:13:33.000000 bdi.example_package_soranito-1.1.0/src/bdi.example_package_soranito.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 08:13:33.356019 bdi.example_package_soranito-1.1.0/src/example_package_soranito/
+-rw-rw-rw-   0        0        0        0 2023-04-04 22:00:47.000000 bdi.example_package_soranito-1.1.0/src/example_package_soranito/__init__.py
+-rw-rw-rw-   0        0        0       93 2023-04-24 11:29:57.000000 bdi.example_package_soranito-1.1.0/src/example_package_soranito/example.py
```

### Comparing `bdi.example_package_soranito-1.0.99/LICENSE` & `bdi.example_package_soranito-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bdi.example_package_soranito-1.0.99/PKG-INFO` & `bdi.example_package_soranito-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdi.example_package_soranito
-Version: 1.0.99
+Version: 1.1.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bdi.example_package_soranito-1.0.99/pyproject.toml` & `bdi.example_package_soranito-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bdi.example_package_soranito"
-version = "1.0.99"
+version = "1.1.0"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `bdi.example_package_soranito-1.0.99/src/bdi.example_package_soranito.egg-info/PKG-INFO` & `bdi.example_package_soranito-1.1.0/src/bdi.example_package_soranito.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdi.example-package-soranito
-Version: 1.0.99
+Version: 1.1.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

