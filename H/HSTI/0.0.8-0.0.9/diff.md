# Comparing `tmp/HSTI-0.0.8.tar.gz` & `tmp/HSTI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HSTI-0.0.8.tar", last modified: Mon Dec 20 10:35:03 2021, max compression
+gzip compressed data, was "HSTI-0.0.9.tar", last modified: Mon Dec 20 10:38:29 2021, max compression
```

## Comparing `HSTI-0.0.8.tar` & `HSTI-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:35:03.421036 HSTI-0.0.8/
--rw-rw-r--   0 alj       (1000) alj       (1000)       24 2021-12-03 11:49:16.000000 HSTI-0.0.8/.gitignore
--rw-rw-r--   0 alj       (1000) alj       (1000)     1023 2021-12-01 09:17:53.000000 HSTI-0.0.8/LICENSE
--rw-rw-r--   0 alj       (1000) alj       (1000)     3488 2021-12-20 10:35:03.421036 HSTI-0.0.8/PKG-INFO
--rw-rw-r--   0 alj       (1000) alj       (1000)     2971 2021-12-20 09:55:55.000000 HSTI-0.0.8/README.md
-drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:35:03.389039 HSTI-0.0.8/hsti-analysis/
-drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:35:03.393039 HSTI-0.0.8/hsti-analysis/HSTI/
--rw-rw-r--   0 alj       (1000) alj       (1000)      748 2021-12-20 10:03:30.000000 HSTI-0.0.8/hsti-analysis/HSTI/__init__.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     1455 2021-12-20 09:42:45.000000 HSTI-0.0.8/hsti-analysis/HSTI/animate_data_cube.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     2129 2021-12-20 09:42:45.000000 HSTI-0.0.8/hsti-analysis/HSTI/basic_math.py
-drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:35:03.393039 HSTI-0.0.8/hsti-analysis/HSTI/data_files/
--rw-rw-r--   0 alj       (1000) alj       (1000) 19660800 2021-12-01 09:13:06.000000 HSTI-0.0.8/hsti-analysis/HSTI/data_files/vignetting_profile.txt
--rw-rw-r--   0 alj       (1000) alj       (1000)     3173 2021-12-01 11:42:37.000000 HSTI-0.0.8/hsti-analysis/HSTI/fill_gaps.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     2389 2021-12-02 13:38:10.000000 HSTI-0.0.8/hsti-analysis/HSTI/fpi_sim.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     4780 2021-12-14 10:48:18.000000 HSTI-0.0.8/hsti-analysis/HSTI/fpi_sim_matrix.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     7138 2021-12-14 10:48:18.000000 HSTI-0.0.8/hsti-analysis/HSTI/fpi_sim_matrix_angular.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     1325 2021-12-13 13:26:42.000000 HSTI-0.0.8/hsti-analysis/HSTI/hsti_export.py
--rw-rw-r--   0 alj       (1000) alj       (1000)      784 2021-12-17 10:38:53.000000 HSTI-0.0.8/hsti-analysis/HSTI/hsti_import.py
--rw-rw-r--   0 alj       (1000) alj       (1000)      314 2021-12-20 10:34:22.000000 HSTI-0.0.8/hsti-analysis/HSTI/import_mirror_sep.py
--rw-rw-r--   0 alj       (1000) alj       (1000)      199 2021-12-01 13:23:09.000000 HSTI-0.0.8/hsti-analysis/HSTI/mse.py
--rwxrwxr-x   0 alj       (1000) alj       (1000)    19977 2021-12-01 12:53:19.000000 HSTI-0.0.8/hsti-analysis/HSTI/remove_bad_px.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     1022 2021-12-01 10:09:54.000000 HSTI-0.0.8/hsti-analysis/HSTI/remove_vignetting.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     2307 2021-12-13 13:26:42.000000 HSTI-0.0.8/hsti-analysis/HSTI/spectral_debending.py
--rw-rw-r--   0 alj       (1000) alj       (1000)     3133 2021-12-01 11:42:53.000000 HSTI-0.0.8/hsti-analysis/HSTI/voronoi_partitioning.py
-drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:35:03.393039 HSTI-0.0.8/hsti-analysis/HSTI.egg-info/
--rw-rw-r--   0 alj       (1000) alj       (1000)     3488 2021-12-20 10:35:03.000000 HSTI-0.0.8/hsti-analysis/HSTI.egg-info/PKG-INFO
--rw-rw-r--   0 alj       (1000) alj       (1000)      815 2021-12-20 10:35:03.000000 HSTI-0.0.8/hsti-analysis/HSTI.egg-info/SOURCES.txt
--rw-rw-r--   0 alj       (1000) alj       (1000)        1 2021-12-20 10:35:03.000000 HSTI-0.0.8/hsti-analysis/HSTI.egg-info/dependency_links.txt
--rw-rw-r--   0 alj       (1000) alj       (1000)        5 2021-12-20 10:35:03.000000 HSTI-0.0.8/hsti-analysis/HSTI.egg-info/top_level.txt
--rw-rw-r--   0 alj       (1000) alj       (1000)      104 2021-12-01 09:54:01.000000 HSTI-0.0.8/pyproject.toml
--rw-rw-r--   0 alj       (1000) alj       (1000)       38 2021-12-20 10:35:03.421036 HSTI-0.0.8/setup.cfg
--rw-rw-r--   0 alj       (1000) alj       (1000)      831 2021-12-20 10:34:41.000000 HSTI-0.0.8/setup.py
+drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:38:29.018051 HSTI-0.0.9/
+-rw-rw-r--   0 alj       (1000) alj       (1000)       24 2021-12-03 11:49:16.000000 HSTI-0.0.9/.gitignore
+-rw-rw-r--   0 alj       (1000) alj       (1000)     1023 2021-12-01 09:17:53.000000 HSTI-0.0.9/LICENSE
+-rw-rw-r--   0 alj       (1000) alj       (1000)     3488 2021-12-20 10:38:29.018051 HSTI-0.0.9/PKG-INFO
+-rw-rw-r--   0 alj       (1000) alj       (1000)     2971 2021-12-20 09:55:55.000000 HSTI-0.0.9/README.md
+drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:38:28.982051 HSTI-0.0.9/hsti-analysis/
+drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:38:28.986051 HSTI-0.0.9/hsti-analysis/HSTI/
+-rw-rw-r--   0 alj       (1000) alj       (1000)      748 2021-12-20 10:03:30.000000 HSTI-0.0.9/hsti-analysis/HSTI/__init__.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     1455 2021-12-20 09:42:45.000000 HSTI-0.0.9/hsti-analysis/HSTI/animate_data_cube.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     2129 2021-12-20 09:42:45.000000 HSTI-0.0.9/hsti-analysis/HSTI/basic_math.py
+drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:38:28.986051 HSTI-0.0.9/hsti-analysis/HSTI/data_files/
+-rw-rw-r--   0 alj       (1000) alj       (1000) 19660800 2021-12-01 09:13:06.000000 HSTI-0.0.9/hsti-analysis/HSTI/data_files/vignetting_profile.txt
+-rw-rw-r--   0 alj       (1000) alj       (1000)     3173 2021-12-01 11:42:37.000000 HSTI-0.0.9/hsti-analysis/HSTI/fill_gaps.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     2389 2021-12-02 13:38:10.000000 HSTI-0.0.9/hsti-analysis/HSTI/fpi_sim.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     4780 2021-12-14 10:48:18.000000 HSTI-0.0.9/hsti-analysis/HSTI/fpi_sim_matrix.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     7138 2021-12-14 10:48:18.000000 HSTI-0.0.9/hsti-analysis/HSTI/fpi_sim_matrix_angular.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     1325 2021-12-13 13:26:42.000000 HSTI-0.0.9/hsti-analysis/HSTI/hsti_export.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)      784 2021-12-17 10:38:53.000000 HSTI-0.0.9/hsti-analysis/HSTI/hsti_import.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)      313 2021-12-20 10:37:00.000000 HSTI-0.0.9/hsti-analysis/HSTI/import_mirror_sep.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)      199 2021-12-01 13:23:09.000000 HSTI-0.0.9/hsti-analysis/HSTI/mse.py
+-rwxrwxr-x   0 alj       (1000) alj       (1000)    19977 2021-12-01 12:53:19.000000 HSTI-0.0.9/hsti-analysis/HSTI/remove_bad_px.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     1022 2021-12-01 10:09:54.000000 HSTI-0.0.9/hsti-analysis/HSTI/remove_vignetting.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     2307 2021-12-13 13:26:42.000000 HSTI-0.0.9/hsti-analysis/HSTI/spectral_debending.py
+-rw-rw-r--   0 alj       (1000) alj       (1000)     3133 2021-12-01 11:42:53.000000 HSTI-0.0.9/hsti-analysis/HSTI/voronoi_partitioning.py
+drwxrwxr-x   0 alj       (1000) alj       (1000)        0 2021-12-20 10:38:28.986051 HSTI-0.0.9/hsti-analysis/HSTI.egg-info/
+-rw-rw-r--   0 alj       (1000) alj       (1000)     3488 2021-12-20 10:38:28.000000 HSTI-0.0.9/hsti-analysis/HSTI.egg-info/PKG-INFO
+-rw-rw-r--   0 alj       (1000) alj       (1000)      815 2021-12-20 10:38:28.000000 HSTI-0.0.9/hsti-analysis/HSTI.egg-info/SOURCES.txt
+-rw-rw-r--   0 alj       (1000) alj       (1000)        1 2021-12-20 10:38:28.000000 HSTI-0.0.9/hsti-analysis/HSTI.egg-info/dependency_links.txt
+-rw-rw-r--   0 alj       (1000) alj       (1000)        5 2021-12-20 10:38:28.000000 HSTI-0.0.9/hsti-analysis/HSTI.egg-info/top_level.txt
+-rw-rw-r--   0 alj       (1000) alj       (1000)      104 2021-12-01 09:54:01.000000 HSTI-0.0.9/pyproject.toml
+-rw-rw-r--   0 alj       (1000) alj       (1000)       38 2021-12-20 10:38:29.018051 HSTI-0.0.9/setup.cfg
+-rw-rw-r--   0 alj       (1000) alj       (1000)      831 2021-12-20 10:38:19.000000 HSTI-0.0.9/setup.py
```

### Comparing `HSTI-0.0.8/LICENSE` & `HSTI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/PKG-INFO` & `HSTI-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSTI
-Version: 0.0.8
+Version: 0.0.9
 Summary: The NEWTEC HSTI package contains fundamental functions for the data analysis of hyperspectral thermal images (HSTI).
 Home-page: UNKNOWN
 Author: Mads Nibe et. al.
 Author-email: mani@newtec.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `HSTI-0.0.8/README.md` & `HSTI-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/__init__.py` & `HSTI-0.0.9/hsti-analysis/HSTI/__init__.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/animate_data_cube.py` & `HSTI-0.0.9/hsti-analysis/HSTI/animate_data_cube.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/basic_math.py` & `HSTI-0.0.9/hsti-analysis/HSTI/basic_math.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/data_files/vignetting_profile.txt` & `HSTI-0.0.9/hsti-analysis/HSTI/data_files/vignetting_profile.txt`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/fill_gaps.py` & `HSTI-0.0.9/hsti-analysis/HSTI/fill_gaps.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/fpi_sim.py` & `HSTI-0.0.9/hsti-analysis/HSTI/fpi_sim.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/fpi_sim_matrix.py` & `HSTI-0.0.9/hsti-analysis/HSTI/fpi_sim_matrix.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/fpi_sim_matrix_angular.py` & `HSTI-0.0.9/hsti-analysis/HSTI/fpi_sim_matrix_angular.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/hsti_export.py` & `HSTI-0.0.9/hsti-analysis/HSTI/hsti_export.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/hsti_import.py` & `HSTI-0.0.9/hsti-analysis/HSTI/hsti_import.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/remove_bad_px.py` & `HSTI-0.0.9/hsti-analysis/HSTI/remove_bad_px.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/remove_vignetting.py` & `HSTI-0.0.9/hsti-analysis/HSTI/remove_vignetting.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/spectral_debending.py` & `HSTI-0.0.9/hsti-analysis/HSTI/spectral_debending.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI/voronoi_partitioning.py` & `HSTI-0.0.9/hsti-analysis/HSTI/voronoi_partitioning.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI.egg-info/PKG-INFO` & `HSTI-0.0.9/hsti-analysis/HSTI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSTI
-Version: 0.0.8
+Version: 0.0.9
 Summary: The NEWTEC HSTI package contains fundamental functions for the data analysis of hyperspectral thermal images (HSTI).
 Home-page: UNKNOWN
 Author: Mads Nibe et. al.
 Author-email: mani@newtec.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `HSTI-0.0.8/hsti-analysis/HSTI.egg-info/SOURCES.txt` & `HSTI-0.0.9/hsti-analysis/HSTI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.8/setup.py` & `HSTI-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HSTI",
-    version="0.0.8",
+    version="0.0.9",
     author="Mads Nibe et. al.",
     author_email="mani@newtec.dk",
     description="The NEWTEC HSTI package contains fundamental functions for the data analysis of hyperspectral thermal images (HSTI).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

