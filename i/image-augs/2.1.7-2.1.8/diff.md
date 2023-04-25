# Comparing `tmp/image_augs-2.1.7.tar.gz` & `tmp/image_augs-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-2.1.7.tar", last modified: Mon Apr 24 09:58:14 2023, max compression
+gzip compressed data, was "dist/image_augs-2.1.8.tar", last modified: Mon Apr 24 10:04:25 2023, max compression
```

## Comparing `image_augs-2.1.7.tar` & `image_augs-2.1.8.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:58:14.000000 image_augs-2.1.7/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.7/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.7/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.7/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.7/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.7/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      496 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       28 2023-04-24 09:58:14.000000 image_augs-2.1.7/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 09:58:14.000000 image_augs-2.1.7/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.7/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.7/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.7/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.7/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.7/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.7/instance_seg/yml_writer_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 09:58:14.000000 image_augs-2.1.7/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.7/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 10:04:25.000000 image_augs-2.1.8/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.8/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.8/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.8/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.8/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.8/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.8/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.8/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.8/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.8/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.8/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.8/instance_seg/yml_writer_poly.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/object_detection_new/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.1.8/object_detection_new/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17484 2023-04-21 13:36:31.000000 image_augs-2.1.8/object_detection_new/augmentation_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.1.8/object_detection_new/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    22268 2023-04-21 14:06:18.000000 image_augs-2.1.8/object_detection_new/txt_reader_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4796 2023-04-21 10:28:10.000000 image_augs-2.1.8/object_detection_new/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-21 12:43:02.000000 image_augs-2.1.8/object_detection_new/yml_writer_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 10:04:25.000000 image_augs-2.1.8/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.8/setup.py
```

### Comparing `image_augs-2.1.7/PKG-INFO` & `image_augs-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 2.1.7
+Version: 2.1.8
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.1.7/README.md` & `image_augs-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/classification/classification_.py` & `image_augs-2.1.8/classification/classification_.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/classification/classification_combined.py` & `image_augs-2.1.8/classification/classification_combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/classification/logging_util.py` & `image_augs-2.1.8/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/image_augs.egg-info/PKG-INFO` & `image_augs-2.1.8/image_augs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-augs
-Version: 2.1.7
+Version: 2.1.8
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `image_augs-2.1.7/instance_seg/augment_poly.py` & `image_augs-2.1.8/instance_seg/augment_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/instance_seg/json_reader_poly.py` & `image_augs-2.1.8/instance_seg/json_reader_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/instance_seg/logging_util.py` & `image_augs-2.1.8/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/instance_seg/utils_poly.py` & `image_augs-2.1.8/instance_seg/utils_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/instance_seg/yml_writer_poly.py` & `image_augs-2.1.8/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.7/setup.py` & `image_augs-2.1.8/setup.py`

 * *Files identical despite different names*

