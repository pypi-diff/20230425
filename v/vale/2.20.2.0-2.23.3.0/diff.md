# Comparing `tmp/vale-2.20.2.0.tar.gz` & `tmp/vale-2.23.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vale-python-package/vale-python-package/dist/tmpubvzk6cv/vale-2.20.2.0.tar", last modified: Wed Sep 28 10:18:44 2022, max compression
+gzip compressed data, was "/home/runner/work/vale-python-package/vale-python-package/dist/.tmp-1bsvk_iq/vale-2.23.3.0.tar", last modified: Tue Apr 25 12:02:54 2023, max compression
```

## Comparing `vale-2.20.2.0.tar` & `vale-2.23.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:18:44.000000 vale-2.20.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-28 10:18:35.000000 vale-2.20.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-28 10:18:35.000000 vale-2.20.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-09-28 10:18:44.000000 vale-2.20.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-09-28 10:18:35.000000 vale-2.20.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-09-28 10:18:35.000000 vale-2.20.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 10:18:44.000000 vale-2.20.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 10:18:35.000000 vale-2.20.2.0/vale/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4301 2022-09-28 10:18:35.000000 vale-2.20.2.0/vale/main.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      195 2022-09-28 10:18:35.000000 vale-2.20.2.0/vale/vale_bin
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-28 10:18:44.000000 vale-2.20.2.0/vale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:02:54.000000 vale-2.23.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 12:02:43.000000 vale-2.23.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 12:02:43.000000 vale-2.23.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-25 12:02:54.000000 vale-2.23.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-25 12:02:43.000000 vale-2.23.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-25 12:02:43.000000 vale-2.23.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 12:02:54.000000 vale-2.23.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:02:43.000000 vale-2.23.3.0/vale/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4296 2023-04-25 12:02:43.000000 vale-2.23.3.0/vale/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-04-25 12:02:43.000000 vale-2.23.3.0/vale/vale_bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 12:02:54.000000 vale-2.23.3.0/vale.egg-info/top_level.txt
```

### Comparing `vale-2.20.2.0/LICENSE` & `vale-2.23.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vale-2.20.2.0/PKG-INFO` & `vale-2.23.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vale
-Version: 2.20.2.0
+Version: 2.23.3.0
 Summary: Install and use Vale (grammar & style check tool) in python environments.
 Author: Dani Perez
 License: MIT
 Project-URL: Homepage, https://github.com/daniperez/vale-python-package
 Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vale-2.20.2.0/README.md` & `vale-2.23.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vale-2.20.2.0/pyproject.toml` & `vale-2.23.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [project]
 name="vale"
 # This version corresponds to the original Vale's version, plus a 4th number to
 # account for fixes to this package. That 4th number is needed because PyPi
 # doesn't allow to re-release or upload deleted versions, every uploaded
 # version must be unique.
-version = "2.20.2.0"
+version = "2.23.3.0"
 authors = [
   { name="Dani Perez"},
 ]
 description = "Install and use Vale (grammar & style check tool) in python environments."
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
```

### Comparing `vale-2.20.2.0/vale/main.py` & `vale-2.23.3.0/vale/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     elif sys.platform.startswith("darwin"):
         operating_system = "macOS"
     elif sys.platform.startswith("win32"):
         operating_system = "Windows"
 
     if os.uname().machine.startswith("x86_64"):
         architecture = "64-bit"
-    elif os.uname().architecture.startswith("arm"):
+    elif os.uname().machine.startswith("arm"):
         # This is a loose match. Theoretical valid values:
         # aarch64_be, aarch64, armv8b, armv8, larm64.
         # I need confirmation.
         architecture = "arm64"
 
     if not operating_system:
         raise RuntimeError(
```

### Comparing `vale-2.20.2.0/vale.egg-info/PKG-INFO` & `vale-2.23.3.0/vale.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vale
-Version: 2.20.2.0
+Version: 2.23.3.0
 Summary: Install and use Vale (grammar & style check tool) in python environments.
 Author: Dani Perez
 License: MIT
 Project-URL: Homepage, https://github.com/daniperez/vale-python-package
 Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

