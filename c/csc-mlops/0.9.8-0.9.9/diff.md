# Comparing `tmp/csc-mlops-0.9.8.tar.gz` & `tmp/csc-mlops-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csc-mlops-0.9.8.tar", last modified: Sun Nov 27 16:34:16 2022, max compression
+gzip compressed data, was "csc-mlops-0.9.9.tar", last modified: Sun Nov 27 19:44:45 2022, max compression
```

## Comparing `csc-mlops-0.9.8.tar` & `csc-mlops-0.9.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    17144 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16661 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.500723 csc-mlops-0.9.8/csc_mlops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17144 2022-11-27 16:34:16.000000 csc-mlops-0.9.8/csc_mlops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      756 2022-11-27 16:34:16.000000 csc-mlops-0.9.8/csc_mlops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2022-11-27 16:34:16.000000 csc-mlops-0.9.8/csc_mlops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2022-11-27 16:34:16.000000 csc-mlops-0.9.8/csc_mlops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      151 2022-11-27 16:34:16.000000 csc-mlops-0.9.8/csc_mlops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-27 16:34:16.000000 csc-mlops-0.9.8/csc_mlops.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.500723 csc-mlops-0.9.8/mlops/
--rw-r--r--   0 runner    (1001) docker     (122)    12176 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/ProjectFile.py
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.500723 csc-mlops-0.9.8/mlops/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.500723 csc-mlops-0.9.8/mlops/data/tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/data/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8421 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/data/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/mlops/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)     4559 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/data/transforms/LoadImageXNATd.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/data/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/mlops/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/mlops/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/tests/mlflow_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlflow_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      502 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlflow_server/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/tests/mlops/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/tests/mlops/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlops/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:16.504722 csc-mlops-0.9.8/tests/mlops/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlops/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4118 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlops/data/transforms/test_LoadImageXNATd.py
--rw-r--r--   0 runner    (1001) docker     (122)     3336 2022-11-27 16:34:05.000000 csc-mlops-0.9.8/tests/mlops/test_Experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.913089 csc-mlops-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    17144 2022-11-27 19:44:45.913089 csc-mlops-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    16661 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/csc_mlops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17144 2022-11-27 19:44:45.000000 csc-mlops-0.9.9/csc_mlops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2022-11-27 19:44:45.000000 csc-mlops-0.9.9/csc_mlops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2022-11-27 19:44:45.000000 csc-mlops-0.9.9/csc_mlops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2022-11-27 19:44:45.000000 csc-mlops-0.9.9/csc_mlops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2022-11-27 19:44:45.000000 csc-mlops-0.9.9/csc_mlops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-27 19:44:45.000000 csc-mlops-0.9.9/csc_mlops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/mlops/
+-rw-r--r--   0 runner    (1001) docker     (122)    12176 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/ProjectFile.py
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/mlops/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/mlops/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/data/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8421 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/data/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/mlops/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)     5089 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/data/transforms/LoadImageXNATd.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/data/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/mlops/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/mlops/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-27 19:44:45.913089 csc-mlops-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.909089 csc-mlops-0.9.9/tests/mlflow_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlflow_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlflow_server/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.913089 csc-mlops-0.9.9/tests/mlops/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.913089 csc-mlops-0.9.9/tests/mlops/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlops/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:45.913089 csc-mlops-0.9.9/tests/mlops/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlops/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlops/data/transforms/test_LoadImageXNATd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3336 2022-11-27 19:44:37.000000 csc-mlops-0.9.9/tests/mlops/test_Experiment.py
```

### Comparing `csc-mlops-0.9.8/LICENSE` & `csc-mlops-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/PKG-INFO` & `csc-mlops-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csc-mlops
-Version: 0.9.8
+Version: 0.9.9
 Summary: An MLOps framework for development of clinical applications
 Home-page: https://github.com/GSTT-CSC/MLOps
 Author: Laurence Jackson
 Author-email: laurence.jackson@gstt.nhs.uk
 Project-URL: Bug Tracker, https://github.com/GSTT-CSC/MLOps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csc-mlops Version: 0.9.8 Summary: An MLOps
+Metadata-Version: 2.1 Name: csc-mlops Version: 0.9.9 Summary: An MLOps
 framework for development of clinical applications Home-page: https://
 github.com/GSTT-CSC/MLOps Author: Laurence Jackson Author-email:
 laurence.jackson@gstt.nhs.uk Project-URL: Bug Tracker, https://github.com/GSTT-
 CSC/MLOps/issues Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
```

### Comparing `csc-mlops-0.9.8/README.md` & `csc-mlops-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/csc_mlops.egg-info/PKG-INFO` & `csc-mlops-0.9.9/csc_mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csc-mlops
-Version: 0.9.8
+Version: 0.9.9
 Summary: An MLOps framework for development of clinical applications
 Home-page: https://github.com/GSTT-CSC/MLOps
 Author: Laurence Jackson
 Author-email: laurence.jackson@gstt.nhs.uk
 Project-URL: Bug Tracker, https://github.com/GSTT-CSC/MLOps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csc-mlops Version: 0.9.8 Summary: An MLOps
+Metadata-Version: 2.1 Name: csc-mlops Version: 0.9.9 Summary: An MLOps
 framework for development of clinical applications Home-page: https://
 github.com/GSTT-CSC/MLOps Author: Laurence Jackson Author-email:
 laurence.jackson@gstt.nhs.uk Project-URL: Bug Tracker, https://github.com/GSTT-
 CSC/MLOps/issues Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
                                     [Logo]
```

### Comparing `csc-mlops-0.9.8/csc_mlops.egg-info/SOURCES.txt` & `csc-mlops-0.9.9/csc_mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/mlops/Experiment.py` & `csc-mlops-0.9.9/mlops/Experiment.py`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/mlops/ProjectFile.py` & `csc-mlops-0.9.9/mlops/ProjectFile.py`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/mlops/cli.py` & `csc-mlops-0.9.9/mlops/cli.py`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/mlops/data/tools/tools.py` & `csc-mlops-0.9.9/mlops/data/tools/tools.py`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/mlops/data/transforms/LoadImageXNATd.py` & `csc-mlops-0.9.9/mlops/data/transforms/LoadImageXNATd.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import xnat
 import os
 import glob
 from monai.transforms import MapTransform, LoadImage
 from monai.config import KeysCollection
 from mlops.utils.logger import logger
 from monai.transforms import Transform
+import time
 
 
 class LoadImageXNATd(MapTransform):
     """
     MapTransform for importing image data from XNAT
     """
 
@@ -66,36 +67,44 @@
                     "Download image from XNAT"
                     for item in d[key]:
                         data_label = item['data_label']
                         if item['data_type'] == 'value':
                             d[data_label] = item['action_data']
                             continue
 
-                        with tempfile.TemporaryDirectory() as tmpdirname:
-                            session_obj = session.create_object(item['action_data'])
-                            session_obj.download_dir(tmpdirname, verbose=self.verbose)
-
-                            images_path = glob.glob(os.path.join(tmpdirname, '**/*' + self.expected_filetype), recursive=True)
-
-                            # image loader needs full path to load single images
-                            # logger.info(f"Downloading images: {images_path}")
+                        attempts = 0
+                        while attempts < 3:
                             try:
+                                with tempfile.TemporaryDirectory() as tmpdirname:
+                                    session_obj = session.create_object(item['action_data'])
+                                    session_obj.download_dir(tmpdirname, verbose=self.verbose)
+
+                                    images_path = glob.glob(os.path.join(tmpdirname, '**/*' + self.expected_filetype), recursive=True)
+
+                                    # image loader needs full path to load single images
+                                    # logger.info(f"Downloading images: {images_path}")
+                                    if not images_path:
+                                        raise Exception
+
+                                    if len(images_path) != session_obj.frames:
+                                        raise Exception(f'Expected {session_obj.frames} files, but received {len(images_path)}')
+
+                                    if len(images_path) == 1:
+                                        image = self.image_loader(images_path)
+
+                                    # image loader needs directory path to load 3D images
+                                    else:
+                                        "find unique directories in list of image paths"
+                                        image_dirs = list(set(os.path.dirname(image_path) for image_path in images_path))
+                                        if len(image_dirs) > 1:
+                                            raise ValueError(f'More than one image series found in {images_path}')
+                                        image = self.image_loader(image_dirs[0])
 
-                                if not images_path:
-                                    raise Exception('No images were retrieved')
-
-                                if len(images_path) == 1:
-                                    image = self.image_loader(images_path)
-
-                                # image loader needs directory path to load 3D images
-                                else:
-                                    "find unique directories in list of image paths"
-                                    image_dirs = list(set(os.path.dirname(image_path) for image_path in images_path))
-                                    if len(image_dirs) > 1:
-                                        raise ValueError(f'More than one image series found in {images_path}')
-                                    image = self.image_loader(image_dirs[0])
                             except Exception as e:
-                                raise Exception(f'Image loader failed on {item} due to {e}')
+                                attempts += 1
+                                time.sleep(0.5)
+                                if attempts == 3:
+                                    raise Exception(f'Image loader failed on {item} after 3 retries due to {e}')
 
                             d[data_label] = image
 
         return d
```

### Comparing `csc-mlops-0.9.8/mlops/utils/logger.py` & `csc-mlops-0.9.9/mlops/utils/logger.py`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/setup.py` & `csc-mlops-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.9.8"
+version = "0.9.9"
 
 install_requires = [
     'mlflow==2.0.1',
     'boto3',
     'docker',
     'minio',
     'colorlog',
```

### Comparing `csc-mlops-0.9.8/tests/mlops/data/transforms/test_LoadImageXNATd.py` & `csc-mlops-0.9.9/tests/mlops/data/transforms/test_LoadImageXNATd.py`

 * *Files identical despite different names*

### Comparing `csc-mlops-0.9.8/tests/mlops/test_Experiment.py` & `csc-mlops-0.9.9/tests/mlops/test_Experiment.py`

 * *Files identical despite different names*

