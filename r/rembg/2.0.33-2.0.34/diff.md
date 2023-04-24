# Comparing `tmp/rembg-2.0.33.tar.gz` & `tmp/rembg-2.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.33.tar", last modified: Sun Apr 23 04:49:09 2023, max compression
+gzip compressed data, was "rembg-2.0.34.tar", last modified: Mon Apr 24 22:21:11 2023, max compression
```

## Comparing `rembg-2.0.33.tar` & `rembg-2.0.34.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.301674 rembg-2.0.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 04:48:58.000000 rembg-2.0.33/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-23 04:48:58.000000 rembg-2.0.33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-23 04:49:09.301674 rembg-2.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-23 04:48:58.000000 rembg-2.0.33/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-23 04:48:58.000000 rembg-2.0.33/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.301674 rembg-2.0.33/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 04:49:09.301674 rembg-2.0.33/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.297674 rembg-2.0.33/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.301674 rembg-2.0.33/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/dis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-23 04:48:58.000000 rembg-2.0.33/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 04:49:09.297674 rembg-2.0.33/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 04:49:09.000000 rembg-2.0.33/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 04:48:58.000000 rembg-2.0.33/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-23 04:48:58.000000 rembg-2.0.33/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 04:49:09.301674 rembg-2.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-23 04:48:58.000000 rembg-2.0.33/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-23 04:48:58.000000 rembg-2.0.33/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:21:11.655944 rembg-2.0.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 22:21:01.000000 rembg-2.0.34/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 22:21:01.000000 rembg-2.0.34/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-24 22:21:11.655944 rembg-2.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-24 22:21:01.000000 rembg-2.0.34/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-24 22:21:01.000000 rembg-2.0.34/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:21:11.655944 rembg-2.0.34/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-24 22:21:11.655944 rembg-2.0.34/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:21:11.655944 rembg-2.0.34/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:21:11.655944 rembg-2.0.34/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/dis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-24 22:21:01.000000 rembg-2.0.34/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:21:11.655944 rembg-2.0.34/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-04-24 22:21:11.000000 rembg-2.0.34/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 22:21:11.000000 rembg-2.0.34/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:21:11.000000 rembg-2.0.34/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 22:21:11.000000 rembg-2.0.34/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-24 22:21:11.000000 rembg-2.0.34/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 22:21:11.000000 rembg-2.0.34/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 22:21:01.000000 rembg-2.0.34/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 22:21:01.000000 rembg-2.0.34/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 22:21:11.655944 rembg-2.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-24 22:21:01.000000 rembg-2.0.34/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-24 22:21:01.000000 rembg-2.0.34/versioneer.py
```

### Comparing `rembg-2.0.33/LICENSE.txt` & `rembg-2.0.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/PKG-INFO` & `rembg-2.0.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.33
+Version: 2.0.34
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.33 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.34 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `rembg-2.0.33/README.md` & `rembg-2.0.34/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/bg.py` & `rembg-2.0.34/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/commands/i_command.py` & `rembg-2.0.34/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/commands/p_command.py` & `rembg-2.0.34/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/commands/s_command.py` & `rembg-2.0.34/rembg/commands/s_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
     class CommonQueryParams:
         def __init__(
             self,
             model: Annotated[
                 str, Query(regex=r"(" + "|".join(sessions_names) + ")")
             ] = Query(
-                default="u2net",
                 description="Model to use when processing image",
             ),
             a: bool = Query(default=False, description="Enable Alpha Matting"),
             af: int = Query(
                 default=240,
                 ge=0,
                 le=255,
@@ -128,15 +127,14 @@
 
     class CommonQueryPostParams:
         def __init__(
             self,
             model: Annotated[
                 str, Form(regex=r"(" + "|".join(sessions_names) + ")")
             ] = Form(
-                default="u2net",
                 description="Model to use when processing image",
             ),
             a: bool = Form(default=False, description="Enable Alpha Matting"),
             af: int = Form(
                 default=240,
                 ge=0,
                 le=255,
```

### Comparing `rembg-2.0.33/rembg/session_factory.py` & `rembg-2.0.34/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/__init__.py` & `rembg-2.0.34/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/base.py` & `rembg-2.0.34/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/dis.py` & `rembg-2.0.34/rembg/sessions/dis.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/sam.py` & `rembg-2.0.34/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/silueta.py` & `rembg-2.0.34/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/u2net.py` & `rembg-2.0.34/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.34/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.34/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg/sessions/u2netp.py` & `rembg-2.0.34/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/rembg.egg-info/PKG-INFO` & `rembg-2.0.34/rembg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.33
+Version: 2.0.34
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.33 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.34 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `rembg-2.0.33/rembg.egg-info/SOURCES.txt` & `rembg-2.0.34/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/setup.py` & `rembg-2.0.34/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.33/versioneer.py` & `rembg-2.0.34/versioneer.py`

 * *Files identical despite different names*

