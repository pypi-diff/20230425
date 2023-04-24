# Comparing `tmp/tom_hermes-0.1.5.tar.gz` & `tmp/tom_hermes-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_hermes-0.1.5.tar", max compression
+gzip compressed data, was "tom_hermes-0.1.7.tar", max compression
```

## Comparing `tom_hermes-0.1.5.tar` & `tom_hermes-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-21 06:47:36.709084 tom_hermes-0.1.5/LICENSE
--rw-r--r--   0        0        0       52 2023-04-21 06:47:36.709084 tom_hermes-0.1.5/README.md
--rw-r--r--   0        0        0     1265 2023-04-21 06:48:03.333259 tom_hermes-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       96 2023-04-21 06:48:03.333259 tom_hermes-0.1.5/tom_hermes/__init__.py
--rw-r--r--   0        0        0    11280 2023-04-21 06:47:36.709084 tom_hermes-0.1.5/tom_hermes/hermes.py
--rw-r--r--   0        0        0     2828 2023-04-21 06:47:36.709084 tom_hermes-0.1.5/tom_hermes/templates/tom_hermes/query_result.html
--rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 tom_hermes-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1363 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/README.md
+-rw-r--r--   0        0        0     1265 2023-04-24 23:51:51.655861 tom_hermes-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-04-24 23:51:51.655861 tom_hermes-0.1.7/tom_hermes/__init__.py
+-rw-r--r--   0        0        0    11280 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/tom_hermes/hermes.py
+-rw-r--r--   0        0        0     2828 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/tom_hermes/templates/tom_hermes/query_result.html
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 tom_hermes-0.1.7/PKG-INFO
```

### Comparing `tom_hermes-0.1.5/LICENSE` & `tom_hermes-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_hermes-0.1.5/pyproject.toml` & `tom_hermes-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tom-hermes"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.1.5"
+version = "0.1.7"
 description = "A TOM Toolkit Broker module for querying the Hermes Alert API"
 authors = ["Lindy Lindstrom <llindstrom@lco.global>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 packages = [{include = "tom_hermes"}]
```

### Comparing `tom_hermes-0.1.5/tom_hermes/hermes.py` & `tom_hermes-0.1.7/tom_hermes/hermes.py`

 * *Files identical despite different names*

### Comparing `tom_hermes-0.1.5/tom_hermes/templates/tom_hermes/query_result.html` & `tom_hermes-0.1.7/tom_hermes/templates/tom_hermes/query_result.html`

 * *Files identical despite different names*

