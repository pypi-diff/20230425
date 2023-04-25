# Comparing `tmp/openxlab-0.0.4.tar.gz` & `tmp/openxlab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.4.tar", last modified: Tue Apr 25 10:04:41 2023, max compression
+gzip compressed data, was "openxlab-0.0.5.tar", last modified: Tue Apr 25 10:09:35 2023, max compression
```

## Comparing `openxlab-0.0.4.tar` & `openxlab-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.588774 openxlab-0.0.4/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:04:41.588483 openxlab-0.0.4/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.4/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.574592 openxlab-0.0.4/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.4/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.4/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.577351 openxlab-0.0.4/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.4/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-25 10:04:20.000000 openxlab-0.0.4/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.577829 openxlab-0.0.4/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.4/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.578318 openxlab-0.0.4/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      337 2023-04-24 11:33:14.000000 openxlab-0.0.4/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.579099 openxlab-0.0.4/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.4/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.4/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     5233 2023-04-25 09:47:26.000000 openxlab-0.0.4/openxlab/model/clients/openapi_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.582112 openxlab-0.0.4/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.4/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.4/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      899 2023-04-25 09:33:47.000000 openxlab-0.0.4/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.4/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.4/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.4/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.4/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.4/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.4/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.583363 openxlab-0.0.4/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.4/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1229 2023-04-25 09:26:21.000000 openxlab-0.0.4/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.4/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.4/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.586497 openxlab-0.0.4/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.4/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.4/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.4/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2506 2023-04-25 10:02:29.000000 openxlab-0.0.4/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.4/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.4/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.4/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.4/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.4/openxlab/model/handler/update_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.4/openxlab/model/handler/update_repository.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.587014 openxlab-0.0.4/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.4/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.4/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.587611 openxlab-0.0.4/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.4/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.4/openxlab/utils/file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.588027 openxlab-0.0.4/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.4/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:04:41.576513 openxlab-0.0.4/openxlab.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:04:41.000000 openxlab-0.0.4/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-25 10:04:41.000000 openxlab-0.0.4/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-25 10:04:41.000000 openxlab-0.0.4/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-25 10:04:41.000000 openxlab-0.0.4/openxlab.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      107 2023-04-25 10:04:41.000000 openxlab-0.0.4/openxlab.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-25 10:04:41.000000 openxlab-0.0.4/openxlab.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.4/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-25 10:04:41.588879 openxlab-0.0.4/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.4/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.898536 openxlab-0.0.5/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:09:35.898220 openxlab-0.0.5/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.5/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.874037 openxlab-0.0.5/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.5/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.5/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.877127 openxlab-0.0.5/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.5/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-25 10:09:32.000000 openxlab-0.0.5/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.877415 openxlab-0.0.5/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.878116 openxlab-0.0.5/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      337 2023-04-24 11:33:14.000000 openxlab-0.0.5/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.879285 openxlab-0.0.5/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.5/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.5/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     5233 2023-04-25 09:47:26.000000 openxlab-0.0.5/openxlab/model/clients/openapi_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.885461 openxlab-0.0.5/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.5/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.5/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      899 2023-04-25 09:33:47.000000 openxlab-0.0.5/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.5/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.5/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.5/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 openxlab-0.0.5/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.5/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.888091 openxlab-0.0.5/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.5/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1229 2023-04-25 09:26:21.000000 openxlab-0.0.5/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.5/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.894551 openxlab-0.0.5/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.5/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.5/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2508 2023-04-25 10:09:32.000000 openxlab-0.0.5/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.5/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.5/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.5/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.5/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 openxlab-0.0.5/openxlab/model/handler/update_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.5/openxlab/model/handler/update_repository.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.895560 openxlab-0.0.5/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.5/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.897123 openxlab-0.0.5/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.897656 openxlab-0.0.5/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.5/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-25 10:09:35.876589 openxlab-0.0.5/openxlab.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      107 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-25 10:09:35.000000 openxlab-0.0.5/openxlab.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.5/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-25 10:09:35.898643 openxlab-0.0.5/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.5/setup.py
```

### Comparing `openxlab-0.0.4/PKG-INFO` & `openxlab-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.4
+Version: 0.0.5
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.4/README.md` & `openxlab-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/cli.py` & `openxlab-0.0.5/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/demo_cmd/__init__.py` & `openxlab-0.0.5/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/clients/openapi_client.py` & `openxlab-0.0.5/openxlab/model/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/__init__.py` & `openxlab-0.0.5/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/create.py` & `openxlab-0.0.5/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/download.py` & `openxlab-0.0.5/openxlab/model/commands/download.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/init.py` & `openxlab-0.0.5/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/list.py` & `openxlab-0.0.5/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/remove.py` & `openxlab-0.0.5/openxlab/model/commands/remove.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/commands/visibility.py` & `openxlab-0.0.5/openxlab/model/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/common/constants.py` & `openxlab-0.0.5/openxlab/model/common/constants.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/common/meta_file_util.py` & `openxlab-0.0.5/openxlab/model/common/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/common/response_dto.py` & `openxlab-0.0.5/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/handler/create_repository.py` & `openxlab-0.0.5/openxlab/model/handler/create_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/handler/download_file.py` & `openxlab-0.0.5/openxlab/model/handler/download_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from openxlab.model.clients.openapi_client import OpenapiClient
 from openxlab.model.common.constants import endpoint, token, default_metafile_template_name
 
 logger = logging.getLogger("openxlab.model")
 
 
-def download(model_repo, file, path) -> None:
+def download(model_repo, file, path=None) -> None:
     """
     download model file|meta file|log filee|readme file
     usage: cli & sdk
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
@@ -75,10 +75,7 @@
         path_file = f"{path}/{file + file_extension}"
     with open(path_file, 'wb') as f:
         for data in response.iter_content(block_size):
             progress_bar.update(len(data))
             f.write(data)
     progress_bar.close()
     return
-
-
-
```

### Comparing `openxlab-0.0.4/openxlab/model/handler/query_repo_model.py` & `openxlab-0.0.5/openxlab/model/handler/query_repo_model.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-0.0.5/openxlab/model/handler/remove_repo_or_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/model/handler/update_repository.py` & `openxlab-0.0.5/openxlab/model/handler/update_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/types/command_type.py` & `openxlab-0.0.5/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab/utils/file.py` & `openxlab-0.0.5/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/openxlab.egg-info/PKG-INFO` & `openxlab-0.0.5/openxlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab
-Version: 0.0.4
+Version: 0.0.5
 Summary: openxlab
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-0.0.4/openxlab.egg-info/SOURCES.txt` & `openxlab-0.0.5/openxlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.4/setup.py` & `openxlab-0.0.5/setup.py`

 * *Files identical despite different names*

