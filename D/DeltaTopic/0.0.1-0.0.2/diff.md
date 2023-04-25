# Comparing `tmp/DeltaTopic-0.0.1.tar.gz` & `tmp/DeltaTopic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeltaTopic-0.0.1.tar", last modified: Tue Apr 25 04:28:13 2023, max compression
+gzip compressed data, was "DeltaTopic-0.0.2.tar", last modified: Tue Apr 25 04:34:56 2023, max compression
```

## Comparing `DeltaTopic-0.0.1.tar` & `DeltaTopic-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/DeltaTopic/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-15 05:16:01.000000 DeltaTopic-0.0.1/DeltaTopic/__init__.py
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/DeltaTopic/nn/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10596 2023-04-15 05:19:11.000000 DeltaTopic-0.0.1/DeltaTopic/nn/TrainingPlan.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-14 21:10:15.000000 DeltaTopic-0.0.1/DeltaTopic/nn/__init__.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    29553 2023-03-10 21:06:37.000000 DeltaTopic-0.0.1/DeltaTopic/nn/base_components.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10652 2023-03-10 21:06:37.000000 DeltaTopic-0.0.1/DeltaTopic/nn/base_model.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     9128 2023-03-10 21:06:37.000000 DeltaTopic-0.0.1/DeltaTopic/nn/dataloader_util.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    40251 2023-04-25 02:21:55.000000 DeltaTopic-0.0.1/DeltaTopic/nn/modelhub.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    14127 2023-04-25 02:16:43.000000 DeltaTopic-0.0.1/DeltaTopic/nn/module.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    27768 2023-04-25 03:32:03.000000 DeltaTopic-0.0.1/DeltaTopic/nn/util.py
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/DeltaTopic/run/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     3459 2023-04-24 23:03:26.000000 DeltaTopic-0.0.1/DeltaTopic/run/BALSAM.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     4088 2023-04-15 05:19:11.000000 DeltaTopic-0.0.1/DeltaTopic/run/DeltaTopic.py
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-14 21:33:20.000000 DeltaTopic-0.0.1/DeltaTopic/run/__init__.py
-drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/DeltaTopic.egg-info/
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      396 2023-04-25 04:28:12.000000 DeltaTopic-0.0.1/DeltaTopic.egg-info/PKG-INFO
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      560 2023-04-25 04:28:12.000000 DeltaTopic-0.0.1/DeltaTopic.egg-info/SOURCES.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        1 2023-04-25 04:28:12.000000 DeltaTopic-0.0.1/DeltaTopic.egg-info/dependency_links.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       99 2023-04-25 04:28:12.000000 DeltaTopic-0.0.1/DeltaTopic.egg-info/entry_points.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      119 2023-04-25 04:28:12.000000 DeltaTopic-0.0.1/DeltaTopic.egg-info/requires.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       11 2023-04-25 04:28:12.000000 DeltaTopic-0.0.1/DeltaTopic.egg-info/top_level.txt
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      396 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/PKG-INFO
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      684 2023-04-15 00:58:13.000000 DeltaTopic-0.0.1/README.md
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       79 2023-04-25 04:28:13.013499 DeltaTopic-0.0.1/setup.cfg
--rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      889 2023-04-25 03:36:05.000000 DeltaTopic-0.0.1/setup.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.488361 DeltaTopic-0.0.2/DeltaTopic/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-15 05:16:01.000000 DeltaTopic-0.0.2/DeltaTopic/__init__.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/DeltaTopic/nn/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10596 2023-04-15 05:19:11.000000 DeltaTopic-0.0.2/DeltaTopic/nn/TrainingPlan.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-14 21:10:15.000000 DeltaTopic-0.0.2/DeltaTopic/nn/__init__.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    29553 2023-03-10 21:06:37.000000 DeltaTopic-0.0.2/DeltaTopic/nn/base_components.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    10652 2023-03-10 21:06:37.000000 DeltaTopic-0.0.2/DeltaTopic/nn/base_model.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     9128 2023-03-10 21:06:37.000000 DeltaTopic-0.0.2/DeltaTopic/nn/dataloader_util.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    40251 2023-04-25 02:21:55.000000 DeltaTopic-0.0.2/DeltaTopic/nn/modelhub.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    14127 2023-04-25 02:16:43.000000 DeltaTopic-0.0.2/DeltaTopic/nn/module.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)    27768 2023-04-25 03:32:03.000000 DeltaTopic-0.0.2/DeltaTopic/nn/util.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/DeltaTopic/run/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     3459 2023-04-24 23:03:26.000000 DeltaTopic-0.0.2/DeltaTopic/run/BALSAM.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)     4088 2023-04-15 05:19:11.000000 DeltaTopic-0.0.2/DeltaTopic/run/DeltaTopic.py
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-14 21:33:20.000000 DeltaTopic-0.0.2/DeltaTopic/run/__init__.py
+drwxr-xr-x   0 yzhang   (1287624208) domain users (1287600513)        0 2023-04-25 04:34:56.488361 DeltaTopic-0.0.2/DeltaTopic.egg-info/
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      396 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/PKG-INFO
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      560 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/SOURCES.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)        1 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/dependency_links.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       99 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/entry_points.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      120 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/requires.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       11 2023-04-25 04:34:56.000000 DeltaTopic-0.0.2/DeltaTopic.egg-info/top_level.txt
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      396 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/PKG-INFO
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      684 2023-04-15 00:58:13.000000 DeltaTopic-0.0.2/README.md
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)       79 2023-04-25 04:34:56.492362 DeltaTopic-0.0.2/setup.cfg
+-rw-r--r--   0 yzhang   (1287624208) domain users (1287600513)      880 2023-04-25 04:34:46.000000 DeltaTopic-0.0.2/setup.py
```

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/TrainingPlan.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/TrainingPlan.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/base_components.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/base_components.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/base_model.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/base_model.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/dataloader_util.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/dataloader_util.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/modelhub.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/modelhub.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/module.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/module.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/nn/util.py` & `DeltaTopic-0.0.2/DeltaTopic/nn/util.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/run/BALSAM.py` & `DeltaTopic-0.0.2/DeltaTopic/run/BALSAM.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic/run/DeltaTopic.py` & `DeltaTopic-0.0.2/DeltaTopic/run/DeltaTopic.py`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/DeltaTopic.egg-info/SOURCES.txt` & `DeltaTopic-0.0.2/DeltaTopic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/README.md` & `DeltaTopic-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `DeltaTopic-0.0.1/setup.py` & `DeltaTopic-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import os
 from setuptools import setup, find_packages
 
 setup(
     name='DeltaTopic',
     packages=find_packages(),
     author='Yichen Zhang',
-    version='0.0.1',
+    version='0.0.2',
     description="Packages to implement BALSAM and DeltaTopic as described in the paper: Unraveling dynamically-encoded latent transcriptomic patterns in pancreatic cancer cells by topic modelling",
     url="https://github.com/causalpathlab/deltaTopic",
     entry_points={'console_scripts':
         ['BALSAM = DeltaTopic.run.BALSAM:main',
         'DeltaTopic = DeltaTopic.run.DeltaTopic:main']
     },
     install_requires=['pandas==1.4.1',
                       'torch==2.0.0', 
                       'h5py==3.6.0', 
                       'numpy==1.21.5', 
                       'anndata==0.7.8',
                       'pytorch_lightning==1.9.0', 
-                      'scanp==1.9.3', 
+                      'scanpy==1.9.3', 
                       'scipy ==1.8.0']
 )
```

