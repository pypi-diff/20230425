# Comparing `tmp/vantage6-client-3.8.2rc1.tar.gz` & `tmp/vantage6-client-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-3.8.2rc1.tar", last modified: Wed Mar 22 14:57:50 2023, max compression
+gzip compressed data, was "vantage6-client-3.8.3.tar", last modified: Tue Apr 25 11:55:42 2023, max compression
```

## Comparing `vantage6-client-3.8.2rc1.tar` & `vantage6-client-3.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:50.438557 vantage6-client-3.8.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-22 14:57:50.438557 vantage6-client-3.8.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:57:50.442556 vantage6-client-3.8.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:50.434557 vantage6-client-3.8.2rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:50.434557 vantage6-client-3.8.2rc1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:50.438557 vantage6-client-3.8.2rc1/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    81359 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:50.438557 vantage6-client-3.8.2rc1/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/dispatch_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-03-22 14:57:38.000000 vantage6-client-3.8.2rc1/vantage6/tools/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:50.438557 vantage6-client-3.8.2rc1/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-22 14:57:50.000000 vantage6-client-3.8.2rc1/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-22 14:57:50.000000 vantage6-client-3.8.2rc1/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:50.000000 vantage6-client-3.8.2rc1/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-22 14:57:50.000000 vantage6-client-3.8.2rc1/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-22 14:57:50.000000 vantage6-client-3.8.2rc1/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    81359 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/algorithm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/vantage6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/dispatch_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-04-25 11:55:29.000000 vantage6-client-3.8.3/vantage6/tools/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.829690 vantage6-client-3.8.3/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 11:55:42.000000 vantage6-client-3.8.3/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 11:55:42.000000 vantage6-client-3.8.3/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:42.000000 vantage6-client-3.8.3/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 11:55:42.000000 vantage6-client-3.8.3/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 11:55:42.000000 vantage6-client-3.8.3/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-3.8.2rc1/PKG-INFO` & `vantage6-client-3.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.2rc1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.3 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.8.2rc1/setup.py` & `vantage6-client-3.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/tests/test_client.py` & `vantage6-client-3.8.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/tests/test_deserialization.py` & `vantage6-client-3.8.3/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/tests/test_docker_wrapper.py` & `vantage6-client-3.8.3/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/tests/test_serialization.py` & `vantage6-client-3.8.3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/__init__.py` & `vantage6-client-3.8.3/vantage6/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/_version.py` & `vantage6-client-3.8.3/vantage6/client/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 2, 'candidate', __build__, 0)))
+version_info = ((( 3, 8, 3, 'final', __build__, 0)))
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/algorithm_client.py` & `vantage6-client-3.8.3/vantage6/client/algorithm_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/deserialization.py` & `vantage6-client-3.8.3/vantage6/client/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/filter.py` & `vantage6-client-3.8.3/vantage6/client/filter.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/serialization.py` & `vantage6-client-3.8.3/vantage6/client/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/client/utils.py` & `vantage6-client-3.8.3/vantage6/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/tools/deserialization.py` & `vantage6-client-3.8.3/vantage6/tools/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/tools/dispatch_rpc.py` & `vantage6-client-3.8.3/vantage6/tools/dispatch_rpc.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/tools/mock_client.py` & `vantage6-client-3.8.3/vantage6/tools/mock_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/tools/serialization.py` & `vantage6-client-3.8.3/vantage6/tools/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/tools/util.py` & `vantage6-client-3.8.3/vantage6/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6/tools/wrapper.py` & `vantage6-client-3.8.3/vantage6/tools/wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.2rc1/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-3.8.3/vantage6_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.2rc1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.3 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.8.2rc1/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-3.8.3/vantage6_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

