# Comparing `tmp/ggshield-1.8.2.tar.gz` & `tmp/ggshield-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggshield-1.8.2.tar", last modified: Thu Sep 23 11:56:28 2021, max compression
+gzip compressed data, was "ggshield-1.9.0.tar", last modified: Mon Oct 11 15:51:14 2021, max compression
```

## Comparing `ggshield-1.8.2.tar` & `ggshield-1.9.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.948103 ggshield-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-09-23 11:56:25.000000 ggshield-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    30554 2021-09-23 11:56:28.948103 ggshield-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    29541 2021-09-23 11:56:25.000000 ggshield-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.936102 ggshield-1.8.2/ggshield/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10178 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    11134 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8692 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/dev_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5512 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3520 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/git_shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/hook_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/ignore.py
--rw-r--r--   0 runner    (1001) docker     (121)     3680 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.940103 ggshield-1.8.2/ggshield/output/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.940103 ggshield-1.8.2/ggshield/output/json/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/json/json_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/json/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/output_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.944103 ggshield-1.8.2/ggshield/output/text/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13459 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/text/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     4243 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/output/text/text_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/quota.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.944103 ggshield-1.8.2/ggshield/scan/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4969 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/scan/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     8907 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/scan/scannable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/scan/scannable_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6862 2021-09-23 11:56:25.000000 ggshield-1.8.2/ggshield/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.940103 ggshield-1.8.2/ggshield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    30554 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 11:56:28.000000 ggshield-1.8.2/ggshield.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-09-23 11:56:25.000000 ggshield-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-09-23 11:56:28.948103 ggshield-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2021-09-23 11:56:25.000000 ggshield-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.932102 ggshield-1.8.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.944103 ggshield-1.8.2/tests/output/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.948103 ggshield-1.8.2/tests/output/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4459 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/snapshots/snap_test_json_output.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/snapshots/snap_test_message.py
--rw-r--r--   0 runner    (1001) docker     (121)    26069 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/snapshots/snap_test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/test_json_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/test_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/output/test_text_output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.948103 ggshield-1.8.2/tests/scan/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.948103 ggshield-1.8.2/tests/scan/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/scan/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/scan/snapshots/snap_test_scannable_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/scan/test_scan_docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5068 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/scan/test_scannable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/scan/test_scannable_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:28.948103 ggshield-1.8.2/tests/snapshots/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-09-23 11:56:25.000000 ggshield-1.8.2/tests/snapshots/snap_test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-10-11 15:51:11.000000 ggshield-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    30889 2021-10-11 15:51:14.512054 ggshield-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    29876 2021-10-11 15:51:11.000000 ggshield-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/ggshield/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10222 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5031 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10729 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8378 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/dev_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5292 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3520 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/git_shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4749 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/hook_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3680 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/install.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/ggshield/output/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/ggshield/output/json/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/json/json_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/json/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/output_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/ggshield/output/text/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13459 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/text/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4243 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/output/text/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4940 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/pre_receive_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/quota.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/ggshield/scan/
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4969 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/scan/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8907 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/scan/scannable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/scan/scannable_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7415 2021-10-11 15:51:11.000000 ggshield-1.9.0/ggshield/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/ggshield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    30889 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-11 15:51:14.000000 ggshield-1.9.0/ggshield.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2021-10-11 15:51:11.000000 ggshield-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-10-11 15:51:14.512054 ggshield-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2021-10-11 15:51:11.000000 ggshield-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.508054 ggshield-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/tests/output/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4459 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/snapshots/snap_test_json_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/snapshots/snap_test_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26069 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/snapshots/snap_test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/test_json_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/output/test_text_output.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/tests/scan/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/tests/scan/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/scan/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/scan/snapshots/snap_test_scannable_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3587 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/scan/test_scan_docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5068 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/scan/test_scannable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/scan/test_scannable_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:14.512054 ggshield-1.9.0/tests/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-10-11 15:51:11.000000 ggshield-1.9.0/tests/snapshots/snap_test_cli.py
```

### Comparing `ggshield-1.8.2/LICENSE` & `ggshield-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/PKG-INFO` & `ggshield-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggshield
-Version: 1.8.2
+Version: 1.9.0
 Summary: Detect secrets from all sources using GitGuardian's brains
 Home-page: https://github.com/GitGuardian/ggshield
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: cli devsecops secrets-detection security-tools gitguardian
@@ -88,26 +88,25 @@
 
 1. [Pre-commit](#pre-commit)
 
    - The pre-commit framework
    - The global and local pre-commit hook
 
 1. [Pre-push](#pre-push)
-
-1) [Pre-receive hook](#git-pre-receive-hooks)
-1) [GitLab](#gitlab)
-1) [GitHub Actions](#github)
-1) [Circle CI](#circle-ci)
-1) [Travis CI](#travis-ci)
-1) [Jenkins](#jenkins)
-1) [Drone](#Drone)
-1) [Azure Pipelines](#Azure)
-1) [Output](#output)
-1) [Contributing](#contributing)
-1) [License](#license)
+1. [Pre-receive](#pre-receive)
+1. [GitLab](#gitlab)
+1. [GitHub Actions](#github)
+1. [Circle CI](#circle-ci)
+1. [Travis CI](#travis-ci)
+1. [Jenkins](#jenkins)
+1. [Drone](#Drone)
+1. [Azure Pipelines](#Azure)
+1. [Output](#output)
+1. [Contributing](#contributing)
+1. [License](#license)
 
 # Installation
 
 Install and update using `pip`:
 
 ```shell
 $ pip install ggshield
@@ -631,46 +630,55 @@
 
 # Pre-receive
 
 A pre-receive hook allows you to reject commits from being pushed to a git repository if they do not validate every check.
 
 You can find **ggshield**'s pre-receive hook samples in the [doc/pre-receive.sample](doc/pre-receive.sample) and [doc/pre-receive-python.sample](doc/pre-receive-python.sample).
 
-### Python git pre-receive hook
+**ggshield**'s pre-receive hook can be skipped if the developer passes the option `breakglass` to the git push.
+
+For this setting to work the remote must have push options enabled. (`git config receive.advertisePushOptions true`)
 
-> ⚠ this pre-receive hook requires the host machine to have python>=3.6 and pip installed
+Examples:
+
+```sh
+$ git push -o breakglass
+$ git push --push-option=breakglass
+```
+
+## Install ggshield git pre-receive hook locally
 
 [**pre-receive-python.sample**](doc/pre-receive-python.sample)
 
-- Install ggshield from pip: `pip install ggshield`
-- Move `pre-receive-python.sample` to `.git/hooks/pre-receive`
-- Do not forget to `chmod +x .git/hooks/pre-receive`
-- either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
+1. This pre-receive hook requires the host machine to have python>=3.8 and pip installed
+1. Install ggshield from pip: `pip install ggshield`
+1. Move `pre-receive-python.sample` to `.git/hooks/pre-receive`
+1. Do not forget to `chmod +x .git/hooks/pre-receive`
+1. either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
 
 **How do I add ignored matches and use a custom config in this pre-receive hook?**
 
 - Create a `gitguardian.yaml` somewhere in the system. An example config file is available [here](.gitguardian.example.yml)
 - Replace in the pre-receive hook
   ```shell
   ggshield scan commit-range "${span}" && continue
   ```
   with:
   ```shell
   ggshield -c <INSERT path to gitguardian.yaml> scan commit-range "${span}" && continue
   ```
 
-### Docker git pre-receive hook
-
-> ⚠ this pre-receive hook requires the host machine to have docker installed.
+## Install ggshield git pre-receive hook with docker
 
 [**pre-receive.sample**](doc/pre-receive.sample)
 
-- Move `pre-receive.sample` to `.git/hooks/pre-receive`
-- Do not forget to `chmod +x .git/hooks/pre-receive`
-- either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
+1. This pre-receive hook requires the host machine to have docker installed.
+1. Move `pre-receive.sample` to `.git/hooks/pre-receive`
+1. Do not forget to `chmod +x .git/hooks/pre-receive`
+1. either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
 
 **How do I add ignored matches and use a custom config in this pre-receive hook?**
 
 - Create a `gitguardian.yaml` somewhere in the system. An example config file is available [here](.gitguardian.example.yml)
 - Replace in the pre-receive hook
   ```shell
   docker run --rm -v $(pwd):/data -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest ggshield scan commit-range "${span}" && continue
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ggshield Version: 1.8.2 Summary: Detect secrets
+Metadata-Version: 2.1 Name: ggshield Version: 1.9.0 Summary: Detect secrets
 from all sources using GitGuardian's brains Home-page: https://github.com/
 GitGuardian/ggshield Author: GitGuardian Author-email: support@gitguardian.com
 Maintainer: GitGuardian License: MIT Keywords: cli devsecops secrets-detection
 security-tools gitguardian Platform: UNKNOWN Classifier: Development Status ::
 5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: End Users/Desktop Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
@@ -50,23 +50,23 @@
 (#travis-ci) ## Table of Contents 1. [Introduction](#introduction) 1.
 [Installation](#installation) 1. [Updating](#updating) 1. [Configuration]
 (#configuration) 1. [Environment Variables](#environment-variables) 2. [On-
 premises](#on-premises-configuration) 3. [Ignoring a secret](#ignoring-a-
 secret) 1. [Commands](#commands) - [Scan](#scan-command) - [Install](#install-
 command) - [Ignore](#ignore-command) - [Quota](#quota-command) - [API Status]
 (#api-status-command) 1. [Pre-commit](#pre-commit) - The pre-commit framework -
-The global and local pre-commit hook 1. [Pre-push](#pre-push) 1) [Pre-receive
-hook](#git-pre-receive-hooks) 1) [GitLab](#gitlab) 1) [GitHub Actions](#github)
-1) [Circle CI](#circle-ci) 1) [Travis CI](#travis-ci) 1) [Jenkins](#jenkins) 1)
-[Drone](#Drone) 1) [Azure Pipelines](#Azure) 1) [Output](#output) 1)
-[Contributing](#contributing) 1) [License](#license) # Installation Install and
-update using `pip`: ```shell $ pip install ggshield ``` ggshield supports
-**Python 3.6 and newer**. The package should run on MacOS, Linux and Windows.
-You'll need an **API Key** from the [GitGuardian dashboard](https://
-dashboard.gitguardian.com/api/v1/auth/user/github_login/
+The global and local pre-commit hook 1. [Pre-push](#pre-push) 1. [Pre-receive]
+(#pre-receive) 1. [GitLab](#gitlab) 1. [GitHub Actions](#github) 1. [Circle CI]
+(#circle-ci) 1. [Travis CI](#travis-ci) 1. [Jenkins](#jenkins) 1. [Drone]
+(#Drone) 1. [Azure Pipelines](#Azure) 1. [Output](#output) 1. [Contributing]
+(#contributing) 1. [License](#license) # Installation Install and update using
+`pip`: ```shell $ pip install ggshield ``` ggshield supports **Python 3.6 and
+newer**. The package should run on MacOS, Linux and Windows. You'll need an
+**API Key** from the [GitGuardian dashboard](https://dashboard.gitguardian.com/
+api/v1/auth/user/github_login/
 authorize?utm_source=github&utm_medium=gg_shield&utm_campaign=shield1) to use
 ggshield. Add the API Key to your environment variables: ```shell
 GITGUARDIAN_API_KEY= ``` # Updating To update ggshield you can add the option
 `-U/--upgrade` to the pip install command. ```shell $ pip install -U ggshield
 ``` # Commands ```shell Usage: ggshield [OPTIONS] COMMAND [ARGS]... Options: -
 c, --config-path FILE Set a custom config file. Ignores local and global config
 files. -v, --verbose Verbose display mode. -h, --help Show this message and
@@ -244,38 +244,43 @@
 override with the `--force` option: ```shell $ ggshield install --mode local --
 force -t "pre-push" ``` Or you can append to the existing `pre-push` script
 with the `--append` option: ```shell $ ggshield install --mode local --force -
 t "pre-push" ``` Now you're good to go! # Pre-receive A pre-receive hook allows
 you to reject commits from being pushed to a git repository if they do not
 validate every check. You can find **ggshield**'s pre-receive hook samples in
 the [doc/pre-receive.sample](doc/pre-receive.sample) and [doc/pre-receive-
-python.sample](doc/pre-receive-python.sample). ### Python git pre-receive hook
-> â  this pre-receive hook requires the host machine to have python>=3.6 and
-pip installed [**pre-receive-python.sample**](doc/pre-receive-python.sample) -
-Install ggshield from pip: `pip install ggshield` - Move `pre-receive-
-python.sample` to `.git/hooks/pre-receive` - Do not forget to `chmod +x .git/
-hooks/pre-receive` - either set an environment variable machine wide
-`GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed
-in the sample file. **How do I add ignored matches and use a custom config in
-this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in the system.
-An example config file is available [here](.gitguardian.example.yml) - Replace
-in the pre-receive hook ```shell ggshield scan commit-range "${span}" &&
-continue ``` with: ```shell ggshield -c
-yaml> scan commit-range "${span}" && continue ``` ### Docker git pre-receive
-hook > â  this pre-receive hook requires the host machine to have docker
-installed. [**pre-receive.sample**](doc/pre-receive.sample) - Move `pre-
-receive.sample` to `.git/hooks/pre-receive` - Do not forget to `chmod +x .git/
-hooks/pre-receive` - either set an environment variable machine wide
-`GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed
-in the sample file. **How do I add ignored matches and use a custom config in
-this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in the system.
-An example config file is available [here](.gitguardian.example.yml) - Replace
-in the pre-receive hook ```shell docker run --rm -v $(pwd):/data -
-e GITGUARDIAN_API_KEY gitguardian/ggshield:latest ggshield scan commit-range "$
-{span}" && continue ``` with: ```shell docker run --rm -v $(pwd):/data -v
+python.sample](doc/pre-receive-python.sample). **ggshield**'s pre-receive hook
+can be skipped if the developer passes the option `breakglass` to the git push.
+For this setting to work the remote must have push options enabled. (`git
+config receive.advertisePushOptions true`) Examples: ```sh $ git push -
+o breakglass $ git push --push-option=breakglass ``` ## Install ggshield git
+pre-receive hook locally [**pre-receive-python.sample**](doc/pre-receive-
+python.sample) 1. This pre-receive hook requires the host machine to have
+python>=3.8 and pip installed 1. Install ggshield from pip: `pip install
+ggshield` 1. Move `pre-receive-python.sample` to `.git/hooks/pre-receive` 1. Do
+not forget to `chmod +x .git/hooks/pre-receive` 1. either set an environment
+variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-
+receive` as instructed in the sample file. **How do I add ignored matches and
+use a custom config in this pre-receive hook?** - Create a `gitguardian.yaml`
+somewhere in the system. An example config file is available [here]
+(.gitguardian.example.yml) - Replace in the pre-receive hook ```shell ggshield
+scan commit-range "${span}" && continue ``` with: ```shell ggshield -c
+yaml> scan commit-range "${span}" && continue ``` ## Install ggshield git pre-
+receive hook with docker [**pre-receive.sample**](doc/pre-receive.sample) 1.
+This pre-receive hook requires the host machine to have docker installed. 1.
+Move `pre-receive.sample` to `.git/hooks/pre-receive` 1. Do not forget to
+`chmod +x .git/hooks/pre-receive` 1. either set an environment variable machine
+wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as
+instructed in the sample file. **How do I add ignored matches and use a custom
+config in this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in
+the system. An example config file is available [here]
+(.gitguardian.example.yml) - Replace in the pre-receive hook ```shell docker
+run --rm -v $(pwd):/data -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest
+ggshield scan commit-range "${span}" && continue ``` with: ```shell docker run
+--rm -v $(pwd):/data -v
 yaml directory>:/config -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest
 ggshield -c /config/gitguardian.yaml scan commit-range "${span}" && continue
 ``` # Docker The GitGuardian Shield docker scanning tool (`ggshield scan
 docker`) is used to scan local docker images for secrets present in the image's
 creation process (`dockerfile` and build arguments) and in the image's layers'
 filesystem. If the image is not available locally on the user's machine,
 GitGuardian shield will attempt to pull the image using `docker pull `. #
```

### Comparing `ggshield-1.8.2/README.md` & `ggshield-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,25 @@
 
 1. [Pre-commit](#pre-commit)
 
    - The pre-commit framework
    - The global and local pre-commit hook
 
 1. [Pre-push](#pre-push)
-
-1) [Pre-receive hook](#git-pre-receive-hooks)
-1) [GitLab](#gitlab)
-1) [GitHub Actions](#github)
-1) [Circle CI](#circle-ci)
-1) [Travis CI](#travis-ci)
-1) [Jenkins](#jenkins)
-1) [Drone](#Drone)
-1) [Azure Pipelines](#Azure)
-1) [Output](#output)
-1) [Contributing](#contributing)
-1) [License](#license)
+1. [Pre-receive](#pre-receive)
+1. [GitLab](#gitlab)
+1. [GitHub Actions](#github)
+1. [Circle CI](#circle-ci)
+1. [Travis CI](#travis-ci)
+1. [Jenkins](#jenkins)
+1. [Drone](#Drone)
+1. [Azure Pipelines](#Azure)
+1. [Output](#output)
+1. [Contributing](#contributing)
+1. [License](#license)
 
 # Installation
 
 Install and update using `pip`:
 
 ```shell
 $ pip install ggshield
@@ -604,46 +603,55 @@
 
 # Pre-receive
 
 A pre-receive hook allows you to reject commits from being pushed to a git repository if they do not validate every check.
 
 You can find **ggshield**'s pre-receive hook samples in the [doc/pre-receive.sample](doc/pre-receive.sample) and [doc/pre-receive-python.sample](doc/pre-receive-python.sample).
 
-### Python git pre-receive hook
+**ggshield**'s pre-receive hook can be skipped if the developer passes the option `breakglass` to the git push.
+
+For this setting to work the remote must have push options enabled. (`git config receive.advertisePushOptions true`)
 
-> ⚠ this pre-receive hook requires the host machine to have python>=3.6 and pip installed
+Examples:
+
+```sh
+$ git push -o breakglass
+$ git push --push-option=breakglass
+```
+
+## Install ggshield git pre-receive hook locally
 
 [**pre-receive-python.sample**](doc/pre-receive-python.sample)
 
-- Install ggshield from pip: `pip install ggshield`
-- Move `pre-receive-python.sample` to `.git/hooks/pre-receive`
-- Do not forget to `chmod +x .git/hooks/pre-receive`
-- either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
+1. This pre-receive hook requires the host machine to have python>=3.8 and pip installed
+1. Install ggshield from pip: `pip install ggshield`
+1. Move `pre-receive-python.sample` to `.git/hooks/pre-receive`
+1. Do not forget to `chmod +x .git/hooks/pre-receive`
+1. either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
 
 **How do I add ignored matches and use a custom config in this pre-receive hook?**
 
 - Create a `gitguardian.yaml` somewhere in the system. An example config file is available [here](.gitguardian.example.yml)
 - Replace in the pre-receive hook
   ```shell
   ggshield scan commit-range "${span}" && continue
   ```
   with:
   ```shell
   ggshield -c <INSERT path to gitguardian.yaml> scan commit-range "${span}" && continue
   ```
 
-### Docker git pre-receive hook
-
-> ⚠ this pre-receive hook requires the host machine to have docker installed.
+## Install ggshield git pre-receive hook with docker
 
 [**pre-receive.sample**](doc/pre-receive.sample)
 
-- Move `pre-receive.sample` to `.git/hooks/pre-receive`
-- Do not forget to `chmod +x .git/hooks/pre-receive`
-- either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
+1. This pre-receive hook requires the host machine to have docker installed.
+1. Move `pre-receive.sample` to `.git/hooks/pre-receive`
+1. Do not forget to `chmod +x .git/hooks/pre-receive`
+1. either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
 
 **How do I add ignored matches and use a custom config in this pre-receive hook?**
 
 - Create a `gitguardian.yaml` somewhere in the system. An example config file is available [here](.gitguardian.example.yml)
 - Replace in the pre-receive hook
   ```shell
   docker run --rm -v $(pwd):/data -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest ggshield scan commit-range "${span}" && continue
```

#### html2text {}

```diff
@@ -37,23 +37,23 @@
 (#travis-ci) ## Table of Contents 1. [Introduction](#introduction) 1.
 [Installation](#installation) 1. [Updating](#updating) 1. [Configuration]
 (#configuration) 1. [Environment Variables](#environment-variables) 2. [On-
 premises](#on-premises-configuration) 3. [Ignoring a secret](#ignoring-a-
 secret) 1. [Commands](#commands) - [Scan](#scan-command) - [Install](#install-
 command) - [Ignore](#ignore-command) - [Quota](#quota-command) - [API Status]
 (#api-status-command) 1. [Pre-commit](#pre-commit) - The pre-commit framework -
-The global and local pre-commit hook 1. [Pre-push](#pre-push) 1) [Pre-receive
-hook](#git-pre-receive-hooks) 1) [GitLab](#gitlab) 1) [GitHub Actions](#github)
-1) [Circle CI](#circle-ci) 1) [Travis CI](#travis-ci) 1) [Jenkins](#jenkins) 1)
-[Drone](#Drone) 1) [Azure Pipelines](#Azure) 1) [Output](#output) 1)
-[Contributing](#contributing) 1) [License](#license) # Installation Install and
-update using `pip`: ```shell $ pip install ggshield ``` ggshield supports
-**Python 3.6 and newer**. The package should run on MacOS, Linux and Windows.
-You'll need an **API Key** from the [GitGuardian dashboard](https://
-dashboard.gitguardian.com/api/v1/auth/user/github_login/
+The global and local pre-commit hook 1. [Pre-push](#pre-push) 1. [Pre-receive]
+(#pre-receive) 1. [GitLab](#gitlab) 1. [GitHub Actions](#github) 1. [Circle CI]
+(#circle-ci) 1. [Travis CI](#travis-ci) 1. [Jenkins](#jenkins) 1. [Drone]
+(#Drone) 1. [Azure Pipelines](#Azure) 1. [Output](#output) 1. [Contributing]
+(#contributing) 1. [License](#license) # Installation Install and update using
+`pip`: ```shell $ pip install ggshield ``` ggshield supports **Python 3.6 and
+newer**. The package should run on MacOS, Linux and Windows. You'll need an
+**API Key** from the [GitGuardian dashboard](https://dashboard.gitguardian.com/
+api/v1/auth/user/github_login/
 authorize?utm_source=github&utm_medium=gg_shield&utm_campaign=shield1) to use
 ggshield. Add the API Key to your environment variables: ```shell
 GITGUARDIAN_API_KEY= ``` # Updating To update ggshield you can add the option
 `-U/--upgrade` to the pip install command. ```shell $ pip install -U ggshield
 ``` # Commands ```shell Usage: ggshield [OPTIONS] COMMAND [ARGS]... Options: -
 c, --config-path FILE Set a custom config file. Ignores local and global config
 files. -v, --verbose Verbose display mode. -h, --help Show this message and
@@ -231,38 +231,43 @@
 override with the `--force` option: ```shell $ ggshield install --mode local --
 force -t "pre-push" ``` Or you can append to the existing `pre-push` script
 with the `--append` option: ```shell $ ggshield install --mode local --force -
 t "pre-push" ``` Now you're good to go! # Pre-receive A pre-receive hook allows
 you to reject commits from being pushed to a git repository if they do not
 validate every check. You can find **ggshield**'s pre-receive hook samples in
 the [doc/pre-receive.sample](doc/pre-receive.sample) and [doc/pre-receive-
-python.sample](doc/pre-receive-python.sample). ### Python git pre-receive hook
-> â  this pre-receive hook requires the host machine to have python>=3.6 and
-pip installed [**pre-receive-python.sample**](doc/pre-receive-python.sample) -
-Install ggshield from pip: `pip install ggshield` - Move `pre-receive-
-python.sample` to `.git/hooks/pre-receive` - Do not forget to `chmod +x .git/
-hooks/pre-receive` - either set an environment variable machine wide
-`GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed
-in the sample file. **How do I add ignored matches and use a custom config in
-this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in the system.
-An example config file is available [here](.gitguardian.example.yml) - Replace
-in the pre-receive hook ```shell ggshield scan commit-range "${span}" &&
-continue ``` with: ```shell ggshield -c
-yaml> scan commit-range "${span}" && continue ``` ### Docker git pre-receive
-hook > â  this pre-receive hook requires the host machine to have docker
-installed. [**pre-receive.sample**](doc/pre-receive.sample) - Move `pre-
-receive.sample` to `.git/hooks/pre-receive` - Do not forget to `chmod +x .git/
-hooks/pre-receive` - either set an environment variable machine wide
-`GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed
-in the sample file. **How do I add ignored matches and use a custom config in
-this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in the system.
-An example config file is available [here](.gitguardian.example.yml) - Replace
-in the pre-receive hook ```shell docker run --rm -v $(pwd):/data -
-e GITGUARDIAN_API_KEY gitguardian/ggshield:latest ggshield scan commit-range "$
-{span}" && continue ``` with: ```shell docker run --rm -v $(pwd):/data -v
+python.sample](doc/pre-receive-python.sample). **ggshield**'s pre-receive hook
+can be skipped if the developer passes the option `breakglass` to the git push.
+For this setting to work the remote must have push options enabled. (`git
+config receive.advertisePushOptions true`) Examples: ```sh $ git push -
+o breakglass $ git push --push-option=breakglass ``` ## Install ggshield git
+pre-receive hook locally [**pre-receive-python.sample**](doc/pre-receive-
+python.sample) 1. This pre-receive hook requires the host machine to have
+python>=3.8 and pip installed 1. Install ggshield from pip: `pip install
+ggshield` 1. Move `pre-receive-python.sample` to `.git/hooks/pre-receive` 1. Do
+not forget to `chmod +x .git/hooks/pre-receive` 1. either set an environment
+variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-
+receive` as instructed in the sample file. **How do I add ignored matches and
+use a custom config in this pre-receive hook?** - Create a `gitguardian.yaml`
+somewhere in the system. An example config file is available [here]
+(.gitguardian.example.yml) - Replace in the pre-receive hook ```shell ggshield
+scan commit-range "${span}" && continue ``` with: ```shell ggshield -c
+yaml> scan commit-range "${span}" && continue ``` ## Install ggshield git pre-
+receive hook with docker [**pre-receive.sample**](doc/pre-receive.sample) 1.
+This pre-receive hook requires the host machine to have docker installed. 1.
+Move `pre-receive.sample` to `.git/hooks/pre-receive` 1. Do not forget to
+`chmod +x .git/hooks/pre-receive` 1. either set an environment variable machine
+wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as
+instructed in the sample file. **How do I add ignored matches and use a custom
+config in this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in
+the system. An example config file is available [here]
+(.gitguardian.example.yml) - Replace in the pre-receive hook ```shell docker
+run --rm -v $(pwd):/data -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest
+ggshield scan commit-range "${span}" && continue ``` with: ```shell docker run
+--rm -v $(pwd):/data -v
 yaml directory>:/config -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest
 ggshield -c /config/gitguardian.yaml scan commit-range "${span}" && continue
 ``` # Docker The GitGuardian Shield docker scanning tool (`ggshield scan
 docker`) is used to scan local docker images for secrets present in the image's
 creation process (`dockerfile` and build arguments) and in the image's layers'
 filesystem. If the image is not available locally on the user's machine,
 GitGuardian shield will attempt to pull the image using `docker pull `. #
```

### Comparing `ggshield-1.8.2/ggshield/ci.py` & `ggshield-1.9.0/ggshield/ci.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import os
-import traceback
 from typing import List
 
 import click
 
-from ggshield.utils import EMPTY_SHA, SupportedCI, SupportedScanMode
+from ggshield.utils import EMPTY_SHA, SupportedCI, SupportedScanMode, handle_exception
 
+from .config import Cache
 from .dev_scan import scan_commit_range
 from .git_shell import check_git_dir, get_list_commit_SHA
 
 
+class ReadOnlyCache(Cache):
+    """
+    A version of Cache which does not write anything to the disk.
+    """
+
+    def save(self) -> bool:  # pragma: no cover
+        return True
+
+
 def jenkins_range(verbose: bool) -> List[str]:  # pragma: no cover
     head_commit = os.getenv("GIT_COMMIT")
     previous_commit = os.getenv("GIT_PREVIOUS_COMMIT")
 
     if verbose:
         click.echo(
             f"\tGIT_COMMIT: {head_commit}" f"\nGIT_PREVIOUS_COMMIT: {previous_commit}"
@@ -269,26 +278,20 @@
         if config.verbose:
             click.echo(f"Commits to scan: {len(commit_list)}")
 
         mode_header = "/".join([SupportedScanMode.CI.value, ci_env.value])
 
         return scan_commit_range(
             client=ctx.obj["client"],
-            cache=ctx.obj["cache"],
+            cache=ReadOnlyCache(),
             commit_list=commit_list,
             output_handler=ctx.obj["output_handler"],
             verbose=config.verbose,
             filter_set=ctx.obj["filter_set"],
             matches_ignore=config.matches_ignore,
             all_policies=config.all_policies,
             scan_id=" ".join(commit_list),
             mode_header=mode_header,
             banlisted_detectors=config.banlisted_detectors,
         )
-    except click.exceptions.Abort:
-        return 0
-    except click.ClickException as exc:
-        raise exc
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
```

### Comparing `ggshield-1.8.2/ggshield/cmd.py` & `ggshield-1.9.0/ggshield/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 from pathlib import Path
 from typing import Any, List, NoReturn, Optional, Type, cast
 
 import click
 
 from ggshield.output import JSONHandler, OutputHandler, TextHandler
+from ggshield.pre_receive_cmd import prereceive_cmd
 
 from .ci import ci_cmd
 from .config import CONTEXT_SETTINGS, Cache, Config, load_dot_env
 from .dev_scan import path_cmd, range_cmd, repo_cmd
 from .docker import docker_archive_cmd, docker_name_cmd
 from .filter import path_filter_set
 from .hook_cmd import precommit_cmd, prepush_cmd
@@ -22,14 +23,15 @@
 
 
 @click.group(
     commands={
         "commit-range": range_cmd,
         "pre-commit": precommit_cmd,
         "pre-push": prepush_cmd,
+        "pre-receive": prereceive_cmd,
         "ci": ci_cmd,
         "path": path_cmd,
         "repo": repo_cmd,
         "docker": docker_name_cmd,
         "docker-archive": docker_archive_cmd,
     },
 )
```

### Comparing `ggshield-1.8.2/ggshield/config.py` & `ggshield-1.9.0/ggshield/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -220,26 +220,16 @@
                     if elem not in attribute:
                         attribute.append(elem)
             else:
                 getattr(self, name).update(value)
         else:
             super().__setattr__(name, value)
 
-    def create_empty_cache(self) -> None:
-        # Creates a new file
-        try:
-            with open(self.CACHE_FILENAME, "w"):
-                pass
-        except PermissionError:
-            # Hotfix: for the time being we skip cache handling if permission denied
-            pass
-
     def load_cache(self) -> bool:
         if not os.path.isfile(self.CACHE_FILENAME):
-            self.create_empty_cache()
             return True
 
         _cache: dict = {}
         if os.stat(self.CACHE_FILENAME).st_size != 0:
             try:
                 f = open(self.CACHE_FILENAME, "r")
             except PermissionError:
@@ -282,17 +272,14 @@
         for key in self.get_attributes_keys():
             value = _cache[key]
             if type(value) is set:
                 _cache[key] = list(value)
         return _cache
 
     def save(self) -> bool:
-        if not os.path.isfile(self.CACHE_FILENAME):
-            return False
-
         try:
             f = open(self.CACHE_FILENAME, "w")
         except PermissionError:
             # Hotfix: for the time being we skip cache handling if permission denied
             return True
         else:
             with f:
```

### Comparing `ggshield-1.8.2/ggshield/dev_scan.py` & `ggshield-1.9.0/ggshield/dev_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import concurrent.futures
 import os
 import tempfile
-import traceback
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Iterable, Iterator, List, Optional, Set
 
 import click
 from pygitguardian import GGClient
 
@@ -13,15 +12,15 @@
 from ggshield.scan import Commit, ScanCollection
 from ggshield.text_utils import STYLE, format_text
 
 from .config import CPU_COUNT, Cache, Config
 from .filter import path_filter_set
 from .git_shell import GIT_PATH, get_list_commit_SHA, is_git_dir, shell
 from .path import get_files_from_paths
-from .utils import REGEX_GIT_URL, SupportedScanMode
+from .utils import REGEX_GIT_URL, SupportedScanMode, handle_exception
 
 
 @contextmanager
 def cd(newdir: str) -> Iterator[None]:
     prevdir = os.getcwd()
     os.chdir(os.path.expanduser(newdir))
     try:
@@ -52,20 +51,16 @@
                 filter_set=path_filter_set(Path(os.getcwd()), []),
                 matches_ignore=config.matches_ignore,
                 all_policies=config.all_policies,
                 scan_id=scan_id,
                 mode_header=SupportedScanMode.REPO.value,
                 banlisted_detectors=config.banlisted_detectors,
             )
-    except click.exceptions.Abort:
-        return 0
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
 
 
 @click.command()
 @click.argument("repository", nargs=1, type=click.STRING, required=True)
 @click.pass_context
 def repo_cmd(ctx: click.Context, repository: str) -> int:  # pragma: no cover
     """
@@ -138,20 +133,16 @@
             filter_set=ctx.obj["filter_set"],
             matches_ignore=config.matches_ignore,
             all_policies=config.all_policies,
             scan_id=commit_range,
             mode_header=SupportedScanMode.COMMIT_RANGE.value,
             banlisted_detectors=config.banlisted_detectors,
         )
-    except click.exceptions.Abort:
-        return 0
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
 
 
 @click.command()
 @click.argument(
     "paths", nargs=-1, type=click.Path(exists=True, resolve_path=True), required=True
 )
 @click.option("--recursive", "-r", is_flag=True, help="Scan directory recursively")
@@ -181,20 +172,16 @@
             all_policies=config.all_policies,
             verbose=config.verbose,
             mode_header=SupportedScanMode.PATH.value,
         )
         scan = ScanCollection(id=" ".join(paths), type="path_scan", results=results)
 
         return output_handler.process_scan(scan)[1]
-    except click.exceptions.Abort:
-        return 0
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
 
 
 def scan_commit(
     commit: Commit,
     client: GGClient,
     cache: Cache,
     verbose: bool,
```

### Comparing `ggshield-1.8.2/ggshield/docker.py` & `ggshield-1.9.0/ggshield/docker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import subprocess
 import tempfile
-import traceback
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Set
 
 import click
 from pygitguardian.client import GGClient
 from yaspin import yaspin
 
 from ggshield.config import Cache
 from ggshield.output import OutputHandler
 from ggshield.scan import ScanCollection, get_files_from_docker_archive
-
-from .utils import SupportedScanMode
+from ggshield.utils import SupportedScanMode, handle_exception
 
 
 # bailout if docker command takes longer than 6 minutes
 DOCKER_COMMAND_TIMEOUT = 360
 
 
 class DockerArchiveCreationError(Exception):
@@ -126,21 +124,16 @@
                 matches_ignore=config.matches_ignore,
                 all_policies=config.all_policies,
                 scan_id=name,
                 banlisted_detectors=config.banlisted_detectors,
             )
 
             return output_handler.process_scan(scan)[1]
-        except click.exceptions.Abort:
-            return 0
         except Exception as error:
-            if config.verbose:
-                traceback.print_exc()
-
-            raise click.ClickException(str(error))
+            return handle_exception(error, config.verbose)
 
 
 @click.command(hidden=True)
 @click.argument(
     "archive", nargs=1, type=click.Path(exists=True, resolve_path=True), required=True
 )
 @click.pass_context
@@ -165,14 +158,9 @@
             matches_ignore=config.matches_ignore,
             all_policies=config.all_policies,
             scan_id=archive,
             banlisted_detectors=config.banlisted_detectors,
         )
 
         return output_handler.process_scan(scan)[1]
-    except click.exceptions.Abort:
-        return 0
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
```

### Comparing `ggshield-1.8.2/ggshield/filter.py` & `ggshield-1.9.0/ggshield/filter.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/git_shell.py` & `ggshield-1.9.0/ggshield/git_shell.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/hook_cmd.py` & `ggshield-1.9.0/ggshield/hook_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import sys
-import traceback
 from typing import List, Optional, Tuple
 
 import click
 
 from ggshield.dev_scan import scan_commit_range
 from ggshield.output import TextHandler
 from ggshield.scan import Commit, ScanCollection
-from ggshield.utils import EMPTY_SHA, EMPTY_TREE, SupportedScanMode
+from ggshield.utils import EMPTY_SHA, EMPTY_TREE, SupportedScanMode, handle_exception
 
 from .git_shell import check_git_dir, get_list_commit_SHA
 
 
 @click.command()
 @click.argument("precommit_args", nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
@@ -37,20 +36,16 @@
             mode_header=SupportedScanMode.PRE_COMMIT.value,
             banlisted_detectors=config.banlisted_detectors,
         )
 
         return output_handler.process_scan(
             ScanCollection(id="cached", type="pre-commit", results=results)
         )[1]
-    except click.exceptions.Abort:
-        return 0
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
 
 
 def collect_from_stdin() -> Tuple[str, str]:
     """
     Collect pre-commit variables from stdin.
     """
     prepush_input = sys.stdin.read().split()
@@ -143,15 +138,9 @@
             filter_set=ctx.obj["filter_set"],
             matches_ignore=config.matches_ignore,
             all_policies=config.all_policies,
             scan_id=" ".join(commit_list),
             mode_header=SupportedScanMode.PRE_PUSH.value,
             banlisted_detectors=config.banlisted_detectors,
         )
-    except click.exceptions.Abort:
-        return 0
-    except click.ClickException as exc:
-        raise exc
     except Exception as error:
-        if config.verbose:
-            traceback.print_exc()
-        raise click.ClickException(str(error))
+        return handle_exception(error, config.verbose)
```

### Comparing `ggshield-1.8.2/ggshield/ignore.py` & `ggshield-1.9.0/ggshield/ignore.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/install.py` & `ggshield-1.9.0/ggshield/install.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/output/json/json_output.py` & `ggshield-1.9.0/ggshield/output/json/json_output.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/output/json/schemas.py` & `ggshield-1.9.0/ggshield/output/json/schemas.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/output/output_handler.py` & `ggshield-1.9.0/ggshield/output/output_handler.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/output/text/message.py` & `ggshield-1.9.0/ggshield/output/text/message.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/output/text/text_output.py` & `ggshield-1.9.0/ggshield/output/text/text_output.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/path.py` & `ggshield-1.9.0/ggshield/path.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/quota.py` & `ggshield-1.9.0/ggshield/quota.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/scan/docker.py` & `ggshield-1.9.0/ggshield/scan/docker.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/scan/scannable.py` & `ggshield-1.9.0/ggshield/scan/scannable.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/scan/scannable_errors.py` & `ggshield-1.9.0/ggshield/scan/scannable_errors.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/status.py` & `ggshield-1.9.0/ggshield/status.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/text_utils.py` & `ggshield-1.9.0/ggshield/text_utils.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/ggshield/utils.py` & `ggshield-1.9.0/ggshield/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import traceback
 from enum import Enum
 from typing import Iterable, List, Optional
 
 import click
 import urllib3
 from pygitguardian import GGClient
 from pygitguardian.models import Match
@@ -24,14 +25,18 @@
 REGEX_HEADER_INFO = re.compile(
     r"Author:\s(?P<author>.+?)\ <(?P<email>.+?)>\nDate:\s+(?P<date>.+)?\n"
 )
 
 EMPTY_SHA = "0000000000000000000000000000000000000000"
 EMPTY_TREE = "4b825dc642cb6eb9a060e54bf8d69288fbee4904"
 
+# GitHub timeouts every pre-receive hook after 5s with an error.
+# We try and anticipate that so we can control the return code
+PRERECEIVE_TIMEOUT = 4.5
+
 
 class Filemode(Enum):
     """
     Enum class for git filemode.
 
     Attributes:
         start (int): The first line to read in this filemode scenario
@@ -194,14 +199,15 @@
 
 class SupportedScanMode(Enum):
     REPO = "repo"
     PATH = "path"
     COMMIT_RANGE = "commit_range"
     PRE_COMMIT = "pre_commit"
     PRE_PUSH = "pre_push"
+    PRE_RECEIVE = "pre_receive"
     CI = "ci"
     DOCKER = "docker"
 
 
 json_output_option_decorator = click.option(
     "--json",
     "json_output",
@@ -227,7 +233,21 @@
     return GGClient(
         api_key=api_key,
         base_uri=base_uri,
         user_agent="ggshield",
         timeout=60,
         session=session,
     )
+
+
+def handle_exception(e: Exception, verbose: bool) -> int:
+    """
+    Handle exception from a scan command.
+    """
+    if isinstance(e, click.exceptions.Abort):
+        return 0
+    elif isinstance(e, click.ClickException):
+        raise e
+    else:
+        if verbose:
+            traceback.print_exc()
+        raise click.ClickException(str(e))
```

### Comparing `ggshield-1.8.2/ggshield.egg-info/PKG-INFO` & `ggshield-1.9.0/ggshield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggshield
-Version: 1.8.2
+Version: 1.9.0
 Summary: Detect secrets from all sources using GitGuardian's brains
 Home-page: https://github.com/GitGuardian/ggshield
 Author: GitGuardian
 Author-email: support@gitguardian.com
 Maintainer: GitGuardian
 License: MIT
 Keywords: cli devsecops secrets-detection security-tools gitguardian
@@ -88,26 +88,25 @@
 
 1. [Pre-commit](#pre-commit)
 
    - The pre-commit framework
    - The global and local pre-commit hook
 
 1. [Pre-push](#pre-push)
-
-1) [Pre-receive hook](#git-pre-receive-hooks)
-1) [GitLab](#gitlab)
-1) [GitHub Actions](#github)
-1) [Circle CI](#circle-ci)
-1) [Travis CI](#travis-ci)
-1) [Jenkins](#jenkins)
-1) [Drone](#Drone)
-1) [Azure Pipelines](#Azure)
-1) [Output](#output)
-1) [Contributing](#contributing)
-1) [License](#license)
+1. [Pre-receive](#pre-receive)
+1. [GitLab](#gitlab)
+1. [GitHub Actions](#github)
+1. [Circle CI](#circle-ci)
+1. [Travis CI](#travis-ci)
+1. [Jenkins](#jenkins)
+1. [Drone](#Drone)
+1. [Azure Pipelines](#Azure)
+1. [Output](#output)
+1. [Contributing](#contributing)
+1. [License](#license)
 
 # Installation
 
 Install and update using `pip`:
 
 ```shell
 $ pip install ggshield
@@ -631,46 +630,55 @@
 
 # Pre-receive
 
 A pre-receive hook allows you to reject commits from being pushed to a git repository if they do not validate every check.
 
 You can find **ggshield**'s pre-receive hook samples in the [doc/pre-receive.sample](doc/pre-receive.sample) and [doc/pre-receive-python.sample](doc/pre-receive-python.sample).
 
-### Python git pre-receive hook
+**ggshield**'s pre-receive hook can be skipped if the developer passes the option `breakglass` to the git push.
+
+For this setting to work the remote must have push options enabled. (`git config receive.advertisePushOptions true`)
 
-> ⚠ this pre-receive hook requires the host machine to have python>=3.6 and pip installed
+Examples:
+
+```sh
+$ git push -o breakglass
+$ git push --push-option=breakglass
+```
+
+## Install ggshield git pre-receive hook locally
 
 [**pre-receive-python.sample**](doc/pre-receive-python.sample)
 
-- Install ggshield from pip: `pip install ggshield`
-- Move `pre-receive-python.sample` to `.git/hooks/pre-receive`
-- Do not forget to `chmod +x .git/hooks/pre-receive`
-- either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
+1. This pre-receive hook requires the host machine to have python>=3.8 and pip installed
+1. Install ggshield from pip: `pip install ggshield`
+1. Move `pre-receive-python.sample` to `.git/hooks/pre-receive`
+1. Do not forget to `chmod +x .git/hooks/pre-receive`
+1. either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
 
 **How do I add ignored matches and use a custom config in this pre-receive hook?**
 
 - Create a `gitguardian.yaml` somewhere in the system. An example config file is available [here](.gitguardian.example.yml)
 - Replace in the pre-receive hook
   ```shell
   ggshield scan commit-range "${span}" && continue
   ```
   with:
   ```shell
   ggshield -c <INSERT path to gitguardian.yaml> scan commit-range "${span}" && continue
   ```
 
-### Docker git pre-receive hook
-
-> ⚠ this pre-receive hook requires the host machine to have docker installed.
+## Install ggshield git pre-receive hook with docker
 
 [**pre-receive.sample**](doc/pre-receive.sample)
 
-- Move `pre-receive.sample` to `.git/hooks/pre-receive`
-- Do not forget to `chmod +x .git/hooks/pre-receive`
-- either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
+1. This pre-receive hook requires the host machine to have docker installed.
+1. Move `pre-receive.sample` to `.git/hooks/pre-receive`
+1. Do not forget to `chmod +x .git/hooks/pre-receive`
+1. either set an environment variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed in the sample file.
 
 **How do I add ignored matches and use a custom config in this pre-receive hook?**
 
 - Create a `gitguardian.yaml` somewhere in the system. An example config file is available [here](.gitguardian.example.yml)
 - Replace in the pre-receive hook
   ```shell
   docker run --rm -v $(pwd):/data -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest ggshield scan commit-range "${span}" && continue
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ggshield Version: 1.8.2 Summary: Detect secrets
+Metadata-Version: 2.1 Name: ggshield Version: 1.9.0 Summary: Detect secrets
 from all sources using GitGuardian's brains Home-page: https://github.com/
 GitGuardian/ggshield Author: GitGuardian Author-email: support@gitguardian.com
 Maintainer: GitGuardian License: MIT Keywords: cli devsecops secrets-detection
 security-tools gitguardian Platform: UNKNOWN Classifier: Development Status ::
 5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: End Users/Desktop Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
@@ -50,23 +50,23 @@
 (#travis-ci) ## Table of Contents 1. [Introduction](#introduction) 1.
 [Installation](#installation) 1. [Updating](#updating) 1. [Configuration]
 (#configuration) 1. [Environment Variables](#environment-variables) 2. [On-
 premises](#on-premises-configuration) 3. [Ignoring a secret](#ignoring-a-
 secret) 1. [Commands](#commands) - [Scan](#scan-command) - [Install](#install-
 command) - [Ignore](#ignore-command) - [Quota](#quota-command) - [API Status]
 (#api-status-command) 1. [Pre-commit](#pre-commit) - The pre-commit framework -
-The global and local pre-commit hook 1. [Pre-push](#pre-push) 1) [Pre-receive
-hook](#git-pre-receive-hooks) 1) [GitLab](#gitlab) 1) [GitHub Actions](#github)
-1) [Circle CI](#circle-ci) 1) [Travis CI](#travis-ci) 1) [Jenkins](#jenkins) 1)
-[Drone](#Drone) 1) [Azure Pipelines](#Azure) 1) [Output](#output) 1)
-[Contributing](#contributing) 1) [License](#license) # Installation Install and
-update using `pip`: ```shell $ pip install ggshield ``` ggshield supports
-**Python 3.6 and newer**. The package should run on MacOS, Linux and Windows.
-You'll need an **API Key** from the [GitGuardian dashboard](https://
-dashboard.gitguardian.com/api/v1/auth/user/github_login/
+The global and local pre-commit hook 1. [Pre-push](#pre-push) 1. [Pre-receive]
+(#pre-receive) 1. [GitLab](#gitlab) 1. [GitHub Actions](#github) 1. [Circle CI]
+(#circle-ci) 1. [Travis CI](#travis-ci) 1. [Jenkins](#jenkins) 1. [Drone]
+(#Drone) 1. [Azure Pipelines](#Azure) 1. [Output](#output) 1. [Contributing]
+(#contributing) 1. [License](#license) # Installation Install and update using
+`pip`: ```shell $ pip install ggshield ``` ggshield supports **Python 3.6 and
+newer**. The package should run on MacOS, Linux and Windows. You'll need an
+**API Key** from the [GitGuardian dashboard](https://dashboard.gitguardian.com/
+api/v1/auth/user/github_login/
 authorize?utm_source=github&utm_medium=gg_shield&utm_campaign=shield1) to use
 ggshield. Add the API Key to your environment variables: ```shell
 GITGUARDIAN_API_KEY= ``` # Updating To update ggshield you can add the option
 `-U/--upgrade` to the pip install command. ```shell $ pip install -U ggshield
 ``` # Commands ```shell Usage: ggshield [OPTIONS] COMMAND [ARGS]... Options: -
 c, --config-path FILE Set a custom config file. Ignores local and global config
 files. -v, --verbose Verbose display mode. -h, --help Show this message and
@@ -244,38 +244,43 @@
 override with the `--force` option: ```shell $ ggshield install --mode local --
 force -t "pre-push" ``` Or you can append to the existing `pre-push` script
 with the `--append` option: ```shell $ ggshield install --mode local --force -
 t "pre-push" ``` Now you're good to go! # Pre-receive A pre-receive hook allows
 you to reject commits from being pushed to a git repository if they do not
 validate every check. You can find **ggshield**'s pre-receive hook samples in
 the [doc/pre-receive.sample](doc/pre-receive.sample) and [doc/pre-receive-
-python.sample](doc/pre-receive-python.sample). ### Python git pre-receive hook
-> â  this pre-receive hook requires the host machine to have python>=3.6 and
-pip installed [**pre-receive-python.sample**](doc/pre-receive-python.sample) -
-Install ggshield from pip: `pip install ggshield` - Move `pre-receive-
-python.sample` to `.git/hooks/pre-receive` - Do not forget to `chmod +x .git/
-hooks/pre-receive` - either set an environment variable machine wide
-`GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed
-in the sample file. **How do I add ignored matches and use a custom config in
-this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in the system.
-An example config file is available [here](.gitguardian.example.yml) - Replace
-in the pre-receive hook ```shell ggshield scan commit-range "${span}" &&
-continue ``` with: ```shell ggshield -c
-yaml> scan commit-range "${span}" && continue ``` ### Docker git pre-receive
-hook > â  this pre-receive hook requires the host machine to have docker
-installed. [**pre-receive.sample**](doc/pre-receive.sample) - Move `pre-
-receive.sample` to `.git/hooks/pre-receive` - Do not forget to `chmod +x .git/
-hooks/pre-receive` - either set an environment variable machine wide
-`GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as instructed
-in the sample file. **How do I add ignored matches and use a custom config in
-this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in the system.
-An example config file is available [here](.gitguardian.example.yml) - Replace
-in the pre-receive hook ```shell docker run --rm -v $(pwd):/data -
-e GITGUARDIAN_API_KEY gitguardian/ggshield:latest ggshield scan commit-range "$
-{span}" && continue ``` with: ```shell docker run --rm -v $(pwd):/data -v
+python.sample](doc/pre-receive-python.sample). **ggshield**'s pre-receive hook
+can be skipped if the developer passes the option `breakglass` to the git push.
+For this setting to work the remote must have push options enabled. (`git
+config receive.advertisePushOptions true`) Examples: ```sh $ git push -
+o breakglass $ git push --push-option=breakglass ``` ## Install ggshield git
+pre-receive hook locally [**pre-receive-python.sample**](doc/pre-receive-
+python.sample) 1. This pre-receive hook requires the host machine to have
+python>=3.8 and pip installed 1. Install ggshield from pip: `pip install
+ggshield` 1. Move `pre-receive-python.sample` to `.git/hooks/pre-receive` 1. Do
+not forget to `chmod +x .git/hooks/pre-receive` 1. either set an environment
+variable machine wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-
+receive` as instructed in the sample file. **How do I add ignored matches and
+use a custom config in this pre-receive hook?** - Create a `gitguardian.yaml`
+somewhere in the system. An example config file is available [here]
+(.gitguardian.example.yml) - Replace in the pre-receive hook ```shell ggshield
+scan commit-range "${span}" && continue ``` with: ```shell ggshield -c
+yaml> scan commit-range "${span}" && continue ``` ## Install ggshield git pre-
+receive hook with docker [**pre-receive.sample**](doc/pre-receive.sample) 1.
+This pre-receive hook requires the host machine to have docker installed. 1.
+Move `pre-receive.sample` to `.git/hooks/pre-receive` 1. Do not forget to
+`chmod +x .git/hooks/pre-receive` 1. either set an environment variable machine
+wide `GITGUARDIAN_API_KEY` or set it in the `.git/hooks/pre-receive` as
+instructed in the sample file. **How do I add ignored matches and use a custom
+config in this pre-receive hook?** - Create a `gitguardian.yaml` somewhere in
+the system. An example config file is available [here]
+(.gitguardian.example.yml) - Replace in the pre-receive hook ```shell docker
+run --rm -v $(pwd):/data -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest
+ggshield scan commit-range "${span}" && continue ``` with: ```shell docker run
+--rm -v $(pwd):/data -v
 yaml directory>:/config -e GITGUARDIAN_API_KEY gitguardian/ggshield:latest
 ggshield -c /config/gitguardian.yaml scan commit-range "${span}" && continue
 ``` # Docker The GitGuardian Shield docker scanning tool (`ggshield scan
 docker`) is used to scan local docker images for secrets present in the image's
 creation process (`dockerfile` and build arguments) and in the image's layers'
 filesystem. If the image is not available locally on the user's machine,
 GitGuardian shield will attempt to pull the image using `docker pull `. #
```

### Comparing `ggshield-1.8.2/ggshield.egg-info/SOURCES.txt` & `ggshield-1.9.0/ggshield.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ggshield/docker.py
 ggshield/filter.py
 ggshield/git_shell.py
 ggshield/hook_cmd.py
 ggshield/ignore.py
 ggshield/install.py
 ggshield/path.py
+ggshield/pre_receive_cmd.py
 ggshield/quota.py
 ggshield/status.py
 ggshield/text_utils.py
 ggshield/utils.py
 ggshield.egg-info/PKG-INFO
 ggshield.egg-info/SOURCES.txt
 ggshield.egg-info/dependency_links.txt
```

### Comparing `ggshield-1.8.2/pyproject.toml` & `ggshield-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/setup.py` & `ggshield-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/output/snapshots/snap_test_json_output.py` & `ggshield-1.9.0/tests/output/snapshots/snap_test_json_output.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/output/snapshots/snap_test_text_output.py` & `ggshield-1.9.0/tests/output/snapshots/snap_test_text_output.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/output/test_json_output.py` & `ggshield-1.9.0/tests/output/test_json_output.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/output/test_message.py` & `ggshield-1.9.0/tests/output/test_message.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/output/test_text_output.py` & `ggshield-1.9.0/tests/output/test_text_output.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/scan/snapshots/snap_test_scannable_errors.py` & `ggshield-1.9.0/tests/scan/snapshots/snap_test_scannable_errors.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/scan/test_scan_docker.py` & `ggshield-1.9.0/tests/scan/test_scan_docker.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/scan/test_scannable.py` & `ggshield-1.9.0/tests/scan/test_scannable.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/scan/test_scannable_errors.py` & `ggshield-1.9.0/tests/scan/test_scannable_errors.py`

 * *Files identical despite different names*

### Comparing `ggshield-1.8.2/tests/snapshots/snap_test_cli.py` & `ggshield-1.9.0/tests/snapshots/snap_test_cli.py`

 * *Files identical despite different names*

