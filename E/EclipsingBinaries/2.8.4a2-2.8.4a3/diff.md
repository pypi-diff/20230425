# Comparing `tmp/EclipsingBinaries-2.8.4a2.tar.gz` & `tmp/EclipsingBinaries-2.8.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.4a2.tar", last modified: Thu Apr 20 19:20:35 2023, max compression
+gzip compressed data, was "EclipsingBinaries-2.8.4a3.tar", last modified: Mon Apr 24 22:07:21 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.4a2.tar` & `EclipsingBinaries-2.8.4a3.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.089782 EclipsingBinaries-2.8.4a2/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/color_light_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/tesscut.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.089782 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-20 19:20:16.000000 EclipsingBinaries-2.8.4a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-20 19:20:16.000000 EclipsingBinaries-2.8.4a2/tests/test_OC_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-04-24 22:07:00.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-24 22:07:21.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-24 22:07:21.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:07:21.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-24 22:07:21.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 22:07:21.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 22:07:21.000000 EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:07:21.075945 EclipsingBinaries-2.8.4a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-24 22:07:05.000000 EclipsingBinaries-2.8.4a3/setup.py
```

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/apass.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/find_min.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/gaia.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/menu.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a2
+Version: 2.8.4a3
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -16,8 +16,12 @@
 EclipsingBinaries/vseq_updated.py
 EclipsingBinaries.egg-info/PKG-INFO
 EclipsingBinaries.egg-info/SOURCES.txt
 EclipsingBinaries.egg-info/dependency_links.txt
 EclipsingBinaries.egg-info/entry_points.txt
 EclipsingBinaries.egg-info/requires.txt
 EclipsingBinaries.egg-info/top_level.txt
-tests/test_OC_plot.py
+EclipsingBinaries/examples/test_B.txt
+EclipsingBinaries/examples/test_R.txt
+EclipsingBinaries/examples/test_V.txt
+EclipsingBinaries/tests/__init__.py
+EclipsingBinaries/tests/test_OC_plot.py
```

### Comparing `EclipsingBinaries-2.8.4a2/LICENSE` & `EclipsingBinaries-2.8.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/PKG-INFO` & `EclipsingBinaries-2.8.4a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a2
+Version: 2.8.4a3
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a2/README.md` & `EclipsingBinaries-2.8.4a3/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a2/setup.py` & `EclipsingBinaries-2.8.4a3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,12 +87,10 @@
         ],
     },
 
     include_package_data=True,
     packages=['EclipsingBinaries'],
     package_dir={'EclipsingBinaries': 'EclipsingBinaries'},
     package_data={
-        'EclipsingBinaries': ['tests/*'],
-        'EclipsingBinaries': ['examples/*'],
+        'EclipsingBinaries': ['tests/*', 'examples/*']
     },
-
 )
```

### Comparing `EclipsingBinaries-2.8.4a2/tests/test_OC_plot.py` & `EclipsingBinaries-2.8.4a3/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

