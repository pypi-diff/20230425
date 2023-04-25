# Comparing `tmp/nextcode_cli-3.0.1.tar.gz` & `tmp/nextcode_cli-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode_cli-3.0.1.tar", max compression
+gzip compressed data, was "nextcode_cli-3.0.2.tar", max compression
```

## Comparing `nextcode_cli-3.0.1.tar` & `nextcode_cli-3.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     4544 2023-04-18 16:40:05.085157 nextcode_cli-3.0.1/README.md
--rw-r--r--   0        0        0       17 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/VERSION
--rw-r--r--   0        0        0      423 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/__init__.py
--rw-r--r--   0        0        0     3195 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/__main__.py
--rw-r--r--   0        0        0       22 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/__init__.py
--rw-r--r--   0        0        0     5171 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/csa.py
--rw-r--r--   0        0        0     8709 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/keycloak.py
--rw-r--r--   0        0        0     2584 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/login.py
--rw-r--r--   0        0        0      755 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/__init__.py
--rw-r--r--   0        0        0    18856 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/instance.py
--rw-r--r--   0        0        0    21113 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/job.py
--rw-r--r--   0        0        0     6491 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/jobs.py
--rw-r--r--   0        0        0      901 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/list.py
--rw-r--r--   0        0        0     4983 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/run.py
--rw-r--r--   0        0        0     1169 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/status.py
--rw-r--r--   0        0        0     5834 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/profile.py
--rw-r--r--   0        0        0     1324 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/project/__init__.py
--rw-r--r--   0        0        0     4272 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/project/fileaccess.py
--rw-r--r--   0        0        0     2914 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/project/status.py
--rw-r--r--   0        0        0     2238 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/project/users.py
--rw-r--r--   0        0        0     1926 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/__init__.py
--rw-r--r--   0        0        0    12181 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/run.py
--rw-r--r--   0        0        0     1135 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/status.py
--rw-r--r--   0        0        0     8361 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/templates.py
--rw-r--r--   0        0        0      472 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/setproject.py
--rw-r--r--   0        0        0     1134 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/token.py
--rw-r--r--   0        0        0      258 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/version.py
--rw-r--r--   0        0        0     1142 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/__init__.py
--rw-r--r--   0        0        0    27570 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/job.py
--rw-r--r--   0        0        0     4690 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/jobs.py
--rw-r--r--   0        0        0     3364 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/pipelines.py
--rw-r--r--   0        0        0      973 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/projects.py
--rw-r--r--   0        0        0     7468 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/run.py
--rw-r--r--   0        0        0     3658 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/status.py
--rwxr-xr-x   0        0        0     5244 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/csa_import.py
--rw-r--r--   0        0        0        0 2023-04-18 16:40:05.165158 nextcode_cli-3.0.1/nextcodecli/pipelines/__init__.py
--rw-r--r--   0        0        0     2697 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/pipelines/cmdutils.py
--rw-r--r--   0        0        0     6760 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/pipelines/jobs.py
--rw-r--r--   0        0        0     3799 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/pipelines/plot.py
--rw-r--r--   0        0        0     1892 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/queryapi.py
--rw-r--r--   0        0        0     2565 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/utils.py
--rw-r--r--   0        0        0        0 2023-04-18 16:40:05.169158 nextcode_cli-3.0.1/nextcodecli/workflow/__init__.py
--rw-r--r--   0        0        0     3498 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/workflow/cmdutils.py
--rw-r--r--   0        0        0      807 2023-04-18 16:40:05.097157 nextcode_cli-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 nextcode_cli-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4544 2023-04-25 10:09:51.020330 nextcode_cli-3.0.2/README.md
+-rw-r--r--   0        0        0       17 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/VERSION
+-rw-r--r--   0        0        0      423 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/__init__.py
+-rw-r--r--   0        0        0     3195 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/__init__.py
+-rw-r--r--   0        0        0     5171 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/csa.py
+-rw-r--r--   0        0        0     8709 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/keycloak.py
+-rw-r--r--   0        0        0     2584 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/login.py
+-rw-r--r--   0        0        0      755 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/__init__.py
+-rw-r--r--   0        0        0    18856 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/instance.py
+-rw-r--r--   0        0        0    21113 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/job.py
+-rw-r--r--   0        0        0     6491 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/jobs.py
+-rw-r--r--   0        0        0      901 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/list.py
+-rw-r--r--   0        0        0     4983 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/run.py
+-rw-r--r--   0        0        0     1169 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/pipelines/status.py
+-rw-r--r--   0        0        0     5834 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/profile.py
+-rw-r--r--   0        0        0     1324 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/project/__init__.py
+-rw-r--r--   0        0        0     4272 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/project/fileaccess.py
+-rw-r--r--   0        0        0     2914 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/project/status.py
+-rw-r--r--   0        0        0     2238 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/project/users.py
+-rw-r--r--   0        0        0     1926 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/query/__init__.py
+-rw-r--r--   0        0        0    12181 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/query/run.py
+-rw-r--r--   0        0        0     1135 2023-04-25 10:09:51.024330 nextcode_cli-3.0.2/nextcodecli/commands/query/status.py
+-rw-r--r--   0        0        0     8361 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/query/templates.py
+-rw-r--r--   0        0        0      472 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/setproject.py
+-rw-r--r--   0        0        0     1134 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/token.py
+-rw-r--r--   0        0        0      258 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/version.py
+-rw-r--r--   0        0        0     1142 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/__init__.py
+-rw-r--r--   0        0        0    27570 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/job.py
+-rw-r--r--   0        0        0     4690 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/jobs.py
+-rw-r--r--   0        0        0     3364 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/pipelines.py
+-rw-r--r--   0        0        0      973 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/projects.py
+-rw-r--r--   0        0        0     7468 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/run.py
+-rw-r--r--   0        0        0     3658 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/commands/workflow/status.py
+-rwxr-xr-x   0        0        0     5244 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/csa_import.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:09:51.060330 nextcode_cli-3.0.2/nextcodecli/pipelines/__init__.py
+-rw-r--r--   0        0        0     2697 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/pipelines/cmdutils.py
+-rw-r--r--   0        0        0     6760 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/pipelines/jobs.py
+-rw-r--r--   0        0        0     3799 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/pipelines/plot.py
+-rw-r--r--   0        0        0     1892 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/queryapi.py
+-rw-r--r--   0        0        0     2565 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/utils.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:09:51.060330 nextcode_cli-3.0.2/nextcodecli/workflow/__init__.py
+-rw-r--r--   0        0        0     3498 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/nextcodecli/workflow/cmdutils.py
+-rw-r--r--   0        0        0      807 2023-04-25 10:09:51.028330 nextcode_cli-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 nextcode_cli-3.0.2/PKG-INFO
```

### Comparing `nextcode_cli-3.0.1/README.md` & `nextcode_cli-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/__main__.py` & `nextcode_cli-3.0.2/nextcodecli/__main__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/csa.py` & `nextcode_cli-3.0.2/nextcodecli/commands/csa.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/keycloak.py` & `nextcode_cli-3.0.2/nextcodecli/commands/keycloak.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/login.py` & `nextcode_cli-3.0.2/nextcodecli/commands/login.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/__init__.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/instance.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/instance.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/job.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/jobs.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/jobs.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/list.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/list.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/run.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/run.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/status.py` & `nextcode_cli-3.0.2/nextcodecli/commands/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/profile.py` & `nextcode_cli-3.0.2/nextcodecli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/project/__init__.py` & `nextcode_cli-3.0.2/nextcodecli/commands/project/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/project/fileaccess.py` & `nextcode_cli-3.0.2/nextcodecli/commands/project/fileaccess.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/project/status.py` & `nextcode_cli-3.0.2/nextcodecli/commands/project/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/project/users.py` & `nextcode_cli-3.0.2/nextcodecli/commands/project/users.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/query/__init__.py` & `nextcode_cli-3.0.2/nextcodecli/commands/query/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/query/run.py` & `nextcode_cli-3.0.2/nextcodecli/commands/query/run.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/query/status.py` & `nextcode_cli-3.0.2/nextcodecli/commands/query/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/query/templates.py` & `nextcode_cli-3.0.2/nextcodecli/commands/query/templates.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/token.py` & `nextcode_cli-3.0.2/nextcodecli/commands/token.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/__init__.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/job.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/jobs.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/jobs.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/pipelines.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/pipelines.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/projects.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/projects.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/run.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/run.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/commands/workflow/status.py` & `nextcode_cli-3.0.2/nextcodecli/commands/workflow/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/csa_import.py` & `nextcode_cli-3.0.2/nextcodecli/csa_import.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/pipelines/cmdutils.py` & `nextcode_cli-3.0.2/nextcodecli/pipelines/cmdutils.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/pipelines/jobs.py` & `nextcode_cli-3.0.2/nextcodecli/pipelines/jobs.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/pipelines/plot.py` & `nextcode_cli-3.0.2/nextcodecli/pipelines/plot.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/queryapi.py` & `nextcode_cli-3.0.2/nextcodecli/queryapi.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/utils.py` & `nextcode_cli-3.0.2/nextcodecli/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/nextcodecli/workflow/cmdutils.py` & `nextcode_cli-3.0.2/nextcodecli/workflow/cmdutils.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.1/pyproject.toml` & `nextcode_cli-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nextcode-cli"
-version = "3.0.1"
+version = "3.0.2"
 description = "WuXi Nextcode commandline utilities"
 license = "MIT"
 authors = ["WUXI NextCODE <support@wuxinextcode.com>"]
 maintainers = ["Genuity Science Software Development <sdev@genuitysci.com>"]
 readme = "README.md"
 homepage = "https://www.wuxinextcode.com"
 packages = [{include = "nextcodecli"}]
@@ -17,17 +17,17 @@
 click = "^8.1.3"
 python-dateutil = "^2.8.2"
 pyyaml = "^6.0"
 requests = "^2.28.2"
 tabulate = "^0.9.0"
 hjson = "^3.1.0"
 jsonpath-rw = "^1.4.0"
-nextcode-sdk = "^2.1.0"
+nextcode-sdk = "^2.1.1"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 vulture = "^2.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nextcode_cli-3.0.1/PKG-INFO` & `nextcode_cli-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-cli
-Version: 3.0.1
+Version: 3.0.2
 Summary: WuXi Nextcode commandline utilities
 Home-page: https://www.wuxinextcode.com
 License: MIT
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 Maintainer: Genuity Science Software Development
 Maintainer-email: sdev@genuitysci.com
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: hjson (>=3.1.0,<4.0.0)
 Requires-Dist: jsonpath-rw (>=1.4.0,<2.0.0)
-Requires-Dist: nextcode-sdk (>=2.1.0,<3.0.0)
+Requires-Dist: nextcode-sdk (>=2.1.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # NextCODE Command Line Interface
```

