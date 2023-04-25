# Comparing `tmp/image_augs-2.1.8.tar.gz` & `tmp/image_augs-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image_augs-2.1.8.tar", last modified: Mon Apr 24 10:04:25 2023, max compression
+gzip compressed data, was "dist/image_augs-2.2.9.tar", last modified: Tue Apr 25 07:32:26 2023, max compression
```

## Comparing `image_augs-2.1.8.tar` & `image_augs-2.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 10:04:25.000000 image_augs-2.1.8/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     7620 2023-04-24 05:37:53.000000 image_augs-2.1.8/README.md
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/classification/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.1.8/classification/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.1.8/classification/classification_.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.1.8/classification/classification_combined.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.1.8/classification/logging_util.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     8200 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/PKG-INFO
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/SOURCES.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/dependency_links.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/requires.txt
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-24 10:04:25.000000 image_augs-2.1.8/image_augs.egg-info/top_level.txt
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/instance_seg/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.1.8/instance_seg/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17369 2023-04-21 13:36:30.000000 image_augs-2.1.8/instance_seg/augment_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    22978 2023-04-21 14:06:43.000000 image_augs-2.1.8/instance_seg/json_reader_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.1.8/instance_seg/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.1.8/instance_seg/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.1.8/instance_seg/yml_writer_poly.py
-drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-24 10:04:25.000000 image_augs-2.1.8/object_detection_new/
--rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.1.8/object_detection_new/__init__.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    17484 2023-04-21 13:36:31.000000 image_augs-2.1.8/object_detection_new/augmentation_rect.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.1.8/object_detection_new/logging_util.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)    22268 2023-04-21 14:06:18.000000 image_augs-2.1.8/object_detection_new/txt_reader_rect.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)     4796 2023-04-21 10:28:10.000000 image_augs-2.1.8/object_detection_new/utils_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-21 12:43:02.000000 image_augs-2.1.8/object_detection_new/yml_writer_poly.py
--rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-24 10:04:25.000000 image_augs-2.1.8/setup.cfg
--rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.1.8/setup.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8486 2023-04-25 07:32:26.000000 image_augs-2.2.9/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     7906 2023-04-25 07:14:06.000000 image_augs-2.2.9/README.md
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/classification/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:53.000000 image_augs-2.2.9/classification/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     9953 2023-03-29 13:10:42.000000 image_augs-2.2.9/classification/classification_.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    12643 2023-04-21 14:07:26.000000 image_augs-2.2.9/classification/classification_combined.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2006 2023-03-27 09:44:23.000000 image_augs-2.2.9/classification/logging_util.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     8486 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/PKG-INFO
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      723 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/SOURCES.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        1 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/dependency_links.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      241 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/requires.txt
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       49 2023-04-25 07:32:26.000000 image_augs-2.2.9/image_augs.egg-info/top_level.txt
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/instance_seg/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2023-03-29 09:58:39.000000 image_augs-2.2.9/instance_seg/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17394 2023-04-25 06:55:24.000000 image_augs-2.2.9/instance_seg/augment_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    23719 2023-04-25 07:05:20.000000 image_augs-2.2.9/instance_seg/json_reader_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-03-29 13:20:57.000000 image_augs-2.2.9/instance_seg/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4364 2023-04-10 10:20:24.000000 image_augs-2.2.9/instance_seg/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      513 2023-03-30 08:41:48.000000 image_augs-2.2.9/instance_seg/yml_writer_poly.py
+drwxrwxr-x   0 souviks   (1001) souviks   (1001)        0 2023-04-25 07:32:26.000000 image_augs-2.2.9/object_detection_new/
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)        0 2022-11-01 10:58:34.000000 image_augs-2.2.9/object_detection_new/__init__.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    17537 2023-04-25 07:25:05.000000 image_augs-2.2.9/object_detection_new/augmentation_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     2133 2023-04-23 18:52:17.000000 image_augs-2.2.9/object_detection_new/logging_util.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)    23341 2023-04-25 07:27:32.000000 image_augs-2.2.9/object_detection_new/txt_reader_rect.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)     4796 2023-04-21 10:28:10.000000 image_augs-2.2.9/object_detection_new/utils_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      510 2023-04-21 12:43:02.000000 image_augs-2.2.9/object_detection_new/yml_writer_poly.py
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)       38 2023-04-25 07:32:26.000000 image_augs-2.2.9/setup.cfg
+-rw-rw-r--   0 souviks   (1001) souviks   (1001)      998 2023-03-29 09:59:13.000000 image_augs-2.2.9/setup.py
```

### Comparing `image_augs-2.1.8/PKG-INFO` & `image_augs-2.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_augs
-Version: 2.1.8
+Version: 2.2.9
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -62,69 +62,71 @@
 # first combination --> for custom image size
 #  image_height = < custom image size > ; 640
 #  image_width = < custom image size > ; 320
 
 
 # second combination --> keep aspect ratio of the image
 #  image_height = 640
-#  image_width  = 'keep_aspect_ratio_true'
+#  image_width  = 'keep_aspect_ratio_False'
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 
-annotation_folder = 'your annotation folder'
-new_aug_saved_folder = 'any folder name'
-train_split = .90
+annotation_folder = 'Vehicle registration plate'
+new_aug_saved_folder = 'new_2'
+train_split = 1.0
 image_H = 640  #check above for height and width setting
 image_W = 'keep_aspect_ratio'
 
 
 rect_aug = RectAugmentation(new_aug_saved_folder)
 
 rect_aug.Image_augmentation(annotation_folder,
                                  
                                 train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=True,  blur_f=0.7,
+                                 blur=False,  blur_f=0.7,
 
-                                 rotate=True, rotate_f = 0.7, 
+                                 rotate=False, rotate_f = 0.7, 
 
-                                 noise=True, noise_f=0.8,
+                                 noise=False, noise_f=0.8,
 
-                                 perspective=True, perspective_f = 0.7,
+                                 perspective=False, perspective_f = 0.7,
 
-                                 affine=True, affine_f=0.7,
+                                 affine=False, affine_f=0.7,
 
-                                 brightness=True, brightness_f=0.7,
+                                 brightness=False, brightness_f=0.7,
                                     
-                                 hue=True, hue_f=0.7,
+                                 hue=False, hue_f=0.7,
 
-                                 removesaturation=True, removesaturation_f=0.8,
+                                 removesaturation=False, removesaturation_f=0.8,
 
-                                 contrast=True, contrast_f=0.5,
+                                 contrast=False, contrast_f=0.5,
 
                                  upflip=False, upflip_f=0.5,
 
-                                 shear=True , shear_f=0.7, 
+                                 shear=False , shear_f=0.7, 
 
-                                 rotate90=True, rotate90_f =0.6,
+                                 rotate90=False, rotate90_f =0.6,
 
-                                 blur_and_noise=True, blur_and_noise_f=0.7,
+                                 blur_and_noise=False, blur_and_noise_f=0.7,
 
-                                 image_cutout = True, image_cutout_f=0.8,
+                                 image_cutout = False, image_cutout_f=0.8,
                                     
-                                 mix_aug=True, mix_aug_f=0.4,
+                                 mix_aug=False, mix_aug_f=0.4, 
                                     
-                                 temperature_change=True, temperature_change_f=0.7), 
+                                 temperature_change=False, temperature_change_f=0.7,  # change color temperature from cool to warm color
+
+                                 weather_change=True,weather_change_f=0.3), # add rain , fog , snow in your images
                                 
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
@@ -197,15 +199,17 @@
 
                                  blur_and_noise=False, blur_and_noise_f=0.8,
 
                                  image_cutout = False, image_cutout_f=0.8,
                                     
                                  mix_aug=False, mix_aug_f=0.8,
                                     
-                                 temperature_change=False, temperature_change_f=0.8)
+                                 temperature_change=False, temperature_change_f=0.8,
+                                 
+                                 weather_change=True,weather_change_f=0.3)
 #results will be saved in < your given folder >
 ```
 
 **This Script is for IMAGE CLASSIFICATION**
 
 ```python
 #import these modules in your created <scriptname>.py file
```

### Comparing `image_augs-2.1.8/README.md` & `image_augs-2.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,69 +47,71 @@
 # first combination --> for custom image size
 #  image_height = < custom image size > ; 640
 #  image_width = < custom image size > ; 320
 
 
 # second combination --> keep aspect ratio of the image
 #  image_height = 640
-#  image_width  = 'keep_aspect_ratio_true'
+#  image_width  = 'keep_aspect_ratio_False'
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 
-annotation_folder = 'your annotation folder'
-new_aug_saved_folder = 'any folder name'
-train_split = .90
+annotation_folder = 'Vehicle registration plate'
+new_aug_saved_folder = 'new_2'
+train_split = 1.0
 image_H = 640  #check above for height and width setting
 image_W = 'keep_aspect_ratio'
 
 
 rect_aug = RectAugmentation(new_aug_saved_folder)
 
 rect_aug.Image_augmentation(annotation_folder,
                                  
                                 train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=True,  blur_f=0.7,
+                                 blur=False,  blur_f=0.7,
 
-                                 rotate=True, rotate_f = 0.7, 
+                                 rotate=False, rotate_f = 0.7, 
 
-                                 noise=True, noise_f=0.8,
+                                 noise=False, noise_f=0.8,
 
-                                 perspective=True, perspective_f = 0.7,
+                                 perspective=False, perspective_f = 0.7,
 
-                                 affine=True, affine_f=0.7,
+                                 affine=False, affine_f=0.7,
 
-                                 brightness=True, brightness_f=0.7,
+                                 brightness=False, brightness_f=0.7,
                                     
-                                 hue=True, hue_f=0.7,
+                                 hue=False, hue_f=0.7,
 
-                                 removesaturation=True, removesaturation_f=0.8,
+                                 removesaturation=False, removesaturation_f=0.8,
 
-                                 contrast=True, contrast_f=0.5,
+                                 contrast=False, contrast_f=0.5,
 
                                  upflip=False, upflip_f=0.5,
 
-                                 shear=True , shear_f=0.7, 
+                                 shear=False , shear_f=0.7, 
 
-                                 rotate90=True, rotate90_f =0.6,
+                                 rotate90=False, rotate90_f =0.6,
 
-                                 blur_and_noise=True, blur_and_noise_f=0.7,
+                                 blur_and_noise=False, blur_and_noise_f=0.7,
 
-                                 image_cutout = True, image_cutout_f=0.8,
+                                 image_cutout = False, image_cutout_f=0.8,
                                     
-                                 mix_aug=True, mix_aug_f=0.4,
+                                 mix_aug=False, mix_aug_f=0.4, 
                                     
-                                 temperature_change=True, temperature_change_f=0.7), 
+                                 temperature_change=False, temperature_change_f=0.7,  # change color temperature from cool to warm color
+
+                                 weather_change=True,weather_change_f=0.3), # add rain , fog , snow in your images
                                 
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
@@ -182,15 +184,17 @@
 
                                  blur_and_noise=False, blur_and_noise_f=0.8,
 
                                  image_cutout = False, image_cutout_f=0.8,
                                     
                                  mix_aug=False, mix_aug_f=0.8,
                                     
-                                 temperature_change=False, temperature_change_f=0.8)
+                                 temperature_change=False, temperature_change_f=0.8,
+                                 
+                                 weather_change=True,weather_change_f=0.3)
 #results will be saved in < your given folder >
 ```
 
 **This Script is for IMAGE CLASSIFICATION**
 
 ```python
 #import these modules in your created <scriptname>.py file
```

### Comparing `image_augs-2.1.8/classification/classification_.py` & `image_augs-2.2.9/classification/classification_.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/classification/classification_combined.py` & `image_augs-2.2.9/classification/classification_combined.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/classification/logging_util.py` & `image_augs-2.2.9/classification/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/image_augs.egg-info/PKG-INFO` & `image_augs-2.2.9/image_augs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-augs
-Version: 2.1.8
+Version: 2.2.9
 Summary: Image Augs supports Augmentation for Object Detection , Instance Segmentation and classification tasks.
 Author: Souvik Saha
 Author-email: ssouvik.191@gmail.com
 Keywords: machine_learning,development,data_augmentations
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -62,69 +62,71 @@
 # first combination --> for custom image size
 #  image_height = < custom image size > ; 640
 #  image_width = < custom image size > ; 320
 
 
 # second combination --> keep aspect ratio of the image
 #  image_height = 640
-#  image_width  = 'keep_aspect_ratio_true'
+#  image_width  = 'keep_aspect_ratio_False'
 
 # Third combination --> keeping original image height and width
 #  image_height = < keep_original_image_height >
 #  image_width = < keep_original_image_width >
 
 
 
-annotation_folder = 'your annotation folder'
-new_aug_saved_folder = 'any folder name'
-train_split = .90
+annotation_folder = 'Vehicle registration plate'
+new_aug_saved_folder = 'new_2'
+train_split = 1.0
 image_H = 640  #check above for height and width setting
 image_W = 'keep_aspect_ratio'
 
 
 rect_aug = RectAugmentation(new_aug_saved_folder)
 
 rect_aug.Image_augmentation(annotation_folder,
                                  
                                 train_split=train_split,
                                  image_height= image_H,
                                  image_width= image_W,
 
 
-                                 blur=True,  blur_f=0.7,
+                                 blur=False,  blur_f=0.7,
 
-                                 rotate=True, rotate_f = 0.7, 
+                                 rotate=False, rotate_f = 0.7, 
 
-                                 noise=True, noise_f=0.8,
+                                 noise=False, noise_f=0.8,
 
-                                 perspective=True, perspective_f = 0.7,
+                                 perspective=False, perspective_f = 0.7,
 
-                                 affine=True, affine_f=0.7,
+                                 affine=False, affine_f=0.7,
 
-                                 brightness=True, brightness_f=0.7,
+                                 brightness=False, brightness_f=0.7,
                                     
-                                 hue=True, hue_f=0.7,
+                                 hue=False, hue_f=0.7,
 
-                                 removesaturation=True, removesaturation_f=0.8,
+                                 removesaturation=False, removesaturation_f=0.8,
 
-                                 contrast=True, contrast_f=0.5,
+                                 contrast=False, contrast_f=0.5,
 
                                  upflip=False, upflip_f=0.5,
 
-                                 shear=True , shear_f=0.7, 
+                                 shear=False , shear_f=0.7, 
 
-                                 rotate90=True, rotate90_f =0.6,
+                                 rotate90=False, rotate90_f =0.6,
 
-                                 blur_and_noise=True, blur_and_noise_f=0.7,
+                                 blur_and_noise=False, blur_and_noise_f=0.7,
 
-                                 image_cutout = True, image_cutout_f=0.8,
+                                 image_cutout = False, image_cutout_f=0.8,
                                     
-                                 mix_aug=True, mix_aug_f=0.4,
+                                 mix_aug=False, mix_aug_f=0.4, 
                                     
-                                 temperature_change=True, temperature_change_f=0.7), 
+                                 temperature_change=False, temperature_change_f=0.7,  # change color temperature from cool to warm color
+
+                                 weather_change=True,weather_change_f=0.3), # add rain , fog , snow in your images
                                 
 
 #results will be saved in < your given folder >
 ```
 
 **This Script is for INSTANCE SEGMENTATION**
 
@@ -197,15 +199,17 @@
 
                                  blur_and_noise=False, blur_and_noise_f=0.8,
 
                                  image_cutout = False, image_cutout_f=0.8,
                                     
                                  mix_aug=False, mix_aug_f=0.8,
                                     
-                                 temperature_change=False, temperature_change_f=0.8)
+                                 temperature_change=False, temperature_change_f=0.8,
+                                 
+                                 weather_change=True,weather_change_f=0.3)
 #results will be saved in < your given folder >
 ```
 
 **This Script is for IMAGE CLASSIFICATION**
 
 ```python
 #import these modules in your created <scriptname>.py file
```

### Comparing `image_augs-2.1.8/image_augs.egg-info/SOURCES.txt` & `image_augs-2.2.9/image_augs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/instance_seg/augment_poly.py` & `image_augs-2.2.9/instance_seg/augment_poly.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,24 +221,24 @@
             new_points_polygons = new_points_polygons.polygons
             yield new_points_polygons , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image rotate90   desc : {e}')
             
 
     # beta mode
-    def image_weatherChange(self,image:np.array,polygons:Polygon,H,W,rain_speed:range=(0.1,0.3)) -> Tuple[Polygon,np.array]:
+    def image_weatherChange(self,image:np.array,polygons:Polygon,H,W,rain_speed:range=(0.09, 0.2)) -> Tuple[Polygon,np.array]:
         try:
             choice = random.choice([0,1,2])
             if choice == 0:
      
-                aug = iaa.Sequential([iaa.imgcorruptlike.Fog(severity=1),
+                aug = iaa.Sequential([iaa.imgcorruptlike.Fog(severity=2),
                                 iaa.Resize({"height": H, "width": W})])
             elif choice == 1:
          
-                aug = iaa.Sequential([iaa.Rain(speed=rain_speed),
+                aug = iaa.Sequential([iaa.Rain(speed=rain_speed,drop_size=(0.009,0.01)),
                                 iaa.Resize({"height": H, "width": W})])
             elif choice == 2:
                 # aug =  aug = iaa.imgcorruptlike.Snow(severity=1)        
                 aug = iaa.Sequential([iaa.imgcorruptlike.Snow(severity=1),
                                 iaa.Resize({"height": H, "width": W})])
 
             new_points_polygons, aug_affine_image = aug(polygons=polygons,image=image)
```

### Comparing `image_augs-2.1.8/instance_seg/json_reader_poly.py` & `image_augs-2.2.9/instance_seg/json_reader_poly.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         except Exception as e:
             logger.error(f'problem : Json converter  desc : {e}')       
                    
                   
     def Combined_augmentation(self,im_read , poly_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640, blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                               brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                               shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                              mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5):
+                              mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
         
         # combining all the augmentations here
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
             
             if blur:
            
@@ -251,22 +251,31 @@
             
             if temperature_change:
                 frac_data  = int(self.split * temperature_change_f)
                 if no_track <= frac_data:
                     points18  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
                     p , im = next(points18.result())
                     utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+
+            if weather_change:
+                frac_data  = int(self.split * weather_change_f)
+                if no_track <= frac_data:
+                    points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,poly_on_image,image_height,image_width) 
+                    p , im = next(points2.result())
+                    utils_poly.create_new_txt(im ,self.labels,p,self.train_images_path,self.train_labels_path,self.store_dict,yolo=self.yolo)
+
+                
              
   
                
     
     def Image_augmentation(self,folder,train_split=1.0,image_height:Union[int,keep_original_image_height]=640 , image_width:Union[int,keep_aspect_ratio,keep_original_image_width]=640,blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                             brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                             shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5):
+                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
         #checking if input folder is a directory or not
         dir_checker = os.path.isdir(folder)
         
         if dir_checker != True:
             shutil.rmtree(self.aug_save_folder_name)
             raise NotADirectoryError(f'Provided Path - {folder} is not a directory...')
@@ -308,15 +317,16 @@
                 'rotation90_f':rotate90_f,
                 'affine_f':affine_f,
                 'perspective_f':perspective_f,
                 'upflip_f' : upflip_f,
                 'shear_f' : shear_f,
                 'image_cut_f':image_cutout_f,
                 'mix_aug_f' : mix_aug_f,
-                'temperaure_change_f' : temperature_change_f
+                'temperaure_change_f' : temperature_change_f,
+                'weather_change_f' : weather_change_f
                 
               }
         
         type_2 = { 
                 'blur':blur,
                 'noise':noise,
                 'NB':blur_and_noise,
@@ -328,15 +338,16 @@
                 'rotation90':rotate90,
                 'affine':affine,
                 'perspective':perspective,
                 'upflip' : upflip,
                 'shear' : shear,
                 'image_cut':image_cutout,
                 'mix_aug' : mix_aug,
-                'temp_change' : temperature_change
+                'temp_change' : temperature_change,
+                'weather_change' : weather_change
                 
               }
 
         # checking the types 
         for types , val in type_1.items():
             if type(val) != float:
                 raise TypeError(f' [-] please provide "{types}" as  "float" , You provided "{types}" as {type(val)}')
@@ -391,15 +402,15 @@
                 #if we want to keep original image height and width -->
                 if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
                     image_height_N , image_width_N , _ = poly[0][0].shape
 
                 self.Combined_augmentation(poly[0][0],poly[0][1],c+1,image_height_N,image_width_N,blur=blur , blur_f = blur_f , rotate=rotate , rotate_f = rotate_f , noise=noise,noise_f=noise_f,perspective=perspective,perspective_f = perspective_f,affine=affine,affine_f=affine_f,
                               brightness=brightness,brightness_f=brightness_f,hue=hue,hue_f=hue_f,removesaturation=removesaturation,removesaturation_f=removesaturation_f,contrast=contrast,contrast_f=contrast_f,upflip=upflip,upflip_f=upflip_f,
                               shear= shear ,shear_f=shear_f, rotate90=rotate90,rotate90_f = rotate90_f,blur_and_noise=blur_and_noise,blur_and_noise_f=blur_and_noise_f,image_cutout = image_cutout,image_cutout_f=image_cutout_f,
-                              mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f)
+                              mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f,weather_change=weather_change,weather_change_f=weather_change_f)
                 
                 
                 
             elif c+1 > self.split:
                 # print(images)
                 
                 poly = list(self.json_converter(f'{images}'))
```

### Comparing `image_augs-2.1.8/instance_seg/logging_util.py` & `image_augs-2.2.9/instance_seg/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/instance_seg/utils_poly.py` & `image_augs-2.2.9/instance_seg/utils_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/instance_seg/yml_writer_poly.py` & `image_augs-2.2.9/instance_seg/yml_writer_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/object_detection_new/augmentation_rect.py` & `image_augs-2.2.9/object_detection_new/augmentation_rect.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 from imgaug.augmentables.bbs import BoundingBox, BoundingBoxesOnImage
 
 import os
 import warnings
 import random
 from typing import Tuple
+import secrets
 
 import instance_seg.logging_util as logging_util
 
 warnings.filterwarnings('ignore')
 
 
 
@@ -226,24 +227,25 @@
                 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
             new_points_bbox = new_points_bbox.bounding_boxes
             yield new_points_bbox , aug_affine_image
         except Exception as e:
             logger.warning(f'problem: Image rotate90   desc : {e}')
     #beta
-    def image_weatherChange(self,image:np.array,bbox:BoundingBox,H,W,rain_speed:range=(0.1,0.3)) -> Tuple[BoundingBoxesOnImage,np.array]:
+    def image_weatherChange(self,image:np.array,bbox:BoundingBox,H,W,rain_speed:range=((0.09, 0.2))) -> Tuple[BoundingBoxesOnImage,np.array]:
         try:
-            choice = random.choice([0,1,2])
+            choice = secrets.choice([0,1,2])
+        
             if choice == 0:
      
-                aug = iaa.Sequential([iaa.imgcorruptlike.Fog(severity=1),
+                aug = iaa.Sequential([iaa.imgcorruptlike.Fog(severity=2),
                                 iaa.Resize({"height": H, "width": W})])
             elif choice == 1:
          
-                aug = iaa.Sequential([iaa.Rain(speed=rain_speed),
+                aug = iaa.Sequential([iaa.Rain(speed=rain_speed,drop_size=(0.009,0.01),),
                                 iaa.Resize({"height": H, "width": W})])
             elif choice == 2:
                 # aug =  aug = iaa.imgcorruptlike.Snow(severity=1)        
                 aug = iaa.Sequential([iaa.imgcorruptlike.Snow(severity=1),
                                 iaa.Resize({"height": H, "width": W})])
 
             aug_affine_image, new_points_bbox = aug(image=image,bounding_boxes=bbox)
```

### Comparing `image_augs-2.1.8/object_detection_new/logging_util.py` & `image_augs-2.2.9/object_detection_new/logging_util.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/object_detection_new/txt_reader_rect.py` & `image_augs-2.2.9/object_detection_new/txt_reader_rect.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         except Exception as e:
             logger.error(f'problem : Json converter  desc : {e}')
 
 
     def Combined_augmentation(self,im_read , rect_on_image, no_track,image_height=640 , image_width:Union[int,keep_aspect_ratio]=640,blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                             brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                             shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5):
+                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
             if rotate:
                 frac_data  = int(self.split * rotate_f)
                 if no_track <= frac_data:
             
                     points2  = executor.submit(self.augment.image_rotate,im_read,rect_on_image,image_height,image_width) 
@@ -266,27 +266,35 @@
             if temperature_change:
                 frac_data  = int(self.split * temperature_change_f)
                 if no_track <= frac_data:
             
                     points2  = executor.submit(self.augment.image_change_colorTemperature,im_read,rect_on_image,image_height,image_width) 
                     p , im = next(points2.result())
                     utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
+            if weather_change:
+                frac_data  = int(self.split * weather_change_f)
+                if no_track <= frac_data:
+                    points20  = executor.submit(self.augment.image_weatherChange,im_read,rect_on_image,image_height,image_width) 
+                    p , im = next(points20.result())
+                    utils_poly.create_new_txt(im,p,self.train_images_path,self.train_labels_path)
+
         
             
 
 
             
 
 
 
     
     def Image_augmentation(self,folder,train_split=1.0,image_height:Union[int,keep_original_image_height]=640 , image_width:Union[int,keep_aspect_ratio,keep_original_image_width]=640,blur=True , blur_f = 0.5 , rotate=True , rotate_f = 0.5 , noise=True,noise_f=0.5,perspective=True,perspective_f = 0.5,affine=True,affine_f=0.5,
                             brightness=True,brightness_f=0.5,hue=True,hue_f=0.5,removesaturation=True,removesaturation_f=0.5,contrast=True,contrast_f=0.5,upflip=True,upflip_f=0.5,
                             shear=True ,shear_f=0.5, rotate90=True,rotate90_f = 0.5,blur_and_noise=True,blur_and_noise_f=0.5,image_cutout = True,image_cutout_f=0.5,
-                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5):
+                            mix_aug=True,mix_aug_f=0.5,temperature_change=True,temperature_change_f=0.5,weather_change=True,weather_change_f=0.5):
         
         #checking if input folder is a directory or not
         dir_checker = os.path.isdir(folder)
         
         if dir_checker != True:
             shutil.rmtree(self.aug_save_folder_name)
             raise NotADirectoryError(f'Provided Path - {folder} is not a directory...')
@@ -308,27 +316,29 @@
                     self.store_dict[index] = classes_name.rstrip()
                     
                 console.print('[bold green] classes.txt found.. [bold green]')
         else:
             raise NotImplementedError('Classes.txt not Found !!')
         
         # checking json and images are same or not and checking their len too
-        if len(all_images) +1 == len(all_txt) and len(all_images) +1 >= 1 and len(all_txt) >=1:
-            del all_txt
-            
-        else:
+        if classes_ != []:
+            if len(all_images)  == len(all_txt) -1 and len(all_images)  >= 1 and len(all_txt) -1 >=1:
+                del all_txt
             
-            raise NotImplementedError(f'Images and Jsons are not equal , recheck your annotation folder! \
-                                       Total Images : {len(all_images)}  |  Total txt : {len(all_txt)}')
+            else:
+                shutil.rmtree(self.aug_save_folder_name)
+                raise NotImplementedError(f'Images and Txt are not equal , recheck your annotation folder! Total Images : {len(all_images)}  |  Total txt : {len(all_txt)-1}')
         # checking train is float or not
         if type(train_split) != float:
+            shutil.rmtree(self.aug_save_folder_name)
             raise TypeError(f'please provide "train split" as "float" , You provided train split as {type(train_split)}')
             
         # checking train split value > 1.0 or not   
         if train_split > 1.0:
+            shutil.rmtree(self.aug_save_folder_name)
             raise ValueError(f'[-] please provide "train split" between "0.5 to 1.0", Your provided train split value is : {train_split}')
 
 
         #checking the types here    
         type_1 = { 
                 'blur_f':blur_f,
                 'noise_f':noise_f,
@@ -341,15 +351,16 @@
                 'rotation90_f':rotate90_f,
                 'affine_f':affine_f,
                 'perspective_f':perspective_f,
                 'upflip_f' : upflip_f,
                 'shear_f' : shear_f,
                 'image_cut_f':image_cutout_f,
                 'mix_aug_f' : mix_aug_f,
-                'temperaure_change_f' : temperature_change_f
+                'temperaure_change_f' : temperature_change_f,
+                'weather_change_f' : weather_change_f
                 
               }
         
         type_2 = { 
                 'blur':blur,
                 'noise':noise,
                 'NB':blur_and_noise,
@@ -361,38 +372,43 @@
                 'rotation90':rotate90,
                 'affine':affine,
                 'perspective':perspective,
                 'upflip' : upflip,
                 'shear' : shear,
                 'image_cut':image_cutout,
                 'mix_aug' : mix_aug,
-                'temp_change' : temperature_change
+                'temp_change' : temperature_change,
+                'weather_change' : weather_change
                 
               }
 
         # checking the types 
         for types , val in type_1.items():
             if type(val) != float:
+                shutil.rmtree(self.aug_save_folder_name)
                 raise TypeError(f' [-] please provide "{types}" as  "float" , You provided "{types}" as {type(val)}')
              
                 
             if val > 1.0:
+                shutil.rmtree(self.aug_save_folder_name)
                 raise ValueError(f'[-] please provide "{types}" value  between "0.1 to 1.0" , Your provided "{types}" value is : "{val}"')
         
         for typess , vals in type_2.items():
 
             if type(vals) != bool:
+                shutil.rmtree(self.aug_save_folder_name)
                 raise TypeError(f'Please provide "{typess}" as bool , you provided "{typess}" as "{vals}"')
         
 
        
         if (type(image_height) , image_width) == (int,'keep_aspect_ratio') or (type(image_height),type(image_width)) == (int,int) or (image_height , image_width) == ('keep_original_image_height','keep_original_image_width'):
             pass
 
         else:
+            shutil.rmtree(self.aug_save_folder_name)
             raise ValueError('You provided a wrong image height and width combination, right combinations are - \n (image height , image width) = (int ,int) \n (image height , image width) = (int , "keep_aspect_ratio") \n (image height , image width) = ("keep_original_image_height","keep_original_image_width") ')
         
         if image_width == 'keep_aspect_ratio' and type(image_height) == int :
             image_width_N = 'keep-aspect-ratio'
             image_height_N = image_height
         
 
@@ -414,39 +430,43 @@
         if train_split == 1.0:
                     shutil.rmtree(f'{self.aug_save_folder_name}/test')
         
         # if c value less than equal to train split then we will add those images in training data and rest will go for test data            
         for c ,images in enumerate(track(all_images,description='Image Augmentation..',total=len(all_images[:self.split]))):
 
             if c+1 <= self.split:
+
+                
               
                 poly = list(self.txt_converter(images))
           
                 #if we want to keep original image height and width -->
                 if image_height == 'keep_original_image_height' and image_width == 'keep_original_image_width':
-                    image_height_N , image_width_N , _ = poly[0][0].shape
+                    image_height_N , image_width_N , channel = poly[0][0].shape
                 
                 # print(poly)
 
                 self.Combined_augmentation(poly[0][0],poly[0][1],c+1,image_height_N,image_width_N,blur=blur , blur_f = blur_f , rotate=rotate , rotate_f = rotate_f , noise=noise,noise_f=noise_f,perspective=perspective,perspective_f = perspective_f,affine=affine,affine_f=affine_f,
                               brightness=brightness,brightness_f=brightness_f,hue=hue,hue_f=hue_f,removesaturation=removesaturation,removesaturation_f=removesaturation_f,contrast=contrast,contrast_f=contrast_f,upflip=upflip,upflip_f=upflip_f,
                               shear= shear ,shear_f=shear_f, rotate90=rotate90,rotate90_f = rotate90_f,blur_and_noise=blur_and_noise,blur_and_noise_f=blur_and_noise_f,image_cutout = image_cutout,image_cutout_f=image_cutout_f,
-                              mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f)
+                              mix_aug=mix_aug,mix_aug_f=mix_aug_f,temperature_change=temperature_change,temperature_change_f=temperature_change_f,weather_change=weather_change,weather_change_f=weather_change_f)
                 
                 
                 
             elif c+1 > self.split:
                 # print(images)
                 
                 poly = list(self.txt_converter(f'{images}'))
 
                 utils_poly.create_new_txt(poly[0][0] ,poly[0][1],self.test_images_path,self.test_labels_path)
                    
         console.print(f'[bold dim cyan] Labels name : [/bold dim cyan] [bold magenta] {list(self.store_dict.values())} [bold magenta]')
-        yml_writer_poly.yaml_writer(len(self.store_dict.keys()),list(self.store_dict.values()),self.aug_save_folder_name)      
+
+        yml_writer_poly.yaml_writer(len(self.store_dict.keys()),list(self.store_dict.values()),self.aug_save_folder_name)   
+
         with open(f'{self.aug_save_folder_name}/classes.txt','w') as f:
             f.write('\n'.join(list(self.store_dict.values()))) 
       
       
       
     @staticmethod
     def image_format_change(folder):
```

### Comparing `image_augs-2.1.8/object_detection_new/utils_poly.py` & `image_augs-2.2.9/object_detection_new/utils_poly.py`

 * *Files identical despite different names*

### Comparing `image_augs-2.1.8/setup.py` & `image_augs-2.2.9/setup.py`

 * *Files identical despite different names*

