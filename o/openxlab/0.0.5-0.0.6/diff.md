# Comparing `tmp/openxlab-0.0.5.tar.gz` & `tmp/openxlab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.5.tar", last modified: Tue Apr 25 10:09:35 2023, max compression
+gzip compressed data, was "openxlab-0.0.6.tar", last modified: Tue Apr 25 10:30:41 2023, max compression
```

## Comparing `openxlab-0.0.5.tar` & `openxlab-0.0.6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.898536 openxlab-0.0.5/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:09:35.898220 openxlab-0.0.5/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.5/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.874037 openxlab-0.0.5/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.5/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.5/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.877127 openxlab-0.0.5/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.5/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-25 10:09:32.000000 openxlab-0.0.5/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.877415 openxlab-0.0.5/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.878116 openxlab-0.0.5/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      337 2023-04-24 11:33:14.000000 openxlab-0.0.5/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.879285 openxlab-0.0.5/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.5/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.5/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     5233 2023-04-25 09:47:26.000000 openxlab-0.0.5/openxlab/model/clients/openapi_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.885461 openxlab-0.0.5/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.5/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.5/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      899 2023-04-25 09:33:47.000000 openxlab-0.0.5/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.5/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.5/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.5/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.5/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.5/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.888091 openxlab-0.0.5/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.5/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1229 2023-04-25 09:26:21.000000 openxlab-0.0.5/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.5/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.894551 openxlab-0.0.5/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.5/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2508 2023-04-25 10:09:32.000000 openxlab-0.0.5/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.5/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.5/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.5/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.5/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.5/openxlab/model/handler/update_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.5/openxlab/model/handler/update_repository.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.895560 openxlab-0.0.5/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.5/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.897123 openxlab-0.0.5/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/utils/file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.897656 openxlab-0.0.5/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.876589 openxlab-0.0.5/openxlab.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      107 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.5/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-25 10:09:35.898643 openxlab-0.0.5/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.5/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.292377 openxlab-0.0.6/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:30:41.292100 openxlab-0.0.6/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.6/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.279630 openxlab-0.0.6/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.6/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.6/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.282048 openxlab-0.0.6/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.6/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-25 10:30:31.000000 openxlab-0.0.6/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.282350 openxlab-0.0.6/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.282729 openxlab-0.0.6/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      337 2023-04-24 11:33:14.000000 openxlab-0.0.6/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.283517 openxlab-0.0.6/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.6/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.6/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     5233 2023-04-25 09:47:26.000000 openxlab-0.0.6/openxlab/model/clients/openapi_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.286242 openxlab-0.0.6/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.6/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.6/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      861 2023-04-25 10:15:10.000000 openxlab-0.0.6/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.6/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.6/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.6/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.6/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.6/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.287330 openxlab-0.0.6/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.6/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1229 2023-04-25 09:26:21.000000 openxlab-0.0.6/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.6/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.290242 openxlab-0.0.6/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.6/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.6/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2550 2023-04-25 10:29:48.000000 openxlab-0.0.6/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.6/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.6/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.6/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.6/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.6/openxlab/model/handler/update_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.6/openxlab/model/handler/update_repository.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.290726 openxlab-0.0.6/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.6/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.291400 openxlab-0.0.6/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.291707 openxlab-0.0.6/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.6/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:30:41.281462 openxlab-0.0.6/openxlab.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      107 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-25 10:30:41.000000 openxlab-0.0.6/openxlab.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.6/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-25 10:30:41.292469 openxlab-0.0.6/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.6/setup.py
```

### Comparing `openxlab-0.0.5/PKG-INFO` & `openxlab-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.5
+Version: 0.0.6
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.5/README.md` & `openxlab-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/cli.py` & `openxlab-0.0.6/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/demo_cmd/__init__.py` & `openxlab-0.0.6/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/clients/openapi_client.py` & `openxlab-0.0.6/openxlab/model/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/commands/__init__.py` & `openxlab-0.0.6/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/commands/create.py` & `openxlab-0.0.6/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/commands/download.py` & `openxlab-0.0.6/openxlab/model/commands/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,9 +17,8 @@
         parser.add_argument('-f', '--file', required=True,
                             help='target file to be download.')
         parser.add_argument('-p', '--path', required=False,
                             help='setting download path.')
 
     def take_action(self, parsed_args: Namespace) -> int:
         download(parsed_args.model_repo, parsed_args.file, parsed_args.path)
-        # print("download something")
         return 0
```

### Comparing `openxlab-0.0.5/openxlab/model/commands/init.py` & `openxlab-0.0.6/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/commands/list.py` & `openxlab-0.0.6/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/commands/remove.py` & `openxlab-0.0.6/openxlab/model/commands/remove.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/commands/visibility.py` & `openxlab-0.0.6/openxlab/model/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/common/constants.py` & `openxlab-0.0.6/openxlab/model/common/constants.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/common/meta_file_util.py` & `openxlab-0.0.6/openxlab/model/common/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/common/response_dto.py` & `openxlab-0.0.6/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/handler/create_repository.py` & `openxlab-0.0.6/openxlab/model/handler/create_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/handler/download_file.py` & `openxlab-0.0.6/openxlab/model/handler/download_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,17 @@
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
         url = client.get_download_url(repository, file)
     except ValueError as e:
         print(f"Error: {e}")
         return
-    _download_to_local(url, file, path)
+    path_file = _download_to_local(url, file, path)
     print("download model repo:{}, file:{}".format(model_repo, file))
+    return path_file
 
 
 def download_metafile_template(path=None) -> None:
     """
     download metafile template file
     """
     try:
@@ -53,15 +54,15 @@
     if not re.match(pattern, model_repo):
         raise ValueError("The input string must be in the format 'didi12/test-d-1'")
 
     values = model_repo.split('/')
     return values[0], values[1]
 
 
-def _download_to_local(url, file, path=None) -> None:
+def _download_to_local(url, file, path=None) -> str:
     """
     download file to local with progress_bar
     """
     filename = os.path.basename(url)
     file_extension = os.path.splitext(filename)[1]
     response = requests.get(url, stream=True)
 
@@ -74,8 +75,8 @@
             os.makedirs(path)
         path_file = f"{path}/{file + file_extension}"
     with open(path_file, 'wb') as f:
         for data in response.iter_content(block_size):
             progress_bar.update(len(data))
             f.write(data)
     progress_bar.close()
-    return
+    return path_file
```

### Comparing `openxlab-0.0.5/openxlab/model/handler/query_repo_model.py` & `openxlab-0.0.6/openxlab/model/handler/query_repo_model.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-0.0.6/openxlab/model/handler/remove_repo_or_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/model/handler/update_repository.py` & `openxlab-0.0.6/openxlab/model/handler/update_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/types/command_type.py` & `openxlab-0.0.6/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab/utils/file.py` & `openxlab-0.0.6/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/openxlab.egg-info/PKG-INFO` & `openxlab-0.0.6/openxlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.5
+Version: 0.0.6
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.5/openxlab.egg-info/SOURCES.txt` & `openxlab-0.0.6/openxlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.5/setup.py` & `openxlab-0.0.6/setup.py`

 * *Files identical despite different names*

