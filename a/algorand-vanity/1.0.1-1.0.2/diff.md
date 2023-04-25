# Comparing `tmp/algorand_vanity-1.0.1.tar.gz` & `tmp/algorand_vanity-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorand_vanity-1.0.1.tar", max compression
+gzip compressed data, was "algorand_vanity-1.0.2.tar", max compression
```

## Comparing `algorand_vanity-1.0.1.tar` & `algorand_vanity-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-24 22:54:10.705139 algorand_vanity-1.0.1/LICENSE
--rw-r--r--   0        0        0     1044 2023-04-24 23:59:26.397562 algorand_vanity-1.0.1/README.md
--rw-r--r--   0        0        0     6692 2023-04-25 00:56:40.396246 algorand_vanity-1.0.1/algorand_vanity/generator.py
--rw-r--r--   0        0        0      669 2023-04-25 00:56:57.477890 algorand_vanity-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 algorand_vanity-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-24 22:54:10.705139 algorand_vanity-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1044 2023-04-24 23:59:26.397562 algorand_vanity-1.0.2/README.md
+-rw-r--r--   0        0        0     6549 2023-04-25 01:41:52.080302 algorand_vanity-1.0.2/algorand_vanity/generator.py
+-rw-r--r--   0        0        0      669 2023-04-25 01:42:24.046559 algorand_vanity-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 algorand_vanity-1.0.2/PKG-INFO
```

### Comparing `algorand_vanity-1.0.1/LICENSE` & `algorand_vanity-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `algorand_vanity-1.0.1/README.md` & `algorand_vanity-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `algorand_vanity-1.0.1/algorand_vanity/generator.py` & `algorand_vanity-1.0.2/algorand_vanity/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,14 @@
 
 def signal_handler(sig, frame):
     terminate_processes(processes)
     end_curses()
     exit()
 
 
-def worker_handler(sig, frame):
-    exit()
-
 
 def terminate_processes(processes):
     for proc in processes:
         proc.terminate()
 
 
 def check(vanity_str):
@@ -88,16 +85,14 @@
 
 
 def get_mnemonic(private_key):
     return mnemonic.from_private_key(private_key)
 
 
 def generate_address(attempts, results, filename, output_lock):
-    signal.signal(signal.SIGINT, worker_handler)
-    signal.signal(signal.SIGTERM, worker_handler)
     count = 0
     cont = True
 
     vanities = results.keys()
 
     while cont:
         count = count + 1
```

### Comparing `algorand_vanity-1.0.1/pyproject.toml` & `algorand_vanity-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "algorand-vanity"
-version = "1.0.1"
+version = "1.0.2"
 description = "Vanity address generator for algorand wallets"
 license = "MIT"
 authors = [ "Kelsey Price <contact@kelsey.dev>"]
 readme = "README.md"
 repository = "https://github.com/sithladyraven/algorand-vanity"
 packages = [{include = "algorand_vanity"}]
 keywords = ["algorand", "crypto", "cryptocurrency", "cryptowallet"]
```

### Comparing `algorand_vanity-1.0.1/PKG-INFO` & `algorand_vanity-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorand-vanity
-Version: 1.0.1
+Version: 1.0.2
 Summary: Vanity address generator for algorand wallets
 Home-page: https://github.com/sithladyraven/algorand-vanity
 License: MIT
 Keywords: algorand,crypto,cryptocurrency,cryptowallet
 Author: Kelsey Price
 Author-email: contact@kelsey.dev
 Requires-Python: >=3.8,<4.0
```

