# Comparing `tmp/statick-md-0.1.1.tar.gz` & `tmp/statick-md-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statick-md-0.1.1.tar", last modified: Mon Oct 10 21:09:05 2022, max compression
+gzip compressed data, was "statick-md-0.1.3.tar", last modified: Tue Apr 25 02:39:22 2023, max compression
```

## Comparing `statick-md-0.1.1.tar` & `statick-md-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.272398 statick-md-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6401 2022-10-10 21:08:58.000000 statick-md-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     6569 2022-10-10 21:09:05.272398 statick-md-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5978 2022-10-10 21:08:58.000000 statick-md-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.268398 statick-md-0.1.1/rsc/
--rw-r--r--   0 runner    (1001) docker     (116)      234 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/.markdownlintrc
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/markdownlint-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1101 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/md-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/md-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/rst-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       18 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/rstcheck-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/rstlint-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       19 2022-10-10 21:08:58.000000 statick-md-0.1.1/rsc/writegood-profile.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-10 21:09:05.272398 statick-md-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2022-10-10 21:08:58.000000 statick-md-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.264398 statick-md-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.264398 statick-md-0.1.1/src/statick_md/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.264398 statick-md-0.1.1/src/statick_md/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.268398 statick-md-0.1.1/src/statick_md/plugins/discovery/
--rw-r--r--   0 runner    (1001) docker     (116)       33 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1412 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/discovery/markdown_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/discovery/markdown_discovery_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     1379 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/discovery/rst_discovery_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/discovery/rst_discovery_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.272398 statick-md-0.1.1/src/statick_md/plugins/tool/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4073 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/markdownlint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       73 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/markdownlint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     3480 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/proselint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/proselint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     2894 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/rstcheck_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       65 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/rstcheck_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     2355 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/rstlint_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       63 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/rstlint_tool_plugin.yapsy-plugin
--rw-r--r--   0 runner    (1001) docker     (116)     2826 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/writegood_tool_plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-10 21:08:58.000000 statick-md-0.1.1/src/statick_md/plugins/tool/writegood_tool_plugin.yapsy-plugin
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-10 21:09:05.272398 statick-md-0.1.1/statick_md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6569 2022-10-10 21:09:05.000000 statick-md-0.1.1/statick_md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2022-10-10 21:09:05.000000 statick-md-0.1.1/statick_md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-10 21:09:05.000000 statick-md-0.1.1/statick_md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       76 2022-10-10 21:09:05.000000 statick-md-0.1.1/statick_md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-10 21:09:05.000000 statick-md-0.1.1/statick_md.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.231299 statick-md-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-25 02:39:17.000000 statick-md-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-25 02:39:22.231299 statick-md-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-25 02:39:17.000000 statick-md-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.227298 statick-md-0.1.3/rsc/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/.markdownlintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/markdownlint-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/md-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/md-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/rst-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/rstcheck-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/rstlint-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 02:39:17.000000 statick-md-0.1.3/rsc/writegood-profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:39:22.231299 statick-md-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-25 02:39:17.000000 statick-md-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.227298 statick-md-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.227298 statick-md-0.1.3/src/statick_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.227298 statick-md-0.1.3/src/statick_md/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.227298 statick-md-0.1.3/src/statick_md/plugins/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/discovery/markdown_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/discovery/markdown_discovery_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/discovery/rst_discovery_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/discovery/rst_discovery_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.231299 statick-md-0.1.3/src/statick_md/plugins/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/markdownlint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/markdownlint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/proselint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/proselint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/rstcheck_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/rstcheck_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/rstlint_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/rstlint_tool_plugin.yapsy-plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/writegood_tool_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 02:39:17.000000 statick-md-0.1.3/src/statick_md/plugins/tool/writegood_tool_plugin.yapsy-plugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:39:22.231299 statick-md-0.1.3/statick_md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-04-25 02:39:22.000000 statick-md-0.1.3/statick_md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-25 02:39:22.000000 statick-md-0.1.3/statick_md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:39:22.000000 statick-md-0.1.3/statick_md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 02:39:22.000000 statick-md-0.1.3/statick_md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 02:39:22.000000 statick-md-0.1.3/statick_md.egg-info/top_level.txt
```

### Comparing `statick-md-0.1.1/LICENSE` & `statick-md-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/PKG-INFO` & `statick-md-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: statick-md
-Version: 0.1.1
+Version: 0.1.3
 Summary: Statick analysis plugins for Markdown files.
 Home-page: https://github.com/sscpac/statick-md
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
 
 # Statick Markdown Plugins
```

### Comparing `statick-md-0.1.1/README.md` & `statick-md-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/rsc/md-config.yaml` & `statick-md-0.1.3/rsc/md-config.yaml`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/setup.py` & `statick-md-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "test": TEST_DEPS,
 }
 
 setup(
     author="NIWC Pacific",
     name="statick-md",
     description="Statick analysis plugins for Markdown files.",
-    version="0.1.1",
+    version="0.1.3",
     packages=[
         "statick_tool",
         "statick_tool.plugins.discovery",
         "statick_tool.plugins.tool",
     ],
     package_dir={
         "statick_tool": ".",
@@ -49,10 +49,11 @@
     url="https://github.com/sscpac/statick-md",
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

### Comparing `statick-md-0.1.1/src/statick_md/plugins/discovery/markdown_discovery_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/discovery/markdown_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/src/statick_md/plugins/discovery/rst_discovery_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/discovery/rst_discovery_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/src/statick_md/plugins/tool/markdownlint_tool_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/tool/markdownlint_tool_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,36 +39,43 @@
         flags: List[str] = []
         if format_file_name is not None:
             flags += ["-c", format_file_name]
         flags += user_flags
 
         total_output: List[str] = []
 
-        for src in files:
-            try:
-                exe = [tool_bin] + flags + [src]
-                output = subprocess.check_output(
-                    exe, stderr=subprocess.STDOUT, universal_newlines=True
-                )
-                total_output.append(output)
-
-            except subprocess.CalledProcessError as ex:
-                if ex.returncode == 1:  # markdownlint returns 1 upon linting errors
-                    total_output.append(ex.output)
-                else:
-                    logging.warning(
-                        "%s failed! Returncode = %d", tool_bin, ex.returncode
-                    )
-                    logging.warning("%s exception: %s", self.get_name(), ex.output)
-                    return None
-
-            except OSError as ex:
-                logging.warning("Couldn't find %s! (%s)", tool_bin, ex)
+        try:
+            exe = [tool_bin] + flags + files
+            output = subprocess.check_output(
+                exe, stderr=subprocess.STDOUT, universal_newlines=True
+            )
+            total_output.append(output)
+
+        except subprocess.CalledProcessError as ex:
+            if (
+                "Error: Cannot find module" in ex.output
+                or "Require stack:" in ex.output
+            ):
+                # nodejs cannot find a module and threw an error
+                # this results in the same returncode `1` that markdownlint
+                # uses to indicate the presence of linting issues.
+                logging.warning("%s failed! Returncode = %d", tool_bin, ex.returncode)
+                logging.warning("%s exception: %s", self.get_name(), ex.output)
+                return None
+            if ex.returncode == 1:  # markdownlint returns 1 upon linting errors
+                total_output.append(ex.output)
+            else:
+                logging.warning("%s failed! Returncode = %d", tool_bin, ex.returncode)
+                logging.warning("%s exception: %s", self.get_name(), ex.output)
                 return None
 
+        except OSError as ex:
+            logging.warning("Couldn't find %s! (%s)", tool_bin, ex)
+            return None
+
         for output in total_output:
             logging.debug("%s", output)
 
         return total_output
 
     # pylint: enable=too-many-locals
```

### Comparing `statick-md-0.1.1/src/statick_md/plugins/tool/proselint_tool_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/tool/proselint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/src/statick_md/plugins/tool/rstcheck_tool_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/tool/rstcheck_tool_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,36 +29,33 @@
         tool_bin = "rstcheck"
 
         flags: List[str] = []
         flags += user_flags
 
         total_output: List[str] = []
 
-        for src in files:
-            try:
-                exe = [tool_bin] + flags + [src]
-                output = subprocess.check_output(
-                    exe, stderr=subprocess.STDOUT, universal_newlines=True
-                )
-                total_output.append(output)
-
-            except subprocess.CalledProcessError as ex:
-                if ex.returncode == 1:  # markdownlint returns 1 upon linting errors
-                    total_output.append(ex.output)
-                else:
-                    logging.warning(
-                        "%s failed! Returncode = %d", tool_bin, ex.returncode
-                    )
-                    logging.warning("%s exception: %s", self.get_name(), ex.output)
-                    return None
-
-            except OSError as ex:
-                logging.warning("Couldn't find %s! (%s)", tool_bin, ex)
+        try:
+            exe = [tool_bin] + flags + files
+            output = subprocess.check_output(
+                exe, stderr=subprocess.STDOUT, universal_newlines=True
+            )
+            total_output.append(output)
+
+        except subprocess.CalledProcessError as ex:
+            if ex.returncode == 1:  # markdownlint returns 1 upon linting errors
+                total_output.append(ex.output)
+            else:
+                logging.warning("%s failed! Returncode = %d", tool_bin, ex.returncode)
+                logging.warning("%s exception: %s", self.get_name(), ex.output)
                 return None
 
+        except OSError as ex:
+            logging.warning("Couldn't find %s! (%s)", tool_bin, ex)
+            return None
+
         for output in total_output:
             logging.debug("%s", str(output))
 
         return total_output
 
     # pylint: enable=too-many-locals
```

### Comparing `statick-md-0.1.1/src/statick_md/plugins/tool/rstlint_tool_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/tool/rstlint_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/src/statick_md/plugins/tool/writegood_tool_plugin.py` & `statick-md-0.1.3/src/statick_md/plugins/tool/writegood_tool_plugin.py`

 * *Files identical despite different names*

### Comparing `statick-md-0.1.1/statick_md.egg-info/PKG-INFO` & `statick-md-0.1.3/statick_md.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: statick-md
-Version: 0.1.1
+Version: 0.1.3
 Summary: Statick analysis plugins for Markdown files.
 Home-page: https://github.com/sscpac/statick-md
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
 
 # Statick Markdown Plugins
```

### Comparing `statick-md-0.1.1/statick_md.egg-info/SOURCES.txt` & `statick-md-0.1.3/statick_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

