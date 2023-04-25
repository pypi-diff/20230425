# Comparing `tmp/halo-reader-0.1.0.tar.gz` & `tmp/halo-reader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halo-reader-0.1.0.tar", last modified: Thu Apr 20 14:35:56 2023, max compression
+gzip compressed data, was "halo-reader-0.1.1.tar", last modified: Tue Apr 25 10:17:28 2023, max compression
```

## Comparing `halo-reader-0.1.0.tar` & `halo-reader-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.973374 halo-reader-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 14:35:35.000000 halo-reader-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-20 14:35:35.000000 halo-reader-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-20 14:35:56.973374 halo-reader-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-20 14:35:35.000000 halo-reader-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-20 14:35:35.000000 halo-reader-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:35:56.973374 halo-reader-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-20 14:35:35.000000 halo-reader-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.965374 halo-reader-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.965374 halo-reader-0.1.0/src/halo_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/halo_reader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.965374 halo-reader-0.1.0/src/haloboard/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloboard/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/halodata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/halodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/halodata/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloreader/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/attenuated_backscatter_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/background_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.969374 halo-reader-0.1.0/src/haloreader/background_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-20 14:35:55.000000 halo-reader-0.1.0/src/haloreader/background_reader/background_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/background_reader/background_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.973374 halo-reader-0.1.0/src/haloreader/data_reader/
--rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-20 14:35:56.000000 halo-reader-0.1.0/src/haloreader/data_reader/data_reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/data_reader/data_reader.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/grammar_header.lark
--rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/halo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/read.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/type_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 14:35:35.000000 halo-reader-0.1.0/src/haloreader/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:35:56.973374 halo-reader-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-20 14:35:35.000000 halo-reader-0.1.0/tests/test_halo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 10:17:06.000000 halo-reader-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-25 10:17:06.000000 halo-reader-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 10:17:28.286955 halo-reader-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-25 10:17:06.000000 halo-reader-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 10:17:06.000000 halo-reader-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:17:28.286955 halo-reader-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 10:17:06.000000 halo-reader-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/halo_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:17:27.000000 halo-reader-0.1.1/src/halo_reader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 10:17:28.000000 halo-reader-0.1.1/src/halo_reader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/haloboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/haloboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/haloboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloboard/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.282955 halo-reader-0.1.1/src/halodata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/halodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/halodata/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/src/haloreader/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/attenuated_backscatter_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/background_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/src/haloreader/background_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   794000 2023-04-25 10:17:26.000000 halo-reader-0.1.1/src/haloreader/background_reader/background_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/background_reader/background_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/src/haloreader/data_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)   834129 2023-04-25 10:17:27.000000 halo-reader-0.1.1/src/haloreader/data_reader/data_reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/data_reader/data_reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/grammar_header.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/halo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/type_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 10:17:06.000000 halo-reader-0.1.1/src/haloreader/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:17:28.286955 halo-reader-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-25 10:17:06.000000 halo-reader-0.1.1/tests/test_halo_reader.py
```

### Comparing `halo-reader-0.1.0/LICENSE` & `halo-reader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/PKG-INFO` & `halo-reader-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.1.0
+Version: 0.1.1
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.1.0/README.md` & `halo-reader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/pyproject.toml` & `halo-reader-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/setup.py` & `halo-reader-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/halo_reader.egg-info/PKG-INFO` & `halo-reader-0.1.1/src/halo_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halo-reader
-Version: 0.1.0
+Version: 0.1.1
 Summary: HALO Photonics wind doppler lidar file reader
 Author-email: Niko Leskinen <niko.leskinen@fmi.fi>
 License: MIT License
         
         Copyright (c) 2022 Finnish Meteorological Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `halo-reader-0.1.0/src/halo_reader.egg-info/SOURCES.txt` & `halo-reader-0.1.1/src/halo_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloboard/app.py` & `halo-reader-0.1.1/src/haloboard/app.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloboard/static/favicon.ico` & `halo-reader-0.1.1/src/haloboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloboard/static/style.css` & `halo-reader-0.1.1/src/haloboard/static/style.css`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloboard/templates/index.html` & `halo-reader-0.1.1/src/haloboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/halodata/datasets.py` & `halo-reader-0.1.1/src/halodata/datasets.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/attenuated_backscatter_coefficient.py` & `halo-reader-0.1.1/src/haloreader/attenuated_backscatter_coefficient.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/attribute.py` & `halo-reader-0.1.1/src/haloreader/attribute.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/background_correction.py` & `halo-reader-0.1.1/src/haloreader/background_correction.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/background_reader/background_reader.c` & `halo-reader-0.1.1/src/haloreader/background_reader/background_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/background_reader/background_reader.pyx` & `halo-reader-0.1.1/src/haloreader/background_reader/background_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/cli.py` & `halo-reader-0.1.1/src/haloreader/cli.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/data_reader/data_reader.c` & `halo-reader-0.1.1/src/haloreader/data_reader/data_reader.c`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/data_reader/data_reader.pyx` & `halo-reader-0.1.1/src/haloreader/data_reader/data_reader.pyx`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/grammar_header.lark` & `halo-reader-0.1.1/src/haloreader/grammar_header.lark`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/halo.py` & `halo-reader-0.1.1/src/haloreader/halo.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/metadata.py` & `halo-reader-0.1.1/src/haloreader/metadata.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/read.py` & `halo-reader-0.1.1/src/haloreader/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,52 +5,66 @@
 from io import BufferedReader, BytesIO
 from pathlib import Path
 from typing import Sequence
 
 import lark
 import numpy as np
 import numpy.typing as npt
+from lark.exceptions import UnexpectedInput
 
 from haloreader.background_reader import read_background
 from haloreader.data_reader import read_data
 from haloreader.exceptions import BackgroundReadError
 from haloreader.halo import Halo, HaloBg
 from haloreader.metadata import Metadata
 from haloreader.utils import UNIX_TIME_UNIT
 from haloreader.variable import Variable
 
-from .exceptions import FileEmpty, HeaderNotFound
+from .exceptions import FileEmpty, HeaderNotFound, UnexpectedDataTokens
 from .transformer import HeaderTransformer
 
 log = logging.getLogger(__name__)
 
 grammar_header = pkgutil.get_data("haloreader", "grammar_header.lark")
 if not isinstance(grammar_header, bytes):
     raise FileNotFoundError("Header grammar file not found")
 header_parser = lark.Lark(
     grammar_header.decode(), parser="lalr", transformer=HeaderTransformer()
 )
 
 
+def _read_single(src: Path | BytesIO) -> Halo:
+    header_end, header_bytes = _read_header(src)
+    metadata, time_vars, time_range_vars, range_func = header_parser.parse(
+        header_bytes.decode()
+    )
+    log.info("Reading data from %s", metadata.filename.value)
+    data_bytes = _read_data(src, header_end)
+    if not isinstance(metadata.ngates.data, int):
+        raise TypeError
+    read_data(data_bytes, metadata.ngates.data, time_vars, time_range_vars)
+    vars_ = {var.name: var for var in time_vars + time_range_vars}
+    vars_["time"] = _decimaltime2timestamp(vars_["time"], metadata)
+    vars_["range"] = range_func(vars_["range"], metadata.gate_range)
+    return Halo(metadata=metadata, **vars_)
+
+
 def read(src_files: Sequence[Path | BytesIO]) -> Halo | None:
     halos = []
     for src in src_files:
-        header_end, header_bytes = _read_header(src)
-        metadata, time_vars, time_range_vars, range_func = header_parser.parse(
-            header_bytes.decode()
-        )
-        log.info("Reading data from %s", metadata.filename.value)
-        data_bytes = _read_data(src, header_end)
-        if not isinstance(metadata.ngates.data, int):
-            raise TypeError
-        read_data(data_bytes, metadata.ngates.data, time_vars, time_range_vars)
-        vars_ = {var.name: var for var in time_vars + time_range_vars}
-        vars_["time"] = _decimaltime2timestamp(vars_["time"], metadata)
-        vars_["range"] = range_func(vars_["range"], metadata.gate_range)
-        halos.append(Halo(metadata=metadata, **vars_))
+        try:
+            halos.append(_read_single(src))
+        except (
+            FileEmpty,
+            HeaderNotFound,
+            UnicodeDecodeError,
+            UnexpectedInput,
+            UnexpectedDataTokens,
+        ) as err:
+            log.warning("Skipping file", exc_info=err)
     log.info("Merging files")
     return Halo.merge(halos)
 
 
 def read_bg(
     src_files: Sequence[Path | BytesIO], filenames: list[str] | None = None
 ) -> HaloBg | None:
```

### Comparing `halo-reader-0.1.0/src/haloreader/scantype.py` & `halo-reader-0.1.1/src/haloreader/scantype.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/screen.py` & `halo-reader-0.1.1/src/haloreader/screen.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/transformer.py` & `halo-reader-0.1.1/src/haloreader/transformer.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/type_guards.py` & `halo-reader-0.1.1/src/haloreader/type_guards.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/utils.py` & `halo-reader-0.1.1/src/haloreader/utils.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/src/haloreader/variable.py` & `halo-reader-0.1.1/src/haloreader/variable.py`

 * *Files identical despite different names*

### Comparing `halo-reader-0.1.0/tests/test_halo_reader.py` & `halo-reader-0.1.1/tests/test_halo_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import numpy as np
 import pytest
 from cfchecker import cfchecks
 
 from haloreader.exceptions import FileEmpty, UnexpectedDataTokens
-from haloreader.read import read, read_bg
+from haloreader.read import _read_single, read, read_bg
 
 raw_files_pass = Path("tests/raw-files/pass/")
 raw_files_xfail = Path("tests/raw-files/xfail/")
 
 
 def _check_cf_conventions(nc_buf):
     f = tempfile.NamedTemporaryFile(suffix=".nc")
@@ -86,21 +86,21 @@
     buf = halo.to_nc()
     _check_cf_conventions(buf)
 
 
 def test_xfail_warsaw():
     src = raw_files_xfail.joinpath("warsaw-2021-10-01-Stare_213_20211001_18.hpl")
     with pytest.raises(UnexpectedDataTokens):
-        read([src])
+        _read_single(src)
 
 
 def test_xfail_empty():
     src = raw_files_xfail.joinpath("empty.hpl")
     with pytest.raises(FileEmpty):
-        read([src])
+        _read_single(src)
 
 
 def test_eriswil_background():
     bg_dir = raw_files_pass.joinpath("eriswil-2022-12-14-background")
     bg_00 = bg_dir.joinpath("Background_141222-000013.txt")
     bg_01 = bg_dir.joinpath("Background_141222-010013.txt")
     halobg = read_bg([bg_00, bg_01])
```

