# Comparing `tmp/vantage6-node-3.8.2rc1.tar.gz` & `tmp/vantage6-node-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-3.8.2rc1.tar", last modified: Wed Mar 22 14:57:51 2023, max compression
+gzip compressed data, was "vantage6-node-3.8.3.tar", last modified: Tue Apr 25 11:55:43 2023, max compression
```

## Comparing `vantage6-node-3.8.2rc1.tar` & `vantage6-node-3.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.630560 vantage6-node-3.8.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-22 14:57:51.630560 vantage6-node-3.8.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 14:57:51.630560 vantage6-node-3.8.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.622560 vantage6-node-3.8.2rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.622560 vantage6-node-3.8.2rc1/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.626560 vantage6-node-3.8.2rc1/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    38230 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.626560 vantage6-node-3.8.2rc1/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.626560 vantage6-node-3.8.2rc1/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/server_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.626560 vantage6-node-3.8.2rc1/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-03-22 14:57:38.000000 vantage6-node-3.8.2rc1/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 14:57:51.630560 vantage6-node-3.8.2rc1/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-22 14:57:51.000000 vantage6-node-3.8.2rc1/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-22 14:57:51.000000 vantage6-node-3.8.2rc1/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 14:57:51.000000 vantage6-node-3.8.2rc1/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 14:57:51.000000 vantage6-node-3.8.2rc1/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-22 14:57:51.000000 vantage6-node-3.8.2rc1/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-22 14:57:51.000000 vantage6-node-3.8.2rc1/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.701693 vantage6-node-3.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.701693 vantage6-node-3.8.3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.701693 vantage6-node-3.8.3/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    38328 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21281 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/server_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-25 11:55:29.000000 vantage6-node-3.8.3/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:43.705693 vantage6-node-3.8.3/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 11:55:43.000000 vantage6-node-3.8.3/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-3.8.2rc1/PKG-INFO` & `vantage6-node-3.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.2rc1 Summary: vantage6
-node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.3 Summary: vantage6 node
+Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
```

### Comparing `vantage6-node-3.8.2rc1/setup.py` & `vantage6-node-3.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/__init__.py` & `vantage6-node-3.8.3/vantage6/node/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,14 +803,17 @@
         self.socketIO.start_background_task(self.__socket_ping_worker)
 
     def __socket_ping_worker(self) -> None:
         """
         Send ping messages periodically to the server over the socketIO
         connection to notify the server that this node is online
         """
+        # Wait for the socket to be connected to the namespaces on startup
+        time.sleep(5)
+
         while True:
             try:
                 self.socketIO.emit('ping', namespace='/tasks')
             except Exception:
                 self.log.exception('Ping thread had an exception')
             # Wait before sending next ping
             time.sleep(PING_INTERVAL_SECONDS)
```

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/_version.py` & `vantage6-node-3.8.3/vantage6/node/_version.py`

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

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/cli/node.py` & `vantage6-node-3.8.3/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/context.py` & `vantage6-node-3.8.3/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/docker/docker_base.py` & `vantage6-node-3.8.3/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/docker/docker_manager.py` & `vantage6-node-3.8.3/vantage6/node/docker/docker_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-3.8.3/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/docker/task_manager.py` & `vantage6-node-3.8.3/vantage6/node/docker/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,22 @@
         Checks if algorithm container is finished
 
         Returns
         -------
         bool:
             True if algorithm container is finished
         """
-        self.container.reload()
+        try:
+            self.container.reload()
+        except docker.errors.NotFound:
+            self.log.error("Container not found")
+            self.log.debug(f"- task id: {self.task_id}")
+            self.log.debug(f"- result id: {self.task_id}")
+            self.status = TaskStatus.UNKNOWN_ERROR
+            return True
         return self.container.status == 'exited'
 
     def report_status(self) -> str:
         """
         Checks if algorithm has exited successfully. If not, it prints an
         error message
```

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/docker/vpn_manager.py` & `vantage6-node-3.8.3/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/globals.py` & `vantage6-node-3.8.3/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/proxy_server.py` & `vantage6-node-3.8.3/vantage6/node/proxy_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/server_io.py` & `vantage6-node-3.8.3/vantage6/node/server_io.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/socket.py` & `vantage6-node-3.8.3/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/util/__init__.py` & `vantage6-node-3.8.3/vantage6/node/util/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6/node/util/colorer.py` & `vantage6-node-3.8.3/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-3.8.2rc1/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-3.8.3/vantage6_node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 3.8.2rc1
+Version: 3.8.3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.2rc1 Summary: vantage6
-node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
+Metadata-Version: 2.1 Name: vantage6-node Version: 3.8.3 Summary: vantage6 node
+Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml) [![PyPI vantage6](https://badge.fury.io/py/vantage6.svg)](https://
```

### Comparing `vantage6-node-3.8.2rc1/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-3.8.3/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

