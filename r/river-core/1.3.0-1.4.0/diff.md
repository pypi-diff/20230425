# Comparing `tmp/river_core-1.3.0.tar.gz` & `tmp/river_core-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/river_core-1.3.0.tar", last modified: Mon Apr 24 05:13:21 2023, max compression
+gzip compressed data, was "dist/river_core-1.4.0.tar", last modified: Tue Apr 25 06:34:41 2023, max compression
```

## Comparing `river_core-1.3.0.tar` & `river_core-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-24 05:13:01.000000 river_core-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-24 05:13:01.000000 river_core-1.3.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-24 05:13:01.000000 river_core-1.3.0/LICENSE.tessolve
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 05:13:01.000000 river_core-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 05:13:21.000000 river_core-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 05:13:01.000000 river_core-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-24 05:13:01.000000 river_core-1.3.0/examples/sample-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42036 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/rivercore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/sim_hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/coverage_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    14432 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/dut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/dut/boot/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/boot/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/sample_gen_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/reference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/sample_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/style.css
--rw-r--r--   0 runner    (1001) docker     (123)    18787 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 05:13:21.000000 river_core-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-24 05:13:01.000000 river_core-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-25 06:34:21.000000 river_core-1.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-25 06:34:21.000000 river_core-1.4.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-25 06:34:21.000000 river_core-1.4.0/LICENSE.tessolve
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-25 06:34:21.000000 river_core-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-25 06:34:41.000000 river_core-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 06:34:21.000000 river_core-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-25 06:34:21.000000 river_core-1.4.0/examples/sample-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42036 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/rivercore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/sim_hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/coverage_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14432 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/templates/setup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/templates/setup/dut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/dut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/templates/setup/dut/boot/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/dut/boot/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/dut/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/dut/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/dut/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/templates/setup/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/generator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/generator/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/generator/sample_gen_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/generator/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core/templates/setup/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/reference/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/reference/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/setup/reference/sample_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/templates/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-04-25 06:34:21.000000 river_core-1.4.0/river_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 06:34:41.000000 river_core-1.4.0/river_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 06:34:41.000000 river_core-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-25 06:34:21.000000 river_core-1.4.0/setup.py
```

### Comparing `river_core-1.3.0/CONTRIBUTING.rst` & `river_core-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/LICENSE.incore` & `river_core-1.4.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/LICENSE.tessolve` & `river_core-1.4.0/LICENSE.tessolve`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/PKG-INFO` & `river_core-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river_core
-Version: 1.3.0
+Version: 1.4.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.3.0/examples/sample-config.ini` & `river_core-1.4.0/examples/sample-config.ini`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/constants.py` & `river_core-1.4.0/river_core/constants.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/log.py` & `river_core-1.4.0/river_core/log.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/main.py` & `river_core-1.4.0/river_core/main.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/rivercore.py` & `river_core-1.4.0/river_core/rivercore.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/sim_hookspecs.py` & `river_core-1.4.0/river_core/sim_hookspecs.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/coverage_report.html` & `river_core-1.4.0/river_core/templates/coverage_report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/report.html` & `river_core-1.4.0/river_core/templates/report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/setup/dut/gen_framework.py` & `river_core-1.4.0/river_core/templates/setup/dut/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/setup/dut/sample_plugin.py` & `river_core-1.4.0/river_core/templates/setup/dut/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/setup/generator/gen_framework.py` & `river_core-1.4.0/river_core/templates/setup/generator/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/setup/generator/sample_plugin.py` & `river_core-1.4.0/river_core/templates/setup/generator/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/setup/reference/gen_framework.py` & `river_core-1.4.0/river_core/templates/setup/reference/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/setup/reference/sample_plugin.py` & `river_core-1.4.0/river_core/templates/setup/reference/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/templates/style.css` & `river_core-1.4.0/river_core/templates/style.css`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/river_core/utils.py` & `river_core-1.4.0/river_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import ruamel
 import signal
 from ruamel.yaml import YAML
 from threading import Timer
 import pathlib
 import difflib
 import shlex
+import riscv_config.isa_validator as isa_val
 
 yaml = YAML(typ="safe")
 yaml.default_flow_style = False
 yaml.allow_unicode = True
 
 def self_check(file1):
   '''
@@ -135,26 +136,19 @@
         with open(input_yaml, "r") as file:
             return dict(yaml.load(file))
     except ruamel.yaml.constructor.DuplicateKeyError as msg:
         raise SystemExit
 
 
 def check_isa(isa):
-    if 'Z' in isa:
-        extensions = isa.split('Z')
-        if extensions[0].upper() != extensions[0]:
-            raise Exception('ISA Error: Ratified extensions should be in '
-                            'uppercase')
-    elif 'z' in isa:
-        raise Exception('ISA Error: unratified extension with lowercase Z')
-    else:
-        if isa.upper() != isa:
-            raise Exception('ISA Error: Ratified extensions should be in '
-                            'uppercase')
-
+    (ext_list, err, err_list) = isa_val.get_extension_list(isa)
+    if err:
+      for e in err_list:
+        logger.error(e)
+      raise SystemExit(1)
 
 def sys_command(command, timeout=240, logging=True):
     '''
         Wrapper function to run shell commands with a timeout.
         Uses :py:mod:`subprocess`, :py:mod:`shlex`, :py:mod:`os`
         to ensure proper termination on timeout
```

### Comparing `river_core-1.3.0/river_core.egg-info/PKG-INFO` & `river_core-1.4.0/river_core.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river-core
-Version: 1.3.0
+Version: 1.4.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.3.0/river_core.egg-info/SOURCES.txt` & `river_core-1.4.0/river_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `river_core-1.3.0/setup.py` & `river_core-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         ]
     },
     setup_requires=setup_requirements,
     test_suite='',
     tests_require=test_requirements,
     url=
     'https://github.com/incoresemi/river_core',
-    version='1.3.0',
+    version='1.4.0',
     zip_safe=False,
 )
```

