# Comparing `tmp/climix-0.18.0rc2.tar.gz` & `tmp/climix-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climix-0.18.0rc2.tar", last modified: Fri Apr 21 17:20:58 2023, max compression
+gzip compressed data, was "climix-0.18.1.tar", last modified: Tue Apr 25 13:31:05 2023, max compression
```

## Comparing `climix-0.18.0rc2.tar` & `climix-0.18.1.tar`

### file list

```diff
@@ -1,71 +1,83 @@
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.142170 climix-0.18.0rc2/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12135 2023-04-21 17:20:00.000000 climix-0.18.0rc2/CHANGELOG.md
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11357 2023-04-20 14:40:21.000000 climix-0.18.0rc2/LICENSE
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      136 2023-04-21 15:55:28.000000 climix-0.18.0rc2/MANIFEST.in
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1402 2023-04-21 17:20:58.142170 climix-0.18.0rc2/PKG-INFO
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      487 2020-01-31 10:13:09.000000 climix-0.18.0rc2/README.md
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.111170 climix-0.18.0rc2/climix/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3759 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/aggregators.py
--rw-r--r--   0 a002160  (66459) smhiprimgrp  (2000)     5029 2023-04-04 13:04:32.000000 climix-0.18.0rc2/climix/dask_setup.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2552 2022-05-10 13:36:30.000000 climix-0.18.0rc2/climix/dask_take_along_axis.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    14730 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/datahandling.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.122170 climix-0.18.0rc2/climix/etc/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2300 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/etc/SMHI_extra.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5591 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/etc/climix_config.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)   107695 2023-04-21 14:07:50.000000 climix-0.18.0rc2/climix/etc/index_definitions.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     6964 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/etc/metadata.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2350 2023-04-21 14:07:50.000000 climix-0.18.0rc2/climix/etc/variables.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2449 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/index.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.125170 climix-0.18.0rc2/climix/index_functions/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      716 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    21861 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/index_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    18224 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/index_functions/percentile_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5197 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/spell_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11954 2023-04-19 14:56:21.000000 climix-0.18.0rc2/climix/index_functions/spell_kernels.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     9543 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/index_functions/support.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5426 2022-05-10 13:36:30.000000 climix-0.18.0rc2/climix/iris.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12580 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/main.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    17790 2023-04-20 14:40:21.000000 climix-0.18.0rc2/climix/metadata.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4911 2023-03-14 14:27:51.000000 climix-0.18.0rc2/climix/period.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.128170 climix-0.18.0rc2/climix/util/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      435 2023-02-08 09:48:44.000000 climix-0.18.0rc2/climix/util/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3949 2022-05-10 13:36:30.000000 climix-0.18.0rc2/climix/util/change_pr_units.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    13809 2023-03-14 14:27:51.000000 climix-0.18.0rc2/climix/util/cube_diffs.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.117170 climix-0.18.0rc2/climix.egg-info/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1402 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/PKG-INFO
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1495 2023-04-21 17:20:58.000000 climix-0.18.0rc2/climix.egg-info/SOURCES.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        1 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/dependency_links.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1488 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/entry_points.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/requires.txt
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       13 2023-04-21 17:20:57.000000 climix-0.18.0rc2/climix.egg-info/top_level.txt
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.131170 climix-0.18.0rc2/docs/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      585 2023-03-30 14:33:33.000000 climix-0.18.0rc2/docs/Makefile
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      791 2019-07-03 09:39:58.000000 climix-0.18.0rc2/docs/make.bat
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       24 2023-04-21 17:15:29.000000 climix-0.18.0rc2/docs/requirements-docs.txt
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.132170 climix-0.18.0rc2/docs/source/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2704 2023-04-21 17:15:29.000000 climix-0.18.0rc2/docs/source/conf.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      446 2023-04-21 17:15:29.000000 climix-0.18.0rc2/docs/source/index.rst
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      546 2023-04-20 14:40:21.000000 climix-0.18.0rc2/environment.yml
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.134170 climix-0.18.0rc2/jobscripts/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      485 2022-12-08 14:42:09.000000 climix-0.18.0rc2/jobscripts/climix-mpi.sh
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3790 2022-12-08 14:42:09.000000 climix-0.18.0rc2/jobscripts/climix.sh
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3236 2023-04-21 17:20:00.000000 climix-0.18.0rc2/pyproject.toml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       38 2023-04-21 17:20:58.142170 climix-0.18.0rc2/setup.cfg
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.135170 climix-0.18.0rc2/tests/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc2/tests/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1130 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/conftest.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.137170 climix-0.18.0rc2/tests/integration/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    10413 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/configuration.yml
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      779 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/conftest.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4158 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/integration/test_indices.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.138170 climix-0.18.0rc2/tests/unit/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc2/tests/unit/__init__.py
-drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 17:20:58.141170 climix-0.18.0rc2/tests/unit/index_functions/
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.0rc2/tests/unit/index_functions/__init__.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2370 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/unit/index_functions/conftest.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    70106 2023-04-21 14:07:50.000000 climix-0.18.0rc2/tests/unit/index_functions/test_index_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3567 2023-03-14 14:27:51.000000 climix-0.18.0rc2/tests/unit/index_functions/test_percentile_functions.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2353 2023-04-19 14:56:21.000000 climix-0.18.0rc2/tests/unit/index_functions/test_support.py
--rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2043 2023-03-14 14:27:51.000000 climix-0.18.0rc2/tests/unit/test_main.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.028443 climix-0.18.1/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      927 2023-04-25 13:26:33.000000 climix-0.18.1/.readthedocs.yaml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12349 2023-04-25 13:30:02.000000 climix-0.18.1/CHANGELOG.md
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11357 2023-04-20 14:40:21.000000 climix-0.18.1/LICENSE
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      136 2023-04-21 15:55:28.000000 climix-0.18.1/MANIFEST.in
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1394 2023-04-25 13:31:05.027444 climix-0.18.1/PKG-INFO
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      482 2023-04-23 13:54:44.000000 climix-0.18.1/README.md
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.005443 climix-0.18.1/climix/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-20 14:40:21.000000 climix-0.18.1/climix/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3759 2023-04-20 14:40:21.000000 climix-0.18.1/climix/aggregators.py
+-rw-r--r--   0 a002160  (66459) smhiprimgrp  (2000)     5029 2023-04-04 13:04:32.000000 climix-0.18.1/climix/dask_setup.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2552 2022-05-10 13:36:30.000000 climix-0.18.1/climix/dask_take_along_axis.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    14730 2023-04-20 14:40:21.000000 climix-0.18.1/climix/datahandling.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.011443 climix-0.18.1/climix/etc/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2300 2023-04-20 14:40:21.000000 climix-0.18.1/climix/etc/SMHI_extra.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5591 2023-04-20 14:40:21.000000 climix-0.18.1/climix/etc/climix_config.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)   107695 2023-04-21 14:07:50.000000 climix-0.18.1/climix/etc/index_definitions.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1846 2023-04-23 13:54:44.000000 climix-0.18.1/climix/etc/indices.md.jinja
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     6964 2023-04-20 14:40:21.000000 climix-0.18.1/climix/etc/metadata.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2350 2023-04-21 14:07:50.000000 climix-0.18.1/climix/etc/variables.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2449 2023-04-20 14:40:21.000000 climix-0.18.1/climix/index.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      941 2023-04-23 13:54:44.000000 climix-0.18.1/climix/index_docs.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.015443 climix-0.18.1/climix/index_functions/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      716 2023-04-19 14:56:21.000000 climix-0.18.1/climix/index_functions/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    21861 2023-04-19 14:56:21.000000 climix-0.18.1/climix/index_functions/index_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    18224 2023-04-20 14:40:21.000000 climix-0.18.1/climix/index_functions/percentile_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5197 2023-04-19 14:56:21.000000 climix-0.18.1/climix/index_functions/spell_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    11954 2023-04-19 14:56:21.000000 climix-0.18.1/climix/index_functions/spell_kernels.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     9543 2023-04-20 14:40:21.000000 climix-0.18.1/climix/index_functions/support.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     5426 2022-05-10 13:36:30.000000 climix-0.18.1/climix/iris.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    12582 2023-04-23 13:54:44.000000 climix-0.18.1/climix/main.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    17812 2023-04-23 13:54:44.000000 climix-0.18.1/climix/metadata.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4911 2023-03-14 14:27:51.000000 climix-0.18.1/climix/period.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.016443 climix-0.18.1/climix/util/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      435 2023-02-08 09:48:44.000000 climix-0.18.1/climix/util/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3949 2022-05-10 13:36:30.000000 climix-0.18.1/climix/util/change_pr_units.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    13809 2023-03-14 14:27:51.000000 climix-0.18.1/climix/util/cube_diffs.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.008443 climix-0.18.1/climix.egg-info/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1394 2023-04-25 13:31:04.000000 climix-0.18.1/climix.egg-info/PKG-INFO
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1728 2023-04-25 13:31:04.000000 climix-0.18.1/climix.egg-info/SOURCES.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        1 2023-04-25 13:31:04.000000 climix-0.18.1/climix.egg-info/dependency_links.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1531 2023-04-25 13:31:04.000000 climix-0.18.1/climix.egg-info/entry_points.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      231 2023-04-25 13:31:04.000000 climix-0.18.1/climix.egg-info/requires.txt
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        7 2023-04-25 13:31:04.000000 climix-0.18.1/climix.egg-info/top_level.txt
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.017444 climix-0.18.1/docs/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      585 2023-03-30 14:33:33.000000 climix-0.18.1/docs/Makefile
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      791 2019-07-03 09:39:58.000000 climix-0.18.1/docs/make.bat
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       71 2023-04-23 13:54:44.000000 climix-0.18.1/docs/requirements-docs.txt
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.018443 climix-0.18.1/docs/source/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3690 2023-04-25 13:26:33.000000 climix-0.18.1/docs/source/conf.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      188 2023-04-23 13:54:44.000000 climix-0.18.1/docs/source/index.md
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.018443 climix-0.18.1/docs/source/user/
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.019443 climix-0.18.1/docs/source/user/advanced/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      101 2023-04-23 13:54:44.000000 climix-0.18.1/docs/source/user/advanced/index.md
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.019443 climix-0.18.1/docs/source/user/basic/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2760 2023-04-23 13:54:44.000000 climix-0.18.1/docs/source/user/basic/index.md
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       79 2023-04-23 13:54:44.000000 climix-0.18.1/docs/source/user/index.md
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.020444 climix-0.18.1/docs/source/user/reference/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       58 2023-04-23 13:54:44.000000 climix-0.18.1/docs/source/user/reference/index.md
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)   121616 2023-04-23 13:54:44.000000 climix-0.18.1/docs/source/user/reference/indices.md
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      546 2023-04-20 14:40:21.000000 climix-0.18.1/environment.yml
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.021443 climix-0.18.1/jobscripts/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      485 2022-12-08 14:42:09.000000 climix-0.18.1/jobscripts/climix-mpi.sh
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3790 2022-12-08 14:42:09.000000 climix-0.18.1/jobscripts/climix.sh
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3208 2023-04-25 13:26:33.000000 climix-0.18.1/pyproject.toml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)       38 2023-04-25 13:31:05.028443 climix-0.18.1/setup.cfg
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.022443 climix-0.18.1/tests/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.1/tests/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     1130 2023-04-21 14:07:50.000000 climix-0.18.1/tests/conftest.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.023444 climix-0.18.1/tests/integration/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-21 14:07:50.000000 climix-0.18.1/tests/integration/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    10413 2023-04-21 14:07:50.000000 climix-0.18.1/tests/integration/configuration.yml
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)      779 2023-04-21 14:07:50.000000 climix-0.18.1/tests/integration/conftest.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     4158 2023-04-21 14:07:50.000000 climix-0.18.1/tests/integration/test_indices.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.024443 climix-0.18.1/tests/unit/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.1/tests/unit/__init__.py
+drwxrwxr-x   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-25 13:31:05.027444 climix-0.18.1/tests/unit/index_functions/
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)        0 2023-04-05 09:49:20.000000 climix-0.18.1/tests/unit/index_functions/__init__.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2370 2023-04-21 14:07:50.000000 climix-0.18.1/tests/unit/index_functions/conftest.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)    70106 2023-04-21 14:07:50.000000 climix-0.18.1/tests/unit/index_functions/test_index_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     3567 2023-03-14 14:27:51.000000 climix-0.18.1/tests/unit/index_functions/test_percentile_functions.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2353 2023-04-19 14:56:21.000000 climix-0.18.1/tests/unit/index_functions/test_support.py
+-rw-rw-r--   0 a002160  (66459) smhiprimgrp  (2000)     2043 2023-03-14 14:27:51.000000 climix-0.18.1/tests/unit/test_main.py
```

### Comparing `climix-0.18.0rc2/CHANGELOG.md` & `climix-0.18.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,33 @@
 ### Removed
 
 ### Fixed
 
 ### Security
 
 
-## [0.18.0rc2] - 2023-04-21
+## [0.18.1] - 2023-04-25
+
+### Changed
+- Improve readthedocs config
+
+### Fixed
+- Fix packaging (closes #312)
+
+
+## [0.18.0] - 2023-04-21
 
 ### Added
 - Reference period defined in Index_definition.yml and command line arg -r/-reference_period (fixes #273)
 - Adds global metadata configuration (fixes #36)
 - Adds unit tests for index functions(fixes #299)
 - Read Clix meta version and add information in cube output attribute (fixes #284)
 - Adding integration tests using a subset of indices in NGCD dataset (fixes #275)
 - Add Apache-2.0 license (closes #50)
+- Create basic documentation (closes #84, #287)
 
 ### Changed
 - Clix meta update to version 0.5.2 (fixes #306)
 - Update build config (Closes #304)
 
 
 ## [0.17.0] - 2023-03-10
@@ -426,16 +436,17 @@
 - Improved directory structure.
 
 ### Removed
 
 - Removed obsolete version.
 
 
-[unreleased]: https://git.smhi.se/climix/climix/compare/0.18.0rc2...HEAD
-[0.18.0rc2]: https://git.smhi.se/climix/climix/compare/0.17.0...0.18.0rc2
+[unreleased]: https://git.smhi.se/climix/climix/compare/0.18.1...HEAD
+[0.18.1]: https://git.smhi.se/climix/climix/compare/0.18.0...0.18.1
+[0.18.0]: https://git.smhi.se/climix/climix/compare/0.17.0...0.18.0
 [0.17.0]: https://git.smhi.se/climix/climix/compare/0.16.0...0.17.0
 [0.16.0]: https://git.smhi.se/climix/climix/compare/0.15.0...0.16.0
 [0.15.0]: https://git.smhi.se/climix/climix/compare/0.14.0...0.15.0
 [0.14.0]: https://git.smhi.se/climix/climix/compare/0.13.2...0.14.0
 [0.13.2]: https://git.smhi.se/climix/climix/compare/0.13.1...0.13.2
 [0.13.1]: https://git.smhi.se/climix/climix/compare/0.13.0...0.13.1
 [0.13.0]: https://git.smhi.se/climix/climix/compare/0.12.0...0.13.0
```

### Comparing `climix-0.18.0rc2/LICENSE` & `climix-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/PKG-INFO` & `climix-0.18.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climix
-Version: 0.18.0rc2
+Version: 0.18.1
 Summary: A climate index package
 Author-email: Lars Bärring <lars.barring@smhi.se>, Klaus Zimmermann <klaus.zimmermann@smhi.se>
 License: Apache-2.0
 Project-URL: Homepage, https://git.smhi.se/climix/climix
 Project-URL: Bug Reports, https://git.smhi.se/climix/climix/issues
 Project-URL: Source, https://git.smhi.se/climix/climix
 Classifier: Development Status :: 4 - Beta
@@ -16,34 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Climix
+# Climix—a climate index package
 
-A climate index thing.
+[![Documentation Status](https://readthedocs.org/projects/climix/badge/?version=latest)](https://climix.readthedocs.io/en/latest/?badge=latest)
+ [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+ ![PyPI](https://img.shields.io/pypi/v/climix)
+ ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/climix)
 
-## Reference Data
-
-We use [git-lfs](https://git-lfs.github.com/) to manage reference datasets. For
-this to work, you need to have git-lfs installed and setup.
-
-### Installing git-lfs
-
-You can install git-lfs with conda via
-```
-conda install git-lfs
-```
-or with yum via
-```
-sudo yum install git-lfs
-```
-
-### Setting up git-lfs
-
-For git-lfs to work, you also need to execute
-```
-git lfs install
-```
-This needs to be done only once after the installation.
+ For documentation, see the https://climix.readthedocs.io.
```

### Comparing `climix-0.18.0rc2/climix/aggregators.py` & `climix-0.18.1/climix/aggregators.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/dask_setup.py` & `climix-0.18.1/climix/dask_setup.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/dask_take_along_axis.py` & `climix-0.18.1/climix/dask_take_along_axis.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/datahandling.py` & `climix-0.18.1/climix/datahandling.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/etc/SMHI_extra.yml` & `climix-0.18.1/climix/etc/SMHI_extra.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/etc/climix_config.yml` & `climix-0.18.1/climix/etc/climix_config.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/etc/index_definitions.yml` & `climix-0.18.1/climix/etc/index_definitions.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/etc/metadata.yml` & `climix-0.18.1/climix/etc/metadata.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/etc/variables.yml` & `climix-0.18.1/climix/etc/variables.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index.py` & `climix-0.18.1/climix/index.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index_functions/__init__.py` & `climix-0.18.1/climix/index_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index_functions/index_functions.py` & `climix-0.18.1/climix/index_functions/index_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index_functions/percentile_functions.py` & `climix-0.18.1/climix/index_functions/percentile_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index_functions/spell_functions.py` & `climix-0.18.1/climix/index_functions/spell_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index_functions/spell_kernels.py` & `climix-0.18.1/climix/index_functions/spell_kernels.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/index_functions/support.py` & `climix-0.18.1/climix/index_functions/support.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/iris.py` & `climix-0.18.1/climix/iris.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/main.py` & `climix-0.18.1/climix/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "error": logging.ERROR,
     "critical": logging.CRITICAL,
 }
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
-        description=(f"A climate index thing, version {__version__}."),
+        description=(f"A climate index package, version {__version__}."),
         formatter_class=RawTextHelpFormatter,
     )
     parser.add_argument(
         "-l",
         "--log-level",
         choices=LOG_LEVELS.keys(),
         default="info",
```

### Comparing `climix-0.18.0rc2/climix/metadata.py` & `climix-0.18.1/climix/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 if sys.version_info[:2] >= (3, 10):
     # pylint: disable=no-name-in-module
     from importlib.metadata import entry_points
 else:
     from importlib_metadata import entry_points
 
 
-@dataclass
+@dataclass(eq=True, frozen=True)
 class Distribution:
     name: str
     version: str
 
 
 @dataclass
 class CellMethod:
```

### Comparing `climix-0.18.0rc2/climix/period.py` & `climix-0.18.1/climix/period.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/util/change_pr_units.py` & `climix-0.18.1/climix/util/change_pr_units.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix/util/cube_diffs.py` & `climix-0.18.1/climix/util/cube_diffs.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/climix.egg-info/PKG-INFO` & `climix-0.18.1/climix.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climix
-Version: 0.18.0rc2
+Version: 0.18.1
 Summary: A climate index package
 Author-email: Lars Bärring <lars.barring@smhi.se>, Klaus Zimmermann <klaus.zimmermann@smhi.se>
 License: Apache-2.0
 Project-URL: Homepage, https://git.smhi.se/climix/climix
 Project-URL: Bug Reports, https://git.smhi.se/climix/climix/issues
 Project-URL: Source, https://git.smhi.se/climix/climix
 Classifier: Development Status :: 4 - Beta
@@ -16,34 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Climix
+# Climix—a climate index package
 
-A climate index thing.
+[![Documentation Status](https://readthedocs.org/projects/climix/badge/?version=latest)](https://climix.readthedocs.io/en/latest/?badge=latest)
+ [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+ ![PyPI](https://img.shields.io/pypi/v/climix)
+ ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/climix)
 
-## Reference Data
-
-We use [git-lfs](https://git-lfs.github.com/) to manage reference datasets. For
-this to work, you need to have git-lfs installed and setup.
-
-### Installing git-lfs
-
-You can install git-lfs with conda via
-```
-conda install git-lfs
-```
-or with yum via
-```
-sudo yum install git-lfs
-```
-
-### Setting up git-lfs
-
-For git-lfs to work, you also need to execute
-```
-git lfs install
-```
-This needs to be done only once after the installation.
+ For documentation, see the https://climix.readthedocs.io.
```

### Comparing `climix-0.18.0rc2/climix.egg-info/SOURCES.txt` & `climix-0.18.1/climix.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+.readthedocs.yaml
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 environment.yml
 pyproject.toml
 climix/__init__.py
 climix/aggregators.py
 climix/dask_setup.py
 climix/dask_take_along_axis.py
 climix/datahandling.py
 climix/index.py
+climix/index_docs.py
 climix/iris.py
 climix/main.py
 climix/metadata.py
 climix/period.py
 climix.egg-info/PKG-INFO
 climix.egg-info/SOURCES.txt
 climix.egg-info/dependency_links.txt
 climix.egg-info/entry_points.txt
 climix.egg-info/requires.txt
 climix.egg-info/top_level.txt
 climix/etc/SMHI_extra.yml
 climix/etc/climix_config.yml
 climix/etc/index_definitions.yml
+climix/etc/indices.md.jinja
 climix/etc/metadata.yml
 climix/etc/variables.yml
 climix/index_functions/__init__.py
 climix/index_functions/index_functions.py
 climix/index_functions/percentile_functions.py
 climix/index_functions/spell_functions.py
 climix/index_functions/spell_kernels.py
@@ -34,15 +37,20 @@
 climix/util/__init__.py
 climix/util/change_pr_units.py
 climix/util/cube_diffs.py
 docs/Makefile
 docs/make.bat
 docs/requirements-docs.txt
 docs/source/conf.py
-docs/source/index.rst
+docs/source/index.md
+docs/source/user/index.md
+docs/source/user/advanced/index.md
+docs/source/user/basic/index.md
+docs/source/user/reference/index.md
+docs/source/user/reference/indices.md
 jobscripts/climix-mpi.sh
 jobscripts/climix.sh
 tests/__init__.py
 tests/conftest.py
 tests/integration/__init__.py
 tests/integration/configuration.yml
 tests/integration/conftest.py
```

### Comparing `climix-0.18.0rc2/climix.egg-info/entry_points.txt` & `climix-0.18.1/climix.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 temperature_sum = climix.index_functions:TemperatureSum
 thresholded_percentile = climix.index_functions:ThresholdedPercentile
 thresholded_running_statistics = climix.index_functions:ThresholdedRunningStatistics
 thresholded_statistics = climix.index_functions:ThresholdedStatistics
 
 [console_scripts]
 climix = climix.main:main
+climix-index-docs = climix.index_docs:main
```

### Comparing `climix-0.18.0rc2/docs/Makefile` & `climix-0.18.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/docs/make.bat` & `climix-0.18.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/docs/source/conf.py` & `climix-0.18.1/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,32 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 from importlib.metadata import version
+from pathlib import Path
 
-sys.path.insert(0, os.path.abspath(".."))
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+root = Path(__file__).absolute().parent.parent.parent
+sys.path.insert(0, str(root))
+
+# -- RTD configuration ------------------------------------------------
+
+# on_rtd is whether we are on readthedocs.org, this line of code grabbed from
+# docs.readthedocs.org
+on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+
+# This is used for linking and such so we link to the thing we're building
+rtd_version = os.environ.get("READTHEDOCS_VERSION", "latest")
+if rtd_version not in ["latest", "stable", "doc"]:
+    rtd_version = "latest"
 
 
 # -- Project information -----------------------------------------------------
 
 project = "Climix"
 copyright = "2019, Lars Bärring, Klaus Zimmermann"
 author = "Lars Bärring, Klaus Zimmermann"
@@ -35,36 +51,45 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.mathjax",
     "sphinx.ext.intersphinx",
     "sphinx.ext.autosummary",
     "sphinx.ext.extlinks",
     "sphinx.ext.napoleon",
+    "myst_parser",
+    "sphinx_toolbox.collapse",
 ]
 
+myst_enable_extensions = ["colon_fence"]
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_rtd_theme"
+# html_theme = "sphinx_rtd_theme"
+html_theme = "pydata_sphinx_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
+# html_static_path = ["_static"]
+
+html_sidebars = {
+    "**": ["search-field.html", "sidebar-nav-bs.html", "sidebar-ethical-ads.html"]
+}
 
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
```

### Comparing `climix-0.18.0rc2/environment.yml` & `climix-0.18.1/environment.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/jobscripts/climix.sh` & `climix-0.18.1/jobscripts/climix.sh`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/pyproject.toml` & `climix-0.18.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 [project.urls]
 Homepage = "https://git.smhi.se/climix/climix"
 "Bug Reports" = "https://git.smhi.se/climix/climix/issues"
 Source = "https://git.smhi.se/climix/climix"
 
 [project.scripts]
 climix = "climix.main:main"
+climix-index-docs = "climix.index_docs:main"
 
 [project.entry-points."climix.index_functions"]
 count_level_crossings = "climix.index_functions:CountLevelCrossings"
 count_occurrences = "climix.index_functions:CountOccurrences"
 count_percentile_occurrences = "climix.index_functions:CountPercentileOccurrences"
 count_thresholded_percentile_occurrences = "climix.index_functions:CountThresholdedPercentileOccurrences"
 count_joint_occurrences_precipitation_temperature = "climix.index_functions:CountJointOccurrencesPrecipitationTemperature"
@@ -75,17 +76,13 @@
 thresholded_percentile = "climix.index_functions:ThresholdedPercentile"
 thresholded_running_statistics = "climix.index_functions:ThresholdedRunningStatistics"
 thresholded_statistics = "climix.index_functions:ThresholdedStatistics"
 
 [tool.setuptools_scm]
 version_scheme = "release-branch-semver"
 
-[tool.setuptools]
-include-package-data = false
-
 [tool.setuptools.packages.find]
-exclude = ["data"] # legacy
-namespaces = false
+include = ["climix*"]
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 testpaths = "tests"
```

### Comparing `climix-0.18.0rc2/tests/conftest.py` & `climix-0.18.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/integration/configuration.yml` & `climix-0.18.1/tests/integration/configuration.yml`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/integration/conftest.py` & `climix-0.18.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/integration/test_indices.py` & `climix-0.18.1/tests/integration/test_indices.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/unit/index_functions/conftest.py` & `climix-0.18.1/tests/unit/index_functions/conftest.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/unit/index_functions/test_index_functions.py` & `climix-0.18.1/tests/unit/index_functions/test_index_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/unit/index_functions/test_percentile_functions.py` & `climix-0.18.1/tests/unit/index_functions/test_percentile_functions.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/unit/index_functions/test_support.py` & `climix-0.18.1/tests/unit/index_functions/test_support.py`

 * *Files identical despite different names*

### Comparing `climix-0.18.0rc2/tests/unit/test_main.py` & `climix-0.18.1/tests/unit/test_main.py`

 * *Files identical despite different names*

