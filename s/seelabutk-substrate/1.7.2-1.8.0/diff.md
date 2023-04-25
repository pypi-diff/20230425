# Comparing `tmp/seelabutk-substrate-1.7.2.tar.gz` & `tmp/seelabutk-substrate-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seelabutk-substrate-1.7.2.tar", last modified: Mon Apr 24 15:27:00 2023, max compression
+gzip compressed data, was "seelabutk-substrate-1.8.0.tar", last modified: Mon Apr 24 15:33:52 2023, max compression
```

## Comparing `seelabutk-substrate-1.7.2.tar` & `seelabutk-substrate-1.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/
--rw-r--r--   0 john      (1000) john      (1000)    16674 2022-03-29 18:24:57.000000 seelabutk-substrate-1.7.2/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     3439 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2997 2022-07-27 03:11:50.000000 seelabutk-substrate-1.7.2/README.md
--rw-r--r--   0 john      (1000) john      (1000)      757 2023-04-24 15:26:50.000000 seelabutk-substrate-1.7.2/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)      444 2023-04-24 15:27:00.682733 seelabutk-substrate-1.7.2/setup.cfg
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.652733 seelabutk-substrate-1.7.2/src/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     3439 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1422 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       55 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)      100 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       10 2023-04-24 15:27:00.000000 seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/top_level.txt
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/substrate/
--rw-r--r--   0 john      (1000) john      (1000)       33 2022-03-15 19:56:07.000000 seelabutk-substrate-1.7.2/src/substrate/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)       37 2022-03-15 20:01:04.000000 seelabutk-substrate-1.7.2/src/substrate/__main__.py
--rwxr-xr-x   0 john      (1000) john      (1000)     4949 2023-04-24 15:23:57.000000 seelabutk-substrate-1.7.2/src/substrate/substrate.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/substrate/targets/
--rw-r--r--   0 john      (1000) john      (1000)       70 2022-04-26 20:17:06.000000 seelabutk-substrate-1.7.2/src/substrate/targets/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     8833 2022-10-27 18:11:48.000000 seelabutk-substrate-1.7.2/src/substrate/targets/aws_stack.py
--rw-r--r--   0 john      (1000) john      (1000)     4013 2022-10-06 16:06:33.000000 seelabutk-substrate-1.7.2/src/substrate/targets/docker_swarm.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/
--rw-r--r--   0 john      (1000) john      (1000)      230 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.2/src/substrate/tools/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)     1861 2022-10-26 12:39:49.000000 seelabutk-substrate-1.7.2/src/substrate/tools/braid.py
--rw-r--r--   0 john      (1000) john      (1000)     1610 2023-04-24 15:25:26.000000 seelabutk-substrate-1.7.2/src/substrate/tools/generic_tool.py
--rw-r--r--   0 john      (1000) john      (1000)     1138 2022-10-03 16:39:17.000000 seelabutk-substrate-1.7.2/src/substrate/tools/hello_world.py
--rw-r--r--   0 john      (1000) john      (1000)     1236 2023-03-29 17:36:36.000000 seelabutk-substrate-1.7.2/src/substrate/tools/nc_slicer.py
--rw-r--r--   0 john      (1000) john      (1000)     1141 2022-10-03 16:41:49.000000 seelabutk-substrate-1.7.2/src/substrate/tools/ospray_studio.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.662733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/
--rw-r--r--   0 john      (1000) john      (1000)       84 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/constants.js
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/css/
--rw-r--r--   0 john      (1000) john      (1000)     3636 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/css/style.css
--rw-r--r--   0 john      (1000) john      (1000)     2604 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/index.html
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/
--rw-r--r--   0 john      (1000) john      (1000)    11262 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/arcball.js
--rw-r--r--   0 john      (1000) john      (1000)    48508 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gremlins.min.js
--rw-r--r--   0 john      (1000) john      (1000)    22951 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gui.js
--rw-r--r--   0 john      (1000) john      (1000)      447 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/main.js
--rw-r--r--   0 john      (1000) john      (1000)     5837 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/math.js
--rw-r--r--   0 john      (1000) john      (1000)    11962 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/smooth.js
--rw-r--r--   0 john      (1000) john      (1000)    13584 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/sylvester.js
--rw-r--r--   0 john      (1000) john      (1000)    27906 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tapestry.js
--rw-r--r--   0 john      (1000) john      (1000)     5322 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/testing.js
--rw-r--r--   0 john      (1000) john      (1000)     4682 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tools.js
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:27:00.672733 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/config/
--rw-r--r--   0 john      (1000) john      (1000)      244 2022-09-23 18:36:10.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/config/data.json
--rw-r--r--   0 john      (1000) john      (1000)     2160 2022-10-04 13:27:23.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tapestry.py
--rw-r--r--   0 john      (1000) john      (1000)     1401 2023-04-24 15:16:24.000000 seelabutk-substrate-1.7.2/src/substrate/tools/tool.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/
+-rw-r--r--   0 john      (1000) john      (1000)    16674 2022-03-29 18:24:57.000000 seelabutk-substrate-1.8.0/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     3608 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     3166 2023-04-24 15:33:03.000000 seelabutk-substrate-1.8.0/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      757 2023-04-24 15:33:21.000000 seelabutk-substrate-1.8.0/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)      444 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.632725 seelabutk-substrate-1.8.0/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.632725 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     3608 2023-04-24 15:33:52.000000 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1422 2023-04-24 15:33:52.000000 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-24 15:33:52.000000 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       55 2023-04-24 15:33:52.000000 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)      100 2023-04-24 15:33:52.000000 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       10 2023-04-24 15:33:52.000000 seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.632725 seelabutk-substrate-1.8.0/src/substrate/
+-rw-r--r--   0 john      (1000) john      (1000)       33 2022-03-15 19:56:07.000000 seelabutk-substrate-1.8.0/src/substrate/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)       37 2022-03-15 20:01:04.000000 seelabutk-substrate-1.8.0/src/substrate/__main__.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     4949 2023-04-24 15:23:57.000000 seelabutk-substrate-1.8.0/src/substrate/substrate.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/src/substrate/targets/
+-rw-r--r--   0 john      (1000) john      (1000)       70 2022-04-26 20:17:06.000000 seelabutk-substrate-1.8.0/src/substrate/targets/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     8833 2022-10-27 18:11:48.000000 seelabutk-substrate-1.8.0/src/substrate/targets/aws_stack.py
+-rw-r--r--   0 john      (1000) john      (1000)     4013 2022-10-06 16:06:33.000000 seelabutk-substrate-1.8.0/src/substrate/targets/docker_swarm.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/src/substrate/tools/
+-rw-r--r--   0 john      (1000) john      (1000)      230 2023-03-29 17:36:36.000000 seelabutk-substrate-1.8.0/src/substrate/tools/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)     1861 2022-10-26 12:39:49.000000 seelabutk-substrate-1.8.0/src/substrate/tools/braid.py
+-rw-r--r--   0 john      (1000) john      (1000)     1610 2023-04-24 15:25:26.000000 seelabutk-substrate-1.8.0/src/substrate/tools/generic_tool.py
+-rw-r--r--   0 john      (1000) john      (1000)     1138 2022-10-03 16:39:17.000000 seelabutk-substrate-1.8.0/src/substrate/tools/hello_world.py
+-rw-r--r--   0 john      (1000) john      (1000)     1236 2023-03-29 17:36:36.000000 seelabutk-substrate-1.8.0/src/substrate/tools/nc_slicer.py
+-rw-r--r--   0 john      (1000) john      (1000)     1141 2022-10-03 16:41:49.000000 seelabutk-substrate-1.8.0/src/substrate/tools/ospray_studio.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.632725 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/
+-rw-r--r--   0 john      (1000) john      (1000)       84 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/constants.js
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/css/
+-rw-r--r--   0 john      (1000) john      (1000)     3636 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/css/style.css
+-rw-r--r--   0 john      (1000) john      (1000)     2604 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/index.html
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/
+-rw-r--r--   0 john      (1000) john      (1000)    11262 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/arcball.js
+-rw-r--r--   0 john      (1000) john      (1000)    48508 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/gremlins.min.js
+-rw-r--r--   0 john      (1000) john      (1000)    22951 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/gui.js
+-rw-r--r--   0 john      (1000) john      (1000)      447 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/main.js
+-rw-r--r--   0 john      (1000) john      (1000)     5837 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/math.js
+-rw-r--r--   0 john      (1000) john      (1000)    11962 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/smooth.js
+-rw-r--r--   0 john      (1000) john      (1000)    13584 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/sylvester.js
+-rw-r--r--   0 john      (1000) john      (1000)    27906 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/tapestry.js
+-rw-r--r--   0 john      (1000) john      (1000)     5322 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/testing.js
+-rw-r--r--   0 john      (1000) john      (1000)     4682 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/tools.js
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-24 15:33:52.642725 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/config/
+-rw-r--r--   0 john      (1000) john      (1000)      244 2022-09-23 18:36:10.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/config/data.json
+-rw-r--r--   0 john      (1000) john      (1000)     2160 2022-10-04 13:27:23.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tapestry.py
+-rw-r--r--   0 john      (1000) john      (1000)     1401 2023-04-24 15:16:24.000000 seelabutk-substrate-1.8.0/src/substrate/tools/tool.py
```

### Comparing `seelabutk-substrate-1.7.2/LICENSE` & `seelabutk-substrate-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/PKG-INFO` & `seelabutk-substrate-1.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: seelabutk-substrate
-Version: 1.7.2
-Summary: Automatically deploys visualization services via Docker Swarm
-Author-email: John Duggan <jduggan1@utk.edu>
-License: CC-BY-4.0
-Project-URL: Homepage, https://github.com/seelabutk/substrate/
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Substrate
 
 Substrate is a tool that allows you to automate the process of deploying visualization tools to different computing environments.
 
 ### Supported Visualization tools
 
 - NetCDF Slicer
@@ -62,19 +49,27 @@
 - tapestry
 - braid
 
 ### Configuration
 
 Substrate is configured using `substrate.config.yaml`. The tool will look for this file starting in your current working directory then look for it in parent folders. You can also provide a path with
 
-	substrate tapestry start -c /path/to/substrate.config.yaml
+	substrate tapestry start -f /path/to/substrate.config.yaml
+
+or
+
+	stack = Substrate('tool_name', {}, path='path/to/substrate.config.yaml')
+
+You may also specify the config directly via JSON/a dictionary with
+
+	substrate tapestry start -c "{ config here... }"
 
 or
 
-	stack = Substrate('tool_name', path='path/to/substrate.config.yaml')
+	stack = Substrate('tool_name', config)
 
 The options for the configuration file can be found [here](api/substrate.config.yaml).
 
 Each tool has static files that are needed to run it. Defaults are provided, but if needed or desired they can be modified. Here are links to get the default files for [Tapestry](src/substrate/tapestry) and [Braid](src/substrate/vci).
 
 For more information on configuring each tool, please refer to each tools documentation:
 - NetCDF Slicer: coming soon
```

### Comparing `seelabutk-substrate-1.7.2/README.md` & `seelabutk-substrate-1.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: seelabutk-substrate
+Version: 1.8.0
+Summary: Automatically deploys visualization services via Docker Swarm
+Author-email: John Duggan <jduggan1@utk.edu>
+License: CC-BY-4.0
+Project-URL: Homepage, https://github.com/seelabutk/substrate/
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Substrate
 
 Substrate is a tool that allows you to automate the process of deploying visualization tools to different computing environments.
 
 ### Supported Visualization tools
 
 - NetCDF Slicer
@@ -49,19 +62,27 @@
 - tapestry
 - braid
 
 ### Configuration
 
 Substrate is configured using `substrate.config.yaml`. The tool will look for this file starting in your current working directory then look for it in parent folders. You can also provide a path with
 
-	substrate tapestry start -c /path/to/substrate.config.yaml
+	substrate tapestry start -f /path/to/substrate.config.yaml
+
+or
+
+	stack = Substrate('tool_name', {}, path='path/to/substrate.config.yaml')
+
+You may also specify the config directly via JSON/a dictionary with
+
+	substrate tapestry start -c "{ config here... }"
 
 or
 
-	stack = Substrate('tool_name', path='path/to/substrate.config.yaml')
+	stack = Substrate('tool_name', config)
 
 The options for the configuration file can be found [here](api/substrate.config.yaml).
 
 Each tool has static files that are needed to run it. Defaults are provided, but if needed or desired they can be modified. Here are links to get the default files for [Tapestry](src/substrate/tapestry) and [Braid](src/substrate/vci).
 
 For more information on configuring each tool, please refer to each tools documentation:
 - NetCDF Slicer: coming soon
```

### Comparing `seelabutk-substrate-1.7.2/pyproject.toml` & `seelabutk-substrate-1.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	'requests ~= 2.27.1'
 ]
 description = "Automatically deploys visualization services via Docker Swarm"
 entry-points = {console_scripts = {substrate = "substrate.substrate:main"}}
 license = {text = "CC-BY-4.0"}
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.7.2"
+version = "1.8.0"
 
 [project.urls]
 Homepage = "https://github.com/seelabutk/substrate/"
 
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
```

### Comparing `seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/PKG-INFO` & `seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seelabutk-substrate
-Version: 1.7.2
+Version: 1.8.0
 Summary: Automatically deploys visualization services via Docker Swarm
 Author-email: John Duggan <jduggan1@utk.edu>
 License: CC-BY-4.0
 Project-URL: Homepage, https://github.com/seelabutk/substrate/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -62,19 +62,27 @@
 - tapestry
 - braid
 
 ### Configuration
 
 Substrate is configured using `substrate.config.yaml`. The tool will look for this file starting in your current working directory then look for it in parent folders. You can also provide a path with
 
-	substrate tapestry start -c /path/to/substrate.config.yaml
+	substrate tapestry start -f /path/to/substrate.config.yaml
 
 or
 
-	stack = Substrate('tool_name', path='path/to/substrate.config.yaml')
+	stack = Substrate('tool_name', {}, path='path/to/substrate.config.yaml')
+
+You may also specify the config directly via JSON/a dictionary with
+
+	substrate tapestry start -c "{ config here... }"
+
+or
+
+	stack = Substrate('tool_name', config)
 
 The options for the configuration file can be found [here](api/substrate.config.yaml).
 
 Each tool has static files that are needed to run it. Defaults are provided, but if needed or desired they can be modified. Here are links to get the default files for [Tapestry](src/substrate/tapestry) and [Braid](src/substrate/vci).
 
 For more information on configuring each tool, please refer to each tools documentation:
 - NetCDF Slicer: coming soon
```

### Comparing `seelabutk-substrate-1.7.2/src/seelabutk_substrate.egg-info/SOURCES.txt` & `seelabutk-substrate-1.8.0/src/seelabutk_substrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/substrate.py` & `seelabutk-substrate-1.8.0/src/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/targets/aws_stack.py` & `seelabutk-substrate-1.8.0/src/substrate/targets/aws_stack.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/targets/docker_swarm.py` & `seelabutk-substrate-1.8.0/src/substrate/targets/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/braid.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/braid.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/generic_tool.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/generic_tool.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/hello_world.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/hello_world.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/nc_slicer.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/nc_slicer.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/ospray_studio.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/ospray_studio.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/css/style.css` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/css/style.css`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/index.html` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/index.html`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/arcball.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/arcball.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gremlins.min.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/gremlins.min.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/gui.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/gui.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/math.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/math.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/smooth.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/smooth.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/sylvester.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/sylvester.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tapestry.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/tapestry.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/testing.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/testing.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry/app/js/tools.js` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry/app/js/tools.js`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tapestry.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/tapestry.py`

 * *Files identical despite different names*

### Comparing `seelabutk-substrate-1.7.2/src/substrate/tools/tool.py` & `seelabutk-substrate-1.8.0/src/substrate/tools/tool.py`

 * *Files identical despite different names*

