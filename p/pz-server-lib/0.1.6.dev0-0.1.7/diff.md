# Comparing `tmp/pz-server-lib-0.1.6.dev0.tar.gz` & `tmp/pz-server-lib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-server-lib-0.1.6.dev0.tar", last modified: Mon Nov  7 20:23:09 2022, max compression
+gzip compressed data, was "pz-server-lib-0.1.7.tar", last modified: Tue Apr 25 12:10:19 2023, max compression
```

## Comparing `pz-server-lib-0.1.6.dev0.tar` & `pz-server-lib-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:23:09.934673 pz-server-lib-0.1.6.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-11-07 20:23:09.934673 pz-server-lib-0.1.6.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:23:09.934673 pz-server-lib-0.1.6.dev0/pz_server/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/pz_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12835 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/pz_server/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8783 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/pz_server/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/pz_server/pz_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:23:09.934673 pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-11-07 20:23:09.000000 pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-07 20:23:09.000000 pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:23:09.000000 pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-07 20:23:09.000000 pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-07 20:23:09.000000 pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-07 20:23:09.938673 pz-server-lib-0.1.6.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-11-07 20:22:15.000000 pz-server-lib-0.1.6.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:10:19.361877 pz-server-lib-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 12:10:19.361877 pz-server-lib-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:10:19.357877 pz-server-lib-0.1.7/pz_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/pz_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16351 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/pz_server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/pz_server/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14397 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/pz_server/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:10:19.361877 pz-server-lib-0.1.7/pz_server_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 12:10:19.000000 pz-server-lib-0.1.7/pz_server_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-25 12:10:19.000000 pz-server-lib-0.1.7/pz_server_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:10:19.000000 pz-server-lib-0.1.7/pz_server_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 12:10:19.000000 pz-server-lib-0.1.7/pz_server_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 12:10:19.000000 pz-server-lib-0.1.7/pz_server_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 12:10:19.361877 pz-server-lib-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:10:19.361877 pz-server-lib-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-25 12:09:53.000000 pz-server-lib-0.1.7/tests/test_get_products.py
```

### Comparing `pz-server-lib-0.1.6.dev0/LICENSE` & `pz-server-lib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-server-lib-0.1.6.dev0/PKG-INFO` & `pz-server-lib-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-server-lib
-Version: 0.1.6.dev0
+Version: 0.1.7
 Summary: Python library to access the Photo-z Server database hosted by the Brazilian LSST IDAC at LIneA. 
 Home-page: https://github.com/linea-it/pz-server-lib
 License: MIT
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pz-server-lib-0.1.6.dev0/README.md` & `pz-server-lib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pz-server-lib-0.1.6.dev0/pz_server_lib.egg-info/PKG-INFO` & `pz-server-lib-0.1.7/pz_server_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-server-lib
-Version: 0.1.6.dev0
+Version: 0.1.7
 Summary: Python library to access the Photo-z Server database hosted by the Brazilian LSST IDAC at LIneA. 
 Home-page: https://github.com/linea-it/pz-server-lib
 License: MIT
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pz-server-lib-0.1.6.dev0/setup.py` & `pz-server-lib-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="pz-server-lib",
     packages=find_packages(include=["pz_server"]),
-    version="0.1.6.dev",
+    version="0.1.7",
     description=(
         "Python library to access the Photo-z Server database"
         " hosted by the Brazilian LSST IDAC at LIneA. "
     ),
     license="MIT",
     python_requires=">=3.9, <4",
     setup_requires=["pytest-runner", "numpy", "astropy"],
     install_requires=[
-        "numpy>=1.19.4",
+        "numpy>=1.23, <1.24",
         "pandas>=1.2.0",
         "requests>=2.23.0",
         "astropy>=5.0.0",
         "matplotlib>=3.6.0",
         "tables_io >=0.7.9",
         "Jinja2>=3.1.2",
         "ipython>=8.5.0"
```

