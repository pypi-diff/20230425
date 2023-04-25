# Comparing `tmp/vantage6-node-3.8.3.tar.gz` & `tmp/vantage6-node-3.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-3.8.3.tar", last modified: Tue Apr 25 11:55:43 2023, max compression
+gzip compressed data, was "vantage6-node-3.8.4.tar", last modified: Tue Apr 25 13:31:04 2023, max compression
```

## Comparing `vantage6-node-3.8.3.tar` & `vantage6-node-3.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.701693 vantage6-node-3.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.701693 vantage6-node-3.8.3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.701693 vantage6-node-3.8.3/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    38328 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/server_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.254246 vantage6-node-3.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 13:31:04.254246 vantage6-node-3.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:31:04.254246 vantage6-node-3.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.246246 vantage6-node-3.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.242246 vantage6-node-3.8.4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.246246 vantage6-node-3.8.4/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    38328 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.250246 vantage6-node-3.8.4/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.250246 vantage6-node-3.8.4/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/server_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.250246 vantage6-node-3.8.4/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-25 13:30:46.000000 vantage6-node-3.8.4/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:04.254246 vantage6-node-3.8.4/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 13:31:04.000000 vantage6-node-3.8.4/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 13:31:04.000000 vantage6-node-3.8.4/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:31:04.000000 vantage6-node-3.8.4/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 13:31:04.000000 vantage6-node-3.8.4/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-25 13:31:04.000000 vantage6-node-3.8.4/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 13:31:04.000000 vantage6-node-3.8.4/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-3.8.3/PKG-INFO` & `vantage6-node-3.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.3
+Version: 3.8.4
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.3 Summary: vantage6 node
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.4 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.8.3/setup.py` & `vantage6-node-3.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/__init__.py` & `vantage6-node-3.8.4/vantage6/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/_version.py` & `vantage6-node-3.8.4/vantage6/node/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 3, 'final', __build__, 0)))
+version_info = ((( 3, 8, 4, 'final', __build__, 0)))
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-node-3.8.3/vantage6/node/cli/node.py` & `vantage6-node-3.8.4/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/context.py` & `vantage6-node-3.8.4/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/docker/docker_base.py` & `vantage6-node-3.8.4/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/docker/docker_manager.py` & `vantage6-node-3.8.4/vantage6/node/docker/docker_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.vpn_manager import VPNManager
 from vantage6.node.docker.task_manager import DockerTaskManager
 from vantage6.node.util import logger_name
 from vantage6.node.server_io import NodeClient
 from vantage6.node.docker.exceptions import (
     UnknownAlgorithmStartFail,
-    PermanentAlgorithmStartFail
+    PermanentAlgorithmStartFail,
+    AlgorithmContainerNotFound
 )
 
 log = logging.getLogger(logger_name(__name__))
 
 
 class Result(NamedTuple):
     # """ Data class to store the result of the docker image."""
@@ -462,15 +463,30 @@
             result of the docker image
         """
 
         # get finished results and get the first one, if no result is available
         # this is blocking
         finished_tasks = []
         while (not finished_tasks) and (not self.failed_tasks):
-            finished_tasks = [t for t in self.active_tasks if t.is_finished()]
+            for task in self.active_tasks:
+
+                try:
+                    if task.is_finished():
+                        finished_tasks.append(task)
+                        self.active_tasks.remove(task)
+                except AlgorithmContainerNotFound:
+                    self.log.exception(f'Failed to find container for '
+                                       f'result {task.result_id}')
+                    self.failed_tasks.append(task)
+                    self.active_tasks.remove(task)
+
+                # when we found the first task we start processing it
+                break
+
+            # sleep for a second before checking again
             time.sleep(1)
 
         if finished_tasks:
             # at least one task is finished
 
             finished_task = finished_tasks.pop()
             self.log.debug(f"Result id={finished_task.result_id} is finished")
@@ -480,26 +496,23 @@
 
             # Cleanup containers
             finished_task.cleanup()
 
             # Retrieve results from file
             results = finished_task.get_results()
 
-            # remove finished tasks from active task list
-            self.active_tasks.remove(finished_task)
-
             # remove the VPN ports of this run from the database
             self.client.request(
                 'port', params={'result_id': finished_task.result_id},
                 method="DELETE"
             )
         else:
             # at least one task failed to start
             finished_task = self.failed_tasks.pop()
-            logs = 'Container failed to start'
+            logs = 'Container failed'
             results = b''
 
         return Result(
             result_id=finished_task.result_id,
             task_id=finished_task.task_id,
             logs=logs,
             data=results,
```

### Comparing `vantage6-node-3.8.3/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-3.8.4/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/docker/task_manager.py` & `vantage6-node-3.8.4/vantage6/node/docker/task_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from vantage6.common.task_status import TaskStatus
 from vantage6.node.util import logger_name, get_parent_id
 from vantage6.node.globals import ALPINE_IMAGE
 from vantage6.node.docker.vpn_manager import VPNManager
 from vantage6.node.docker.docker_base import DockerBaseManager
 from vantage6.node.docker.exceptions import (
     UnknownAlgorithmStartFail,
-    PermanentAlgorithmStartFail
+    PermanentAlgorithmStartFail,
+    AlgorithmContainerNotFound
 )
 
 
 class DockerTaskManager(DockerBaseManager):
     """
     Manager for running a vantage6 algorithm container within docker.
 
@@ -113,15 +114,16 @@
         try:
             self.container.reload()
         except docker.errors.NotFound:
             self.log.error("Container not found")
             self.log.debug(f"- task id: {self.task_id}")
             self.log.debug(f"- result id: {self.task_id}")
             self.status = TaskStatus.UNKNOWN_ERROR
-            return True
+            raise AlgorithmContainerNotFound
+
         return self.container.status == 'exited'
 
     def report_status(self) -> str:
         """
         Checks if algorithm has exited successfully. If not, it prints an
         error message
```

### Comparing `vantage6-node-3.8.3/vantage6/node/docker/vpn_manager.py` & `vantage6-node-3.8.4/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/globals.py` & `vantage6-node-3.8.4/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/proxy_server.py` & `vantage6-node-3.8.4/vantage6/node/proxy_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/server_io.py` & `vantage6-node-3.8.4/vantage6/node/server_io.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/socket.py` & `vantage6-node-3.8.4/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/util/__init__.py` & `vantage6-node-3.8.4/vantage6/node/util/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6/node/util/colorer.py` & `vantage6-node-3.8.4/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.3/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-3.8.4/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.3
+Version: 3.8.4
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.3 Summary: vantage6 node
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.4 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-node-3.8.3/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-3.8.4/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

