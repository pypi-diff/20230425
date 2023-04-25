# Comparing `tmp/bitget-python-connector-0.0.1.tar.gz` & `tmp/bitget-python-connector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitget-python-connector-0.0.1.tar", last modified: Tue Apr 25 11:25:48 2023, max compression
+gzip compressed data, was "bitget-python-connector-0.0.4.tar", last modified: Tue Apr 25 13:24:38 2023, max compression
```

## Comparing `bitget-python-connector-0.0.1.tar` & `bitget-python-connector-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,43 @@
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
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.171166 bitget-python-connector-0.0.4/
+-rw-rw-rw-   0        0        0     1076 2023-04-25 10:21:00.000000 bitget-python-connector-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      592 2023-04-25 13:24:38.171166 bitget-python-connector-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:20:16.000000 bitget-python-connector-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.115631 bitget-python-connector-0.0.4/bitget-python-connector/
+-rw-rw-rw-   0        0        0      193 2023-04-25 13:24:24.000000 bitget-python-connector-0.0.4/bitget-python-connector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.117631 bitget-python-connector-0.0.4/bitget-python-connector/broker/
+-rw-rw-rw-   0        0        0     4261 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/broker/account_api.py
+-rw-rw-rw-   0        0        0     1668 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/broker/manage_api.py
+-rw-rw-rw-   0        0        0     3078 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/client.py
+-rw-rw-rw-   0        0        0     1535 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/consts.py
+-rw-rw-rw-   0        0        0     1208 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.124634 bitget-python-connector-0.0.4/bitget-python-connector/mix/
+-rw-rw-rw-   0        0        0       18 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/__init__.py
+-rw-rw-rw-   0        0        0     5556 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/account_api.py
+-rw-rw-rw-   0        0        0     5582 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/market_api.py
+-rw-rw-rw-   0        0        0     5435 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/order_api.py
+-rw-rw-rw-   0        0        0     8974 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/plan_api.py
+-rw-rw-rw-   0        0        0     1306 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/position_api.py
+-rw-rw-rw-   0        0        0     6103 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/mix/trace_api.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.132632 bitget-python-connector-0.0.4/bitget-python-connector/spot/
+-rw-rw-rw-   0        0        0       18 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/account_api.py
+-rw-rw-rw-   0        0        0     2362 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/market_api.py
+-rw-rw-rw-   0        0        0     4562 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/order_api.py
+-rw-rw-rw-   0        0        0     2811 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/plan_api.py
+-rw-rw-rw-   0        0        0     1182 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/public_api.py
+-rw-rw-rw-   0        0        0     3823 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/spot/wallet_api.py
+-rw-rw-rw-   0        0        0     1625 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.133631 bitget-python-connector-0.0.4/bitget-python-connector/ws/
+-rw-rw-rw-   0        0        0    10899 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/ws/bitget_ws_client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.134632 bitget-python-connector-0.0.4/bitget-python-connector/ws/utils/
+-rw-rw-rw-   0        0        0      485 2023-04-25 10:10:38.000000 bitget-python-connector-0.0.4/bitget-python-connector/ws/utils/sign_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.168166 bitget-python-connector-0.0.4/bitget_python_connector.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-04-25 13:24:38.000000 bitget-python-connector-0.0.4/bitget_python_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2023-04-25 13:24:38.000000 bitget-python-connector-0.0.4/bitget_python_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:24:38.000000 bitget-python-connector-0.0.4/bitget_python_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 13:24:38.000000 bitget-python-connector-0.0.4/bitget_python_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-04-25 13:24:38.000000 bitget-python-connector-0.0.4/bitget_python_connector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:24:38.170166 bitget-python-connector-0.0.4/examples/
+-rw-rw-rw-   0        0        0      247 2023-04-25 11:01:35.000000 bitget-python-connector-0.0.4/examples/spot_example.py
+-rw-rw-rw-   0        0        0      751 2023-04-25 13:24:25.000000 bitget-python-connector-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:24:38.171166 bitget-python-connector-0.0.4/setup.cfg
```

### Comparing `bitget-python-connector-0.0.1/LICENSE` & `bitget-python-connector-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bitget-python-connector-0.0.1/PKG-INFO` & `bitget-python-connector-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitget-python-connector
-Version: 0.0.1
+Version: 0.0.4
 Summary: A tool to easily connect to bitget api.
 Author-email: "Cheng, Chuan-Yi" <parker178912.en08@nycu.edu.tw>
 Project-URL: Homepage, https://github.com/parker178912/bitget-python-connector
 Project-URL: Bug Tracker, https://github.com/parker178912/bitget-python-connector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitget-python-connector-0.0.1/bitget_python_connector.egg-info/PKG-INFO` & `bitget-python-connector-0.0.4/bitget_python_connector.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitget-python-connector
-Version: 0.0.1
+Version: 0.0.4
 Summary: A tool to easily connect to bitget api.
 Author-email: "Cheng, Chuan-Yi" <parker178912.en08@nycu.edu.tw>
 Project-URL: Homepage, https://github.com/parker178912/bitget-python-connector
 Project-URL: Bug Tracker, https://github.com/parker178912/bitget-python-connector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitget-python-connector-0.0.1/pyproject.toml` & `bitget-python-connector-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitget-python-connector"
-version = "0.0.1"
+version = "0.0.4"
 authors = [
   { name="Cheng, Chuan-Yi", email="parker178912.en08@nycu.edu.tw" },
 ]
 description = "A tool to easily connect to bitget api."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests",
+]
+
+[tool.setuptools.packages]
+find = {}
 
 [project.urls]
 "Homepage" = "https://github.com/parker178912/bitget-python-connector"
 "Bug Tracker" = "https://github.com/parker178912/bitget-python-connector/issues"
```

