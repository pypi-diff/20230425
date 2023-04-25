# Comparing `tmp/geomapdemo-0.2.0.tar.gz` & `tmp/geomapdemo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.2.0.tar", last modified: Mon Apr 24 04:09:29 2023, max compression
+gzip compressed data, was "geomapdemo-0.2.1.tar", last modified: Tue Apr 25 04:12:52 2023, max compression
```

## Comparing `geomapdemo-0.2.0.tar` & `geomapdemo-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:09:29.549603 geomapdemo-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 04:09:18.000000 geomapdemo-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 04:09:18.000000 geomapdemo-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 04:09:29.549603 geomapdemo-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-24 04:09:18.000000 geomapdemo-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:09:29.549603 geomapdemo-0.2.0/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-24 04:09:19.000000 geomapdemo-0.2.0/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-24 04:09:19.000000 geomapdemo-0.2.0/geomapdemo/foliumap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-24 04:09:19.000000 geomapdemo-0.2.0/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:09:29.549603 geomapdemo-0.2.0/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 04:09:29.000000 geomapdemo-0.2.0/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 04:09:29.000000 geomapdemo-0.2.0/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 04:09:29.000000 geomapdemo-0.2.0/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 04:09:29.000000 geomapdemo-0.2.0/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 04:09:29.000000 geomapdemo-0.2.0/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 04:09:29.000000 geomapdemo-0.2.0/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 04:09:19.000000 geomapdemo-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 04:09:29.549603 geomapdemo-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 04:09:19.000000 geomapdemo-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:12:52.590925 geomapdemo-0.2.1/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/geomapdemo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-25 04:12:52.000000 geomapdemo-0.2.1/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 04:12:52.594925 geomapdemo-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-25 04:12:39.000000 geomapdemo-0.2.1/setup.py
```

### Comparing `geomapdemo-0.2.0/LICENSE` & `geomapdemo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.2.0/PKG-INFO` & `geomapdemo-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -39,11 +39,13 @@
     
 
 ## Features
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
+-   Ipyleaflet based interactive map function
+-   Folium based interactive map function
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.2.0/README.md` & `geomapdemo-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,11 +17,13 @@
     
 
 ## Features
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
+-   Ipyleaflet based interactive map function
+-   Folium based interactive map function
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.2.0/geomapdemo/geomapdemo.py` & `geomapdemo-0.2.1/geomapdemo/geomapdemo.py`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.2.0/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.2.1/geomapdemo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.2.0
+Version: 0.2.1
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -39,11 +39,13 @@
     
 
 ## Features
 
 -   Create random numbers and random text
 -   Basic Mapping and drawing
 -   Vector and raster layer function available
+-   Ipyleaflet based interactive map function
+-   Folium based interactive map function
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geomapdemo-0.2.0/setup.py` & `geomapdemo-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

