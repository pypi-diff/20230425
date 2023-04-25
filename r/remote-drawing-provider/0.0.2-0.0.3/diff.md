# Comparing `tmp/remote-drawing-provider-0.0.2.tar.gz` & `tmp/remote-drawing-provider-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-drawing-provider-0.0.2.tar", last modified: Tue Apr 25 05:44:35 2023, max compression
+gzip compressed data, was "remote-drawing-provider-0.0.3.tar", last modified: Tue Apr 25 05:59:49 2023, max compression
```

## Comparing `remote-drawing-provider-0.0.2.tar` & `remote-drawing-provider-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 05:44:35.138240 remote-drawing-provider-0.0.2/
--rw-rw-rw-   0        0        0     1066 2023-04-25 05:29:24.000000 remote-drawing-provider-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      797 2023-04-25 05:44:35.138240 remote-drawing-provider-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-25 05:02:34.000000 remote-drawing-provider-0.0.2/README.md
--rw-rw-rw-   0        0        0      565 2023-04-25 05:43:53.000000 remote-drawing-provider-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 05:44:35.138240 remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/
--rw-rw-rw-   0        0        0      797 2023-04-25 05:44:35.000000 remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-04-25 05:44:35.000000 remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 05:44:35.000000 remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-25 05:44:35.000000 remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 05:44:35.000000 remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 05:44:35.138240 remote-drawing-provider-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-04-25 05:44:16.000000 remote-drawing-provider-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 05:44:35.138240 remote-drawing-provider-0.0.2/src/
--rw-rw-rw-   0        0        0     1198 2023-04-25 02:41:07.000000 remote-drawing-provider-0.0.2/src/logger.py
--rw-rw-rw-   0        0        0      984 2023-04-25 05:01:43.000000 remote-drawing-provider-0.0.2/src/provider.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:59:49.826904 remote-drawing-provider-0.0.3/
+-rw-rw-rw-   0        0        0     1066 2023-04-25 05:29:24.000000 remote-drawing-provider-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      797 2023-04-25 05:59:49.826904 remote-drawing-provider-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-25 05:02:34.000000 remote-drawing-provider-0.0.3/README.md
+-rw-rw-rw-   0        0        0      565 2023-04-25 05:52:04.000000 remote-drawing-provider-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 05:59:49.826904 remote-drawing-provider-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-04-25 05:54:06.000000 remote-drawing-provider-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:59:49.811274 remote-drawing-provider-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 05:59:49.826904 remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-04-25 05:59:49.000000 remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-04-25 05:59:49.000000 remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 05:59:49.000000 remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-25 05:59:49.000000 remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 05:59:49.000000 remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/top_level.txt
```

### Comparing `remote-drawing-provider-0.0.2/LICENSE` & `remote-drawing-provider-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remote-drawing-provider-0.0.2/PKG-INFO` & `remote-drawing-provider-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-drawing-provider
-Version: 0.0.2
+Version: 0.0.3
 Summary: Remote Drawing Provider
 Home-page: https://github.com/XiaoyanQian/remote-drawing
 Author: XiaoyanQian
 Author-email: thinkershare <thinkershare@163.com>
 Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
 Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `remote-drawing-provider-0.0.2/pyproject.toml` & `remote-drawing-provider-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "remote-drawing-provider"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="thinkershare", email="thinkershare@163.com" },
 ]
 description = "Remote Drawing Provider"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `remote-drawing-provider-0.0.2/remote_drawing_provider.egg-info/PKG-INFO` & `remote-drawing-provider-0.0.3/src/remote_drawing_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-drawing-provider
-Version: 0.0.2
+Version: 0.0.3
 Summary: Remote Drawing Provider
 Home-page: https://github.com/XiaoyanQian/remote-drawing
 Author: XiaoyanQian
 Author-email: thinkershare <thinkershare@163.com>
 Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
 Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
 Classifier: Programming Language :: Python :: 3
```

