# Comparing `tmp/airgiant-0.0.9.tar.gz` & `tmp/airgiant-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgiant-0.0.9.tar", last modified: Tue Apr 25 13:18:22 2023, max compression
+gzip compressed data, was "airgiant-0.1.0.tar", last modified: Tue Apr 25 13:26:38 2023, max compression
```

## Comparing `airgiant-0.0.9.tar` & `airgiant-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:18:22.192531 airgiant-0.0.9/
--rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      544 2023-04-25 13:18:22.188275 airgiant-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.0.9/README.md
--rw-rw-rw-   0        0        0      595 2023-04-25 13:16:52.000000 airgiant-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 13:18:22.192531 airgiant-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 13:18:22.077542 airgiant-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:18:22.136379 airgiant-0.0.9/src/airgiant/
--rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.0.9/src/airgiant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:18:22.179925 airgiant-0.0.9/src/airgiant/state/
--rw-rw-rw-   0        0        0       24 2023-04-19 15:07:26.000000 airgiant-0.0.9/src/airgiant/state/__init__.py
--rw-rw-rw-   0        0        0    15474 2023-04-24 13:17:08.000000 airgiant-0.0.9/src/airgiant/state/behavior.py
--rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.0.9/src/airgiant/state/hello.py
--rw-rw-rw-   0        0        0      279 2023-04-21 10:59:30.000000 airgiant-0.0.9/src/airgiant/state/imports.py
--rw-rw-rw-   0        0        0      538 2023-04-21 12:02:06.000000 airgiant-0.0.9/src/airgiant/state/main.py
--rw-rw-rw-   0        0        0     1854 2023-04-24 12:45:05.000000 airgiant-0.0.9/src/airgiant/state/make_decision.py
--rw-rw-rw-   0        0        0      233 2023-04-21 12:08:38.000000 airgiant-0.0.9/src/airgiant/state/tempCodeRunnerFile.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:18:22.188275 airgiant-0.0.9/src/airgiant/zed/
--rw-rw-rw-   0        0        0      212 2023-04-25 13:14:01.000000 airgiant-0.0.9/src/airgiant/zed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:18:22.167899 airgiant-0.0.9/src/airgiant.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-25 13:18:22.000000 airgiant-0.0.9/src/airgiant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-25 13:18:22.000000 airgiant-0.0.9/src/airgiant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:18:22.000000 airgiant-0.0.9/src/airgiant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 13:18:22.000000 airgiant-0.0.9/src/airgiant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.491857 airgiant-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-04-25 13:26:38.487854 airgiant-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.1.0/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-25 13:24:29.000000 airgiant-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:26:38.491857 airgiant-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.439598 airgiant-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.447654 airgiant-0.1.0/src/airgiant/
+-rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.1.0/src/airgiant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.483857 airgiant-0.1.0/src/airgiant/state/
+-rw-rw-rw-   0        0        0       21 2023-04-25 13:24:38.000000 airgiant-0.1.0/src/airgiant/state/__init__.py
+-rw-rw-rw-   0        0        0    15474 2023-04-24 13:17:08.000000 airgiant-0.1.0/src/airgiant/state/behavior.py
+-rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.1.0/src/airgiant/state/hello.py
+-rw-rw-rw-   0        0        0      279 2023-04-21 10:59:30.000000 airgiant-0.1.0/src/airgiant/state/imports.py
+-rw-rw-rw-   0        0        0      538 2023-04-21 12:02:06.000000 airgiant-0.1.0/src/airgiant/state/main.py
+-rw-rw-rw-   0        0        0     1854 2023-04-24 12:45:05.000000 airgiant-0.1.0/src/airgiant/state/make_decision.py
+-rw-rw-rw-   0        0        0      233 2023-04-21 12:08:38.000000 airgiant-0.1.0/src/airgiant/state/tempCodeRunnerFile.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.487854 airgiant-0.1.0/src/airgiant/zed/
+-rw-rw-rw-   0        0        0      212 2023-04-25 13:14:01.000000 airgiant-0.1.0/src/airgiant/zed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.471856 airgiant-0.1.0/src/airgiant.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/top_level.txt
```

### Comparing `airgiant-0.0.9/LICENSE` & `airgiant-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.9/PKG-INFO` & `airgiant-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `airgiant-0.0.9/pyproject.toml` & `airgiant-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "airgiant"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airgiant-0.0.9/src/airgiant/state/behavior.py` & `airgiant-0.1.0/src/airgiant/state/behavior.py`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.9/src/airgiant/state/main.py` & `airgiant-0.1.0/src/airgiant/state/main.py`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.9/src/airgiant/state/make_decision.py` & `airgiant-0.1.0/src/airgiant/state/make_decision.py`

 * *Files identical despite different names*

### Comparing `airgiant-0.0.9/src/airgiant.egg-info/PKG-INFO` & `airgiant-0.1.0/src/airgiant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

