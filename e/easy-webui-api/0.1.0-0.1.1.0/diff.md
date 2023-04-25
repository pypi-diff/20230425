# Comparing `tmp/easy-webui-api-0.1.0.tar.gz` & `tmp/easy-webui-api-0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-webui-api-0.1.0.tar", last modified: Tue Apr 25 05:28:26 2023, max compression
+gzip compressed data, was "easy-webui-api-0.1.1.0.tar", last modified: Tue Apr 25 05:40:46 2023, max compression
```

## Comparing `easy-webui-api-0.1.0.tar` & `easy-webui-api-0.1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      221 2023-04-25 04:58:27.213782 easy-webui-api-0.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2022-10-04 15:29:52.313000 easy-webui-api-0.1.0/.coveragerc
--rw-r--r--   0        0        0      386 2022-10-13 19:34:07.197000 easy-webui-api-0.1.0/.editorconfig
--rw-r--r--   0        0        0     6436 2023-04-25 05:14:35.808282 easy-webui-api-0.1.0/.gitignore
--rw-r--r--   0        0        0       53 2022-10-01 03:44:33.733000 easy-webui-api-0.1.0/.isort.cfg
--rw-r--r--   0        0        0      907 2022-10-01 03:44:33.734000 easy-webui-api-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-04-25 04:59:26.902754 easy-webui-api-0.1.0/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542782 easy-webui-api-0.1.0/LICENSE
--rw-r--r--   0        0        0     1265 2023-04-25 04:56:25.514999 easy-webui-api-0.1.0/Makefile
--rw-r--r--   0        0        0    10643 2023-04-25 05:18:31.185886 easy-webui-api-0.1.0/README.md
--rw-r--r--   0        0        0      423 2023-04-25 05:27:13.543994 easy-webui-api-0.1.0/easyai/__init__.py
--rw-r--r--   0        0        0     6537 2023-04-25 05:12:33.213081 easy-webui-api-0.1.0/easyai/base.py
--rw-r--r--   0        0        0     1349 2023-04-25 04:48:44.444575 easy-webui-api-0.1.0/easyai/image.py
--rw-r--r--   0        0        0    10790 2023-04-25 05:08:17.872719 easy-webui-api-0.1.0/easyai/interfaces.py
--rw-r--r--   0        0        0    11501 2023-04-25 05:12:33.219091 easy-webui-api-0.1.0/easyai/main.py
--rw-r--r--   0        0        0      183 2023-04-25 04:56:58.354407 easy-webui-api-0.1.0/easyai/result.py
--rw-r--r--   0        0        0     1664 2023-04-25 05:28:25.148265 easy-webui-api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2612 2022-11-08 14:38:16.374000 easy-webui-api-0.1.0/setup.cfg
--rw-r--r--   0        0        0 10310124 2023-04-25 05:21:32.750847 easy-webui-api-0.1.0/webuiapi_demo.ipynb
--rw-r--r--   0        0        0    12583 1970-01-01 00:00:00.000000 easy-webui-api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      224 2023-04-25 05:34:55.146675 easy-webui-api-0.1.1.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2022-10-04 15:29:52.313000 easy-webui-api-0.1.1.0/.coveragerc
+-rw-r--r--   0        0        0      386 2022-10-13 19:34:07.197000 easy-webui-api-0.1.1.0/.editorconfig
+-rw-r--r--   0        0        0     6436 2023-04-25 05:14:35.808282 easy-webui-api-0.1.1.0/.gitignore
+-rw-r--r--   0        0        0       53 2022-10-01 03:44:33.733000 easy-webui-api-0.1.1.0/.isort.cfg
+-rw-r--r--   0        0        0      907 2022-10-01 03:44:33.734000 easy-webui-api-0.1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-04-25 04:59:26.902754 easy-webui-api-0.1.1.0/.pylintrc
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542782 easy-webui-api-0.1.1.0/LICENSE
+-rw-r--r--   0        0        0     1265 2023-04-25 04:56:25.514999 easy-webui-api-0.1.1.0/Makefile
+-rw-r--r--   0        0        0    10643 2023-04-25 05:18:31.185886 easy-webui-api-0.1.1.0/README.md
+-rw-r--r--   0        0        0      425 2023-04-25 05:34:55.146138 easy-webui-api-0.1.1.0/easyai/__init__.py
+-rw-r--r--   0        0        0     6537 2023-04-25 05:12:33.213081 easy-webui-api-0.1.1.0/easyai/base.py
+-rw-r--r--   0        0        0     1349 2023-04-25 04:48:44.444575 easy-webui-api-0.1.1.0/easyai/image.py
+-rw-r--r--   0        0        0    10790 2023-04-25 05:08:17.872719 easy-webui-api-0.1.1.0/easyai/interfaces.py
+-rw-r--r--   0        0        0    11501 2023-04-25 05:12:33.219091 easy-webui-api-0.1.1.0/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-04-25 04:56:58.354407 easy-webui-api-0.1.1.0/easyai/result.py
+-rw-r--r--   0        0        0     1652 2023-04-25 05:30:52.934483 easy-webui-api-0.1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2612 2022-11-08 14:38:16.374000 easy-webui-api-0.1.1.0/setup.cfg
+-rw-r--r--   0        0        0 10310124 2023-04-25 05:21:32.750847 easy-webui-api-0.1.1.0/webuiapi_demo.ipynb
+-rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 easy-webui-api-0.1.1.0/PKG-INFO
```

### Comparing `easy-webui-api-0.1.0/.gitignore` & `easy-webui-api-0.1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/.pre-commit-config.yaml` & `easy-webui-api-0.1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/LICENSE` & `easy-webui-api-0.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/Makefile` & `easy-webui-api-0.1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/README.md` & `easy-webui-api-0.1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/easyai/base.py` & `easy-webui-api-0.1.1.0/easyai/base.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/easyai/image.py` & `easy-webui-api-0.1.1.0/easyai/image.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/easyai/interfaces.py` & `easy-webui-api-0.1.1.0/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/easyai/main.py` & `easy-webui-api-0.1.1.0/easyai/main.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/pyproject.toml` & `easy-webui-api-0.1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 requires = [
-    "flit",
     "requests",
     "Pillow",
 ]
 description-file = "README.md"
 requires-python = ">=3.7"
```

### Comparing `easy-webui-api-0.1.0/setup.cfg` & `easy-webui-api-0.1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/webuiapi_demo.ipynb` & `easy-webui-api-0.1.1.0/webuiapi_demo.ipynb`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.0/PKG-INFO` & `easy-webui-api-0.1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-webui-api
-Version: 0.1.0
+Version: 0.1.1.0
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -24,15 +24,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Dist: flit
 Requires-Dist: requests
 Requires-Dist: Pillow
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: pre_commit ; extra == "dev"
 Requires-Dist: bumpversion==0.6.0 ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
```

