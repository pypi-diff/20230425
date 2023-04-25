# Comparing `tmp/videoprocessor-0.0.2.tar.gz` & `tmp/videoprocessor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videoprocessor-0.0.2.tar", last modified: Tue Apr 25 01:45:08 2023, max compression
+gzip compressed data, was "videoprocessor-0.0.3.tar", last modified: Tue Apr 25 02:07:39 2023, max compression
```

## Comparing `videoprocessor-0.0.2.tar` & `videoprocessor-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 01:45:08.678514 videoprocessor-0.0.2/
--rw-rw-r--   0 luffy     (1000) luffy     (1000)     1068 2023-04-25 01:12:54.000000 videoprocessor-0.0.2/LICENSE
--rw-rw-r--   0 luffy     (1000) luffy     (1000)     3839 2023-04-25 01:45:08.678514 videoprocessor-0.0.2/PKG-INFO
--rw-rw-r--   0 luffy     (1000) luffy     (1000)     3434 2023-04-24 05:50:26.000000 videoprocessor-0.0.2/README.md
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      613 2023-04-25 01:44:38.000000 videoprocessor-0.0.2/pyproject.toml
--rw-rw-r--   0 luffy     (1000) luffy     (1000)       38 2023-04-25 01:45:08.678514 videoprocessor-0.0.2/setup.cfg
-drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 01:45:08.674514 videoprocessor-0.0.2/src/
-drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 01:45:08.678514 videoprocessor-0.0.2/src/videoprocessor/
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      164 2023-04-25 01:38:49.000000 videoprocessor-0.0.2/src/videoprocessor/__init__.py
--rw-rw-r--   0 luffy     (1000) luffy     (1000)     9387 2023-04-25 01:04:24.000000 videoprocessor-0.0.2/src/videoprocessor/videoprocessor.py
-drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 01:45:08.678514 videoprocessor-0.0.2/src/videoprocessor.egg-info/
--rw-rw-r--   0 luffy     (1000) luffy     (1000)     3839 2023-04-25 01:45:08.000000 videoprocessor-0.0.2/src/videoprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 luffy     (1000) luffy     (1000)      268 2023-04-25 01:45:08.000000 videoprocessor-0.0.2/src/videoprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)        1 2023-04-25 01:45:08.000000 videoprocessor-0.0.2/src/videoprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 luffy     (1000) luffy     (1000)       15 2023-04-25 01:45:08.000000 videoprocessor-0.0.2/src/videoprocessor.egg-info/top_level.txt
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 02:07:39.820776 videoprocessor-0.0.3/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)     1068 2023-04-25 01:12:54.000000 videoprocessor-0.0.3/LICENSE
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)     3839 2023-04-25 02:07:39.820776 videoprocessor-0.0.3/PKG-INFO
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)     3434 2023-04-24 05:50:26.000000 videoprocessor-0.0.3/README.md
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)      613 2023-04-25 02:06:13.000000 videoprocessor-0.0.3/pyproject.toml
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       38 2023-04-25 02:07:39.820776 videoprocessor-0.0.3/setup.cfg
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 02:07:39.820776 videoprocessor-0.0.3/src/
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 02:07:39.820776 videoprocessor-0.0.3/src/videoprocessor/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       84 2023-04-25 02:02:50.000000 videoprocessor-0.0.3/src/videoprocessor/__init__.py
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)     9387 2023-04-25 01:04:24.000000 videoprocessor-0.0.3/src/videoprocessor/videoprocessor.py
+drwxrwxr-x   0 luffy     (1000) luffy     (1000)        0 2023-04-25 02:07:39.820776 videoprocessor-0.0.3/src/videoprocessor.egg-info/
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)     3839 2023-04-25 02:07:39.000000 videoprocessor-0.0.3/src/videoprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)      268 2023-04-25 02:07:39.000000 videoprocessor-0.0.3/src/videoprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)        1 2023-04-25 02:07:39.000000 videoprocessor-0.0.3/src/videoprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 luffy     (1000) luffy     (1000)       15 2023-04-25 02:07:39.000000 videoprocessor-0.0.3/src/videoprocessor.egg-info/top_level.txt
```

### Comparing `videoprocessor-0.0.2/LICENSE` & `videoprocessor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `videoprocessor-0.0.2/PKG-INFO` & `videoprocessor-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoprocessor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package base on ffmpeg and ffmpeg-python to process video.
 Author-email: FogSalary <Kairong_Wu@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `videoprocessor-0.0.2/README.md` & `videoprocessor-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `videoprocessor-0.0.2/pyproject.toml` & `videoprocessor-0.0.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "videoprocessor"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="FogSalary", email="Kairong_Wu@163.com" },
 ]
 description = "A package base on ffmpeg and ffmpeg-python to process video."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `videoprocessor-0.0.2/src/videoprocessor/videoprocessor.py` & `videoprocessor-0.0.3/src/videoprocessor/videoprocessor.py`

 * *Files identical despite different names*

### Comparing `videoprocessor-0.0.2/src/videoprocessor.egg-info/PKG-INFO` & `videoprocessor-0.0.3/src/videoprocessor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoprocessor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package base on ffmpeg and ffmpeg-python to process video.
 Author-email: FogSalary <Kairong_Wu@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

