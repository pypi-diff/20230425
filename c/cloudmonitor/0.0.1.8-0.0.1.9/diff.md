# Comparing `tmp/cloudmonitor-0.0.1.8.tar.gz` & `tmp/cloudmonitor-0.0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmonitor-0.0.1.8.tar", last modified: Mon Apr 24 14:48:59 2023, max compression
+gzip compressed data, was "dist/cloudmonitor-0.0.1.9.tar", last modified: Tue Apr 25 05:53:24 2023, max compression
```

## Comparing `cloudmonitor-0.0.1.8.tar` & `cloudmonitor-0.0.1.9.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1044 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      284 2023-04-23 14:47:47.000000 cloudmonitor-0.0.1.8/README.md
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/cloudmonitor/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-24 14:48:57.000000 cloudmonitor-0.0.1.8/cloudmonitor/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.8/cloudmonitor/__main__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2683 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.8/cloudmonitor/config.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2139 2023-04-24 14:48:11.000000 cloudmonitor-0.0.1.8/cloudmonitor/server.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/cloudmonitor/ssh/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.8/cloudmonitor/ssh/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1135 2023-04-23 14:10:51.000000 cloudmonitor-0.0.1.8/cloudmonitor/ssh/client.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/cloudmonitor/status/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.8/cloudmonitor/status/__init__.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.8/cloudmonitor/status/define.py
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.8/cloudmonitor/status/query.py
-drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1044 2023-04-24 14:48:59.000000 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/PKG-INFO
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      479 2023-04-24 14:48:59.000000 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-24 14:48:59.000000 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       85 2023-04-24 14:48:59.000000 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/entry_points.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       41 2023-04-24 14:48:59.000000 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/requires.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-24 14:48:59.000000 cloudmonitor-0.0.1.8/cloudmonitor.egg-info/top_level.txt
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-24 14:48:59.271594 cloudmonitor-0.0.1.8/setup.cfg
--rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2539 2023-04-24 13:17:17.000000 cloudmonitor-0.0.1.8/setup.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       86 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/entry_points.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1112 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       41 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/requires.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)        1 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      525 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       13 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor.egg-info/top_level.txt
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       37 2023-04-25 05:53:10.000000 cloudmonitor-0.0.1.9/MANIFEST.in
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       49 2023-04-25 05:48:46.000000 cloudmonitor-0.0.1.9/cloudmonitor/__init__.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/ssh/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       22 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/ssh/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1135 2023-04-23 14:10:51.000000 cloudmonitor-0.0.1.9/cloudmonitor/ssh/client.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2786 2023-04-25 05:38:08.000000 cloudmonitor-0.0.1.9/cloudmonitor/config.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2139 2023-04-24 14:48:11.000000 cloudmonitor-0.0.1.9/cloudmonitor/server.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       64 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/__main__.py
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/templates/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     9262 2023-04-24 14:09:06.000000 cloudmonitor-0.0.1.9/cloudmonitor/templates/index.html
+drwxr-xr-x   0 wnjxyk    (1000) wnjxyk    (1000)        0 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       21 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/__init__.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      630 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/define.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2327 2023-04-23 13:11:47.000000 cloudmonitor-0.0.1.9/cloudmonitor/status/query.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     1112 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/PKG-INFO
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)     2714 2023-04-25 05:52:04.000000 cloudmonitor-0.0.1.9/setup.py
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)      284 2023-04-23 14:47:47.000000 cloudmonitor-0.0.1.9/README.md
+-rw-r--r--   0 wnjxyk    (1000) wnjxyk    (1000)       38 2023-04-25 05:53:24.000000 cloudmonitor-0.0.1.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cloudmonitor-0.0.1.8/PKG-INFO` & `cloudmonitor-0.0.1.9/cloudmonitor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: A Web-GUI Monitor for Academic Linux Servers
 Home-page: https://github.com/WNJXYK/cloudmonitor
+Author: Zhi Zhou
+Author-email: wnjxyk@gmail.com
 License: MIT Licence
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,7 +24,9 @@
 ![pypi](https://badgen.net/pypi/v/cloudmonitor)
 ![visitors](https://visitor-badge.glitch.me/badge?page_id=WNJXYK.cloudmonitor)
 [![Downloads](https://pepy.tech/badge/cloudmonitor)](https://pepy.tech/project/cloudmonitor)
 
 ### ATTENTION!
 
 This project is currently under development…
+
+
```

### Comparing `cloudmonitor-0.0.1.8/cloudmonitor/config.py` & `cloudmonitor-0.0.1.9/cloudmonitor/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -80,17 +80,19 @@
 
 def load_args(args):
     C.workers = args.workers
     C.port = args.port
 
 
 ROOT_DIRPATH = os.path.dirname(os.path.abspath(__file__))
+TEMPLATE_PATH = os.path.join(os.path.expanduser('~'), "templates")
 
 _DEFAULT_CONFIG = {
     "root_path": ROOT_DIRPATH,
+    "template_path": TEMPLATE_PATH,
     "servers": {},
     "refresh": 60,
     "status": {},
     "workers": 4,
     "port": 8899,
 }
```

### Comparing `cloudmonitor-0.0.1.8/cloudmonitor/server.py` & `cloudmonitor-0.0.1.9/cloudmonitor/server.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.8/cloudmonitor/ssh/client.py` & `cloudmonitor-0.0.1.9/cloudmonitor/ssh/client.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.8/cloudmonitor/status/define.py` & `cloudmonitor-0.0.1.9/cloudmonitor/status/define.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.8/cloudmonitor/status/query.py` & `cloudmonitor-0.0.1.9/cloudmonitor/status/query.py`

 * *Files identical despite different names*

### Comparing `cloudmonitor-0.0.1.8/cloudmonitor.egg-info/PKG-INFO` & `cloudmonitor-0.0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: cloudmonitor
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: A Web-GUI Monitor for Academic Linux Servers
 Home-page: https://github.com/WNJXYK/cloudmonitor
+Author: Zhi Zhou
+Author-email: wnjxyk@gmail.com
 License: MIT Licence
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,7 +24,9 @@
 ![pypi](https://badgen.net/pypi/v/cloudmonitor)
 ![visitors](https://visitor-badge.glitch.me/badge?page_id=WNJXYK.cloudmonitor)
 [![Downloads](https://pepy.tech/badge/cloudmonitor)](https://pepy.tech/project/cloudmonitor)
 
 ### ATTENTION!
 
 This project is currently under development…
+
+
```

### Comparing `cloudmonitor-0.0.1.8/setup.py` & `cloudmonitor-0.0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     setup(
         name=NAME,
         version=VERSION,
         license="MIT Licence",
         url="https://github.com/WNJXYK/cloudmonitor",
         packages=find_packages(),
         include_package_data=True,
+        # package_dir={"": "cloudmonitor"},
+        # package_data={"cloudmonitor.templates": ["*.html"]},
+        author="Zhi Zhou",
+        author_email="wnjxyk@gmail.com",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type="text/markdown",
         python_requires=REQUIRES_PYTHON,
         install_requires=REQUIRED,
         classifiers=[
             "Intended Audience :: Science/Research",
```

