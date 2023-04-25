# Comparing `tmp/connect_reports_runner-27.2.tar.gz` & `tmp/connect_reports_runner-27.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_reports_runner-27.2.tar", max compression
+gzip compressed data, was "connect_reports_runner-27.3.tar", max compression
```

## Comparing `connect_reports_runner-27.2.tar` & `connect_reports_runner-27.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/LICENSE
--rw-r--r--   0        0        0      140 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/README.md
--rw-r--r--   0        0        0        0 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/executor/__init__.py
--rw-r--r--   0        0        0     3443 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/executor/exception_handler.py
--rw-r--r--   0        0        0       43 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/executor/exceptions.py
--rw-r--r--   0        0        0     6131 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/executor/executor.py
--rw-r--r--   0        0        0     1738 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/executor/runner.py
--rw-r--r--   0        0        0     3660 2023-03-21 12:06:38.468556 connect_reports_runner-27.2/executor/utils.py
--rw-r--r--   0        0        0     2783 2023-03-21 12:07:35.453269 connect_reports_runner-27.2/pyproject.toml
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 connect_reports_runner-27.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/LICENSE
+-rw-r--r--   0        0        0      140 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/__init__.py
+-rw-r--r--   0        0        0     3443 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/exception_handler.py
+-rw-r--r--   0        0        0       43 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/exceptions.py
+-rw-r--r--   0        0        0     6131 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/executor.py
+-rw-r--r--   0        0        0     1738 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/runner.py
+-rw-r--r--   0        0        0     3730 2023-04-25 13:14:04.572828 connect_reports_runner-27.3/executor/utils.py
+-rw-r--r--   0        0        0     2783 2023-04-25 13:15:06.965207 connect_reports_runner-27.3/pyproject.toml
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 connect_reports_runner-27.3/PKG-INFO
```

### Comparing `connect_reports_runner-27.2/LICENSE` & `connect_reports_runner-27.3/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.2/executor/exception_handler.py` & `connect_reports_runner-27.3/executor/exception_handler.py`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.2/executor/executor.py` & `connect_reports_runner-27.3/executor/executor.py`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.2/executor/runner.py` & `connect_reports_runner-27.3/executor/runner.py`

 * *Files identical despite different names*

### Comparing `connect_reports_runner-27.2/executor/utils.py` & `connect_reports_runner-27.3/executor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,20 +104,21 @@
             f' {os.getenv("REPORT_ID", None)}'
         ),
     }
 
 
 def upload_file(client, report_name, report_id, owner_id):
     report_filename = os.path.basename(report_name)
+    _, report_extension = report_filename.rsplit('.', 1)
     reports_media_api = client.ns('media').ns('folders').collection('reports_report_file')
     media_file = reports_media_api[owner_id].action('files').post(
         data=open(report_name, 'rb'),
         headers={
             'Content-Type': 'application/octet-stream',
-            'Content-Disposition': f'attachment; filename="{report_filename}"',
+            'Content-Disposition': f'attachment; filename="{report_id}.{report_extension}"',
         },
     )
 
     return client.ns('reporting').reports[report_id].action('upload').post(
         payload={'file': {'id': json.loads(media_file)['id']}},
         headers=get_user_agent(),
     )
```

### Comparing `connect_reports_runner-27.2/pyproject.toml` & `connect_reports_runner-27.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-reports-runner"
-version = "27.2"
+version = "27.3"
 description = "Connect Reports Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "executor" }
 ]
 readme = "./README.md"
```

### Comparing `connect_reports_runner-27.2/PKG-INFO` & `connect_reports_runner-27.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-reports-runner
-Version: 27.2
+Version: 27.3
 Summary: Connect Reports Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Keywords: utility,connect,cloudblue,reports
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
```

