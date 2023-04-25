# Comparing `tmp/jupyterhub-backendspawner-0.1.2.tar.gz` & `tmp/jupyterhub-backendspawner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.1.2.tar", last modified: Tue Apr 25 12:36:59 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.1.3.tar", last modified: Tue Apr 25 13:09:27 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.1.2.tar` & `jupyterhub-backendspawner-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 12:36:58.996497 jupyterhub-backendspawner-0.1.2/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 12:36:58.996497 jupyterhub-backendspawner-0.1.2/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.2/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 12:36:58.996497 jupyterhub-backendspawner-0.1.2/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.2/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4546 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.2/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-25 12:26:26.000000 jupyterhub-backendspawner-0.1.2/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10031 2023-04-25 12:36:17.000000 jupyterhub-backendspawner-0.1.2/backendspawner/eventspawner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 12:36:58.996497 jupyterhub-backendspawner-0.1.2/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 12:36:58.000000 jupyterhub-backendspawner-0.1.2/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-25 12:36:58.000000 jupyterhub-backendspawner-0.1.2/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 12:36:58.000000 jupyterhub-backendspawner-0.1.2/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 12:36:58.000000 jupyterhub-backendspawner-0.1.2/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-25 12:36:58.000000 jupyterhub-backendspawner-0.1.2/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 12:36:58.996497 jupyterhub-backendspawner-0.1.2/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-25 12:26:49.000000 jupyterhub-backendspawner-0.1.2/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.3/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.3/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.3/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4625 2023-04-25 13:08:09.000000 jupyterhub-backendspawner-0.1.3/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-25 12:26:26.000000 jupyterhub-backendspawner-0.1.3/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10031 2023-04-25 12:36:17.000000 jupyterhub-backendspawner-0.1.3/backendspawner/eventspawner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-25 13:09:06.000000 jupyterhub-backendspawner-0.1.3/setup.py
```

### Comparing `jupyterhub-backendspawner-0.1.2/LICENSE` & `jupyterhub-backendspawner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.2/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.1.3/backendspawner/api_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,26 +62,27 @@
                         "uuidcode": uuidcode,
                         "log_name": f"{user_name}:{server_name}",
                         "user": user_name,
                         "action": "cancel",
                         "event": event,
                     },
                 )
+                asyncio.create_task(spawner.stop(cancel=True, event=None))
             else:
                 self.log.debug(
                     "APICall: SpawnUpdate",
                     extra={
                         "uuidcode": uuidcode,
                         "log_name": f"{user_name}:{server_name}",
                         "user": user_name,
                         "action": "failed",
                         "event": event,
                     },
                 )
-            asyncio.create_task(spawner.stop(cancel=True, event=event))
+                asyncio.create_task(spawner.stop(cancel=True, event=event))
             self.set_header("Content-Type", "text/plain")
             self.set_status(204)
             return
 
         if event.get("html_message", ""):
             # Add timestamp
             now = datetime.datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
```

### Comparing `jupyterhub-backendspawner-0.1.2/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.1.3/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.2/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.1.3/backendspawner/eventspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.2/setup.py` & `jupyterhub-backendspawner-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.1.2",
+    version="0.1.3",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

