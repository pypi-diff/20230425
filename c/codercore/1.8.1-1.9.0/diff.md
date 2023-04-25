# Comparing `tmp/codercore-1.8.1.tar.gz` & `tmp/codercore-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codercore-1.8.1.tar", last modified: Wed Feb 15 09:50:02 2023, max compression
+gzip compressed data, was "codercore-1.9.0.tar", last modified: Thu Mar 16 16:04:26 2023, max compression
```

## Comparing `codercore-1.8.1.tar` & `codercore-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.491005 codercore-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-15 09:50:02.491005 codercore-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-15 09:49:25.000000 codercore-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.483004 codercore-1.8.1/codercore/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.487004 codercore-1.8.1/codercore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.487004 codercore-1.8.1/codercore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.487004 codercore-1.8.1/codercore/lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/schemas/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.491005 codercore-1.8.1/codercore/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-15 09:49:25.000000 codercore-1.8.1/codercore/test/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:50:02.483004 codercore-1.8.1/codercore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-15 09:50:02.000000 codercore-1.8.1/codercore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-15 09:50:02.000000 codercore-1.8.1/codercore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:50:02.000000 codercore-1.8.1/codercore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-15 09:50:02.000000 codercore-1.8.1/codercore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-15 09:50:02.000000 codercore-1.8.1/codercore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-15 09:49:25.000000 codercore-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 09:50:02.491005 codercore-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.577226 codercore-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-16 16:04:26.577226 codercore-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-16 16:03:59.000000 codercore-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore/lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/schemas/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.577226 codercore-1.9.0/codercore/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-16 16:03:59.000000 codercore-1.9.0/codercore/test/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:04:26.573226 codercore-1.9.0/codercore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 16:04:26.000000 codercore-1.9.0/codercore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-16 16:03:59.000000 codercore-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:04:26.577226 codercore-1.9.0/setup.cfg
```

### Comparing `codercore-1.8.1/codercore/db/__init__.py` & `codercore-1.9.0/codercore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `codercore-1.8.1/codercore/lib/hash.py` & `codercore-1.9.0/codercore/lib/hash.py`

 * *Files identical despite different names*

### Comparing `codercore-1.8.1/codercore/lib/settings.py` & `codercore-1.9.0/codercore/lib/settings.py`

 * *Files identical despite different names*

### Comparing `codercore-1.8.1/codercore/test/fixtures.py` & `codercore-1.9.0/codercore/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `codercore-1.8.1/codercore/test/pydantic.py` & `codercore-1.9.0/codercore/test/pydantic.py`

 * *Files identical despite different names*

### Comparing `codercore-1.8.1/codercore.egg-info/SOURCES.txt` & `codercore-1.9.0/codercore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codercore-1.8.1/pyproject.toml` & `codercore-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codercore"
-version = "1.8.1"
+version = "1.9.0"
 description = "codercore"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'asyncpg ~= 0.27',
     'bcrypt ~= 4.0',
     'cloud-sql-python-connector[asyncpg] ~= 1.1',
@@ -30,15 +30,15 @@
 dev = [
     'black ~= 22.10',
     'flake8 ~= 6.0',
     'isort ~= 5.11',
 ]
 
 [tool.bumpver]
-current_version = "1.8.1"
+current_version = "1.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

