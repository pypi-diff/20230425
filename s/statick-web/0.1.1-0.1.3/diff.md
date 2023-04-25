# Comparing `tmp/statick-web-0.1.1.tar.gz` & `tmp/statick-web-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statick-web-0.1.1.tar", last modified: Tue Oct 11 21:27:48 2022, max compression
+gzip compressed data, was "statick-web-0.1.3.tar", last modified: Tue Apr 25 02:36:21 2023, max compression
```

## Comparing `statick-web-0.1.1.tar` & `statick-web-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.712887 statick-web-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6401 2022-10-11 21:27:39.000000 statick-web-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     6545 2022-10-11 21:27:48.712887 statick-web-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5941 2022-10-11 21:27:39.000000 statick-web-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.708887 statick-web-0.1.1/rsc/
--rw-r--r--   0 runner    (1001) docker     (116)      229 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/.eslintrc
--rw-r--r--   0 runner    (1001) docker     (116)       26 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/.htmllintrc
--rw-r--r--   0 runner    (1001) docker     (116)       21 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/.jshintrc
--rw-r--r--   0 runner    (1001) docker     (116)      277 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/.stylelintrc
--rw-r--r--   0 runner    (1001) docker     (116)       16 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/eslint-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       18 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/htmllint-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       16 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/jshint-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       19 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/stylelint-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      944 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/web-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       25 2022-10-11 21:27:39.000000 statick-web-0.1.1/rsc/web-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-11 21:27:48.712887 statick-web-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1491 2022-10-11 21:27:39.000000 statick-web-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.704887 statick-web-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.704887 statick-web-0.1.1/src/statick_web/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.704887 statick-web-0.1.1/src/statick_web/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.708887 statick-web-0.1.1/src/statick_web/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (116)       34 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1442 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/css_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/css_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     1470 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/html_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/html_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     1517 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/javascript_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       79 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/discovery/javascript_discovery_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.712887 statick-web-0.1.1/src/statick_web/plugins/tool/
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5941 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/eslint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/eslint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     3495 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/htmllint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/htmllint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     3526 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/jshint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/jshint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     3707 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/stylelint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-11 21:27:39.000000 statick-web-0.1.1/src/statick_web/plugins/tool/stylelint_tool_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-11 21:27:48.712887 statick-web-0.1.1/statick_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6545 2022-10-11 21:27:48.000000 statick-web-0.1.1/statick_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1362 2022-10-11 21:27:48.000000 statick-web-0.1.1/statick_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-11 21:27:48.000000 statick-web-0.1.1/statick_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-10-11 21:27:48.000000 statick-web-0.1.1/statick_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-11 21:27:48.000000 statick-web-0.1.1/statick_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.234745 statick-web-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-25 02:36:15.000000 statick-web-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-25 02:36:21.234745 statick-web-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-25 02:36:15.000000 statick-web-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.230745 statick-web-0.1.3/rsc/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/.eslintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/.htmllintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/.jshintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/.stylelintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/eslint-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/htmllint-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/jshint-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/stylelint-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/web-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 02:36:15.000000 statick-web-0.1.3/rsc/web-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:36:21.234745 statick-web-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-25 02:36:15.000000 statick-web-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.226745 statick-web-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.226745 statick-web-0.1.3/src/statick_web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.226745 statick-web-0.1.3/src/statick_web/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.230745 statick-web-0.1.3/src/statick_web/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/css_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/css_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/html_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/html_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/javascript_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/discovery/javascript_discovery_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.234745 statick-web-0.1.3/src/statick_web/plugins/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/eslint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/eslint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/htmllint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/htmllint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/jshint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/jshint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/stylelint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:36:15.000000 statick-web-0.1.3/src/statick_web/plugins/tool/stylelint_tool_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:36:21.234745 statick-web-0.1.3/statick_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-25 02:36:21.000000 statick-web-0.1.3/statick_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 02:36:21.000000 statick-web-0.1.3/statick_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:36:21.000000 statick-web-0.1.3/statick_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-25 02:36:21.000000 statick-web-0.1.3/statick_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 02:36:21.000000 statick-web-0.1.3/statick_web.egg-info/top_level.txt
```

### Comparing `statick-web-0.1.1/LICENSE` & `statick-web-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/PKG-INFO` & `statick-web-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: statick-web
-Version: 0.1.1
+Version: 0.1.3
 Summary: Statick analysis plugins for Web (css, html, js) files.
 Home-page: https://github.com/sscpac/statick-web
 Author: NIWC Pacific
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Statick Web Plugins
```

### Comparing `statick-web-0.1.1/README.md` & `statick-web-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/rsc/web-config.yaml` & `statick-web-0.1.3/rsc/web-config.yaml`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/setup.py` & `statick-web-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "test": TEST_DEPS,
 }
 
 setup(
     author="NIWC Pacific",
     name="statick-web",
     description="Statick analysis plugins for Web (css, html, js) files.",
-    version="0.1.1",
+    version="0.1.3",
     packages=[
         "statick_tool",
         "statick_tool.plugins.discovery",
         "statick_tool.plugins.tool",
     ],
     package_dir={
         "statick_tool": ".",
@@ -43,10 +43,11 @@
     url="https://github.com/sscpac/statick-web",
     classifiers=[
         "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Testing",
     ],
 )
```

### Comparing `statick-web-0.1.1/src/statick_web/plugins/discovery/css_discovery_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/discovery/css_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/src/statick_web/plugins/discovery/html_discovery_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/discovery/html_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/src/statick_web/plugins/discovery/javascript_discovery_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/discovery/javascript_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/src/statick_web/plugins/tool/eslint_tool_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/tool/eslint_tool_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,27 @@
                 exe = [tool_bin] + flags + [src]
                 output = subprocess.check_output(
                     exe, stderr=subprocess.STDOUT, universal_newlines=True
                 )
                 total_output.append(output)
 
             except subprocess.CalledProcessError as ex:
+                if (
+                    "Error: Cannot find module" in ex.output
+                    or "Require stack:" in ex.output
+                ):
+                    # nodejs cannot find a module and threw an error
+                    # this results in the same returncode `1` that markdownlint
+                    # uses to indicate the presence of linting issues.
+                    logging.warning(
+                        "%s failed! Returncode = %d", tool_bin, ex.returncode
+                    )
+                    logging.warning("%s exception: %s", self.get_name(), ex.output)
+                    return None
+
                 if ex.returncode == 1:  # eslint returns 1 upon linting errors
                     total_output.append(ex.output)
                 else:
                     logging.warning(
                         "%s failed! Returncode = %d", tool_bin, ex.returncode
                     )
                     logging.warning("%s exception: %s", self.get_name(), ex.output)
```

### Comparing `statick-web-0.1.1/src/statick_web/plugins/tool/htmllint_tool_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/tool/htmllint_tool_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,27 @@
                 exe = [tool_bin] + flags + [src]
                 output = subprocess.check_output(
                     exe, stderr=subprocess.STDOUT, universal_newlines=True
                 )
                 total_output.append(output)
 
             except subprocess.CalledProcessError as ex:
+                if (
+                    "Error: Cannot find module" in ex.output
+                    or "Require stack:" in ex.output
+                ):
+                    # nodejs cannot find a module and threw an error
+                    # this results in the same returncode `1` that markdownlint
+                    # uses to indicate the presence of linting issues.
+                    logging.warning(
+                        "%s failed! Returncode = %d", tool_bin, ex.returncode
+                    )
+                    logging.warning("%s exception: %s", self.get_name(), ex.output)
+                    return None
+
                 # tool returns 1 upon warnings and 2 upon errors
                 if ex.returncode not in [1, 2]:
                     logging.warning(
                         "%s failed! Returncode = %d", tool_bin, ex.returncode
                     )
                     logging.warning("%s exception: %s", self.get_name(), ex.output)
                     return None
```

### Comparing `statick-web-0.1.1/src/statick_web/plugins/tool/jshint_tool_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/tool/jshint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/src/statick_web/plugins/tool/stylelint_tool_plugin.py` & `statick-web-0.1.3/src/statick_web/plugins/tool/stylelint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-web-0.1.1/statick_web.egg-info/PKG-INFO` & `statick-web-0.1.3/statick_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: statick-web
-Version: 0.1.1
+Version: 0.1.3
 Summary: Statick analysis plugins for Web (css, html, js) files.
 Home-page: https://github.com/sscpac/statick-web
 Author: NIWC Pacific
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Statick Web Plugins
```

### Comparing `statick-web-0.1.1/statick_web.egg-info/SOURCES.txt` & `statick-web-0.1.3/statick_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

