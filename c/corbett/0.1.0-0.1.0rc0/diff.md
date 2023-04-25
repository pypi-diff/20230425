# Comparing `tmp/corbett-0.1.0.tar.gz` & `tmp/corbett-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corbett-0.1.0.tar", last modified: Tue Apr 25 11:42:14 2023, max compression
+gzip compressed data, was "corbett-0.1.0rc0.tar", last modified: Tue Apr 25 11:29:26 2023, max compression
```

## Comparing `corbett-0.1.0.tar` & `corbett-0.1.0rc0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.983751 corbett-0.1.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      316 2023-04-25 11:42:14.982761 corbett-0.1.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-25 06:22:47.000000 corbett-0.1.0/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      876 2023-04-25 11:42:02.000000 corbett-0.1.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-25 11:42:14.984275 corbett-0.1.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-08 19:03:11.000000 corbett-0.1.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.802384 corbett-0.1.0/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.917838 corbett-0.1.0/src/corbett/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       32 2023-04-25 11:18:48.000000 corbett-0.1.0/src/corbett/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-04-08 19:07:44.000000 corbett-0.1.0/src/corbett/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1975 2023-04-25 07:04:50.000000 corbett-0.1.0/src/corbett/app.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.806822 corbett-0.1.0/src/corbett/apps/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.959978 corbett-0.1.0/src/corbett/apps/debugger/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-04-25 06:49:39.000000 corbett-0.1.0/src/corbett/apps/debugger/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2500 2023-04-25 06:48:23.000000 corbett-0.1.0/src/corbett/apps/debugger/app.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-04-25 06:47:15.000000 corbett-0.1.0/src/corbett/apps/debugger/credentials.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      212 2023-04-25 06:47:15.000000 corbett-0.1.0/src/corbett/apps/debugger/handler.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.974491 corbett-0.1.0/src/corbett/apps/gsheets/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       27 2023-04-25 06:49:43.000000 corbett-0.1.0/src/corbett/apps/gsheets/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3583 2023-04-25 06:48:33.000000 corbett-0.1.0/src/corbett/apps/gsheets/app.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      532 2023-04-25 06:48:40.000000 corbett-0.1.0/src/corbett/apps/gsheets/credentials.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      264 2023-04-25 06:47:34.000000 corbett-0.1.0/src/corbett/apps/gsheets/handler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4557 2023-04-25 06:56:56.000000 corbett-0.1.0/src/corbett/cli.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1947 2023-04-25 06:32:41.000000 corbett-0.1.0/src/corbett/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1365 2023-04-25 06:55:15.000000 corbett-0.1.0/src/corbett/config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4095 2023-04-25 06:32:41.000000 corbett-0.1.0/src/corbett/installer.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1268 2023-04-25 06:32:41.000000 corbett-0.1.0/src/corbett/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-04-18 16:48:31.000000 corbett-0.1.0/src/corbett/services.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      431 2023-04-12 15:25:34.000000 corbett-0.1.0/src/corbett/snowflake.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.943225 corbett-0.1.0/src/corbett.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      316 2023-04-25 11:42:14.000000 corbett-0.1.0/src/corbett.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      783 2023-04-25 11:42:14.000000 corbett-0.1.0/src/corbett.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-25 11:42:14.000000 corbett-0.1.0/src/corbett.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       44 2023-04-25 11:42:14.000000 corbett-0.1.0/src/corbett.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      200 2023-04-25 11:42:14.000000 corbett-0.1.0/src/corbett.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-25 11:42:14.000000 corbett-0.1.0/src/corbett.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:42:14.979515 corbett-0.1.0/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      172 2023-04-25 06:37:05.000000 corbett-0.1.0/tests/test_cli.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.738337 corbett-0.1.0rc0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      319 2023-04-25 11:29:26.737094 corbett-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-25 06:22:47.000000 corbett-0.1.0rc0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      879 2023-04-25 11:19:01.000000 corbett-0.1.0rc0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-25 11:29:26.739015 corbett-0.1.0rc0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-08 19:03:11.000000 corbett-0.1.0rc0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.600778 corbett-0.1.0rc0/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.651431 corbett-0.1.0rc0/src/corbett/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       32 2023-04-25 11:18:48.000000 corbett-0.1.0rc0/src/corbett/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       21 2023-04-08 19:07:44.000000 corbett-0.1.0rc0/src/corbett/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1975 2023-04-25 07:04:50.000000 corbett-0.1.0rc0/src/corbett/app.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.605159 corbett-0.1.0rc0/src/corbett/apps/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.705628 corbett-0.1.0rc0/src/corbett/apps/debugger/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-04-25 06:49:39.000000 corbett-0.1.0rc0/src/corbett/apps/debugger/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2500 2023-04-25 06:48:23.000000 corbett-0.1.0rc0/src/corbett/apps/debugger/app.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-04-25 06:47:15.000000 corbett-0.1.0rc0/src/corbett/apps/debugger/credentials.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      212 2023-04-25 06:47:15.000000 corbett-0.1.0rc0/src/corbett/apps/debugger/handler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.729489 corbett-0.1.0rc0/src/corbett/apps/gsheets/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       27 2023-04-25 06:49:43.000000 corbett-0.1.0rc0/src/corbett/apps/gsheets/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3583 2023-04-25 06:48:33.000000 corbett-0.1.0rc0/src/corbett/apps/gsheets/app.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      532 2023-04-25 06:48:40.000000 corbett-0.1.0rc0/src/corbett/apps/gsheets/credentials.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      264 2023-04-25 06:47:34.000000 corbett-0.1.0rc0/src/corbett/apps/gsheets/handler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4557 2023-04-25 06:56:56.000000 corbett-0.1.0rc0/src/corbett/cli.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1947 2023-04-25 06:32:41.000000 corbett-0.1.0rc0/src/corbett/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1365 2023-04-25 06:55:15.000000 corbett-0.1.0rc0/src/corbett/config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4095 2023-04-25 06:32:41.000000 corbett-0.1.0rc0/src/corbett/installer.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1268 2023-04-25 06:32:41.000000 corbett-0.1.0rc0/src/corbett/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-04-18 16:48:31.000000 corbett-0.1.0rc0/src/corbett/services.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      431 2023-04-12 15:25:34.000000 corbett-0.1.0rc0/src/corbett/snowflake.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.687697 corbett-0.1.0rc0/src/corbett.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      319 2023-04-25 11:29:26.000000 corbett-0.1.0rc0/src/corbett.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      783 2023-04-25 11:29:26.000000 corbett-0.1.0rc0/src/corbett.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-25 11:29:26.000000 corbett-0.1.0rc0/src/corbett.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       44 2023-04-25 11:29:26.000000 corbett-0.1.0rc0/src/corbett.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      200 2023-04-25 11:29:26.000000 corbett-0.1.0rc0/src/corbett.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-25 11:29:26.000000 corbett-0.1.0rc0/src/corbett.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-25 11:29:26.734071 corbett-0.1.0rc0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      172 2023-04-25 06:37:05.000000 corbett-0.1.0rc0/tests/test_cli.py
```

### Comparing `corbett-0.1.0/pyproject.toml` & `corbett-0.1.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "click==8.1.3",
     "snowflake-connector-python==3.0",
     "python-dotenv==1.0.0",
     "pydantic==1.10.7",
     "pynamodb==5.4.1",
     "argon2-cffi==21.2.0"
 ]
-version = "0.1.0"
+version = "0.1.0rc0"
 
 [project.optional-dependencies]
 pdf = ["ReportLab>=1.2", "RXP"]
 rest = ["docutils>=0.3", "pack ==1.1, ==1.3"]
 
 [project.scripts]
 corbett = "corbett.cli:cli"
```

### Comparing `corbett-0.1.0/src/corbett/app.py` & `corbett-0.1.0rc0/src/corbett/app.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/apps/debugger/app.py` & `corbett-0.1.0rc0/src/corbett/apps/debugger/app.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/apps/gsheets/app.py` & `corbett-0.1.0rc0/src/corbett/apps/gsheets/app.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/apps/gsheets/credentials.py` & `corbett-0.1.0rc0/src/corbett/apps/gsheets/credentials.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/cli.py` & `corbett-0.1.0rc0/src/corbett/cli.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/client.py` & `corbett-0.1.0rc0/src/corbett/client.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/config.py` & `corbett-0.1.0rc0/src/corbett/config.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/installer.py` & `corbett-0.1.0rc0/src/corbett/installer.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/models.py` & `corbett-0.1.0rc0/src/corbett/models.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett/services.py` & `corbett-0.1.0rc0/src/corbett/services.py`

 * *Files identical despite different names*

### Comparing `corbett-0.1.0/src/corbett.egg-info/SOURCES.txt` & `corbett-0.1.0rc0/src/corbett.egg-info/SOURCES.txt`

 * *Files identical despite different names*

