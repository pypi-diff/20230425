# Comparing `tmp/blyss-0.1.8.tar.gz` & `tmp/blyss-0.1.9.tar.gz`

## Comparing `blyss-0.1.8.tar` & `blyss-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 blyss-0.1.8/local_dependencies/spiral-rs/Cargo.toml
--rw-r--r--   0     1001      123       82 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/.cargo/config.toml
--rw-r--r--   0     1001      123      194 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/README.md
--rw-r--r--   0     1001      123     2523 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/aligned_memory.rs
--rw-r--r--   0     1001      123    15010 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/arith.rs
--rw-r--r--   0     1001      123    32652 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/client.rs
--rw-r--r--   0     1001      123     5686 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/discrete_gaussian.rs
--rw-r--r--   0     1001      123     2882 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/gadget.rs
--rw-r--r--   0     1001      123     2358 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/key_value.rs
--rw-r--r--   0     1001      123      267 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/lib.rs
--rw-r--r--   0     1001      123     5078 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/noise_estimate.rs
--rw-r--r--   0     1001      123    17652 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/ntt.rs
--rw-r--r--   0     1001      123     2386 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/number_theory.rs
--rw-r--r--   0     1001      123     7852 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/params.rs
--rw-r--r--   0     1001      123    23492 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/poly.rs
--rw-r--r--   0     1001      123    36705 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/server.rs
--rw-r--r--   0     1001      123    11665 2023-04-20 22:59:51.000000 blyss-0.1.8/local_dependencies/spiral-rs/src/util.rs
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 blyss-0.1.8/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-04-20 22:59:51.000000 blyss-0.1.8/.gitignore
--rw-r--r--   0     1001      123       19 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/__init__.py
--rw-r--r--   0     1001      123     9589 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/api.py
--rw-r--r--   0     1001      123     1275 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/bloom.py
--rw-r--r--   0     1001      123     3564 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/blyss_lib.py
--rw-r--r--   0     1001      123    12241 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/bucket.py
--rw-r--r--   0     1001      123     4155 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/bucket_service.py
--rw-r--r--   0     1001      123      139 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/main.py
--rw-r--r--   0     1001      123     2277 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/req_compression.py
--rw-r--r--   0     1001      123     1299 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/seed.py
--rw-r--r--   0     1001      123     1946 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/serializer.py
--rw-r--r--   0     1001      123     1520 2023-04-20 22:59:51.000000 blyss-0.1.8/blyss/varint.py
--rw-r--r--   0     1001      123      383 2023-04-20 22:59:51.000000 blyss-0.1.8/pyproject.toml
--rw-r--r--   0     1001      123     2160 2023-04-20 22:59:51.000000 blyss-0.1.8/src/lib.rs
--rw-r--r--   0     1001      123     3167 2023-04-20 22:59:51.000000 blyss-0.1.8/tests/test_service.py
--rw-r--r--   0     1001      123    13791 2023-04-20 22:59:51.000000 blyss-0.1.8/Cargo.lock
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 blyss-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 blyss-0.1.9/local_dependencies/spiral-rs/Cargo.toml
+-rw-r--r--   0     1001      123       82 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/.cargo/config.toml
+-rw-r--r--   0     1001      123      194 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/README.md
+-rw-r--r--   0     1001      123     2523 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/aligned_memory.rs
+-rw-r--r--   0     1001      123    15010 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/arith.rs
+-rw-r--r--   0     1001      123    32652 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/client.rs
+-rw-r--r--   0     1001      123     5686 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/discrete_gaussian.rs
+-rw-r--r--   0     1001      123     2882 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/gadget.rs
+-rw-r--r--   0     1001      123     2358 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/key_value.rs
+-rw-r--r--   0     1001      123      267 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/lib.rs
+-rw-r--r--   0     1001      123     5078 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/noise_estimate.rs
+-rw-r--r--   0     1001      123    17652 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/ntt.rs
+-rw-r--r--   0     1001      123     2386 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/number_theory.rs
+-rw-r--r--   0     1001      123     7852 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/params.rs
+-rw-r--r--   0     1001      123    23492 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/poly.rs
+-rw-r--r--   0     1001      123    36705 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/server.rs
+-rw-r--r--   0     1001      123    11665 2023-04-24 23:44:52.000000 blyss-0.1.9/local_dependencies/spiral-rs/src/util.rs
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 blyss-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-04-24 23:44:52.000000 blyss-0.1.9/.gitignore
+-rw-r--r--   0     1001      123       19 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/__init__.py
+-rw-r--r--   0     1001      123     9589 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/api.py
+-rw-r--r--   0     1001      123     1275 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/bloom.py
+-rw-r--r--   0     1001      123     3564 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/blyss_lib.py
+-rw-r--r--   0     1001      123    12241 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/bucket.py
+-rw-r--r--   0     1001      123     4155 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/bucket_service.py
+-rw-r--r--   0     1001      123      139 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/main.py
+-rw-r--r--   0     1001      123     2277 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/req_compression.py
+-rw-r--r--   0     1001      123     1299 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/seed.py
+-rw-r--r--   0     1001      123     1946 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/serializer.py
+-rw-r--r--   0     1001      123     1520 2023-04-24 23:44:52.000000 blyss-0.1.9/blyss/varint.py
+-rw-r--r--   0     1001      123      734 2023-04-24 23:44:52.000000 blyss-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      123     2160 2023-04-24 23:44:52.000000 blyss-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      123     3167 2023-04-24 23:44:52.000000 blyss-0.1.9/tests/test_service.py
+-rw-r--r--   0     1001      123    13791 2023-04-24 23:44:52.000000 blyss-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 blyss-0.1.9/PKG-INFO
```

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/Cargo.toml` & `blyss-0.1.9/local_dependencies/spiral-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/aligned_memory.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/aligned_memory.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/arith.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/arith.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/client.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/client.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/discrete_gaussian.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/discrete_gaussian.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/gadget.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/gadget.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/key_value.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/key_value.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/noise_estimate.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/noise_estimate.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/ntt.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/ntt.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/number_theory.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/number_theory.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/params.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/params.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/poly.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/poly.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/server.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/server.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/local_dependencies/spiral-rs/src/util.rs` & `blyss-0.1.9/local_dependencies/spiral-rs/src/util.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/.gitignore` & `blyss-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/api.py` & `blyss-0.1.9/blyss/api.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/bloom.py` & `blyss-0.1.9/blyss/bloom.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/blyss_lib.py` & `blyss-0.1.9/blyss/blyss_lib.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/bucket.py` & `blyss-0.1.9/blyss/bucket.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/bucket_service.py` & `blyss-0.1.9/blyss/bucket_service.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/req_compression.py` & `blyss-0.1.9/blyss/req_compression.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/seed.py` & `blyss-0.1.9/blyss/seed.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/serializer.py` & `blyss-0.1.9/blyss/serializer.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/blyss/varint.py` & `blyss-0.1.9/blyss/varint.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/src/lib.rs` & `blyss-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/tests/test_service.py` & `blyss-0.1.9/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `blyss-0.1.8/Cargo.lock` & `blyss-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "blyss-client-python"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "pyo3",
  "spiral-rs",
 ]
 
 [[package]]
 name = "bumpalo"
```

