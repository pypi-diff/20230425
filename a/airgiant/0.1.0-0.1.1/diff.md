# Comparing `tmp/airgiant-0.1.0.tar.gz` & `tmp/airgiant-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airgiant-0.1.0.tar", last modified: Tue Apr 25 13:26:38 2023, max compression
+gzip compressed data, was "airgiant-0.1.1.tar", last modified: Tue Apr 25 13:31:52 2023, max compression
```

## Comparing `airgiant-0.1.0.tar` & `airgiant-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.491857 airgiant-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      544 2023-04-25 13:26:38.487854 airgiant-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.1.0/README.md
--rw-rw-rw-   0        0        0      595 2023-04-25 13:24:29.000000 airgiant-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 13:26:38.491857 airgiant-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.439598 airgiant-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.447654 airgiant-0.1.0/src/airgiant/
--rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.1.0/src/airgiant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.483857 airgiant-0.1.0/src/airgiant/state/
--rw-rw-rw-   0        0        0       21 2023-04-25 13:24:38.000000 airgiant-0.1.0/src/airgiant/state/__init__.py
--rw-rw-rw-   0        0        0    15474 2023-04-24 13:17:08.000000 airgiant-0.1.0/src/airgiant/state/behavior.py
--rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.1.0/src/airgiant/state/hello.py
--rw-rw-rw-   0        0        0      279 2023-04-21 10:59:30.000000 airgiant-0.1.0/src/airgiant/state/imports.py
--rw-rw-rw-   0        0        0      538 2023-04-21 12:02:06.000000 airgiant-0.1.0/src/airgiant/state/main.py
--rw-rw-rw-   0        0        0     1854 2023-04-24 12:45:05.000000 airgiant-0.1.0/src/airgiant/state/make_decision.py
--rw-rw-rw-   0        0        0      233 2023-04-21 12:08:38.000000 airgiant-0.1.0/src/airgiant/state/tempCodeRunnerFile.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.487854 airgiant-0.1.0/src/airgiant/zed/
--rw-rw-rw-   0        0        0      212 2023-04-25 13:14:01.000000 airgiant-0.1.0/src/airgiant/zed/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 13:26:38.471856 airgiant-0.1.0/src/airgiant.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 13:26:38.000000 airgiant-0.1.0/src/airgiant.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.530736 airgiant-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-18 15:04:47.000000 airgiant-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      544 2023-04-25 13:31:52.526736 airgiant-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-18 15:22:04.000000 airgiant-0.1.1/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-25 13:31:26.000000 airgiant-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:31:52.530736 airgiant-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.395120 airgiant-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.401789 airgiant-0.1.1/src/airgiant/
+-rw-rw-rw-   0        0        0       46 2023-04-19 14:01:17.000000 airgiant-0.1.1/src/airgiant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.526736 airgiant-0.1.1/src/airgiant/state/
+-rw-rw-rw-   0        0        0       21 2023-04-25 13:24:38.000000 airgiant-0.1.1/src/airgiant/state/__init__.py
+-rw-rw-rw-   0        0        0    15475 2023-04-25 13:31:02.000000 airgiant-0.1.1/src/airgiant/state/behavior.py
+-rw-rw-rw-   0        0        0       38 2023-04-19 15:00:21.000000 airgiant-0.1.1/src/airgiant/state/hello.py
+-rw-rw-rw-   0        0        0      279 2023-04-21 10:59:30.000000 airgiant-0.1.1/src/airgiant/state/imports.py
+-rw-rw-rw-   0        0        0      539 2023-04-25 13:31:03.000000 airgiant-0.1.1/src/airgiant/state/main.py
+-rw-rw-rw-   0        0        0     1856 2023-04-25 13:31:04.000000 airgiant-0.1.1/src/airgiant/state/make_decision.py
+-rw-rw-rw-   0        0        0      233 2023-04-21 12:08:38.000000 airgiant-0.1.1/src/airgiant/state/tempCodeRunnerFile.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.526736 airgiant-0.1.1/src/airgiant/zed/
+-rw-rw-rw-   0        0        0      212 2023-04-25 13:14:01.000000 airgiant-0.1.1/src/airgiant/zed/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:31:52.425781 airgiant-0.1.1/src/airgiant.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 13:31:52.000000 airgiant-0.1.1/src/airgiant.egg-info/top_level.txt
```

### Comparing `airgiant-0.1.0/LICENSE` & `airgiant-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airgiant-0.1.0/PKG-INFO` & `airgiant-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `airgiant-0.1.0/pyproject.toml` & `airgiant-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "airgiant"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `airgiant-0.1.0/src/airgiant/state/behavior.py` & `airgiant-0.1.1/src/airgiant/state/behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from imports import *
+from .imports import *
 
 async def SkelCoord():                          # return xyz coordinates of person1
     # Define the keypoints
     global person1, lwristperson, rwristperson
     
     keypoints = {
         0: 'nose',
```

### Comparing `airgiant-0.1.0/src/airgiant/state/main.py` & `airgiant-0.1.1/src/airgiant/state/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 finalstate = 0              # confident state > see decision()
 i = 1                       # true condition
 p = 0                       # person detected (0 not, 1 detected)
 ac=3
 
 
 from behavior import *
-from make_decision import *
+from .make_decision import *
 
 
 logging.basicConfig(
     format="%(asctime)s %(message)s",
     level=logging.CRITICAL #.DEBUG,
 )
 asyncio.run(auto())
```

### Comparing `airgiant-0.1.0/src/airgiant/state/make_decision.py` & `airgiant-0.1.1/src/airgiant/state/make_decision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from behavior import *
-from imports import *
+from .behavior import *
+from .imports import *
 
 
 async def control():
     async with websockets.connect(f"ws://10.20.24.10:5555/ws", ping_interval=5, ping_timeout=5) as ws:
         while True:
             a = input("input your cmd:")
             if a == "ask":
```

### Comparing `airgiant-0.1.0/src/airgiant.egg-info/PKG-INFO` & `airgiant-0.1.1/src/airgiant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airgiant
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

