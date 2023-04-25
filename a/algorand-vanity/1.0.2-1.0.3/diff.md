# Comparing `tmp/algorand_vanity-1.0.2.tar.gz` & `tmp/algorand_vanity-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorand_vanity-1.0.2.tar", max compression
+gzip compressed data, was "algorand_vanity-1.0.3.tar", max compression
```

## Comparing `algorand_vanity-1.0.2.tar` & `algorand_vanity-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-24 22:54:10.705139 algorand_vanity-1.0.2/LICENSE
--rw-r--r--   0        0        0     1044 2023-04-24 23:59:26.397562 algorand_vanity-1.0.2/README.md
--rw-r--r--   0        0        0     6549 2023-04-25 01:41:52.080302 algorand_vanity-1.0.2/algorand_vanity/generator.py
--rw-r--r--   0        0        0      669 2023-04-25 01:42:24.046559 algorand_vanity-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 algorand_vanity-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-24 22:54:10.705139 algorand_vanity-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1045 2023-04-25 01:44:22.570390 algorand_vanity-1.0.3/README.md
+-rw-r--r--   0        0        0     6549 2023-04-25 01:41:52.080302 algorand_vanity-1.0.3/algorand_vanity/generator.py
+-rw-r--r--   0        0        0      669 2023-04-25 01:45:25.159153 algorand_vanity-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 algorand_vanity-1.0.3/PKG-INFO
```

### Comparing `algorand_vanity-1.0.2/LICENSE` & `algorand_vanity-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `algorand_vanity-1.0.2/README.md` & `algorand_vanity-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 Python utility for generating vanity algorand wallet addresses.
 
 ## Installing from source
 ```bash
 poetry install
 ```
 
-##Installing with pip
+## Installing with pip
 ```bash
 pip install algorand-vanity
 ```
 
 ## Usage
 ```bash
-algorand-vanity ADDRESS1 ADDRESS2
+algorand_vanity ADDRESS1 ADDRESS2
 ```
 
 ## Options
 Option | Description | Default
 --- | --- | ---
 --threads, -t {start, end} | Number of threads to use for address generation | # of CPU cores
 --filename, -f {start, end} | Filename to output addresses to | vanity_addresses
```

### Comparing `algorand_vanity-1.0.2/algorand_vanity/generator.py` & `algorand_vanity-1.0.3/algorand_vanity/generator.py`

 * *Files identical despite different names*

### Comparing `algorand_vanity-1.0.2/pyproject.toml` & `algorand_vanity-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "algorand-vanity"
-version = "1.0.2"
+version = "1.0.3"
 description = "Vanity address generator for algorand wallets"
 license = "MIT"
 authors = [ "Kelsey Price <contact@kelsey.dev>"]
 readme = "README.md"
 repository = "https://github.com/sithladyraven/algorand-vanity"
 packages = [{include = "algorand_vanity"}]
 keywords = ["algorand", "crypto", "cryptocurrency", "cryptowallet"]
```

### Comparing `algorand_vanity-1.0.2/PKG-INFO` & `algorand_vanity-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorand-vanity
-Version: 1.0.2
+Version: 1.0.3
 Summary: Vanity address generator for algorand wallets
 Home-page: https://github.com/sithladyraven/algorand-vanity
 License: MIT
 Keywords: algorand,crypto,cryptocurrency,cryptowallet
 Author: Kelsey Price
 Author-email: contact@kelsey.dev
 Requires-Python: >=3.8,<4.0
@@ -25,22 +25,22 @@
 Python utility for generating vanity algorand wallet addresses.
 
 ## Installing from source
 ```bash
 poetry install
 ```
 
-##Installing with pip
+## Installing with pip
 ```bash
 pip install algorand-vanity
 ```
 
 ## Usage
 ```bash
-algorand-vanity ADDRESS1 ADDRESS2
+algorand_vanity ADDRESS1 ADDRESS2
 ```
 
 ## Options
 Option | Description | Default
 --- | --- | ---
 --threads, -t {start, end} | Number of threads to use for address generation | # of CPU cores
 --filename, -f {start, end} | Filename to output addresses to | vanity_addresses
```

