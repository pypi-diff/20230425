# Comparing `tmp/easy-webui-api-0.1.1.0.tar.gz` & `tmp/easy-webui-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-webui-api-0.1.1.0.tar", last modified: Tue Apr 25 05:40:46 2023, max compression
+gzip compressed data, was "easy-webui-api-0.1.2.tar", last modified: Tue Apr 25 06:32:48 2023, max compression
```

## Comparing `easy-webui-api-0.1.1.0.tar` & `easy-webui-api-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      224 2023-04-25 05:34:55.146675 easy-webui-api-0.1.1.0/.bumpversion.cfg
--rw-r--r--   0        0        0      270 2022-10-04 15:29:52.313000 easy-webui-api-0.1.1.0/.coveragerc
--rw-r--r--   0        0        0      386 2022-10-13 19:34:07.197000 easy-webui-api-0.1.1.0/.editorconfig
--rw-r--r--   0        0        0     6436 2023-04-25 05:14:35.808282 easy-webui-api-0.1.1.0/.gitignore
--rw-r--r--   0        0        0       53 2022-10-01 03:44:33.733000 easy-webui-api-0.1.1.0/.isort.cfg
--rw-r--r--   0        0        0      907 2022-10-01 03:44:33.734000 easy-webui-api-0.1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      228 2023-04-25 04:59:26.902754 easy-webui-api-0.1.1.0/.pylintrc
--rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542782 easy-webui-api-0.1.1.0/LICENSE
--rw-r--r--   0        0        0     1265 2023-04-25 04:56:25.514999 easy-webui-api-0.1.1.0/Makefile
--rw-r--r--   0        0        0    10643 2023-04-25 05:18:31.185886 easy-webui-api-0.1.1.0/README.md
--rw-r--r--   0        0        0      425 2023-04-25 05:34:55.146138 easy-webui-api-0.1.1.0/easyai/__init__.py
--rw-r--r--   0        0        0     6537 2023-04-25 05:12:33.213081 easy-webui-api-0.1.1.0/easyai/base.py
--rw-r--r--   0        0        0     1349 2023-04-25 04:48:44.444575 easy-webui-api-0.1.1.0/easyai/image.py
--rw-r--r--   0        0        0    10790 2023-04-25 05:08:17.872719 easy-webui-api-0.1.1.0/easyai/interfaces.py
--rw-r--r--   0        0        0    11501 2023-04-25 05:12:33.219091 easy-webui-api-0.1.1.0/easyai/main.py
--rw-r--r--   0        0        0      183 2023-04-25 04:56:58.354407 easy-webui-api-0.1.1.0/easyai/result.py
--rw-r--r--   0        0        0     1652 2023-04-25 05:30:52.934483 easy-webui-api-0.1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2612 2022-11-08 14:38:16.374000 easy-webui-api-0.1.1.0/setup.cfg
--rw-r--r--   0        0        0 10310124 2023-04-25 05:21:32.750847 easy-webui-api-0.1.1.0/webuiapi_demo.ipynb
--rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 easy-webui-api-0.1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-04-25 06:32:35.338110 easy-webui-api-0.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0      270 2023-04-25 06:32:35.338580 easy-webui-api-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      386 2023-04-25 06:32:35.338983 easy-webui-api-0.1.2/.editorconfig
+-rw-r--r--   0        0        0     6362 2023-04-25 06:32:37.032590 easy-webui-api-0.1.2/.gitignore
+-rw-r--r--   0        0        0       53 2023-04-25 06:32:35.339976 easy-webui-api-0.1.2/.isort.cfg
+-rw-r--r--   0        0        0      907 2023-04-25 06:32:35.340381 easy-webui-api-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      228 2023-04-25 06:32:35.340772 easy-webui-api-0.1.2/.pylintrc
+-rw-r--r--   0        0        0  1660611 2023-04-25 06:32:35.367054 easy-webui-api-0.1.2/API demo.ipynb
+-rw-r--r--   0        0        0     1079 2023-04-25 04:05:59.542000 easy-webui-api-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1265 2023-04-25 06:32:35.367759 easy-webui-api-0.1.2/Makefile
+-rw-r--r--   0        0        0    10643 2023-04-25 06:32:35.369037 easy-webui-api-0.1.2/README.md
+-rw-r--r--   0        0        0      509 2023-04-25 06:32:35.369628 easy-webui-api-0.1.2/easyai/__init__.py
+-rw-r--r--   0        0        0     6537 2023-04-25 06:32:35.370102 easy-webui-api-0.1.2/easyai/base.py
+-rw-r--r--   0        0        0     1349 2023-04-25 06:32:35.370543 easy-webui-api-0.1.2/easyai/image.py
+-rw-r--r--   0        0        0    10790 2023-04-25 06:32:35.371024 easy-webui-api-0.1.2/easyai/interfaces.py
+-rw-r--r--   0        0        0    11501 2023-04-25 06:32:35.371492 easy-webui-api-0.1.2/easyai/main.py
+-rw-r--r--   0        0        0      183 2023-04-25 06:32:35.371921 easy-webui-api-0.1.2/easyai/result.py
+-rwxr-xr-x   0        0        0       99 2023-04-25 06:02:41.087346 easy-webui-api-0.1.2/publish.sh
+-rw-r--r--   0        0        0     1652 2023-04-25 06:32:35.372343 easy-webui-api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2612 2023-04-25 06:32:35.372771 easy-webui-api-0.1.2/setup.cfg
+-rw-r--r--   0        0        0    12563 1970-01-01 00:00:00.000000 easy-webui-api-0.1.2/PKG-INFO
```

### Comparing `easy-webui-api-0.1.1.0/.gitignore` & `easy-webui-api-0.1.2/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 # Local History for Visual Studio Code
 .history/
 
 
 # Provided default Pycharm Run/Debug Configurations should be tracked by git
 # In case of local modifications made by Pycharm, use update-index command
 # for each changed file, like this:
-# git update-index --assume-unchanged .idea/easy.iml
+# git update-index --assume-unchanged .idea/project.iml
 ### JetBrains template
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio and Webstorm
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 # User-specific stuff:
 .idea/**/workspace.xml
 .idea/**/tasks.xml
@@ -369,26 +369,23 @@
 # Temporary
 .netrwhist
 
 # Auto-generated tag files
 tags
 
 ### Project template
-easy/media/
-
 .pytest_cache/
 .ipython/
 
 
 .envs/*
 !.envs/.local/
+/.idea
 /.idea/inspectionProfiles/profiles_settings.xml
 /.idea/inspectionProfiles/Project_Default.xml
 /.idea/.gitignore
-/.idea/django-easy-api.iml
-/.idea/misc.xml
+/.idea/*.iml
+/.idea/*.xml
 /.idea/modules.xml
 /.idea/vcs.xml
-/.idea/django-api-framework.iml
 /.idea/shelf/
 /.idea/git_toolbox_prj.xml
-/.idea/sdwebuiapi.iml
```

### Comparing `easy-webui-api-0.1.1.0/.pre-commit-config.yaml` & `easy-webui-api-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/LICENSE` & `easy-webui-api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/Makefile` & `easy-webui-api-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/README.md` & `easy-webui-api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/easyai/base.py` & `easy-webui-api-0.1.2/easyai/base.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/easyai/image.py` & `easy-webui-api-0.1.2/easyai/image.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/easyai/interfaces.py` & `easy-webui-api-0.1.2/easyai/interfaces.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/easyai/main.py` & `easy-webui-api-0.1.2/easyai/main.py`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/pyproject.toml` & `easy-webui-api-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/setup.cfg` & `easy-webui-api-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `easy-webui-api-0.1.1.0/PKG-INFO` & `easy-webui-api-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-webui-api
-Version: 0.1.1.0
+Version: 0.1.2
 Summary: Easy SDWebUI API - Easy API for SDWebUI, forked from mix1009/sdwebuiapi
 Home-page: https://github.com/freemindcore/sdwebuiapi
 Author: Freemind Core
 Author-email: freemindcore@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

