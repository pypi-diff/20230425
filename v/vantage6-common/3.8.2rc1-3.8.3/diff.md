# Comparing `tmp/vantage6-common-3.8.2rc1.tar.gz` & `tmp/vantage6-common-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-3.8.2rc1.tar", last modified: Wed Mar 22 14:57:49 2023, max compression
+gzip compressed data, was "vantage6-common-3.8.3.tar", last modified: Tue Apr 25 11:55:42 2023, max compression
```

## Comparing `vantage6-common-3.8.2rc1.tar` & `vantage6-common-3.8.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:49.786555 vantage6-common-3.8.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-22 14:57:49.786555 vantage6-common-3.8.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:57:49.786555 vantage6-common-3.8.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:49.782554 vantage6-common-3.8.2rc1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:49.782554 vantage6-common-3.8.2rc1/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:49.782554 vantage6-common-3.8.2rc1/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-03-22 14:57:38.000000 vantage6-common-3.8.2rc1/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:49.786555 vantage6-common-3.8.2rc1/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-22 14:57:49.000000 vantage6-common-3.8.2rc1/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-22 14:57:49.000000 vantage6-common-3.8.2rc1/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:49.000000 vantage6-common-3.8.2rc1/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-22 14:57:49.000000 vantage6-common-3.8.2rc1/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-22 14:57:49.000000 vantage6-common-3.8.2rc1/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.233688 vantage6-common-3.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 11:55:42.233688 vantage6-common-3.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:55:42.233688 vantage6-common-3.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.221688 vantage6-common-3.8.3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.229688 vantage6-common-3.8.3/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.229688 vantage6-common-3.8.3/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-25 11:55:29.000000 vantage6-common-3.8.3/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:42.229688 vantage6-common-3.8.3/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 11:55:42.000000 vantage6-common-3.8.3/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 11:55:42.000000 vantage6-common-3.8.3/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:42.000000 vantage6-common-3.8.3/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 11:55:42.000000 vantage6-common-3.8.3/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 11:55:42.000000 vantage6-common-3.8.3/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-3.8.2rc1/PKG-INFO` & `vantage6-common-3.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.2rc1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.3 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.8.2rc1/setup.py` & `vantage6-common-3.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/__init__.py` & `vantage6-common-3.8.3/vantage6/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/_version.py` & `vantage6-common-3.8.3/vantage6/common/_version.py`

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

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/colors.py` & `vantage6-common-3.8.3/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/configuration_manager.py` & `vantage6-common-3.8.3/vantage6/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/context.py` & `vantage6-common-3.8.3/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/docker/addons.py` & `vantage6-common-3.8.3/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/docker/network_manager.py` & `vantage6-common-3.8.3/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/encryption.py` & `vantage6-common-3.8.3/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/globals.py` & `vantage6-common-3.8.3/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/task_status.py` & `vantage6-common-3.8.3/vantage6/common/task_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     NO_DOCKER_IMAGE = 'non-existing Docker image'
     # Container had a non zero exit code
     CRASHED = 'crashed'
     # Container was killed by user
     KILLED = 'killed by user'
     # Task was not allowed by node policies
     NOT_ALLOWED = 'not allowed'
+    # Task failed without exit code
+    UNKNOWN_ERROR = 'unknown error'
 
 
 def has_task_failed(status: TaskStatus) -> bool:
     """
     Check if task has failed to run to completion
 
     Parameters
```

### Comparing `vantage6-common-3.8.2rc1/vantage6/common/utest.py` & `vantage6-common-3.8.3/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.2rc1/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-3.8.3/vantage6_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.2rc1 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.3 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.8.2rc1/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-3.8.3/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

