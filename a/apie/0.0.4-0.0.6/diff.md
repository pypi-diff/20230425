# Comparing `tmp/apie-0.0.4.tar.gz` & `tmp/apie-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apie-0.0.4.tar", last modified: Thu Apr  6 23:00:34 2023, max compression
+gzip compressed data, was "apie-0.0.6.tar", last modified: Mon Apr 24 23:05:55 2023, max compression
```

## Comparing `apie-0.0.4.tar` & `apie-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 23:00:34.947008 apie-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-06 23:00:34.947008 apie-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-06 23:00:16.000000 apie-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 23:00:34.943008 apie-0.0.4/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 23:00:34.943008 apie-0.0.4/pkg/apie/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 23:00:25.000000 apie-0.0.4/pkg/apie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 23:00:25.000000 apie-0.0.4/pkg/apie/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 23:00:34.947008 apie-0.0.4/pkg/apie/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 23:00:25.000000 apie-0.0.4/pkg/apie/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-06 23:00:09.000000 apie-0.0.4/pkg/apie/api/api_hack.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-06 23:00:09.000000 apie-0.0.4/pkg/apie/api/api_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-06 23:00:09.000000 apie-0.0.4/pkg/apie/api/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-06 23:00:25.000000 apie-0.0.4/pkg/apie/apie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 23:00:34.947008 apie-0.0.4/pkg/apie/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 23:00:25.000000 apie-0.0.4/pkg/apie/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-06 23:00:09.000000 apie-0.0.4/pkg/apie/auth/auth_from_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-06 23:00:09.000000 apie-0.0.4/pkg/apie/auth/auth_noauth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 23:00:34.947008 apie-0.0.4/pkg/apie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-06 23:00:34.000000 apie-0.0.4/pkg/apie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-06 23:00:34.000000 apie-0.0.4/pkg/apie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 23:00:34.000000 apie-0.0.4/pkg/apie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-06 23:00:34.000000 apie-0.0.4/pkg/apie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-06 23:00:34.000000 apie-0.0.4/pkg/apie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 23:00:34.000000 apie-0.0.4/pkg/apie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-06 23:00:25.000000 apie-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-06 23:00:34.947008 apie-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-24 23:05:55.427378 apie-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-24 23:05:38.000000 apie-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.423378 apie-0.0.6/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/api/api_hack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/api/api_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/api/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16245 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/apie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:46.000000 apie-0.0.6/pkg/apie/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/auth/auth_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 23:05:31.000000 apie-0.0.6/pkg/apie/auth/auth_noauth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:05:55.427378 apie-0.0.6/pkg/apie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 23:05:55.000000 apie-0.0.6/pkg/apie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 23:05:46.000000 apie-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 23:05:55.427378 apie-0.0.6/setup.cfg
```

### Comparing `apie-0.0.4/PKG-INFO` & `apie-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apie
-Version: 0.0.4
+Version: 0.0.6
 Summary: Application Program Interface with eons
 Home-page: https://github.com/eons-dev/bin_apie
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_apie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `apie-0.0.4/README.md` & `apie-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apie-0.0.4/pkg/apie/api/api_hack.py` & `apie-0.0.6/pkg/apie/api/api_hack.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.4/pkg/apie/api/api_help.py` & `apie-0.0.6/pkg/apie/api/api_help.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.4/pkg/apie/api/api_multi.py` & `apie-0.0.6/pkg/apie/api/api_multi.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.4/pkg/apie/apie.py` & `apie-0.0.6/pkg/apie/apie.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 		super().__init__(name="Application Program Interface with Eons", descriptionStr="A readily extensible take on APIs.")
 
 		# this.RegisterDirectory("ebbs")
 
 		this.optionalKWArgs['host'] = "0.0.0.0"
 		this.optionalKWArgs['port'] = 80
 		this.optionalKWArgs['dev'] = False
-		this.optionalKWArgs['clean_start'] = True
+		this.optionalKWArgs['clean_start'] = False
 		this.optionalKWArgs['authenticator'] = "noauth"
 		this.optionalKWArgs['preprocessor'] = ""
 
 		this.supportedMethods = [
 			'POST',
 			'GET',
 			'PUT',
```

### Comparing `apie-0.0.4/pkg/apie/auth/auth_from_config.py` & `apie-0.0.6/pkg/apie/auth/auth_from_config.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.4/pkg/apie/auth/auth_noauth.py` & `apie-0.0.6/pkg/apie/auth/auth_noauth.py`

 * *Files identical despite different names*

### Comparing `apie-0.0.4/pkg/apie.egg-info/PKG-INFO` & `apie-0.0.6/pkg/apie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apie
-Version: 0.0.4
+Version: 0.0.6
 Summary: Application Program Interface with eons
 Home-page: https://github.com/eons-dev/bin_apie
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_apie/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `apie-0.0.4/setup.cfg` & `apie-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apie
-version = 0.0.4
+version = 0.0.6
 author = eons
 author_email = support@eons.llc
 description = Application Program Interface with eons
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_apie
@@ -18,18 +18,18 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	eons
+	flask
 	waitress
+	eons
 	jsonpickle
-	flask
 
 [options.packages.find]
 where = pkg
 
 [options.entry_points]
 console_scripts = 
 	apie = apie:apie
```

