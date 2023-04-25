# Comparing `tmp/gbd_tools-4.4.7.tar.gz` & `tmp/gbd_tools-4.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.4.7.tar", last modified: Sun Apr 23 09:07:43 2023, max compression
+gzip compressed data, was "gbd_tools-4.4.8.tar", last modified: Tue Apr 25 13:21:52 2023, max compression
```

## Comparing `gbd_tools-4.4.7.tar` & `gbd_tools-4.4.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.7/README.md
--rwxrwxr-x   0 root         (0) root         (0)    11281 2023-04-21 07:57:32.000000 gbd_tools-4.4.7/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.7/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8597 2023-04-23 09:05:25.000000 gbd_tools-4.4.7/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10190 2023-04-20 15:30:43.000000 gbd_tools-4.4.7/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.7/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5786 2023-04-20 15:29:05.000000 gbd_tools-4.4.7/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12276 2023-04-20 15:44:03.000000 gbd_tools-4.4.7/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3333 2023-04-21 07:48:32.000000 gbd_tools-4.4.7/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.7/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.4.7/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.347466 gbd_tools-4.4.7/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.351466 gbd_tools-4.4.7/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.7/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.7/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.7/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.351466 gbd_tools-4.4.7/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.7/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-23 09:07:43.000000 gbd_tools-4.4.7/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.4.7/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 09:07:43.355466 gbd_tools-4.4.7/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-23 09:05:59.000000 gbd_tools-4.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.556314 gbd_tools-4.4.8/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.4.8/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.4.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-25 13:21:52.556314 gbd_tools-4.4.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.4.8/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    11281 2023-04-21 07:57:32.000000 gbd_tools-4.4.8/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.548314 gbd_tools-4.4.8/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.4.8/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8597 2023-04-23 09:05:25.000000 gbd_tools-4.4.8/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.4.8/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10190 2023-04-20 15:30:43.000000 gbd_tools-4.4.8/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     5050 2023-02-07 16:30:01.000000 gbd_tools-4.4.8/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5786 2023-04-20 15:29:05.000000 gbd_tools-4.4.8/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12282 2023-04-25 13:17:48.000000 gbd_tools-4.4.8/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.4.8/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3333 2023-04-21 07:48:32.000000 gbd_tools-4.4.8/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.552314 gbd_tools-4.4.8/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.4.8/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.4.8/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.4.8/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.4.8/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.4.8/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.552314 gbd_tools-4.4.8/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.4.8/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.552314 gbd_tools-4.4.8/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.556314 gbd_tools-4.4.8/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.4.8/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.4.8/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.4.8/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.4.8/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.4.8/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.556314 gbd_tools-4.4.8/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.4.8/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:21:52.556314 gbd_tools-4.4.8/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-04-25 13:21:52.000000 gbd_tools-4.4.8/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-25 13:21:52.000000 gbd_tools-4.4.8/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 13:21:52.000000 gbd_tools-4.4.8/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-25 13:21:52.000000 gbd_tools-4.4.8/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 13:21:52.000000 gbd_tools-4.4.8/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 13:21:52.000000 gbd_tools-4.4.8/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.4.8/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 13:21:52.556314 gbd_tools-4.4.8/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-04-25 13:21:26.000000 gbd_tools-4.4.8/setup.py
```

### Comparing `gbd_tools-4.4.7/LICENSE` & `gbd_tools-4.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/PKG-INFO` & `gbd_tools-4.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.4.7
+Version: 4.4.8
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.7/README.md` & `gbd_tools-4.4.8/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd.py` & `gbd_tools-4.4.8/gbd.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/api.py` & `gbd_tools-4.4.8/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/contexts.py` & `gbd_tools-4.4.8/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/database.py` & `gbd_tools-4.4.8/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/grammar.py` & `gbd_tools-4.4.8/gbd_core/grammar.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/query.py` & `gbd_tools-4.4.8/gbd_core/query.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/schema.py` & `gbd_tools-4.4.8/gbd_core/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             return pair[0]
         else:
             return 'cnf'
 
 
     @classmethod
     def dbname_from_path(cls, path):
-        filename = os.path.basename(path)
+        filename = "_" + os.path.basename(path)
         return re.sub("[^a-zA-Z0-9]", "_", filename)
 
     @classmethod
     def valid_feature_or_raise(cls, name):
         if not re.match("[a-zA-Z][a-zA-Z0-9_]*", name):
             raise SchemaException("Feature name '{}' must be alphanumeric (incl. underline) and start with a letter.".format(name))
         gbd_keywords = [ 'hash', 'value', 'local', 'filename', 'features' ]
```

### Comparing `gbd_tools-4.4.7/gbd_core/util.py` & `gbd_tools-4.4.8/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_core/util_argparse.py` & `gbd_tools-4.4.8/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_init/cnf_extractors.py` & `gbd_tools-4.4.8/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_init/cnf_transformers.py` & `gbd_tools-4.4.8/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_init/gbdhash.py` & `gbd_tools-4.4.8/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_init/initializer.py` & `gbd_tools-4.4.8/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.4.8/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.4.8/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.4.8/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_server/static/main.css` & `gbd_tools-4.4.8/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_server/static/w3.js` & `gbd_tools-4.4.8/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_server/templates/index.html` & `gbd_tools-4.4.8/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.4.8/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.4.7
+Version: 4.4.8
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.4.7/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.4.8/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/server.py` & `gbd_tools-4.4.8/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.4.7/setup.py` & `gbd_tools-4.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.4.7',
+  version='4.4.8',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

