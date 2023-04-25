# Comparing `tmp/jupyterhub-backendspawner-0.1.0.tar.gz` & `tmp/jupyterhub-backendspawner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.1.0.tar", last modified: Mon Apr 24 08:31:56 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.1.1.tar", last modified: Tue Apr 25 09:45:28 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.1.0.tar` & `jupyterhub-backendspawner-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 08:31:56.006498 jupyterhub-backendspawner-0.1.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-24 08:31:56.006498 jupyterhub-backendspawner-0.1.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 08:31:56.006498 jupyterhub-backendspawner-0.1.0/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.0/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4546 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.0/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.0/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10027 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.0/backendspawner/eventspawner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 08:31:56.006498 jupyterhub-backendspawner-0.1.0/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-24 08:31:55.000000 jupyterhub-backendspawner-0.1.0/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-24 08:31:56.000000 jupyterhub-backendspawner-0.1.0/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-24 08:31:55.000000 jupyterhub-backendspawner-0.1.0/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-24 08:31:55.000000 jupyterhub-backendspawner-0.1.0/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-24 08:31:55.000000 jupyterhub-backendspawner-0.1.0/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-24 08:31:56.006498 jupyterhub-backendspawner-0.1.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-24 08:30:59.000000 jupyterhub-backendspawner-0.1.0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 09:45:28.402346 jupyterhub-backendspawner-0.1.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 09:45:28.402346 jupyterhub-backendspawner-0.1.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.1/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 09:45:28.392346 jupyterhub-backendspawner-0.1.1/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.1/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4546 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.1/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.1/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10080 2023-04-25 09:41:49.000000 jupyterhub-backendspawner-0.1.1/backendspawner/eventspawner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 09:45:28.402346 jupyterhub-backendspawner-0.1.1/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 09:45:28.000000 jupyterhub-backendspawner-0.1.1/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-25 09:45:28.000000 jupyterhub-backendspawner-0.1.1/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 09:45:28.000000 jupyterhub-backendspawner-0.1.1/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 09:45:28.000000 jupyterhub-backendspawner-0.1.1/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-25 09:45:28.000000 jupyterhub-backendspawner-0.1.1/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 09:45:28.402346 jupyterhub-backendspawner-0.1.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-25 09:43:42.000000 jupyterhub-backendspawner-0.1.1/setup.py
```

### Comparing `jupyterhub-backendspawner-0.1.0/LICENSE` & `jupyterhub-backendspawner-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.0/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.1.1/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.0/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.1.1/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.0/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.1.1/backendspawner/eventspawner.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,17 +263,18 @@
         if self.already_stopped:
             return
 
         if cancel:
             cancelling_event = await self.get_cancelling_event()
             self.latest_events.append(cancelling_event)
 
-        # always use cancel=False, and call the function later if neccessary.
-        # Otherwise the stop_event would be attached after run_post_stop_hook was called.
-        await super().stop(now, cancel=False)
-
-        if not event:
-            event = await self.get_stop_event()
-        self.latest_events.append(event)
+        try:
+            # always use cancel=False, and call the function later if neccessary.
+            # Otherwise the stop_event would be attached after run_post_stop_hook was called.
+            await super().stop(now, cancel=False)
+        finally:
+            if not event:
+                event = await self.get_stop_event()
+            self.latest_events.append(event)
 
         if cancel:
             await self.cancel()
```

### Comparing `jupyterhub-backendspawner-0.1.0/setup.py` & `jupyterhub-backendspawner-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.1.0",
+    version="0.1.1",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

