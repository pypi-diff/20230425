# Comparing `tmp/here-search-demo-0.8.0.tar.gz` & `tmp/here-search-demo-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "here-search-demo-0.8.0.tar", last modified: Tue Apr 25 10:25:51 2023, max compression
+gzip compressed data, was "here-search-demo-0.8.1.tar", last modified: Tue Apr 25 12:44:56 2023, max compression
```

## Comparing `here-search-demo-0.8.0.tar` & `here-search-demo-0.8.1.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.835400 here-search-demo-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/docs/developers.md
--rw-r--r--   0 runner    (1001) docker     (123)   678996 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/docs/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.835400 here-search-demo-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/requirements/lite_run.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/requirements/util.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.835400 here-search-demo-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.835400 here-search-demo-0.8.0/src/here_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.835400 here-search-demo-0.8.0/src/here_search/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/api_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/src/here_search/demo/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/entity/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/entity/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/entity/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/entity/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/entity/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/lite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/src/here_search/demo/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/scripts/here-search-notebooks
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/scripts/lite-run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/src/here_search/demo/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/widgets/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/widgets/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/widgets/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/src/here_search/demo/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/src/here_search_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-25 10:25:51.000000 here-search-demo-0.8.0/src/here_search_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-25 10:25:51.000000 here-search-demo-0.8.0/src/here_search_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:25:51.000000 here-search-demo-0.8.0/src/here_search_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:25:51.000000 here-search-demo-0.8.0/src/here_search_demo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 10:25:51.000000 here-search-demo-0.8.0/src/here_search_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 10:25:51.000000 here-search-demo-0.8.0/src/here_search_demo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:25:51.839401 here-search-demo-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-25 10:25:31.000000 here-search-demo-0.8.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.304422 here-search-demo-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/docs/developers.md
+-rw-r--r--   0 runner    (1001) docker     (123)   678996 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/docs/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.304422 here-search-demo-0.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/requirements/lite_run.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/requirements/util.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.300422 here-search-demo-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.300422 here-search-demo-0.8.1/src/here_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.304422 here-search-demo-0.8.1/src/here_search/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/api_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/src/here_search/demo/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/entity/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/entity/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/entity/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/entity/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/entity/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/lite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/src/here_search/demo/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/notebooks/obm_1_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/notebooks/obm_2_api.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/notebooks/obm_3_widget.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/src/here_search/demo/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/scripts/here-search-notebooks
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/scripts/lite-run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/src/here_search/demo/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/widgets/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/widgets/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/widgets/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/src/here_search/demo/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/src/here_search_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-25 12:44:56.000000 here-search-demo-0.8.1/src/here_search_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 12:44:56.000000 here-search-demo-0.8.1/src/here_search_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:44:56.000000 here-search-demo-0.8.1/src/here_search_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:44:56.000000 here-search-demo-0.8.1/src/here_search_demo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 12:44:56.000000 here-search-demo-0.8.1/src/here_search_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 12:44:56.000000 here-search-demo-0.8.1/src/here_search_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:44:56.308422 here-search-demo-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-25 12:44:39.000000 here-search-demo-0.8.1/tests/test_util.py
```

### Comparing `here-search-demo-0.8.0/LICENSE` & `here-search-demo-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/PKG-INFO` & `here-search-demo-0.8.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: here-search-demo
-Version: 0.8.0
+Version: 0.8.1
 Summary: HERE Geocoding and Search demo and widgets
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
+Project-URL: Bug Tracker, https://github.com/heremaps/here-search-demo/issues
+Project-URL: Source, https://github.com/heremaps/here-search-demo
 Keywords: HERE,Search,Ipywidgets,GS7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,28 +22,28 @@
 License-File: LICENSE
 
 [![Python package](https://github.com/heremaps/here-search-demo/actions/workflows/test.yml/badge.svg)](https://github.com/heremaps/here-search-demo/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/heremaps/here-search-demo/branch/main/graph/badge.svg?token=MVFCS4BUFN)](https://codecov.io/gh/heremaps/here-search-demo)
 
 # HERE Search notebooks
 
-A set of jupyter notebooks demonstrating the use of HERE Geocoding & Search endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
+A set of jupyter notebooks demonstrating the use of [HERE Geocoding & Search][4] endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
 
 ![searching for restaurants](docs/screenshot.png)
 
 Requirements: a [HERE API key][1] and a Python environment.
 
 The notebooks can be [used in your browser][3] without further installation.
 
 ## Installation
 
 If you need to install the notebooks or the underlying library on your workstation, run preferably in a virtual environment:
 
    ```
-   pip -v install here-search-demo
+   pip install here-search-demo
    ```
 
 Link the virtual environment to a IPython kernel:
 
    ```
    python -m ipykernel install \
      --prefix $(python -c "import sys; print(sys.prefix)") \
@@ -59,10 +61,11 @@
 
 ## License
 
 Copyright (C) 2022-2023 HERE Europe B.V.
 
 This project is licensed under the MIT license - see the [LICENSE](./LICENSE) file in the root of this project for license details.
 
-[1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start-dhc.html#get-an-api-key
+[1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start.html#get-an-api-key
 [2]: docs/developers.md#setup-a-notebook-python-environment
 [3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
+[4]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
```

### Comparing `here-search-demo-0.8.0/README.md` & `here-search-demo-0.8.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [![Python package](https://github.com/heremaps/here-search-demo/actions/workflows/test.yml/badge.svg)](https://github.com/heremaps/here-search-demo/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/heremaps/here-search-demo/branch/main/graph/badge.svg?token=MVFCS4BUFN)](https://codecov.io/gh/heremaps/here-search-demo)
 
 # HERE Search notebooks
 
-A set of jupyter notebooks demonstrating the use of HERE Geocoding & Search endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
+A set of jupyter notebooks demonstrating the use of [HERE Geocoding & Search][4] endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
 
 ![searching for restaurants](docs/screenshot.png)
 
 Requirements: a [HERE API key][1] and a Python environment.
 
 The notebooks can be [used in your browser][3] without further installation.
 
 ## Installation
 
 If you need to install the notebooks or the underlying library on your workstation, run preferably in a virtual environment:
 
    ```
-   pip -v install here-search-demo
+   pip install here-search-demo
    ```
 
 Link the virtual environment to a IPython kernel:
 
    ```
    python -m ipykernel install \
      --prefix $(python -c "import sys; print(sys.prefix)") \
@@ -38,10 +38,11 @@
 
 ## License
 
 Copyright (C) 2022-2023 HERE Europe B.V.
 
 This project is licensed under the MIT license - see the [LICENSE](./LICENSE) file in the root of this project for license details.
 
-[1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start-dhc.html#get-an-api-key
+[1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start.html#get-an-api-key
 [2]: docs/developers.md#setup-a-notebook-python-environment
-[3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
+[3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
+[4]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
```

### Comparing `here-search-demo-0.8.0/docs/developers.md` & `here-search-demo-0.8.1/docs/developers.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ## Developer notes
 
 ### Setup a Notebook Python environment
 
 It is recommended to use a Python virtual environment. The below recipe uses the python batteries `venv` module.
-It has only been tested on a Macos Monterey machine, but it should not be too difficult to use it on another Unix-like workstation.
 
 1. Virtual environment
 
    ```
    mkdir -p ~/virtualenv; (cd ~/virtualenv; python -m venv search-notebook)
    source ~/virtualenv/search-notebook/bin/activate
    ```
@@ -37,22 +36,14 @@
 To run the notebook on Jupyter Classic, you will need:
 
    ```
    jupyter nbextension enable --py widgetsnbextension
    jupyter labextension install @jupyterlab/geojson-extension
    ```
 
-### Upload a new package to a pypa repository
-
-   ```
-   pip install -r requirements/util.txt
-   python -m build --sdist --wheel
-   twine upload dist/*
-   ```
-
 ### Test on MacOS / python3.7
 
 1. Build Python 3.7.9 for `pyenv`
 
    ```
    brew install zlib bzip2 openssl@1.1 readline xz
    CFLAGS="-I$(brew --prefix openssl)/include -I$(brew --prefix bzip2)/include -I$(brew --prefix readline)/include -I$(xcrun --show-sdk-path)/usr/include"
@@ -62,16 +53,14 @@
 
 2. Create virtual environment
 
    ```
    pyenv virtualenv 3.7.9 venv3.7
    pyenv activate venv3.7
    pyenv local venv3.7 && python -V
-   pip install -e .
-   pip install -r requirements_dev.txt
    ```
 
 ### JupyterLite
 
 [JupyterLite](https://jupyterlite.readthedocs.io/en/latest/) is a JupyterLab distribution that runs entirely in the browser.
 The Python kernels are backed by [`Pyodide`](https://pyodide.org/en/stable/) running in a Web Worker.
 
@@ -85,15 +74,15 @@
    ```
 
 For the Pyodide kernels to be able to use certain packages, those need to be installed from the notebook itself:
 
    ```
    try:
       import piplite
-      await piplite.install(["ipywidgets==7.7.1", "ipyleaflet==0.17.1", "emfs:here_search_widget-0.6.1-py3-none-any.whl"], keep_going=True)
+      await piplite.install(["ipywidgets==7.7.1", "ipyleaflet==0.17.1", "emfs:here_search_widget-0.8.1-py3-none-any.whl"], keep_going=True)
    except ImportError:
       pass
    ```
 
 #### From a local git clone
 
 To test the jupyterlite page locally, run from the local git repository:
```

### Comparing `here-search-demo-0.8.0/docs/screenshot.png` & `here-search-demo-0.8.1/docs/screenshot.png`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/setup.cfg` & `here-search-demo-0.8.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
+project_urls = 
+	Bug Tracker = https://github.com/heremaps/here-search-demo/issues
+	Source = https://github.com/heremaps/here-search-demo
 
 [options]
 zip_safe = False
 python_requires = >=3.8
 package_dir = 
 	= src
 scripts = 
@@ -32,15 +35,15 @@
 	src/here_search/demo/scripts/lite-run.sh
 install_requires = file: requirements/build.txt
 
 [options.packages.find]
 where = src
 
 [options.package_data]
-here_search.notebooks = 
+here_search.demo.notebooks = 
 	*.ipynb
 * = 
 	requirements/*.txt; setup.py; setup.cfg; pyproject.toml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `here-search-demo-0.8.0/src/here_search/demo/api.py` & `here-search-demo-0.8.1/src/here_search/demo/api.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/api_options.py` & `here-search-demo-0.8.1/src/here_search/demo/api_options.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/base.py` & `here-search-demo-0.8.1/src/here_search/demo/base.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/entity/endpoint.py` & `here-search-demo-0.8.1/src/here_search/demo/entity/endpoint.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/entity/intent.py` & `here-search-demo-0.8.1/src/here_search/demo/entity/intent.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/entity/place.py` & `here-search-demo-0.8.1/src/here_search/demo/entity/place.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/entity/request.py` & `here-search-demo-0.8.1/src/here_search/demo/entity/request.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/event.py` & `here-search-demo-0.8.1/src/here_search/demo/event.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/lite.py` & `here-search-demo-0.8.1/src/here_search/demo/lite.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/scripts/lite-run.sh` & `here-search-demo-0.8.1/src/here_search/demo/scripts/lite-run.sh`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/user.py` & `here-search-demo-0.8.1/src/here_search/demo/user.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/util.py` & `here-search-demo-0.8.1/src/here_search/demo/util.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/widgets/app.py` & `here-search-demo-0.8.1/src/here_search/demo/widgets/app.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/widgets/input.py` & `here-search-demo-0.8.1/src/here_search/demo/widgets/input.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/widgets/output.py` & `here-search-demo-0.8.1/src/here_search/demo/widgets/output.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search/demo/widgets/util.py` & `here-search-demo-0.8.1/src/here_search/demo/widgets/util.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/src/here_search_demo.egg-info/PKG-INFO` & `here-search-demo-0.8.1/src/here_search_demo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: here-search-demo
-Version: 0.8.0
+Version: 0.8.1
 Summary: HERE Geocoding and Search demo and widgets
 Home-page: https://here.com
 Author: HERE Europe B.V.
 Author-email: emmanuel.decitre@here.com
 License: The MIT License
+Project-URL: Bug Tracker, https://github.com/heremaps/here-search-demo/issues
+Project-URL: Source, https://github.com/heremaps/here-search-demo
 Keywords: HERE,Search,Ipywidgets,GS7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,28 +22,28 @@
 License-File: LICENSE
 
 [![Python package](https://github.com/heremaps/here-search-demo/actions/workflows/test.yml/badge.svg)](https://github.com/heremaps/here-search-demo/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/heremaps/here-search-demo/branch/main/graph/badge.svg?token=MVFCS4BUFN)](https://codecov.io/gh/heremaps/here-search-demo)
 
 # HERE Search notebooks
 
-A set of jupyter notebooks demonstrating the use of HERE Geocoding & Search endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
+A set of jupyter notebooks demonstrating the use of [HERE Geocoding & Search][4] endpoints `/autosuggest`,  `/discover`, `/browse`, and `/lookup`.
 
 ![searching for restaurants](docs/screenshot.png)
 
 Requirements: a [HERE API key][1] and a Python environment.
 
 The notebooks can be [used in your browser][3] without further installation.
 
 ## Installation
 
 If you need to install the notebooks or the underlying library on your workstation, run preferably in a virtual environment:
 
    ```
-   pip -v install here-search-demo
+   pip install here-search-demo
    ```
 
 Link the virtual environment to a IPython kernel:
 
    ```
    python -m ipykernel install \
      --prefix $(python -c "import sys; print(sys.prefix)") \
@@ -59,10 +61,11 @@
 
 ## License
 
 Copyright (C) 2022-2023 HERE Europe B.V.
 
 This project is licensed under the MIT license - see the [LICENSE](./LICENSE) file in the root of this project for license details.
 
-[1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start-dhc.html#get-an-api-key
+[1]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/topics/quick-start.html#get-an-api-key
 [2]: docs/developers.md#setup-a-notebook-python-environment
 [3]: https://heremaps.github.io/here-search-demo/lab/?path=demo.ipynb
+[4]: https://developer.here.com/documentation/geocoding-search-api/dev_guide/index.html
```

### Comparing `here-search-demo-0.8.0/src/here_search_demo.egg-info/SOURCES.txt` & `here-search-demo-0.8.1/src/here_search_demo.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 src/here_search/demo/util.py
 src/here_search/demo/entity/__init__.py
 src/here_search/demo/entity/constants.py
 src/here_search/demo/entity/endpoint.py
 src/here_search/demo/entity/intent.py
 src/here_search/demo/entity/place.py
 src/here_search/demo/entity/request.py
+src/here_search/demo/notebooks/demo.ipynb
+src/here_search/demo/notebooks/obm_1_api.ipynb
+src/here_search/demo/notebooks/obm_2_api.ipynb
+src/here_search/demo/notebooks/obm_3_widget.ipynb
 src/here_search/demo/scripts/here-search-notebooks
 src/here_search/demo/scripts/lite-run.sh
 src/here_search/demo/widgets/__init__.py
 src/here_search/demo/widgets/app.py
 src/here_search/demo/widgets/input.py
 src/here_search/demo/widgets/output.py
 src/here_search/demo/widgets/util.py
```

### Comparing `here-search-demo-0.8.0/tests/test_api.py` & `here-search-demo-0.8.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/tests/test_base.py` & `here-search-demo-0.8.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/tests/test_entities.py` & `here-search-demo-0.8.1/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `here-search-demo-0.8.0/tests/test_util.py` & `here-search-demo-0.8.1/tests/test_util.py`

 * *Files identical despite different names*

