# Comparing `tmp/mpc_orb-0.1.4.tar.gz` & `tmp/mpc_orb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_orb-0.1.4.tar", last modified: Sat Feb 11 19:32:56 2023, max compression
+gzip compressed data, was "mpc_orb-0.1.6.tar", last modified: Tue Apr 25 01:47:39 2023, max compression
```

## Comparing `mpc_orb-0.1.4.tar` & `mpc_orb-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 19:32:56.488605 mpc_orb-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-02-11 19:32:56.488605 mpc_orb-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 19:32:56.484605 mpc_orb-0.1.4/mpc_orb/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 19:32:56.484605 mpc_orb-0.1.4/mpc_orb/schema_json/
--rw-r--r--   0 runner    (1001) docker     (122)    35791 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_latest.json
--rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.1.json
--rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.2.json
--rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.3.json
--rw-r--r--   0 runner    (1001) docker     (122)    35791 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.4.json
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/mpc_orb/validate_mpcorb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 19:32:56.484605 mpc_orb-0.1.4/mpc_orb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-02-11 19:32:56.000000 mpc_orb-0.1.4/mpc_orb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-02-11 19:32:56.000000 mpc_orb-0.1.4/mpc_orb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-11 19:32:56.000000 mpc_orb-0.1.4/mpc_orb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-11 19:32:56.000000 mpc_orb-0.1.4/mpc_orb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-02-11 19:32:56.000000 mpc_orb-0.1.4/mpc_orb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-02-11 19:32:56.000000 mpc_orb-0.1.4/mpc_orb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-11 19:32:56.488605 mpc_orb-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-11 19:32:56.488605 mpc_orb-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/tests/filepaths_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/tests/test_filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/tests/test_interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-02-11 19:32:40.000000 mpc_orb-0.1.4/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb/demo_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb/schema_json/
+-rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_latest.json
+-rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.4.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/validate_mpcorb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/filepaths_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_validation.py
```

### Comparing `mpc_orb-0.1.4/LICENSE` & `mpc_orb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb/interpret.py` & `mpc_orb-0.1.6/mpc_orb/interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb/parse.py` & `mpc_orb-0.1.6/mpc_orb/parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_latest.json` & `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_latest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8749934238215489%*

 * *Differences: {"'properties'": "{'COM': {'properties': {'coefficient_specification': {'description': "*

 * *                 "'Description of allowed fitted quantities within the cometary coordinate "*

 * *                 "specification system. '}}}}",*

 * * 'delete': "['$schema']"}*

```diff
@@ -476,15 +476,14 @@
                     ],
                     "type": "string"
                 }
             },
             "type": "object"
         }
     },
-    "$schema": "http://json-schema.org/schema#",
     "description": "Standardized MPC JSON format for the exchange of orbit-fit data. Designed to communicate the best-fit orbit for a single minor planet or comet.",
     "properties": {
         "CAR": {
             "description": "Cartesian Element Specification: Description of the best-fit orbit based on a cartesian coordinate system (plus any non-gravs). Contains the best-fit orbit and covariance matrix. Heliocentric coordinates.",
             "properties": {
                 "coefficient_names": {
                     "description": "Names of the cartesian elements (and any non-grav components) used in this fit. Of length 6 if gravity-only, or 7-10 if we have non-gravs.",
@@ -596,15 +595,15 @@
                         "type": "string"
                     },
                     "maxItems": 10,
                     "minItems": 6,
                     "type": "array"
                 },
                 "coefficient_specification": {
-                    "description": "Description of allowedd fitted quantities within the cometary coordinate specification system. ",
+                    "description": "Description of allowed fitted quantities within the cometary coordinate specification system. ",
                     "properties": {
                         "A1": {
                             "$ref": "#/$defs/A123_coeff"
                         },
                         "A2": {
                             "$ref": "#/$defs/A123_coeff"
                         },
```

### Comparing `mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.1.json` & `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.1.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.2.json` & `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.2.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.3.json` & `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.3.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb/schema_json/mpcorb_schema_v0.4.json` & `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.4.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8749934238215489%*

 * *Differences: {"'properties'": "{'COM': {'properties': {'coefficient_specification': {'description': "*

 * *                 "'Description of allowed fitted quantities within the cometary coordinate "*

 * *                 "specification system. '}}}}",*

 * * 'delete': "['$schema']"}*

```diff
@@ -476,15 +476,14 @@
                     ],
                     "type": "string"
                 }
             },
             "type": "object"
         }
     },
-    "$schema": "http://json-schema.org/schema#",
     "description": "Standardized MPC JSON format for the exchange of orbit-fit data. Designed to communicate the best-fit orbit for a single minor planet or comet.",
     "properties": {
         "CAR": {
             "description": "Cartesian Element Specification: Description of the best-fit orbit based on a cartesian coordinate system (plus any non-gravs). Contains the best-fit orbit and covariance matrix. Heliocentric coordinates.",
             "properties": {
                 "coefficient_names": {
                     "description": "Names of the cartesian elements (and any non-grav components) used in this fit. Of length 6 if gravity-only, or 7-10 if we have non-gravs.",
@@ -596,15 +595,15 @@
                         "type": "string"
                     },
                     "maxItems": 10,
                     "minItems": 6,
                     "type": "array"
                 },
                 "coefficient_specification": {
-                    "description": "Description of allowedd fitted quantities within the cometary coordinate specification system. ",
+                    "description": "Description of allowed fitted quantities within the cometary coordinate specification system. ",
                     "properties": {
                         "A1": {
                             "$ref": "#/$defs/A123_coeff"
                         },
                         "A2": {
                             "$ref": "#/$defs/A123_coeff"
                         },
```

### Comparing `mpc_orb-0.1.4/mpc_orb/validate_mpcorb.py` & `mpc_orb-0.1.6/mpc_orb/validate_mpcorb.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/mpc_orb.egg-info/SOURCES.txt` & `mpc_orb-0.1.6/mpc_orb.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 README.md
 setup.py
 mpc_orb/__init__.py
+mpc_orb/demo.py
 mpc_orb/filepaths.py
 mpc_orb/interpret.py
 mpc_orb/parse.py
 mpc_orb/validate_mpcorb.py
 mpc_orb.egg-info/PKG-INFO
 mpc_orb.egg-info/SOURCES.txt
 mpc_orb.egg-info/dependency_links.txt
 mpc_orb.egg-info/not-zip-safe
 mpc_orb.egg-info/requires.txt
 mpc_orb.egg-info/top_level.txt
+mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
 mpc_orb/schema_json/mpcorb_schema_latest.json
 mpc_orb/schema_json/mpcorb_schema_v0.1.json
 mpc_orb/schema_json/mpcorb_schema_v0.2.json
 mpc_orb/schema_json/mpcorb_schema_v0.3.json
 mpc_orb/schema_json/mpcorb_schema_v0.4.json
 tests/__init__.py
 tests/filepaths_for_testing.py
```

### Comparing `mpc_orb-0.1.4/setup.py` & `mpc_orb-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mpc_orb',
-    version='0.1.4',
+    version='0.1.6',
     long_description=long_description,  
     long_description_content_type="text/markdown",
     author='MJP:MPC',
     author_email='mpayne@cfa.harvard.edu',
     url='https://github.com/Smithsonian/mpc-public',
     install_requires=[
         'jsonschema',
         'numpy',
         'pytest'],
     packages=setuptools.find_packages(),#where="mpc_orb"),
-    package_data={"": ["schema_json/*.json"]},
+    package_data={"": ["schema_json/*.json" , "demo_json/*.json"]},
     zip_safe=False)
```

### Comparing `mpc_orb-0.1.4/tests/test_interpret.py` & `mpc_orb-0.1.6/tests/test_interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/tests/test_parse.py` & `mpc_orb-0.1.6/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.4/tests/test_validation.py` & `mpc_orb-0.1.6/tests/test_validation.py`

 * *Files identical despite different names*

