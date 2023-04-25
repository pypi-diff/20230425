# Comparing `tmp/cloudnetpy_qc-1.9.0.tar.gz` & `tmp/cloudnetpy_qc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudnetpy_qc-1.9.0.tar", last modified: Fri Apr 14 09:53:09 2023, max compression
+gzip compressed data, was "cloudnetpy_qc-1.9.1.tar", last modified: Tue Apr 25 07:47:23 2023, max compression
```

## Comparing `cloudnetpy_qc-1.9.0.tar` & `cloudnetpy_qc-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.985345 cloudnetpy_qc-1.9.0/cloudnetpy_qc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/area-type-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/data_quality_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/metadata_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/standardized-region-list.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15828 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30001 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.985345 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:23.164299 cloudnetpy_qc-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-25 07:47:23.164299 cloudnetpy_qc-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:23.152299 cloudnetpy_qc-1.9.1/cloudnetpy_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:23.164299 cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/area-type-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/data_quality_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/metadata_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/standardized-region-list.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30001 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:47:23.156299 cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-25 07:47:23.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-25 07:47:23.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:47:23.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 07:47:23.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 07:47:23.000000 cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:47:23.164299 cloudnetpy_qc-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-25 07:47:06.000000 cloudnetpy_qc-1.9.1/setup.py
```

### Comparing `cloudnetpy_qc-1.9.0/LICENSE` & `cloudnetpy_qc-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/PKG-INFO` & `cloudnetpy_qc-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy_qc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.0/README.md` & `cloudnetpy_qc-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/area-type-table.xml` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/area-type-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/cf-standard-name-table.xml` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/data_quality_config.ini` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/data_quality_config.ini`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/standardized-region-list.xml` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/data/standardized-region-list.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/quality.py` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             beta_raw = self.nc["beta_raw"]
         except IndexError:
             return
         n_top_ranges = 200
         x = range_var[-n_top_ranges:] ** 2
         y = np.std(beta_raw[:, -n_top_ranges:], axis=0)
         res = scipy.stats.pearsonr(x, y)
-        if res.statistic < 0.5:
+        if res.statistic < 0.75:
             self._add_message("Data might not be range corrected.")
 
 
 @test(
     "Instrument PID",
     "Test that valid instrument PID exists.",
     ErrorLevel.WARNING,
```

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/utils.py` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/utils.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc/variables.py` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc/variables.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/PKG-INFO` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy-qc
-Version: 1.9.0
+Version: 1.9.1
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/SOURCES.txt` & `cloudnetpy_qc-1.9.1/cloudnetpy_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.0/setup.py` & `cloudnetpy_qc-1.9.1/setup.py`

 * *Files identical despite different names*

