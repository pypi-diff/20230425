# Comparing `tmp/edman_web-2023.4.4.1.tar.gz` & `tmp/edman_web-2023.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2023.4.4.1.tar", last modified: Tue Apr  4 06:23:03 2023, max compression
+gzip compressed data, was "edman_web-2023.4.5.tar", last modified: Wed Apr  5 05:26:27 2023, max compression
```

## Comparing `edman_web-2023.4.4.1.tar` & `edman_web-2023.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-04 06:23:03.483284 edman_web-2023.4.4.1/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.4.4.1/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2023-03-29 09:20:48.000000 edman_web-2023.4.4.1/MANIFEST.in
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1092 2023-04-04 06:23:03.483284 edman_web-2023.4.4.1/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.4.4.1/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-04 06:23:03.483284 edman_web-2023.4.4.1/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.4.4.1/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5632 2023-04-04 05:55:42.000000 edman_web-2023.4.4.1/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.4.4.1/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-04 06:23:03.483284 edman_web-2023.4.4.1/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1092 2023-04-04 06:23:03.000000 edman_web-2023.4.4.1/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      349 2023-04-04 06:23:03.000000 edman_web-2023.4.4.1/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-04-04 06:23:03.000000 edman_web-2023.4.4.1/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       62 2023-04-04 06:23:03.000000 edman_web-2023.4.4.1/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       10 2023-04-04 06:23:03.000000 edman_web-2023.4.4.1/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      716 2023-04-04 06:23:03.493284 edman_web-2023.4.4.1/setup.cfg
--rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2023-03-29 09:20:48.000000 edman_web-2023.4.4.1/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-04 06:23:03.483284 edman_web-2023.4.4.1/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    12368 2023-04-04 05:55:42.000000 edman_web-2023.4.4.1/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.4.4.1/tests/test_search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2023.4.5/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2023-03-29 09:20:48.000000 edman_web-2023.4.5/MANIFEST.in
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-04-05 05:26:27.278967 edman_web-2023.4.5/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      626 2023-03-30 03:11:16.000000 edman_web-2023.4.5/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       80 2023-04-04 05:55:42.000000 edman_web-2023.4.5/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5632 2023-04-04 05:55:42.000000 edman_web-2023.4.5/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2639 2023-03-29 09:20:48.000000 edman_web-2023.4.5/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1090 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      349 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       61 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       10 2023-04-05 05:26:27.000000 edman_web-2023.4.5/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      713 2023-04-05 05:26:27.278967 edman_web-2023.4.5/setup.cfg
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       41 2023-03-29 09:20:48.000000 edman_web-2023.4.5/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-04-05 05:26:27.278967 edman_web-2023.4.5/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    12368 2023-04-04 05:55:42.000000 edman_web-2023.4.5/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5059 2023-04-04 05:55:42.000000 edman_web-2023.4.5/tests/test_search_manager.py
```

### Comparing `edman_web-2023.4.4.1/LICENSE.txt` & `edman_web-2023.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.4.1/PKG-INFO` & `edman_web-2023.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2023.4.4.1
+Version: 2023.4.5
 Summary: sub-package of edman for web applications.
 Home-page: https://github.com/ryde/edman_web
 Author: Masaki Ohno
 Author-email: masakio@post.kek.jp
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
```

### Comparing `edman_web-2023.4.4.1/README.rst` & `edman_web-2023.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.4.1/edman_web/file_manager.py` & `edman_web-2023.4.5/edman_web/file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.4.1/edman_web/search_manager.py` & `edman_web-2023.4.5/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.4.1/edman_web.egg-info/PKG-INFO` & `edman_web-2023.4.5/edman_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman-web
-Version: 2023.4.4.1
+Version: 2023.4.5
 Summary: sub-package of edman for web applications.
 Home-page: https://github.com/ryde/edman_web
 Author: Masaki Ohno
 Author-email: masakio@post.kek.jp
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
```

### Comparing `edman_web-2023.4.4.1/setup.cfg` & `edman_web-2023.4.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edman_web
-version = 2023.4.4.1
+version = 2023.4.5
 author = Masaki Ohno
 author_email = masakio@post.kek.jp
 license = MIT License
 description = sub-package of edman for web applications.
 url = https://github.com/ryde/edman_web
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -16,17 +16,17 @@
 
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.11
 install_requires = 
 	pymongo>=4.3.3
-	edman>=2023.3.15
+	edman>=2023.4.5
 	Werkzeug>=2.2.3
-	Pillow>=9.4.0
+	Pillow>=9.5.0
 
 [options.packages.find]
 exclude = 
 	tests
 
 [egg_info]
 tag_build =
```

### Comparing `edman_web-2023.4.4.1/tests/test_file_manager.py` & `edman_web-2023.4.5/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2023.4.4.1/tests/test_search_manager.py` & `edman_web-2023.4.5/tests/test_search_manager.py`

 * *Files identical despite different names*

