# Comparing `tmp/rest-api-supporter-0.0.3.tar.gz` & `tmp/rest-api-supporter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest-api-supporter-0.0.3.tar", last modified: Fri Mar 24 09:06:56 2023, max compression
+gzip compressed data, was "rest-api-supporter-0.0.4.tar", last modified: Tue Apr 25 06:10:00 2023, max compression
```

## Comparing `rest-api-supporter-0.0.3.tar` & `rest-api-supporter-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:06:56.632587 rest-api-supporter-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      808 2023-03-24 09:06:56.631587 rest-api-supporter-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      526 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:06:56.629587 rest-api-supporter-0.0.3/rest_api_supporter/
--rw-r--r--   0 root         (0) root         (0)       42 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:06:56.630587 rest-api-supporter-0.0.3/rest_api_supporter/servers/
--rw-r--r--   0 root         (0) root         (0)       91 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/servers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/servers/flask_rest_api_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:06:56.631587 rest-api-supporter-0.0.3/rest_api_supporter/utils/
--rw-r--r--   0 root         (0) root         (0)      121 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/utils/base64_to_image.py
--rw-r--r--   0 root         (0) root         (0)      292 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/utils/image_to_base64.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/rest_api_supporter/utils/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:06:56.630587 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      808 2023-03-24 09:06:56.000000 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2023-03-24 09:06:56.000000 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 09:06:56.000000 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 09:06:56.000000 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-24 09:06:56.000000 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-24 09:06:56.000000 rest-api-supporter-0.0.3/rest_api_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 09:06:56.632587 rest-api-supporter-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-03-24 09:06:55.000000 rest-api-supporter-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:10:00.129093 rest-api-supporter-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-25 06:10:00.129093 rest-api-supporter-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      526 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:10:00.126093 rest-api-supporter-0.0.4/rest_api_supporter/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:10:00.128093 rest-api-supporter-0.0.4/rest_api_supporter/servers/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/servers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/servers/flask_rest_api_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:10:00.129093 rest-api-supporter-0.0.4/rest_api_supporter/utils/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/utils/base64_to_image.py
+-rw-r--r--   0 root         (0) root         (0)      292 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/utils/image_to_base64.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter/utils/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 06:10:00.127093 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/rest_api_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 06:10:00.129093 rest-api-supporter-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-04-25 06:09:59.000000 rest-api-supporter-0.0.4/setup.py
```

### Comparing `rest-api-supporter-0.0.3/PKG-INFO` & `rest-api-supporter-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-api-supporter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Rest api supporter
 Home-page: https://github.com/automatethem/rest-api-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `rest-api-supporter-0.0.3/README.md` & `rest-api-supporter-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rest-api-supporter-0.0.3/rest_api_supporter/servers/flask_rest_api_server.py` & `rest-api-supporter-0.0.4/rest_api_supporter/servers/flask_rest_api_server.py`

 * *Files identical despite different names*

### Comparing `rest-api-supporter-0.0.3/rest_api_supporter.egg-info/PKG-INFO` & `rest-api-supporter-0.0.4/rest_api_supporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-api-supporter
-Version: 0.0.3
+Version: 0.0.4
 Summary: Rest api supporter
 Home-page: https://github.com/automatethem/rest-api-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `rest-api-supporter-0.0.3/rest_api_supporter.egg-info/SOURCES.txt` & `rest-api-supporter-0.0.4/rest_api_supporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rest-api-supporter-0.0.3/setup.py` & `rest-api-supporter-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='rest-api-supporter',
-	version='0.0.3',
+	version='0.0.4',
 	description='Rest api supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/rest-api-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

