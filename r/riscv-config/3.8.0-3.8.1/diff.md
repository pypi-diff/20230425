# Comparing `tmp/riscv_config-3.8.0.tar.gz` & `tmp/riscv_config-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_config-3.8.0.tar", last modified: Mon Apr 24 03:40:11 2023, max compression
+gzip compressed data, was "dist/riscv_config-3.8.1.tar", last modified: Tue Apr 25 10:52:37 2023, max compression
```

## Comparing `riscv_config-3.8.0.tar` & `riscv_config-3.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 03:39:49.000000 riscv_config-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 03:40:11.000000 riscv_config-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 03:39:49.000000 riscv_config-3.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93762 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/isa_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemaValidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemas/schema_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemas/schema_isa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/schemas/schema_platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-24 03:39:49.000000 riscv_config-3.8.0/riscv_config/warl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 03:40:11.000000 riscv_config-3.8.0/riscv_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 03:40:11.000000 riscv_config-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-24 03:39:49.000000 riscv_config-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 10:52:09.000000 riscv_config-3.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 10:52:37.000000 riscv_config-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 10:52:09.000000 riscv_config-3.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/riscv_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93762 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/isa_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemaValidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/riscv_config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemas/schema_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemas/schema_isa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemas/schema_platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/warl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/riscv_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-25 10:52:37.000000 riscv_config-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-25 10:52:09.000000 riscv_config-3.8.1/setup.py
```

### Comparing `riscv_config-3.8.0/PKG-INFO` & `riscv_config-3.8.1/riscv_config.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: riscv_config
-Version: 3.8.0
+Name: riscv-config
+Version: 3.8.1
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
```

### Comparing `riscv_config-3.8.0/riscv_config/checker.py` & `riscv_config-3.8.1/riscv_config/checker.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/constants.py` & `riscv_config-3.8.1/riscv_config/constants.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/errors.py` & `riscv_config-3.8.1/riscv_config/errors.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/isa_validator.py` & `riscv_config-3.8.1/riscv_config/isa_validator.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/main.py` & `riscv_config-3.8.1/riscv_config/main.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/schemaValidator.py` & `riscv_config-3.8.1/riscv_config/schemaValidator.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/schemas/schema_debug.yaml` & `riscv_config-3.8.1/riscv_config/schemas/schema_debug.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/schemas/schema_isa.yaml` & `riscv_config-3.8.1/riscv_config/schemas/schema_isa.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -13240,15 +13240,15 @@
             mnstatus also holds the NMIE bit. When NMIE=1, nonmaskable interrupts are enabled. When
             NMIE=0, all interrupts are disabled.
             When NMIE=0, the hart behaves as though mstatus.MPRV were clear, regardless of the current
             setting of mstatus.MPRV.
 
             Upon reset, NMIE contains the value 0.
 
-        address: {type: integer, default: 0x742, allowed: [0x742]}
+        address: {type: integer, default: 0x744, allowed: [0x744]}
         priv_mode: {type: string, default: M, allowed: [M]}
         reset-val:
           type: integer
           check_with: max_length
           default: 0
         rv32:
           type: dict
```

### Comparing `riscv_config-3.8.0/riscv_config/schemas/schema_platform.yaml` & `riscv_config-3.8.1/riscv_config/schemas/schema_platform.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/utils.py` & `riscv_config-3.8.1/riscv_config/utils.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config/warl.py` & `riscv_config-3.8.1/riscv_config/warl.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/riscv_config.egg-info/SOURCES.txt` & `riscv_config-3.8.1/riscv_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.0/setup.py` & `riscv_config-3.8.1/setup.py`

 * *Files identical despite different names*

