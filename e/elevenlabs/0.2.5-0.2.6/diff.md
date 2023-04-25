# Comparing `tmp/elevenlabs-0.2.5.tar.gz` & `tmp/elevenlabs-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.5.tar", last modified: Sun Apr 23 18:36:14 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.6.tar", last modified: Tue Apr 25 07:02:45 2023, max compression
```

## Comparing `elevenlabs-0.2.5.tar` & `elevenlabs-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:36:14.000000 elevenlabs-0.2.5/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:36:14.323181 elevenlabs-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-23 18:35:56.000000 elevenlabs-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.949905 elevenlabs-0.2.6/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 07:02:45.000000 elevenlabs-0.2.6/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:02:45.953905 elevenlabs-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-25 07:02:34.000000 elevenlabs-0.2.6/setup.py
```

### Comparing `elevenlabs-0.2.5/PKG-INFO` & `elevenlabs-0.2.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.5
+Version: 0.2.6
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.5/README.md` & `elevenlabs-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.5/elevenlabs/__init__.py` & `elevenlabs-0.2.6/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.5/elevenlabs/api/base.py` & `elevenlabs-0.2.6/elevenlabs/api/base.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.5/elevenlabs/api/history.py` & `elevenlabs-0.2.6/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.5/elevenlabs/api/tts.py` & `elevenlabs-0.2.6/elevenlabs/api/tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.5/elevenlabs/api/voice.py` & `elevenlabs-0.2.6/elevenlabs/api/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.5/elevenlabs/utils.py` & `elevenlabs-0.2.6/elevenlabs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import shutil
 import subprocess
-import wave
 from collections.abc import Iterator
 from pathlib import Path
 
 from IPython.display import Audio, display
 
 
 def is_installed(lib_name: str) -> bool:
@@ -31,19 +30,16 @@
             stderr=subprocess.PIPE,
         )
         out, err = proc.communicate(input=audio)
         proc.poll()
 
 
 def save(audio: bytes, filename: str) -> None:
-    with wave.open(filename, "w") as f:
-        f.setnchannels(2)
-        f.setsampwidth(2)
-        f.setframerate(44100)
-        f.writeframes(audio)
+    with open(filename, "wb") as f:
+        f.write(audio)
 
 
 def stream(audio_stream: Iterator[bytes]) -> None:
     if not is_installed("mpv"):
         raise ValueError("mpv not found, necessary to stream audio.")
 
     mpv_command = ["mpv", "--no-cache", "--no-terminal", "--", "fd://0"]
```

### Comparing `elevenlabs-0.2.5/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.6/elevenlabs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.5
+Version: 0.2.6
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.5/setup.py` & `elevenlabs-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.5",
+    version="0.2.6",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
     install_requires=["pydantic>=1.10", "ipython>=7.0"],
     classifiers=[
```

