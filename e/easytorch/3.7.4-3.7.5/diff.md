# Comparing `tmp/easytorch-3.7.4.tar.gz` & `tmp/easytorch-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.4.tar", last modified: Fri Apr 21 12:59:18 2023, max compression
+gzip compressed data, was "easytorch-3.7.5.tar", last modified: Mon Apr 24 22:35:59 2023, max compression
```

## Comparing `easytorch-3.7.4.tar` & `easytorch-3.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.626684 easytorch-3.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 12:59:06.000000 easytorch-3.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 12:59:18.626684 easytorch-3.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-21 12:59:06.000000 easytorch-3.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.622684 easytorch-3.7.4/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.622684 easytorch-3.7.4/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.622684 easytorch-3.7.4/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.622684 easytorch-3.7.4/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.626684 easytorch-3.7.4/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.626684 easytorch-3.7.4/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-21 12:59:06.000000 easytorch-3.7.4/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:59:18.622684 easytorch-3.7.4/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 12:59:18.000000 easytorch-3.7.4/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-21 12:59:18.000000 easytorch-3.7.4/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:59:18.000000 easytorch-3.7.4/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 12:59:18.000000 easytorch-3.7.4/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 12:59:18.000000 easytorch-3.7.4/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:59:18.626684 easytorch-3.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-21 12:59:06.000000 easytorch-3.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.986572 easytorch-3.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 22:35:47.000000 easytorch-3.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-24 22:35:59.986572 easytorch-3.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-24 22:35:47.000000 easytorch-3.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.982572 easytorch-3.7.5/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.982572 easytorch-3.7.5/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.982572 easytorch-3.7.5/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.986572 easytorch-3.7.5/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.986572 easytorch-3.7.5/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.986572 easytorch-3.7.5/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-24 22:35:47.000000 easytorch-3.7.5/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:35:59.982572 easytorch-3.7.5/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-24 22:35:59.000000 easytorch-3.7.5/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-24 22:35:59.000000 easytorch-3.7.5/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:35:59.000000 easytorch-3.7.5/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 22:35:59.000000 easytorch-3.7.5/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 22:35:59.000000 easytorch-3.7.5/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:35:59.986572 easytorch-3.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-24 22:35:47.000000 easytorch-3.7.5/setup.py
```

### Comparing `easytorch-3.7.4/LICENSE` & `easytorch-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/PKG-INFO` & `easytorch-3.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.4
+Version: 3.7.5
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -170,21 +170,26 @@
         # Extra preprocessing, if needed.
         # Apply transforms, if needed.
 
         return image, label
 ```
 
 #### 3. Entry point (say main.py)
+### Run as:
+
+`python main.py -ph train -b 512 -e 10 -gpus 0`
 
+One can also directly pass arguments as below which overrides all.
 ```python
 from easytorch import EasyTorch
 
-runner = EasyTorch(phase="train", batch_size=4, epochs=21,
-                   num_channel=1, num_class=2,
-                   split_ratio=[0.6, 0.2, 0.2])
+runner = EasyTorch(phase="train", batch_size=4, epochs=10,
+                   gpus=[0], num_channel=1, 
+                   num_class=2, data_source="<some_data>/data_split.json")
+runner.run(MyTrainer, MyDataset)
 ```
 
 ### All the best! Cheers! 🎉
 
 #### Cite the following papers if you use this library:
 
 ```
```

### Comparing `easytorch-3.7.4/README.md` & `easytorch-3.7.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -157,21 +157,26 @@
         # Extra preprocessing, if needed.
         # Apply transforms, if needed.
 
         return image, label
 ```
 
 #### 3. Entry point (say main.py)
+### Run as:
 
+`python main.py -ph train -b 512 -e 10 -gpus 0`
+
+One can also directly pass arguments as below which overrides all.
 ```python
 from easytorch import EasyTorch
 
-runner = EasyTorch(phase="train", batch_size=4, epochs=21,
-                   num_channel=1, num_class=2,
-                   split_ratio=[0.6, 0.2, 0.2])
+runner = EasyTorch(phase="train", batch_size=4, epochs=10,
+                   gpus=[0], num_channel=1, 
+                   num_class=2, data_source="<some_data>/data_split.json")
+runner.run(MyTrainer, MyDataset)
 ```
 
 ### All the best! Cheers! 🎉
 
 #### Cite the following papers if you use this library:
 
 ```
```

### Comparing `easytorch-3.7.4/easytorch/config/__init__.py` & `easytorch-3.7.5/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/config/state.py` & `easytorch-3.7.5/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/data/data.py` & `easytorch-3.7.5/easytorch/data/data.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/data/datautils.py` & `easytorch-3.7.5/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/data/multiproc.py` & `easytorch-3.7.5/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/easytorch.py` & `easytorch-3.7.5/easytorch/easytorch.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/metrics/loss.py` & `easytorch-3.7.5/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/metrics/metrics.py` & `easytorch-3.7.5/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/runner.py` & `easytorch-3.7.5/easytorch/runner.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/utils/__init__.py` & `easytorch-3.7.5/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/utils/ddp_check.py` & `easytorch-3.7.5/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/utils/tensorutils.py` & `easytorch-3.7.5/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/vision/imageutils.py` & `easytorch-3.7.5/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/vision/plotter.py` & `easytorch-3.7.5/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch/vision/transforms.py` & `easytorch-3.7.5/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/easytorch.egg-info/PKG-INFO` & `easytorch-3.7.5/easytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.4
+Version: 3.7.5
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -170,21 +170,26 @@
         # Extra preprocessing, if needed.
         # Apply transforms, if needed.
 
         return image, label
 ```
 
 #### 3. Entry point (say main.py)
+### Run as:
+
+`python main.py -ph train -b 512 -e 10 -gpus 0`
 
+One can also directly pass arguments as below which overrides all.
 ```python
 from easytorch import EasyTorch
 
-runner = EasyTorch(phase="train", batch_size=4, epochs=21,
-                   num_channel=1, num_class=2,
-                   split_ratio=[0.6, 0.2, 0.2])
+runner = EasyTorch(phase="train", batch_size=4, epochs=10,
+                   gpus=[0], num_channel=1, 
+                   num_class=2, data_source="<some_data>/data_split.json")
+runner.run(MyTrainer, MyDataset)
 ```
 
 ### All the best! Cheers! 🎉
 
 #### Cite the following papers if you use this library:
 
 ```
```

### Comparing `easytorch-3.7.4/easytorch.egg-info/SOURCES.txt` & `easytorch-3.7.5/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.4/setup.py` & `easytorch-3.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.4",
+    version="3.7.5",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

