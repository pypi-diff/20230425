# Comparing `tmp/openxlab-0.0.2.tar.gz` & `tmp/openxlab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.2.tar", last modified: Sun Apr 23 02:04:37 2023, max compression
+gzip compressed data, was "openxlab-0.0.3.tar", last modified: Tue Apr 25 09:58:58 2023, max compression
```

## Comparing `openxlab-0.0.2.tar` & `openxlab-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.274855 openxlab-0.0.2/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-23 02:04:37.274516 openxlab-0.0.2/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.2/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.258949 openxlab-0.0.2/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.2/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.2/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.262584 openxlab-0.0.2/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.2/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-23 01:54:21.000000 openxlab-0.0.2/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.263016 openxlab-0.0.2/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.263514 openxlab-0.0.2/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        7 2023-04-14 08:49:35.000000 openxlab-0.0.2/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.264392 openxlab-0.0.2/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.2/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.2/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2473 2023-04-20 11:54:06.000000 openxlab-0.0.2/openxlab/model/clients/openapi_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.267373 openxlab-0.0.2/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.2/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      770 2023-04-18 03:48:11.000000 openxlab-0.0.2/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      422 2023-04-18 03:48:11.000000 openxlab-0.0.2/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      358 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      366 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.2/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.268437 openxlab-0.0.2/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.2/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      898 2023-04-23 01:59:35.000000 openxlab-0.0.2/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.2/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.272263 openxlab-0.0.2/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      111 2023-04-18 03:48:11.000000 openxlab-0.0.2/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.2/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2842 2023-04-20 11:36:51.000000 openxlab-0.0.2/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       29 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/query_meta_info.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       41 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.2/openxlab/model/handler/update_file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.272798 openxlab-0.0.2/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.2/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.273560 openxlab-0.0.2/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/utils/file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.274062 openxlab-0.0.2/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.2/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-23 02:04:37.261724 openxlab-0.0.2/openxlab.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1402 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       79 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-23 02:04:37.000000 openxlab-0.0.2/openxlab.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.2/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-23 02:04:37.275002 openxlab-0.0.2/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.2/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.614221 openxlab-0.0.3/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 09:58:58.613942 openxlab-0.0.3/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.3/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.591580 openxlab-0.0.3/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.3/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.3/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.594094 openxlab-0.0.3/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.3/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-25 09:58:41.000000 openxlab-0.0.3/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.594363 openxlab-0.0.3/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.3/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.595052 openxlab-0.0.3/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      337 2023-04-24 11:33:14.000000 openxlab-0.0.3/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.596027 openxlab-0.0.3/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.3/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.3/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     5233 2023-04-25 09:47:26.000000 openxlab-0.0.3/openxlab/model/clients/openapi_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.601619 openxlab-0.0.3/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.3/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.3/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      899 2023-04-25 09:33:47.000000 openxlab-0.0.3/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.3/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.3/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.3/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.3/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.3/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.3/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.603799 openxlab-0.0.3/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.3/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1229 2023-04-25 09:26:21.000000 openxlab-0.0.3/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.3/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.3/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.610099 openxlab-0.0.3/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.3/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.3/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.3/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2489 2023-04-25 09:56:32.000000 openxlab-0.0.3/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.3/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.3/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.3/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.3/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.3/openxlab/model/handler/update_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.3/openxlab/model/handler/update_repository.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.611318 openxlab-0.0.3/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.3/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.3/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.612684 openxlab-0.0.3/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.3/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.3/openxlab/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.613277 openxlab-0.0.3/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.3/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 09:58:58.593510 openxlab-0.0.3/openxlab.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 09:58:58.000000 openxlab-0.0.3/openxlab.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-25 09:58:58.000000 openxlab-0.0.3/openxlab.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-25 09:58:58.000000 openxlab-0.0.3/openxlab.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-25 09:58:58.000000 openxlab-0.0.3/openxlab.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      107 2023-04-25 09:58:58.000000 openxlab-0.0.3/openxlab.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-25 09:58:58.000000 openxlab-0.0.3/openxlab.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.3/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-25 09:58:58.614328 openxlab-0.0.3/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.3/setup.py
```

### Comparing `openxlab-0.0.2/PKG-INFO` & `openxlab-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.2
+Version: 0.0.3
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.2/README.md` & `openxlab-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab/cli.py` & `openxlab-0.0.3/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab/demo_cmd/__init__.py` & `openxlab-0.0.3/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab/model/commands/__init__.py` & `openxlab-0.0.3/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab/model/commands/download.py` & `openxlab-0.0.3/openxlab/model/commands/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 download model file|meta file|log file|readme file-cli
 """
 from openxlab.types.command_type import *
-from openxlab.model.handler import download
+from openxlab.model import download
 
 
 class Download(BaseCommand):
     """download"""
 
     def get_name(self) -> str:
         return "download"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument('-m', '--model-repo', required=True,
+        parser.add_argument('-r', '--model-repo', required=True,
                             help='model repository address. format:username/repository.')
         parser.add_argument('-f', '--file', required=True,
                             help='target file to be download.')
+        parser.add_argument('-p', '--path', required=False,
+                            help='setting download path.')
 
     def take_action(self, parsed_args: Namespace) -> int:
-        download(parsed_args.model_repo, parsed_args.file)
+        download(parsed_args.model_repo, parsed_args.file, parsed_args.path)
         # print("download something")
         return 0
```

### Comparing `openxlab-0.0.2/openxlab/model/common/response_dto.py` & `openxlab-0.0.3/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab/model/handler/download_file.py` & `openxlab-0.0.3/openxlab/model/handler/download_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 """
 Download function for related files in the reality model library
 """
 import logging
 import re
 from tqdm import tqdm
 import requests
+import os
 
 from openxlab.model.clients.openapi_client import OpenapiClient
 from openxlab.model.common.constants import endpoint, token, default_metafile_template_name
 
 logger = logging.getLogger("openxlab.model")
 
 
-def _download(model_repo, file) -> None:
+def download(model_repo, file, path) -> None:
     """
     download model file|meta file|log filee|readme file
     usage: cli & sdk
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
         url = client.get_download_url(repository, file)
     except ValueError as e:
         print(f"Error: {e}")
         return
-    _download_to_local(url, file)
+    _download_to_local(url, file, path)
     print("download model repo:{}, file:{}".format(model_repo, file))
 
 
-def _download_metafile_template(file=None) -> None:
+def download_metafile_template(path=None) -> None:
     """
     download metafile template file
     """
     try:
         # split params
         client = OpenapiClient(endpoint, token)
         url = client.get_metafile_template_download_url()
-        print(f"url.{url}")
     except ValueError as e:
         print(f"Error: {e}")
         return
-    file = file if file is not None else default_metafile_template_name
-    _download_to_local(url, file)
-    print("download metafile file:{}".format(file))
+    _download_to_local(url, file=default_metafile_template_name, path=path)
 
 
 def _split_repo(model_repo) -> (str, str):
     """
     Split a full repository name into two separate strings: the username and the repository name.
     """
     # username/repository format check
@@ -55,34 +53,32 @@
     if not re.match(pattern, model_repo):
         raise ValueError("The input string must be in the format 'didi12/test-d-1'")
 
     values = model_repo.split('/')
     return values[0], values[1]
 
 
-def _download_to_local(url, file) -> None:
+def _download_to_local(url, file, path=None) -> None:
     """
     download file to local with progress_bar
     """
+    filename = os.path.basename(url)
+    file_extension = os.path.splitext(filename)[1]
     response = requests.get(url, stream=True)
 
     total_size_in_bytes = int(response.headers.get('content-length', 0))
     block_size = 1024
     progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
-
-    with open(file, 'wb') as file:
+    path_file = file
+    if path is not None:
+        if not os.path.exists(path):
+            os.makedirs(path)
+        path_file = f"{path}/{file + file_extension}"
+    with open(path_file, 'wb') as f:
         for data in response.iter_content(block_size):
             progress_bar.update(len(data))
-            file.write(data)
+            f.write(data)
     progress_bar.close()
+    return
+
+
 
-# def _get_download_url(url, payload) -> dict:
-#     """
-#     获取文件下载路径
-#     """
-#     response = requests.post(url, json=payload)
-#     response.raise_for_status()  # 抛出异常如果状态码不是200
-#     response_dict = response.json()  # 转换为Python字典格式
-#     response_dto = ReturnDto.from_camel_case(response_dict)
-#     if response_dto.msg_code != '10000':
-#         raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-#     return response_dto.data['url']
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openxlab-0.0.2/openxlab/types/command_type.py` & `openxlab-0.0.3/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab/utils/file.py` & `openxlab-0.0.3/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.2/openxlab.egg-info/PKG-INFO` & `openxlab-0.0.3/openxlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.2
+Version: 0.0.3
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.2/openxlab.egg-info/SOURCES.txt` & `openxlab-0.0.3/openxlab.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 openxlab/model/commands/init.py
 openxlab/model/commands/list.py
 openxlab/model/commands/remove.py
 openxlab/model/commands/upload.py
 openxlab/model/commands/visibility.py
 openxlab/model/common/__init__.py
 openxlab/model/common/constants.py
+openxlab/model/common/meta_file_util.py
 openxlab/model/common/response_dto.py
 openxlab/model/handler/__init__.py
 openxlab/model/handler/common.py
 openxlab/model/handler/create_repository.py
 openxlab/model/handler/download_file.py
 openxlab/model/handler/model_inference.py
 openxlab/model/handler/model_list.py
-openxlab/model/handler/query_meta_info.py
+openxlab/model/handler/query_repo_model.py
 openxlab/model/handler/remove_repo_or_file.py
 openxlab/model/handler/update_file.py
+openxlab/model/handler/update_repository.py
 openxlab/types/__init__.py
 openxlab/types/command_type.py
 openxlab/utils/__init__.py
 openxlab/utils/file.py
 openxlab/xlab/__init__.py
```

### Comparing `openxlab-0.0.2/setup.py` & `openxlab-0.0.3/setup.py`

 * *Files identical despite different names*

