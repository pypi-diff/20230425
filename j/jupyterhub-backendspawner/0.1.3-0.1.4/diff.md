# Comparing `tmp/jupyterhub-backendspawner-0.1.3.tar.gz` & `tmp/jupyterhub-backendspawner-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.1.3.tar", last modified: Tue Apr 25 13:09:27 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.1.4.tar", last modified: Tue Apr 25 13:31:28 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.1.3.tar` & `jupyterhub-backendspawner-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.3/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.3/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.3/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4625 2023-04-25 13:08:09.000000 jupyterhub-backendspawner-0.1.3/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-25 12:26:26.000000 jupyterhub-backendspawner-0.1.3/backendspawner/backendspawner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10031 2023-04-25 12:36:17.000000 jupyterhub-backendspawner-0.1.3/backendspawner/eventspawner.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-25 13:09:27.000000 jupyterhub-backendspawner-0.1.3/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 13:09:27.085981 jupyterhub-backendspawner-0.1.3/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-25 13:09:06.000000 jupyterhub-backendspawner-0.1.3/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.1.4/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.1.4/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.1.4/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4625 2023-04-25 13:08:09.000000 jupyterhub-backendspawner-0.1.4/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17611 2023-04-25 12:26:26.000000 jupyterhub-backendspawner-0.1.4/backendspawner/backendspawner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10080 2023-04-25 13:29:32.000000 jupyterhub-backendspawner-0.1.4/backendspawner/eventspawner.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-04-25 13:31:28.000000 jupyterhub-backendspawner-0.1.4/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-25 13:31:28.975634 jupyterhub-backendspawner-0.1.4/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-04-25 13:31:23.000000 jupyterhub-backendspawner-0.1.4/setup.py
```

### Comparing `jupyterhub-backendspawner-0.1.3/LICENSE` & `jupyterhub-backendspawner-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.3/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.1.4/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.3/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.1.4/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.1.3/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.1.4/backendspawner/eventspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,32 +181,34 @@
         now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
         event = {
             "progress": 99,
             "failed": False,
             "html_message": f"<details><summary>{now}: JupyterLab start failed. Deleting related resources...</summary>This may take a few seconds.</details>",
         }
         self.latest_events.append(event)
+        msg = "Unknown Error"
+        if hasattr(exception, "args") and len(exception.args) > 1:
+            msg = f"{exception.args[0]} - {exception.args[1]}"
         if hasattr(exception, "args") and len(exception.args) > 2:
             try:
                 body = json.loads(exception.args[2].body.decode())
+                msg += f": {body}"
             except:
                 self.log.exception("Could not load detailed error message")
-                body = "unknown error"
-            msg = f"{exception.args[0]} - {exception.args[1]}: {body}"
 
-            async def _get_stop_event(spawner):
-                now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
-                event = {
-                    "progress": 100,
-                    "failed": True,
-                    "html_message": f"<details><summary>{now}: JupyterLab stopped.</summary>{msg}</details>",
-                }
-                return event
+        async def _get_stop_event(spawner):
+            now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
+            event = {
+                "progress": 100,
+                "failed": True,
+                "html_message": f"<details><summary>{now}: JupyterLab stopped.</summary>{msg}</details>",
+            }
+            return event
 
-            self.stop_event = _get_stop_event
+        self.stop_event = _get_stop_event
         return super().run_failed_spawn_request_hook(exception)
 
     def run_pre_spawn_hook(self):
         """Some commands are required."""
         if self.already_stopped:
             raise Exception("Server is in the process of stopping, please wait.")
```

### Comparing `jupyterhub-backendspawner-0.1.3/setup.py` & `jupyterhub-backendspawner-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.1.3",
+    version="0.1.4",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

