# Comparing `tmp/algorand_vanity-0.1.0.tar.gz` & `tmp/algorand_vanity-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algorand_vanity-0.1.0.tar", max compression
+gzip compressed data, was "algorand_vanity-1.0.1.tar", max compression
```

## Comparing `algorand_vanity-0.1.0.tar` & `algorand_vanity-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-04-24 22:54:10.705139 algorand_vanity-0.1.0/LICENSE
--rw-r--r--   0        0        0     1044 2023-04-24 23:59:26.397562 algorand_vanity-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-24 23:50:08.305745 algorand_vanity-0.1.0/algorand_vanity/__init__.py
--rw-r--r--   0        0        0      790 2023-04-25 00:16:04.423004 algorand_vanity-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 algorand_vanity-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-24 22:54:10.705139 algorand_vanity-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1044 2023-04-24 23:59:26.397562 algorand_vanity-1.0.1/README.md
+-rw-r--r--   0        0        0     6692 2023-04-25 00:56:40.396246 algorand_vanity-1.0.1/algorand_vanity/generator.py
+-rw-r--r--   0        0        0      669 2023-04-25 00:56:57.477890 algorand_vanity-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 algorand_vanity-1.0.1/PKG-INFO
```

### Comparing `algorand_vanity-0.1.0/LICENSE` & `algorand_vanity-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `algorand_vanity-0.1.0/README.md` & `algorand_vanity-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `algorand_vanity-0.1.0/pyproject.toml` & `algorand_vanity-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [tool.poetry]
 name = "algorand-vanity"
-version = "0.1.0"
+version = "1.0.1"
 description = "Vanity address generator for algorand wallets"
 license = "MIT"
 authors = [ "Kelsey Price <contact@kelsey.dev>"]
 readme = "README.md"
 repository = "https://github.com/sithladyraven/algorand-vanity"
 packages = [{include = "algorand_vanity"}]
 keywords = ["algorand", "crypto", "cryptocurrency", "cryptowallet"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 py-algorand-sdk = "^2.1.2"
 windows-curses = {version = "^2.3.1", platform = "linux"}
 
 [tool.poetry.scripts]
-algorand-vanity = "algorand_vanity:main"
+algorand_vanity = "algorand_vanity.generator:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `algorand_vanity-0.1.0/PKG-INFO` & `algorand_vanity-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algorand-vanity
-Version: 0.1.0
+Version: 1.0.1
 Summary: Vanity address generator for algorand wallets
 Home-page: https://github.com/sithladyraven/algorand-vanity
 License: MIT
 Keywords: algorand,crypto,cryptocurrency,cryptowallet
 Author: Kelsey Price
 Author-email: contact@kelsey.dev
 Requires-Python: >=3.8,<4.0
```

