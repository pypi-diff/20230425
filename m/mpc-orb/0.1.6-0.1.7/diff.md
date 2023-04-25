# Comparing `tmp/mpc_orb-0.1.6.tar.gz` & `tmp/mpc_orb-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_orb-0.1.6.tar", last modified: Tue Apr 25 01:47:39 2023, max compression
+gzip compressed data, was "mpc_orb-0.1.7.tar", last modified: Tue Apr 25 02:15:20 2023, max compression
```

## Comparing `mpc_orb-0.1.6.tar` & `mpc_orb-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb/demo_json/
--rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb/schema_json/
--rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_latest.json
--rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.1.json
--rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.2.json
--rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.3.json
--rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.4.json
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/mpc_orb/validate_mpcorb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/mpc_orb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-25 01:47:39.000000 mpc_orb-0.1.6/mpc_orb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:39.323226 mpc_orb-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/filepaths_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_filepaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_interpret.py
--rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-25 01:47:23.000000 mpc_orb-0.1.6/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb/
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb/demo_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     8036 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb/schema_json/
+-rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_latest.json
+-rw-r--r--   0 runner    (1001) docker     (122)    36609 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.1.json
+-rw-r--r--   0 runner    (1001) docker     (122)    47079 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.2.json
+-rw-r--r--   0 runner    (1001) docker     (122)    56881 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.3.json
+-rw-r--r--   0 runner    (1001) docker     (122)    35741 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.4.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/mpc_orb/validate_mpcorb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.416579 mpc_orb-0.1.7/mpc_orb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-25 02:15:20.000000 mpc_orb-0.1.7/mpc_orb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 02:15:20.420580 mpc_orb-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/filepaths_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4316 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2204 2023-04-25 02:14:57.000000 mpc_orb-0.1.7/tests/test_validation.py
```

### Comparing `mpc_orb-0.1.6/LICENSE` & `mpc_orb-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/PKG-INFO` & `mpc_orb-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_orb
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/Smithsonian/mpc-public
 Author: MJP:MPC
 Author-email: mpayne@cfa.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpc-public/mpc_orb
```

### Comparing `mpc_orb-0.1.6/README.md` & `mpc_orb-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/demo.py` & `mpc_orb-0.1.7/mpc_orb/demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
  - Code to provide a quick demo (post-install) of how to use the MPCORB
    class
    
 Author(s)
 MJP
 """
 
+# standard imports
+# -----------------------
+import os
 
 # local imports
 # -----------------------
 from mpc_orb.parse import MPCORB, COORD
 
 def tprint(lft,rght,width=20):
     print(f'\t{lft:<{width}}:\t{rght}')
@@ -27,15 +30,15 @@
     
     returns:
     --------
     ???
     
     """
     # Define a filepath to an example json file provided in the package
-    demo_filepath = 'demo_json/2012HN13_mpcorb_yarkovski.json'
+    demo_filepath = os.path.join( os.path.dirname(os.path.abspath(__file__)), 'demo_json/2012HN13_mpcorb_yarkovski.json')
     print(f'\nAccessing a sample json file:\n\t{demo_filepath}')
 
     # Instantiate an MPCORB object & use it to parse the above json file
     # & Demonstrate the available variables
     M = MPCORB(demo_filepath)
     print(f'\nWe instantiated an MPCORB object using the sample json')
     tprint('code','MPCORB(demo_filepath)')
```

### Comparing `mpc_orb-0.1.6/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json` & `mpc_orb-0.1.7/mpc_orb/demo_json/2012HN13_mpcorb_yarkovski.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/interpret.py` & `mpc_orb-0.1.7/mpc_orb/interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/parse.py` & `mpc_orb-0.1.7/mpc_orb/parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_latest.json` & `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_latest.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.1.json` & `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.1.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.2.json` & `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.2.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.3.json` & `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.3.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/schema_json/mpcorb_schema_v0.4.json` & `mpc_orb-0.1.7/mpc_orb/schema_json/mpcorb_schema_v0.4.json`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb/validate_mpcorb.py` & `mpc_orb-0.1.7/mpc_orb/validate_mpcorb.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/mpc_orb.egg-info/PKG-INFO` & `mpc_orb-0.1.7/mpc_orb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-orb
-Version: 0.1.6
+Version: 0.1.7
 Home-page: https://github.com/Smithsonian/mpc-public
 Author: MJP:MPC
 Author-email: mpayne@cfa.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mpc-public/mpc_orb
```

### Comparing `mpc_orb-0.1.6/mpc_orb.egg-info/SOURCES.txt` & `mpc_orb-0.1.7/mpc_orb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/setup.py` & `mpc_orb-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mpc_orb',
-    version='0.1.6',
+    version='0.1.7',
     long_description=long_description,  
     long_description_content_type="text/markdown",
     author='MJP:MPC',
     author_email='mpayne@cfa.harvard.edu',
     url='https://github.com/Smithsonian/mpc-public',
     install_requires=[
         'jsonschema',
```

### Comparing `mpc_orb-0.1.6/tests/test_interpret.py` & `mpc_orb-0.1.7/tests/test_interpret.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/tests/test_parse.py` & `mpc_orb-0.1.7/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `mpc_orb-0.1.6/tests/test_validation.py` & `mpc_orb-0.1.7/tests/test_validation.py`

 * *Files identical despite different names*

