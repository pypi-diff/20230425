# Comparing `tmp/bitget-python-connector-0.0.1.tar.gz` & `tmp/bitget-python-connector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitget-python-connector-0.0.1.tar", last modified: Tue Apr 25 11:25:48 2023, max compression
+gzip compressed data, was "bitget-python-connector-0.0.2.tar", last modified: Tue Apr 25 11:58:04 2023, max compression
```

## Comparing `bitget-python-connector-0.0.1.tar` & `bitget-python-connector-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 11:25:48.062762 bitget-python-connector-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-04-25 10:21:00.000000 bitget-python-connector-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      592 2023-04-25 11:25:48.062762 bitget-python-connector-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:20:16.000000 bitget-python-connector-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 11:25:48.061761 bitget-python-connector-0.0.1/bitget_python_connector.egg-info/
--rw-rw-rw-   0        0        0      592 2023-04-25 11:25:48.000000 bitget-python-connector-0.0.1/bitget_python_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-25 11:25:48.000000 bitget-python-connector-0.0.1/bitget_python_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 11:25:48.000000 bitget-python-connector-0.0.1/bitget_python_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 11:25:48.000000 bitget-python-connector-0.0.1/bitget_python_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      672 2023-04-25 11:24:45.000000 bitget-python-connector-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 11:25:48.063768 bitget-python-connector-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 11:58:04.015669 bitget-python-connector-0.0.2/
+-rw-rw-rw-   0        0        0     1076 2023-04-25 10:21:00.000000 bitget-python-connector-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      592 2023-04-25 11:58:04.015669 bitget-python-connector-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:20:16.000000 bitget-python-connector-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 11:58:03.997707 bitget-python-connector-0.0.2/bitget_python_connector.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-04-25 11:58:03.000000 bitget-python-connector-0.0.2/bitget_python_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-25 11:58:03.000000 bitget-python-connector-0.0.2/bitget_python_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 11:58:03.000000 bitget-python-connector-0.0.2/bitget_python_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 11:58:03.000000 bitget-python-connector-0.0.2/bitget_python_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      672 2023-04-25 11:57:29.000000 bitget-python-connector-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 11:58:04.015669 bitget-python-connector-0.0.2/setup.cfg
```

### Comparing `bitget-python-connector-0.0.1/LICENSE` & `bitget-python-connector-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.1/PKG-INFO` & `bitget-python-connector-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitget-python-connector
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to easily connect to bitget api.
 Author-email: "Cheng, Chuan-Yi" <parker178912.en08@nycu.edu.tw>
 Project-URL: Homepage, https://github.com/parker178912/bitget-python-connector
 Project-URL: Bug Tracker, https://github.com/parker178912/bitget-python-connector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitget-python-connector-0.0.1/bitget_python_connector.egg-info/PKG-INFO` & `bitget-python-connector-0.0.2/bitget_python_connector.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitget-python-connector
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to easily connect to bitget api.
 Author-email: "Cheng, Chuan-Yi" <parker178912.en08@nycu.edu.tw>
 Project-URL: Homepage, https://github.com/parker178912/bitget-python-connector
 Project-URL: Bug Tracker, https://github.com/parker178912/bitget-python-connector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitget-python-connector-0.0.1/pyproject.toml` & `bitget-python-connector-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitget-python-connector"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Cheng, Chuan-Yi", email="parker178912.en08@nycu.edu.tw" },
 ]
 description = "A tool to easily connect to bitget api."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

