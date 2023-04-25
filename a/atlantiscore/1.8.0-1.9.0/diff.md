# Comparing `tmp/atlantiscore-1.8.0.tar.gz` & `tmp/atlantiscore-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantiscore-1.8.0.tar", last modified: Fri Feb 17 10:49:18 2023, max compression
+gzip compressed data, was "atlantiscore-1.9.0.tar", last modified: Thu Mar 16 16:10:57 2023, max compression
```

## Comparing `atlantiscore-1.8.0.tar` & `atlantiscore-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.455803 atlantiscore-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-17 10:49:18.455803 atlantiscore-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.447803 atlantiscore-1.8.0/atlantiscore/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.451803 atlantiscore-1.8.0/atlantiscore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.451803 atlantiscore-1.8.0/atlantiscore/db/types/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/db/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/db/types/evm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.451803 atlantiscore-1.8.0/atlantiscore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.455803 atlantiscore-1.8.0/atlantiscore/types/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/types/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/atlantiscore/types/key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.451803 atlantiscore-1.8.0/atlantiscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-17 10:49:18.000000 atlantiscore-1.8.0/atlantiscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-17 10:49:18.000000 atlantiscore-1.8.0/atlantiscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 10:49:18.000000 atlantiscore-1.8.0/atlantiscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-17 10:49:18.000000 atlantiscore-1.8.0/atlantiscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-17 10:49:18.000000 atlantiscore-1.8.0/atlantiscore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 10:49:18.455803 atlantiscore-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:49:18.455803 atlantiscore-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-17 10:48:43.000000 atlantiscore-1.8.0/tests/test_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.522632 atlantiscore-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-16 16:10:57.522632 atlantiscore-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.514632 atlantiscore-1.9.0/atlantiscore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.518632 atlantiscore-1.9.0/atlantiscore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.518632 atlantiscore-1.9.0/atlantiscore/db/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/db/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/db/types/evm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.518632 atlantiscore-1.9.0/atlantiscore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.518632 atlantiscore-1.9.0/atlantiscore/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/types/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/atlantiscore/types/key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.518632 atlantiscore-1.9.0/atlantiscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-16 16:10:57.000000 atlantiscore-1.9.0/atlantiscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-16 16:10:57.000000 atlantiscore-1.9.0/atlantiscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:10:57.000000 atlantiscore-1.9.0/atlantiscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-16 16:10:57.000000 atlantiscore-1.9.0/atlantiscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-16 16:10:57.000000 atlantiscore-1.9.0/atlantiscore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:10:57.522632 atlantiscore-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:10:57.518632 atlantiscore-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-16 16:10:28.000000 atlantiscore-1.9.0/tests/test_finder.py
```

### Comparing `atlantiscore-1.8.0/atlantiscore/__init__.py` & `atlantiscore-1.9.0/atlantiscore/__init__.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-1.8.0/atlantiscore/db/types/evm.py` & `atlantiscore-1.9.0/atlantiscore/db/types/evm.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-1.8.0/atlantiscore/types/evm.py` & `atlantiscore-1.9.0/atlantiscore/types/evm.py`

 * *Files identical despite different names*

### Comparing `atlantiscore-1.8.0/pyproject.toml` & `atlantiscore-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlantiscore"
-version = "1.8.0"
+version = "1.9.0"
 description = "atlantiscore"
 readme = "README.md"
 authors = [{ name = "Atlantis Labs", email = "r00tail@protonmail.com" }]
 dependencies = [
-    "codercore ~= 1.8",
+    "codercore ~= 1.9",
     "coincurve ~= 18.0",
     "eth-hash[pycryptodome]~=0.5",
     "eth-utils ~= 2.1",
     "sqlalchemy[asyncio] ~= 1.4",
 ]
 
 [project.optional-dependencies]
@@ -31,15 +31,15 @@
     "flake8 ~= 6.0",
     "isort ~= 5.12",
     "pre-commit ~= 2.21",
 ]
 
 
 [tool.bumpver]
-current_version = "1.8.0"
+current_version = "1.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `atlantiscore-1.8.0/tests/test_finder.py` & `atlantiscore-1.9.0/tests/test_finder.py`

 * *Files identical despite different names*

