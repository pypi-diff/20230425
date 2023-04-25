# Comparing `tmp/perpetuo-0.1.0.tar.gz` & `tmp/perpetuo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perpetuo-0.1.0.tar", last modified: Mon Apr 24 21:49:25 2023, max compression
+gzip compressed data, was "perpetuo-0.2.0.tar", last modified: Tue Apr 25 01:54:44 2023, max compression
```

## Comparing `perpetuo-0.1.0.tar` & `perpetuo-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    49965 2023-04-24 21:49:14.000000 perpetuo-0.1.0/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 21:49:14.000000 perpetuo-0.1.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:49:14.000000 perpetuo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 21:49:14.000000 perpetuo-0.1.0/LICENSE.APACHE2
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-24 21:49:14.000000 perpetuo-0.1.0/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 21:49:14.000000 perpetuo-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-24 21:49:25.053749 perpetuo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-24 21:49:14.000000 perpetuo-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 21:49:14.000000 perpetuo-0.1.0/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 21:49:14.000000 perpetuo-0.1.0/prep-manylinux-container.sh
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-24 21:49:14.000000 perpetuo-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.049749 perpetuo-0.1.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/python/perpetuo/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/_perpetuo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/python/perpetuo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:24.000000 perpetuo-0.1.0/python/perpetuo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:49:25.053749 perpetuo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 21:49:14.000000 perpetuo-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 21:49:14.000000 perpetuo-0.1.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-24 21:49:14.000000 perpetuo-0.1.0/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-24 21:49:14.000000 perpetuo-0.1.0/src/shmem.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.552439 perpetuo-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    50176 2023-04-25 01:54:36.000000 perpetuo-0.2.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 01:54:36.000000 perpetuo-0.2.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 01:54:36.000000 perpetuo-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 01:54:36.000000 perpetuo-0.2.0/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 01:54:36.000000 perpetuo-0.2.0/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-25 01:54:36.000000 perpetuo-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-25 01:54:44.552439 perpetuo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-25 01:54:36.000000 perpetuo-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 01:54:36.000000 perpetuo-0.2.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-25 01:54:36.000000 perpetuo-0.2.0/prep-manylinux-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-25 01:54:36.000000 perpetuo-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.548439 perpetuo-0.2.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.548439 perpetuo-0.2.0/python/perpetuo/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/_perpetuo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:36.000000 perpetuo-0.2.0/python/perpetuo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.552439 perpetuo-0.2.0/python/perpetuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 01:54:44.000000 perpetuo-0.2.0/python/perpetuo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 01:54:44.552439 perpetuo-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-25 01:54:36.000000 perpetuo-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 01:54:44.552439 perpetuo-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-25 01:54:36.000000 perpetuo-0.2.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-25 01:54:36.000000 perpetuo-0.2.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-25 01:54:36.000000 perpetuo-0.2.0/src/shmem.rs
```

### Comparing `perpetuo-0.1.0/Cargo.lock` & `perpetuo-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -754,14 +754,20 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "indoc"
+version = "2.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f2cb48b81b1dc9f39676bf99f5499babfec7cd8fe14307f7b3d747208fb5690"
+
+[[package]]
 name = "inferno"
 version = "0.11.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fb7c1b80a1dfa604bb4a649a5c5aeef3d913f7c520cb42b40e534e8a61bcdfc"
 dependencies = [
  "ahash 0.8.3",
  "clap 4.2.2",
@@ -1113,14 +1119,15 @@
 [[package]]
 name = "perpetuo"
 version = "0.1.0"
 dependencies = [
  "anyhow",
  "bytemuck",
  "clap 4.2.2",
+ "indoc 2.0.1",
  "libc",
  "memmap",
  "once_cell",
  "proc-maps 0.3.0",
  "py-spy",
  "pyo3",
  "pyo3-build-config",
@@ -1239,15 +1246,15 @@
 [[package]]
 name = "pyo3"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
- "indoc",
+ "indoc 1.0.9",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
```

### Comparing `perpetuo-0.1.0/Cargo.toml` & `perpetuo-0.2.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "perpetuo"
-version = "0.1.0"
+version = "0.2.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "perpetuo"
@@ -13,14 +13,15 @@
 [[bin]]
 name = "perpetuo"
 
 [dependencies]
 anyhow = "1.0.70"
 bytemuck = { version = "1.13.1", features = ["derive", "zeroable_atomics"] }
 clap = { version = "4.2.2", features = ["derive"] }
+indoc = "2.0.1"
 memmap = "0.7.0"
 once_cell = "1.17.1"
 proc-maps = "0.3.0"
 py-spy = "0.3.14"
 pyo3 = { version = "0.18.3", features = ["extension-module", "abi3", "abi3-py39"] }
 remoteprocess = "0.4.11"
```

### Comparing `perpetuo-0.1.0/LICENSE.APACHE2` & `perpetuo-0.2.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `perpetuo-0.1.0/LICENSE.MIT` & `perpetuo-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `perpetuo-0.1.0/PKG-INFO` & `perpetuo-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.1.0
+Version: 0.2.0
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.1.0/README.md` & `perpetuo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `perpetuo-0.1.0/prep-manylinux-container.sh` & `perpetuo-0.2.0/prep-manylinux-container.sh`

 * *Files identical despite different names*

### Comparing `perpetuo-0.1.0/pyproject.toml` & `perpetuo-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 
 [project]
 name = "perpetuo"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   {name = "Nathaniel J. Smith", email = "njs@pobox.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT OR Apache-2.0"}
 description = "A stall tracker for Python's GIL and Trio tasks"
```

### Comparing `perpetuo-0.1.0/python/perpetuo/_setup.py` & `perpetuo-0.2.0/python/perpetuo/_setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -70,19 +70,11 @@
             instrument_trio()
         except RuntimeError:
             pass
         else:
             did.append("instrumented Trio")
 
     if did:
-        if sys.platform == "darwin" and os.geteuid() != 0:
-            warnings.warn(
-                "Can't start perpetuo watcher automatically on macOS\n"
-                "To watch for stalls, run:\n"
-                f"  sudo perpetuo watch {os.getpid()}",
-                stacklevel=1,
-            )
-        else:
-            start_watcher()
-            did.append("started out of process watcher")
+        start_watcher()
+        did.append("started out of process watcher")
 
     return did
```

### Comparing `perpetuo-0.1.0/python/perpetuo.egg-info/PKG-INFO` & `perpetuo-0.2.0/python/perpetuo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perpetuo
-Version: 0.1.0
+Version: 0.2.0
 Summary: A stall tracker for Python's GIL and Trio tasks
 Author-email: "Nathaniel J. Smith" <njs@pobox.com>
 License: MIT OR Apache-2.0
 Project-URL: repository, https://github.com/njsmith/perpetuo
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
```

### Comparing `perpetuo-0.1.0/src/lib.rs` & `perpetuo-0.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `perpetuo-0.1.0/src/shmem.rs` & `perpetuo-0.2.0/src/shmem.rs`

 * *Files 4% similar despite different names*

```diff
@@ -163,30 +163,19 @@
     slots_ptr: usize,
     slots_count: usize,
     last_updates: Vec<StallTrackerSnapshot>,
     pub spy: py_spy::PythonSpy,
 }
 
 impl PerpetuoProc {
-    // Err means something is broken (or process doesn't exist). Either way, give up.
-    // None means everything is fine but process isn't ready yet (python not yet loaded,
-    // perpetuo instrumentation not yet loaded, etc.)
-    pub fn new(pid: u32, config: &py_spy::Config) -> Result<Option<PerpetuoProc>> {
-        let spy = match py_spy::PythonSpy::new(pid.try_into()?, config) {
-            Ok(spy) => spy,
-            Err(_) => {
-                if remoteprocess::Process::new(pid.try_into()?).is_err() {
-                    bail!("Process {pid} doesn't seem to exist (maybe it exited)");
-                } else {
-                    return Ok(None);
-                }
-            }
-        };
+    pub fn new(pid: u32, config: &py_spy::Config) -> Result<PerpetuoProc> {
+        let spy = py_spy::PythonSpy::new(pid.try_into()?, config)?;
 
         let maps = proc_maps::get_process_maps(pid as proc_maps::Pid)?;
+        let mut read_any = false;
         for map in maps {
             // Exported slots page will be...
             // - exactly one page long
             if map.size() != *PAGE_SIZE {
                 continue;
             }
             // - anonymous
@@ -202,14 +191,15 @@
                 Err(_) => {
                     // Sometimes we fail to read b/c the page is marked
                     // non-readable, e.g. b/c it's a malloc guard page. So this is
                     // normal, not a real error.
                     continue;
                 }
                 Ok(header) => {
+                    read_any = true;
                     if &header.magic != MAGIC {
                         continue;
                     }
                     if header.self_address != map.start() {
                         continue;
                     }
                     // We found it! Can we use it?
@@ -234,24 +224,27 @@
                     let last_updates = slots
                         .into_iter()
                         .map(|stall_tracker| StallTrackerSnapshot {
                             stall_tracker,
                             last_updated: now,
                         })
                         .collect();
-                    return Ok(Some(PerpetuoProc {
+                    return Ok(PerpetuoProc {
                         slots_ptr,
                         slots_count,
                         last_updates,
                         spy,
-                    }));
+                    });
                 }
             };
         }
-        Ok(None)
+        if !read_any {
+            bail!("Couldn't access any process memory -- maybe you need ptrace permission?");
+        }
+        bail!("Couldn't find perpetuo instrumentation (did you enable it?)");
     }
 
     pub fn check_stalls(&mut self) -> Result<Vec<StallReport>> {
         let now = Instant::now();
         let current_slots = self
             .spy
             .process
```

