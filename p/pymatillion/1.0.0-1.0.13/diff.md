# Comparing `tmp/pymatillion-1.0.0.tar.gz` & `tmp/pymatillion-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatillion-1.0.0.tar", last modified: Sat Apr 15 00:25:25 2023, max compression
+gzip compressed data, was "pymatillion-1.0.13.tar", last modified: Tue Apr 25 05:49:05 2023, max compression
```

## Comparing `pymatillion-1.0.0.tar` & `pymatillion-1.0.13.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 abhinavyogeshtiwari   (501) staff       (20)        0 2023-04-15 00:25:25.022214 pymatillion-1.0.0/
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)      386 2023-04-15 00:25:25.022003 pymatillion-1.0.0/PKG-INFO
-drwxr-xr-x   0 abhinavyogeshtiwari   (501) staff       (20)        0 2023-04-15 00:25:25.021720 pymatillion-1.0.0/pymatillion.egg-info/
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)      386 2023-04-15 00:25:25.000000 pymatillion-1.0.0/pymatillion.egg-info/PKG-INFO
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)      188 2023-04-15 00:25:25.000000 pymatillion-1.0.0/pymatillion.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)        1 2023-04-15 00:25:25.000000 pymatillion-1.0.0/pymatillion.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)       28 2023-04-15 00:25:25.000000 pymatillion-1.0.0/pymatillion.egg-info/requires.txt
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)       12 2023-04-15 00:25:25.000000 pymatillion-1.0.0/pymatillion.egg-info/top_level.txt
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)      906 2023-04-15 00:24:26.000000 pymatillion-1.0.0/pyproject.toml
--rw-r--r--   0 abhinavyogeshtiwari   (501) staff       (20)       38 2023-04-15 00:25:25.022276 pymatillion-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:49:05.237594 pymatillion-1.0.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-25 05:49:05.237594 pymatillion-1.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 05:48:56.000000 pymatillion-1.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:49:05.237594 pymatillion-1.0.13/pymatillion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-25 05:49:05.000000 pymatillion-1.0.13/pymatillion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 05:49:05.000000 pymatillion-1.0.13/pymatillion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 05:49:05.000000 pymatillion-1.0.13/pymatillion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 05:49:05.000000 pymatillion-1.0.13/pymatillion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 05:49:05.000000 pymatillion-1.0.13/pymatillion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-25 05:48:56.000000 pymatillion-1.0.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 05:49:05.237594 pymatillion-1.0.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:49:05.237594 pymatillion-1.0.13/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-25 05:48:56.000000 pymatillion-1.0.13/tests/test_matillion_client.py
```

### Comparing `pymatillion-1.0.0/pyproject.toml` & `pymatillion-1.0.13/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymatillion"
-version = "1.0.0"
+version = "1.0.13"
+description = "This is a Python wrapper for interacting with the REST API for Matillion."
+readme = "README.md"
 authors = [
     {name = "Abhinav Tiwari", email = "abhinavtiwariusa84@gmail.com"},
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Intended Audience :: Developers",
+
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     "requests",
 ]
 
 [project.optional-dependencies]
-dev = ["black", "isort"]
+dev = ["black", "bumpver", "isort", "build", "twine", "mkdocs"]
 
 [project.urls]
 Homepage = "https://github.com/tiwari-abhi/PyMatillion"
 Docs = "https://tiwari-abhi.github.io/PyMatillion/reference"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.13"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
+    'version = "{version}"',
 ]
 
 [tool.setuptools]
 py-modules = ["pymatillion"]
```

