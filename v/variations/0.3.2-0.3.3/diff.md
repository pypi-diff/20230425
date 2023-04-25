# Comparing `tmp/variations-0.3.2.tar.gz` & `tmp/variations-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variations-0.3.2.tar", last modified: Tue Oct 25 12:34:11 2022, max compression
+gzip compressed data, was "variations-0.3.3.tar", last modified: Tue Apr 25 07:36:56 2023, max compression
```

## Comparing `variations-0.3.2.tar` & `variations-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:34:11.577998 variations-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-10-25 12:33:51.000000 variations-0.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-10-25 12:33:51.000000 variations-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-10-25 12:33:51.000000 variations-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-25 12:33:51.000000 variations-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-10-25 12:34:11.577998 variations-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-10-25 12:33:51.000000 variations-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-10-25 12:34:11.581998 variations-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-25 12:33:51.000000 variations-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:34:11.577998 variations-0.3.2/variations/
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-10-25 12:33:51.000000 variations-0.3.2/variations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-25 12:33:51.000000 variations-0.3.2/variations/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:34:11.577998 variations-0.3.2/variations/processors/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-10-25 12:33:51.000000 variations-0.3.2/variations/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-10-25 12:33:51.000000 variations-0.3.2/variations/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-25 12:33:51.000000 variations-0.3.2/variations/processors/crop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-25 12:33:51.000000 variations-0.3.2/variations/processors/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-10-25 12:33:51.000000 variations-0.3.2/variations/processors/overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-10-25 12:33:51.000000 variations-0.3.2/variations/processors/resize.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-10-25 12:33:51.000000 variations-0.3.2/variations/scaler.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-10-25 12:33:51.000000 variations-0.3.2/variations/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-10-25 12:33:51.000000 variations-0.3.2/variations/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11764 2022-10-25 12:33:51.000000 variations-0.3.2/variations/variation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 12:34:11.577998 variations-0.3.2/variations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-10-25 12:34:11.000000 variations-0.3.2/variations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-10-25 12:34:11.000000 variations-0.3.2/variations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 12:34:11.000000 variations-0.3.2/variations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 12:34:11.000000 variations-0.3.2/variations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-25 12:34:11.000000 variations-0.3.2/variations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-25 12:34:11.000000 variations-0.3.2/variations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:36:56.562098 variations-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-25 07:36:39.000000 variations-0.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 07:36:39.000000 variations-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-25 07:36:39.000000 variations-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 07:36:39.000000 variations-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-25 07:36:56.562098 variations-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-25 07:36:39.000000 variations-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-25 07:36:56.562098 variations-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 07:36:39.000000 variations-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:36:56.558098 variations-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-04-25 07:36:39.000000 variations-0.3.3/tests/test_variation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:36:56.558098 variations-0.3.3/variations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-25 07:36:39.000000 variations-0.3.3/variations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-25 07:36:39.000000 variations-0.3.3/variations/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:36:56.562098 variations-0.3.3/variations/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 07:36:39.000000 variations-0.3.3/variations/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-25 07:36:39.000000 variations-0.3.3/variations/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 07:36:39.000000 variations-0.3.3/variations/processors/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-25 07:36:39.000000 variations-0.3.3/variations/processors/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-25 07:36:39.000000 variations-0.3.3/variations/processors/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-25 07:36:39.000000 variations-0.3.3/variations/processors/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-25 07:36:39.000000 variations-0.3.3/variations/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 07:36:39.000000 variations-0.3.3/variations/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-25 07:36:39.000000 variations-0.3.3/variations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-04-25 07:36:39.000000 variations-0.3.3/variations/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:36:56.562098 variations-0.3.3/variations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-25 07:36:56.000000 variations-0.3.3/variations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-25 07:36:56.000000 variations-0.3.3/variations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:36:56.000000 variations-0.3.3/variations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:36:56.000000 variations-0.3.3/variations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 07:36:56.000000 variations-0.3.3/variations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 07:36:56.000000 variations-0.3.3/variations.egg-info/top_level.txt
```

### Comparing `variations-0.3.2/CHANGELOG.md` & `variations-0.3.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## [0.3.3](https://github.com/dldevinc/variations/tree/v0.3.3) - 2024-04-25
+
+### Features
+
+-   Add support for Python 3.11.
+
 ## [0.3.2](https://github.com/dldevinc/variations/tree/v0.3.2) - 2022-10-25
 
 ### Features
 
 -   `Scaler` class now supports `float` values for image dimensions.
 
 ## [0.3.1](https://github.com/dldevinc/variations/tree/v0.3.1) - 2022-01-31
```

### Comparing `variations-0.3.2/CONTRIBUTING.md` & `variations-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/LICENSE` & `variations-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/PKG-INFO` & `variations-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variations
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple interface that allows processing of images.
 Home-page: https://github.com/dldevinc/variations
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: facedetection
 Provides-Extra: stackblur
 Provides-Extra: full
 License-File: LICENSE
```

### Comparing `variations-0.3.2/README.md` & `variations-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/setup.cfg` & `variations-0.3.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [bdist_wheel]
 universal = 1
 
 [options]
 zip_safe = false
@@ -40,14 +41,19 @@
 [options.extras_require]
 facedetection = face_recognition
 stackblur = pillow-stackblur
 full = 
 	face_recognition
 	pillow-stackblur
 
+[options.packages.find]
+exclude = 
+	tests
+	tests.*
+
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 90
 known_first_party = app
```

### Comparing `variations-0.3.2/variations/__init__.py` & `variations-0.3.3/variations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,8 @@
         description     Дополнительные опции. Опции с именами, совпадающими с
                         названиями формата (jpeg / png / webp / ...) передаются
                         в метод Image.save().
 
     * P.S. "основным действием вариации" является ресайз и/или кадрирование,
     в зависимости от параметров size, crop, upscale и размера исходного изображения.
 """
-__version__ = "0.3.2"
+__version__ = "0.3.3"
```

### Comparing `variations-0.3.2/variations/processors/base.py` & `variations-0.3.3/variations/processors/base.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations/processors/filters.py` & `variations-0.3.3/variations/processors/filters.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations/processors/overlay.py` & `variations-0.3.3/variations/processors/overlay.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations/processors/resize.py` & `variations-0.3.3/variations/processors/resize.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations/scaler.py` & `variations-0.3.3/variations/scaler.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations/utils.py` & `variations-0.3.3/variations/utils.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations/variation.py` & `variations-0.3.3/variations/variation.py`

 * *Files identical despite different names*

### Comparing `variations-0.3.2/variations.egg-info/PKG-INFO` & `variations-0.3.3/variations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variations
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple interface that allows processing of images.
 Home-page: https://github.com/dldevinc/variations
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: facedetection
 Provides-Extra: stackblur
 Provides-Extra: full
 License-File: LICENSE
```

