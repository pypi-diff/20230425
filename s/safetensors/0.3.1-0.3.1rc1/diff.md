# Comparing `tmp/safetensors-0.3.1.tar.gz` & `tmp/safetensors-0.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safetensors-0.3.1.tar", last modified: Tue Apr 25 08:28:59 2023, max compression
+gzip compressed data, was "safetensors-0.3.1rc1.tar", last modified: Mon Apr 24 15:00:13 2023, max compression
```

## Comparing `safetensors-0.3.1.tar` & `safetensors-0.3.1rc1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-25 08:28:58.000000 safetensors-0.3.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 08:28:32.000000 safetensors-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-25 08:28:59.778367 safetensors-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-25 08:28:32.000000 safetensors-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.774367 safetensors-0.3.1/py_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.774367 safetensors-0.3.1/py_src/safetensors/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 08:28:32.000000 safetensors-0.3.1/py_src/safetensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-25 08:28:32.000000 safetensors-0.3.1/py_src/safetensors/flax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-25 08:28:32.000000 safetensors-0.3.1/py_src/safetensors/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-25 08:28:32.000000 safetensors-0.3.1/py_src/safetensors/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-25 08:28:32.000000 safetensors-0.3.1/py_src/safetensors/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-04-25 08:28:32.000000 safetensors-0.3.1/py_src/safetensors/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/py_src/safetensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-25 08:28:59.000000 safetensors-0.3.1/py_src/safetensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 08:28:59.000000 safetensors-0.3.1/py_src/safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:28:59.000000 safetensors-0.3.1/py_src/safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:28:59.000000 safetensors-0.3.1/py_src/safetensors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-25 08:28:59.000000 safetensors-0.3.1/py_src/safetensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 08:28:59.000000 safetensors-0.3.1/py_src/safetensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-25 08:28:32.000000 safetensors-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/safetensors-lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/README.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/safetensors-lib/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/benches/benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/safetensors-lib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/safetensors-lib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/safetensors-lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/src/slice.rs
--rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-04-25 08:28:32.000000 safetensors-0.3.1/safetensors-lib/src/tensor.rs
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-25 08:28:59.778367 safetensors-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-25 08:28:32.000000 safetensors-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:28:59.778367 safetensors-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    33654 2023-04-25 08:28:32.000000 safetensors-0.3.1/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 15:00:12.000000 safetensors-0.3.1rc1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.598883 safetensors-0.3.1rc1/py_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.598883 safetensors-0.3.1rc1/py_src/safetensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/flax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/py_src/safetensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/README.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/benches/benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/tensor.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    33654 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/src/lib.rs
```

### Comparing `safetensors-0.3.1/PKG-INFO` & `safetensors-0.3.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.3.1
+Version: 0.3.1rc1
 Summary: Fast and Safe Tensor serialization
 Home-page: https://github.com/huggingface/safetensors
 Author: 
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `safetensors-0.3.1/README.md` & `safetensors-0.3.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors/flax.py` & `safetensors-0.3.1rc1/py_src/safetensors/flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors/numpy.py` & `safetensors-0.3.1rc1/py_src/safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors/paddle.py` & `safetensors-0.3.1rc1/py_src/safetensors/paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors/tensorflow.py` & `safetensors-0.3.1rc1/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors/torch.py` & `safetensors-0.3.1rc1/py_src/safetensors/torch.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors.egg-info/PKG-INFO` & `safetensors-0.3.1rc1/py_src/safetensors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.3.1
+Version: 0.3.1rc1
 Summary: Fast and Safe Tensor serialization
 Home-page: https://github.com/huggingface/safetensors
 Author: 
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `safetensors-0.3.1/py_src/safetensors.egg-info/SOURCES.txt` & `safetensors-0.3.1rc1/py_src/safetensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/py_src/safetensors.egg-info/requires.txt` & `safetensors-0.3.1rc1/py_src/safetensors.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/Cargo.toml` & `safetensors-0.3.1rc1/safetensors-lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/README.md` & `safetensors-0.3.1rc1/safetensors-lib/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/README.tpl` & `safetensors-0.3.1rc1/safetensors-lib/README.tpl`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/benches/benchmark.rs` & `safetensors-0.3.1rc1/safetensors-lib/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/src/lib.rs` & `safetensors-0.3.1rc1/safetensors-lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/src/slice.rs` & `safetensors-0.3.1rc1/safetensors-lib/src/slice.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/safetensors-lib/src/tensor.rs` & `safetensors-0.3.1rc1/safetensors-lib/src/tensor.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/setup.cfg` & `safetensors-0.3.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/setup.py` & `safetensors-0.3.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1/src/lib.rs` & `safetensors-0.3.1rc1/src/lib.rs`

 * *Files identical despite different names*

