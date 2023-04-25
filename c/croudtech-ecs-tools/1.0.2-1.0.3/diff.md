# Comparing `tmp/croudtech-ecs-tools-1.0.2.tar.gz` & `tmp/croudtech-ecs-tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croudtech-ecs-tools-1.0.2.tar", last modified: Tue Apr 25 09:31:45 2023, max compression
+gzip compressed data, was "croudtech-ecs-tools-1.0.3.tar", last modified: Tue Apr 25 09:43:27 2023, max compression
```

## Comparing `croudtech-ecs-tools-1.0.2.tar` & `croudtech-ecs-tools-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:31:45.066523 croudtech-ecs-tools-1.0.2/
--rw-r--r--   0 vsts      (1001) docker     (123)    11357 2023-04-25 09:31:10.000000 croudtech-ecs-tools-1.0.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-25 09:31:45.066523 croudtech-ecs-tools-1.0.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1370 2023-04-25 09:31:10.000000 croudtech-ecs-tools-1.0.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:31:45.066523 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 09:31:10.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8136 2023-04-25 09:31:10.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools/cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9088 2023-04-25 09:31:10.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools/ecs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:31:45.066523 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-25 09:31:44.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      372 2023-04-25 09:31:45.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 09:31:44.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-25 09:31:44.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-04-25 09:31:44.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-04-25 09:31:44.000000 croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-25 09:31:45.066523 croudtech-ecs-tools-1.0.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1762 2023-04-25 09:31:10.000000 croudtech-ecs-tools-1.0.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11357 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1370 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8136 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9094 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/ecs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      372 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       20 2023-04-25 09:43:27.000000 croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-25 09:43:27.417009 croudtech-ecs-tools-1.0.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1762 2023-04-25 09:42:46.000000 croudtech-ecs-tools-1.0.3/setup.py
```

### Comparing `croudtech-ecs-tools-1.0.2/LICENSE` & `croudtech-ecs-tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-1.0.2/PKG-INFO` & `croudtech-ecs-tools-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-1.0.2/README.md` & `croudtech-ecs-tools-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-1.0.2/croudtech_ecs_tools/cli.py` & `croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/cli.py`

 * *Files identical despite different names*

### Comparing `croudtech-ecs-tools-1.0.2/croudtech_ecs_tools/ecs.py` & `croudtech-ecs-tools-1.0.3/croudtech_ecs_tools/ecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,19 +140,19 @@
             for task in self.get_task_descriptions(cluster):
                 for attachment in task["attachments"]:
                     if attachment["type"] == "ElasticNetworkInterface":
                         for detail in attachment["details"]:
                             if detail["name"] == "privateIPv4Address":                                
                                 if (not ip_filter) or detail["value"] in ip_filter:
                                     if task["group"] not in services:
-                                        services[task["group"]] = {}
-                                    services[task["group"]] = {
+                                        services[task["group"]] = []
+                                    services[task["group"]].append({
                                         "task_arn": task["taskArn"],
                                         "ip_address": detail["value"]
-                                    }
+                                    })
         return services
 
 
         
 
 class EcsScaler:
     def __init__(self, environment) -> None:
```

### Comparing `croudtech-ecs-tools-1.0.2/croudtech_ecs_tools.egg-info/PKG-INFO` & `croudtech-ecs-tools-1.0.3/croudtech_ecs_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croudtech-ecs-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for managing ECS Services and Tasks
 Home-page: https://github.com/CroudTech/croudtech-ecs-tools
 Author: Jim Robinson
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/CroudTech/croudtech-ecs-tools/issues
 Project-URL: CI, https://github.com/CroudTech/croudtech-ecs-tools/actions
 Project-URL: Changelog, https://github.com/CroudTech/croudtech-ecs-tools/releases
```

### Comparing `croudtech-ecs-tools-1.0.2/setup.py` & `croudtech-ecs-tools-1.0.3/setup.py`

 * *Files identical despite different names*

