# Comparing `tmp/vantage6-3.8.2rc1.tar.gz` & `tmp/vantage6-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-3.8.2rc1.tar", last modified: Wed Mar 22 14:57:51 2023, max compression
+gzip compressed data, was "vantage6-3.8.3.tar", last modified: Tue Apr 25 11:55:43 2023, max compression
```

## Comparing `vantage6-3.8.2rc1.tar` & `vantage6-3.8.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.038558 vantage6-3.8.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-03-22 14:57:51.038558 vantage6-3.8.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:57:51.038558 vantage6-3.8.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.034558 vantage6-3.8.2rc1/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.034558 vantage6-3.8.2rc1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.038558 vantage6-3.8.2rc1/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.038558 vantage6-3.8.2rc1/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/rabbitmq/rabbitmq.config
--rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-22 14:57:38.000000 vantage6-3.8.2rc1/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.034558 vantage6-3.8.2rc1/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-03-22 14:57:50.000000 vantage6-3.8.2rc1/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-22 14:57:50.000000 vantage6-3.8.2rc1/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:50.000000 vantage6-3.8.2rc1/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-22 14:57:50.000000 vantage6-3.8.2rc1/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-22 14:57:50.000000 vantage6-3.8.2rc1/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-22 14:57:50.000000 vantage6-3.8.2rc1/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.265691 vantage6-3.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-25 11:55:43.265691 vantage6-3.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:55:43.265691 vantage6-3.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-25 11:55:29.000000 vantage6-3.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.265691 vantage6-3.8.3/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-3.8.3/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 11:55:29.000000 vantage6-3.8.3/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-04-25 11:55:29.000000 vantage6-3.8.3/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-25 11:55:29.000000 vantage6-3.8.3/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-25 11:55:29.000000 vantage6-3.8.3/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.265691 vantage6-3.8.3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.265691 vantage6-3.8.3/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.265691 vantage6-3.8.3/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/rabbitmq/rabbitmq.config
+-rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 11:55:29.000000 vantage6-3.8.3/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.265691 vantage6-3.8.3/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-25 11:55:43.000000 vantage6-3.8.3/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 11:55:43.000000 vantage6-3.8.3/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:43.000000 vantage6-3.8.3/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 11:55:43.000000 vantage6-3.8.3/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-25 11:55:43.000000 vantage6-3.8.3/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 11:55:43.000000 vantage6-3.8.3/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-3.8.2rc1/PKG-INFO` & `vantage6-3.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.8.2rc1 Summary: vantage6
-command line interface Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-dev
+Metadata-Version: 2.1 Name: vantage6 Version: 3.8.3 Summary: vantage6 command
+line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
+>=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
 badge.fury.io/py/vantage6) [![Unittests](https://github.com/vantage6/vantage6/
```

### Comparing `vantage6-3.8.2rc1/setup.py` & `vantage6-3.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/tests_cli/test_node_cli.py` & `vantage6-3.8.3/tests_cli/test_node_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/tests_cli/test_server_cli.py` & `vantage6-3.8.3/tests_cli/test_server_cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/tests_cli/test_wizard.py` & `vantage6-3.8.3/tests_cli/test_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/_version.py` & `vantage6-3.8.3/vantage6/cli/_version.py`

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
 pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-3.8.2rc1/vantage6/cli/configuration_manager.py` & `vantage6-3.8.3/vantage6/cli/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/configuration_wizard.py` & `vantage6-3.8.3/vantage6/cli/configuration_wizard.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/context.py` & `vantage6-3.8.3/vantage6/cli/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/globals.py` & `vantage6-3.8.3/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/node.py` & `vantage6-3.8.3/vantage6/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/rabbitmq/__init__.py` & `vantage6-3.8.3/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/rabbitmq/definitions.py` & `vantage6-3.8.3/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-3.8.3/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/server.py` & `vantage6-3.8.3/vantage6/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6/cli/utils.py` & `vantage6-3.8.3/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-3.8.2rc1/vantage6.egg-info/PKG-INFO` & `vantage6-3.8.3/vantage6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 3.8.2rc1 Summary: vantage6
-command line interface Home-page: https://github.com/vantage6/vantage6
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-dev
+Metadata-Version: 2.1 Name: vantage6 Version: 3.8.3 Summary: vantage6 command
+line interface Home-page: https://github.com/vantage6/vantage6 Requires-Python:
+>=3.6 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
 badge.fury.io/py/vantage6) [![Unittests](https://github.com/vantage6/vantage6/
```

### Comparing `vantage6-3.8.2rc1/vantage6.egg-info/SOURCES.txt` & `vantage6-3.8.3/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

