# Comparing `tmp/mlops_core-0.2.5.tar.gz` & `tmp/mlops_core-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_core-0.2.5.tar", max compression
+gzip compressed data, was "mlops_core-0.2.6.tar", max compression
```

## Comparing `mlops_core-0.2.5.tar` & `mlops_core-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       13 2023-04-25 04:25:05.336475 mlops_core-0.2.5/README.md
--rw-r--r--   0        0        0      449 2023-04-25 04:25:05.337086 mlops_core-0.2.5/mlops_core/bootstrap.py
--rw-r--r--   0        0        0     5483 2023-04-25 04:25:05.337678 mlops_core-0.2.5/mlops_core/connectivity/networking.py
--rw-r--r--   0        0        0      878 2023-04-25 04:25:05.338269 mlops_core-0.2.5/mlops_core/connector/kaggle.py
--rw-r--r--   0        0        0      973 2023-04-25 04:25:05.338982 mlops_core-0.2.5/mlops_core/detection/project_arguments.py
--rw-r--r--   0        0        0     3654 2023-04-25 04:25:05.339441 mlops_core-0.2.5/mlops_core/detection/project_configurations.py
--rw-r--r--   0        0        0     4251 2023-04-25 04:25:05.339927 mlops_core-0.2.5/mlops_core/detection/project_structure.py
--rw-r--r--   0        0        0     6616 2023-04-25 04:25:05.340638 mlops_core-0.2.5/mlops_core/generator/project_generator.py
--rw-r--r--   0        0        0      165 2023-04-25 04:25:05.341011 mlops_core-0.2.5/mlops_core/runtime.py
--rw-r--r--   0        0        0      366 2023-04-25 04:25:05.341616 mlops_core-0.2.5/mlops_core/utils/strings.py
--rw-r--r--   0        0        0      441 2023-04-25 05:08:08.118246 mlops_core-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      143 2023-04-25 04:25:05.343114 mlops_core-0.2.5/templates/ISSUE_TEMPLATE.md.jinja
--rw-r--r--   0        0        0       46 2023-04-25 04:25:05.343455 mlops_core-0.2.5/templates/PULL_REQUEST_TEMPLATE.md.jinja
--rw-r--r--   0        0        0       20 2023-04-25 04:25:05.343741 mlops_core-0.2.5/templates/README.md.jinja
--rw-r--r--   0        0        0      266 2023-04-25 04:25:05.344084 mlops_core-0.2.5/templates/devcontainer.json
--rw-r--r--   0        0        0      737 2023-04-25 04:25:05.344644 mlops_core-0.2.5/templates/src/evaluate.py.jinja
--rw-r--r--   0        0        0      560 2023-04-25 04:25:05.345020 mlops_core-0.2.5/templates/src/ingestion.py.jinja
--rw-r--r--   0        0        0     1155 2023-04-25 04:25:05.345373 mlops_core-0.2.5/templates/src/train.py.jinja
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 mlops_core-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-04-25 04:25:05.336475 mlops_core-0.2.6/README.md
+-rw-r--r--   0        0        0      328 2023-04-25 05:27:11.612916 mlops_core-0.2.6/mlops_core/bootstrap.py
+-rw-r--r--   0        0        0     5474 2023-04-25 05:20:47.645700 mlops_core-0.2.6/mlops_core/connectivity/networking.py
+-rw-r--r--   0        0        0     2595 2023-04-25 06:26:41.792027 mlops_core-0.2.6/mlops_core/connector/remote_storage.py
+-rw-r--r--   0        0        0     3674 2023-04-25 05:30:36.796983 mlops_core-0.2.6/mlops_core/detection/project_configurations.py
+-rw-r--r--   0        0        0     4250 2023-04-25 05:23:46.936113 mlops_core-0.2.6/mlops_core/detection/project_structure.py
+-rw-r--r--   0        0        0     6616 2023-04-25 05:26:57.310579 mlops_core-0.2.6/mlops_core/generator/project_generator.py
+-rw-r--r--   0        0        0      165 2023-04-25 04:25:05.341011 mlops_core-0.2.6/mlops_core/runtime.py
+-rw-r--r--   0        0        0     1545 2023-04-25 05:41:16.294193 mlops_core-0.2.6/mlops_core/utils/conversions.py
+-rw-r--r--   0        0        0     1421 2023-04-25 05:55:57.392949 mlops_core-0.2.6/mlops_core/utils/strings.py
+-rw-r--r--   0        0        0      538 2023-04-25 06:27:13.725337 mlops_core-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-04-25 04:25:05.343114 mlops_core-0.2.6/templates/ISSUE_TEMPLATE.md.jinja
+-rw-r--r--   0        0        0       46 2023-04-25 04:25:05.343455 mlops_core-0.2.6/templates/PULL_REQUEST_TEMPLATE.md.jinja
+-rw-r--r--   0        0        0       20 2023-04-25 04:25:05.343741 mlops_core-0.2.6/templates/README.md.jinja
+-rw-r--r--   0        0        0      266 2023-04-25 04:25:05.344084 mlops_core-0.2.6/templates/devcontainer.json
+-rw-r--r--   0        0        0      737 2023-04-25 04:25:05.344644 mlops_core-0.2.6/templates/src/evaluate.py.jinja
+-rw-r--r--   0        0        0      560 2023-04-25 04:25:05.345020 mlops_core-0.2.6/templates/src/ingestion.py.jinja
+-rw-r--r--   0        0        0     1155 2023-04-25 04:25:05.345373 mlops_core-0.2.6/templates/src/train.py.jinja
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 mlops_core-0.2.6/PKG-INFO
```

### Comparing `mlops_core-0.2.5/mlops_core/connectivity/networking.py` & `mlops_core-0.2.6/mlops_core/connectivity/networking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import os
 import socket
 
 import dns.resolver
 
 from typing import List
-from os import cpu_count
 from functools import partial
 from contextlib import closing
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 CONNECTIVITY_CHECK_TIMEOUT = 5
 
 MIN_PORT = 0
@@ -101,15 +101,15 @@
     Returns:
         List[QueryResult]: List of QueryResult objects
     """
     # Create a partial function to pass to the thread pool
     fn = partial(is_port_open, host)
 
     # Create a thread pool executor to run the thread pool
-    with ThreadPoolExecutor(max_workers=cpu_count() * 50) as executor:
+    with ThreadPoolExecutor(max_workers=os.cpu_count() * 50) as executor:
         # Create a list of threads to run. Each thread will run the is_port_open function
         # with the given host and the port in the range.
         result = [executor.submit(fn, port, timeout)
                   for port in range(start, end)]
 
         # Wait for all threads to finish
         searches = [r.result() for r in as_completed(result)]
@@ -134,15 +134,15 @@
 
         Returns:
             List[QueryResult]: List of QueryResult objects
     """
     common_ports = [7, 20, 21, 22, 23, 25, 69, 88, 53, 80, 110, 119, 123,
                     143, 161, 179, 194, 443, 465, 500, 587, 636, 2483, 3306, 3389, 5432]
     fn = partial(is_port_open, host)
-    with ThreadPoolExecutor(max_workers=cpu_count() * 50) as executor:
+    with ThreadPoolExecutor(max_workers=os.cpu_count() * 50) as executor:
         result = [executor.submit(fn, port, timeout) for port in common_ports]
 
         searches = [r.result() for r in result]
 
         # Filter out inaccessible ports if only accessible ports are requested
         def do_filter_or_not(search):
             return search.open == show_open if show_open else True
```

### Comparing `mlops_core-0.2.5/mlops_core/detection/project_configurations.py` & `mlops_core-0.2.6/mlops_core/detection/project_configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os
 import re
 import yaml
 import json
 import tomli
 import configparser
 
-from project_structure import ProjectStructure
-
+from mlops_core.detection.project_structure import ProjectStructure
 
 class ConfigLoader:
     def __init__(self, project: ProjectStructure) -> None:
         self.project = project
 
     def load_config(self, env: str):
         file_path = self.project.find_config_file(env)
```

### Comparing `mlops_core-0.2.5/mlops_core/detection/project_structure.py` & `mlops_core-0.2.6/mlops_core/detection/project_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 from mlops_core.utils.strings import to_snake_case
 
-
 class ProjectStructure():
     """
     This class is used to detect the project structure and create the required directories.
     The project structure is as follows:
     - .github
         - pull_request_template.md
     - .vscode
```

### Comparing `mlops_core-0.2.5/mlops_core/generator/project_generator.py` & `mlops_core-0.2.6/mlops_core/generator/project_generator.py`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.5/templates/src/evaluate.py.jinja` & `mlops_core-0.2.6/templates/src/evaluate.py.jinja`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.5/templates/src/ingestion.py.jinja` & `mlops_core-0.2.6/templates/src/ingestion.py.jinja`

 * *Files identical despite different names*

### Comparing `mlops_core-0.2.5/templates/src/train.py.jinja` & `mlops_core-0.2.6/templates/src/train.py.jinja`

 * *Files identical despite different names*

