# Comparing `tmp/croudtech-ecs-tools-1.0.0.tar.gz` & `tmp/croudtech-ecs-tools-1.0.1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croudtech-ecs-tools-1.0.0.tar", last modified: Mon Apr 24 11:43:35 2023, max compression
+gzip compressed data, was "croudtech-ecs-tools-1.0.1.linux-x86_64.tar", last modified: Mon Apr 24 11:45:55 2023, max compression
```

## Comparing `croudtech-ecs-tools-1.0.0.tar` & `croudtech-ecs-tools-1.0.1.linux-x86_64.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 11:43:35.354020 croudtech-ecs-tools-1.0.0/
--rw-r--r--   0 vsts      (1001) docker     (123)    11357 2023-04-24 11:43:07.000000 croudtech-ecs-tools-1.0.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-24 11:43:35.354020 croudtech-ecs-tools-1.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1370 2023-04-24 11:43:07.000000 croudtech-ecs-tools-1.0.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 11:43:35.350021 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-24 11:43:07.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8044 2023-04-24 11:43:07.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools/cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6871 2023-04-24 11:43:07.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools/ecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-24 11:43:35.354020 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-24 11:43:35.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      372 2023-04-24 11:43:35.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-24 11:43:35.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-24 11:43:35.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-04-24 11:43:35.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-04-24 11:43:35.000000 croudtech-ecs-tools-1.0.0/croudtech_ecs_tools.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-24 11:43:35.354020 croudtech-ecs-tools-1.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1762 2023-04-24 11:43:07.000000 croudtech-ecs-tools-1.0.0/setup.py
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/.local/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/.local/share/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/.local/share/virtualenvs/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.351608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.351608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/bin/
+-rwxr-xr-x   0 jim       (1000) jim       (1000)     1083 2023-04-24 11:45:55.351608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/bin/croudtech-ecs-tools
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.331608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.311608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools/
+-rw-r--r--   0 jim       (1000) jim       (1000)        0 2022-01-05 12:18:38.000000 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools/__init__.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     8044 2023-04-24 10:32:31.000000 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools/cli.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     6871 2023-04-24 10:36:57.000000 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools/ecs.py
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-04-24 11:45:55.331608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/
+-rw-r--r--   0 jim       (1000) jim       (1000)     1962 2023-04-24 11:45:55.321608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 jim       (1000) jim       (1000)      372 2023-04-24 11:45:55.321608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)        1 2023-04-24 11:45:55.321608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)       87 2023-04-24 11:45:55.321608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/entry_points.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)      430 2023-04-24 11:45:55.321608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/requires.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)       20 2023-04-24 11:45:55.321608 ./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/top_level.txt
```

### Comparing `croudtech-ecs-tools-1.0.0/PKG-INFO` & `./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools-1.0.1-py3.8.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
-Description: # croudtech-ecs-tools
-        
-        [![PyPI](https://img.shields.io/pypi/v/croudtech-ecs-tools.svg)](https://pypi.org/project/croudtech-ecs-tools/)
-        [![Changelog](https://img.shields.io/github/v/release/CroudTech/croudtech-ecs-tools?include_prereleases&label=changelog)](https://github.com/CroudTech/croudtech-ecs-tools/releases)
-        [![Tests](https://github.com/CroudTech/croudtech-ecs-tools/workflows/Test/badge.svg)](https://github.com/CroudTech/croudtech-ecs-tools/actions?query=workflow%3ATest)
-        [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/CroudTech/croudtech-ecs-tools/blob/master/LICENSE)
-        
-        Tools for managing ECS Services and Tasks
-        
-        ## Installation
-        
-        Install this tool using `pip`:
-        
-            $ pip install croudtech-ecs-tools
-        
-        ## Usage
-        
-        Usage: python -m croudtech_ecs_tools.cli [OPTIONS] COMMAND [ARGS]...
-        
-          Tools for managing ECS Services and Tasks
-        
-        Options:
-          --version  Show the version and exit.
-          --help     Show this message and exit.
-        
-        Commands:
-          ecs-shell
-          croudtech-ecs-tools
-        
-        ## Development
-        
-        To contribute to this tool, first checkout the code. Then create a new virtual environment:
-        
-            cd croudtech-ecs-tools
-            python -m venv venv
-            source venv/bin/activate
-        
-        Or if you are using `pipenv`:
-        
-            pipenv shell
-        
-        Now install the dependencies and test dependencies:
-        
-            pip install -e '.[test]'
-        
-        To run the tests:
-        
-            pytest
-        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# croudtech-ecs-tools
+
+[![PyPI](https://img.shields.io/pypi/v/croudtech-ecs-tools.svg)](https://pypi.org/project/croudtech-ecs-tools/)
+[![Changelog](https://img.shields.io/github/v/release/CroudTech/croudtech-ecs-tools?include_prereleases&label=changelog)](https://github.com/CroudTech/croudtech-ecs-tools/releases)
+[![Tests](https://github.com/CroudTech/croudtech-ecs-tools/workflows/Test/badge.svg)](https://github.com/CroudTech/croudtech-ecs-tools/actions?query=workflow%3ATest)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/CroudTech/croudtech-ecs-tools/blob/master/LICENSE)
+
+Tools for managing ECS Services and Tasks
+
+## Installation
+
+Install this tool using `pip`:
+
+    $ pip install croudtech-ecs-tools
+
+## Usage
+
+Usage: python -m croudtech_ecs_tools.cli [OPTIONS] COMMAND [ARGS]...
+
+  Tools for managing ECS Services and Tasks
+
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  ecs-shell
+  croudtech-ecs-tools
+
+## Development
+
+To contribute to this tool, first checkout the code. Then create a new virtual environment:
+
+    cd croudtech-ecs-tools
+    python -m venv venv
+    source venv/bin/activate
+
+Or if you are using `pipenv`:
+
+    pipenv shell
+
+Now install the dependencies and test dependencies:
+
+    pip install -e '.[test]'
+
+To run the tests:
+
+    pytest
+
+
```

### Comparing `croudtech-ecs-tools-1.0.0/croudtech_ecs_tools/cli.py` & `./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools/cli.py`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-1.0.0/croudtech_ecs_tools/ecs.py` & `./home/jim/.local/share/virtualenvs/croudtech-python-ecs-tools-8IKA3a6-/lib/python3.8/site-packages/croudtech_ecs_tools/ecs.py`

 * *Files identical despite different names*

