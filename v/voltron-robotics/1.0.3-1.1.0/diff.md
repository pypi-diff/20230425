# Comparing `tmp/voltron-robotics-1.0.3.tar.gz` & `tmp/voltron-robotics-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltron-robotics-1.0.3.tar", last modified: Wed Apr  5 12:47:18 2023, max compression
+gzip compressed data, was "voltron-robotics-1.1.0.tar", last modified: Tue Apr 25 08:57:44 2023, max compression
```

## Comparing `voltron-robotics-1.0.3.tar` & `voltron-robotics-1.1.0.tar`

### file list

```diff
@@ -1,60 +1,80 @@
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.918933 voltron-robotics-1.0.3/
--rw-r--r--   0 sidd       (501) staff       (20)     1110 2023-02-27 07:13:40.000000 voltron-robotics-1.0.3/LICENSE
--rw-r--r--   0 sidd       (501) staff       (20)    10757 2023-04-05 12:47:18.918232 voltron-robotics-1.0.3/PKG-INFO
--rw-r--r--   0 sidd       (501) staff       (20)     8271 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/README.md
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.885396 voltron-robotics-1.0.3/examples/
--rw-r--r--   0 sidd       (501) staff       (20)     1775 2023-02-27 06:13:31.000000 voltron-robotics-1.0.3/examples/adapt.py
--rw-r--r--   0 sidd       (501) staff       (20)     2691 2023-02-27 06:13:31.000000 voltron-robotics-1.0.3/examples/verify.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.887274 voltron-robotics-1.0.3/examples/xla-reference/
--rw-r--r--   0 sidd       (501) staff       (20)     3508 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/examples/xla-reference/xpreprocess.py
--rw-r--r--   0 sidd       (501) staff       (20)    37964 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/examples/xla-reference/xpretrain.py
--rw-r--r--   0 sidd       (501) staff       (20)     2038 2023-04-05 12:46:33.000000 voltron-robotics-1.0.3/pyproject.toml
--rw-r--r--   0 sidd       (501) staff       (20)       38 2023-04-05 12:47:18.919100 voltron-robotics-1.0.3/setup.cfg
--rw-r--r--   0 sidd       (501) staff       (20)      187 2023-02-27 07:20:54.000000 voltron-robotics-1.0.3/setup.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.888605 voltron-robotics-1.0.3/voltron/
--rw-r--r--   0 sidd       (501) staff       (20)      102 2023-02-27 07:21:53.000000 voltron-robotics-1.0.3/voltron/__init__.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.891900 voltron-robotics-1.0.3/voltron/conf/
--rw-r--r--   0 sidd       (501) staff       (20)      149 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/conf/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)     1267 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/conf/accelerators.py
--rw-r--r--   0 sidd       (501) staff       (20)     2781 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/conf/datasets.py
--rw-r--r--   0 sidd       (501) staff       (20)    11947 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/conf/models.py
--rw-r--r--   0 sidd       (501) staff       (20)     1641 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/conf/tracking.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.893522 voltron-robotics-1.0.3/voltron/models/
--rw-r--r--   0 sidd       (501) staff       (20)      201 2023-02-27 07:22:13.000000 voltron-robotics-1.0.3/voltron/models/__init__.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.896790 voltron-robotics-1.0.3/voltron/models/core/
--rw-r--r--   0 sidd       (501) staff       (20)        0 2023-02-27 07:22:17.000000 voltron-robotics-1.0.3/voltron/models/core/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)    20832 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/core/vcond.py
--rw-r--r--   0 sidd       (501) staff       (20)    24483 2023-03-20 01:08:54.000000 voltron-robotics-1.0.3/voltron/models/core/vdual.py
--rw-r--r--   0 sidd       (501) staff       (20)    36705 2023-04-05 12:45:54.000000 voltron-robotics-1.0.3/voltron/models/core/vgen.py
--rw-r--r--   0 sidd       (501) staff       (20)     5380 2023-04-05 12:45:54.000000 voltron-robotics-1.0.3/voltron/models/materialize.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.899806 voltron-robotics-1.0.3/voltron/models/reproductions/
--rw-r--r--   0 sidd       (501) staff       (20)        0 2023-02-27 07:24:34.000000 voltron-robotics-1.0.3/voltron/models/reproductions/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)    15924 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/reproductions/vmvp.py
--rw-r--r--   0 sidd       (501) staff       (20)    17436 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/reproductions/vr3m.py
--rw-r--r--   0 sidd       (501) staff       (20)    13930 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/reproductions/vrn3m.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.903645 voltron-robotics-1.0.3/voltron/models/util/
--rw-r--r--   0 sidd       (501) staff       (20)       46 2023-02-27 07:23:32.000000 voltron-robotics-1.0.3/voltron/models/util/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)     4095 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/util/extraction.py
--rw-r--r--   0 sidd       (501) staff       (20)     1994 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/util/optimization.py
--rw-r--r--   0 sidd       (501) staff       (20)     8787 2023-02-27 07:25:25.000000 voltron-robotics-1.0.3/voltron/models/util/transformer.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.905298 voltron-robotics-1.0.3/voltron/overwatch/
--rw-r--r--   0 sidd       (501) staff       (20)       37 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/overwatch/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)     2209 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/overwatch/overwatch.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.909944 voltron-robotics-1.0.3/voltron/preprocessing/
--rw-r--r--   0 sidd       (501) staff       (20)      100 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/preprocessing/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)    15035 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/preprocessing/process.py
--rw-r--r--   0 sidd       (501) staff       (20)    40177 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/preprocessing/stream_datasets.py
--rw-r--r--   0 sidd       (501) staff       (20)     2988 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/preprocessing/transforms.py
--rw-r--r--   0 sidd       (501) staff       (20)     9080 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/preprocessing/utils.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.913417 voltron-robotics-1.0.3/voltron/util/
--rw-r--r--   0 sidd       (501) staff       (20)       85 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/util/__init__.py
--rw-r--r--   0 sidd       (501) staff       (20)     4807 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/util/checkpointing.py
--rw-r--r--   0 sidd       (501) staff       (20)     3405 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/util/distributed.py
--rw-r--r--   0 sidd       (501) staff       (20)     3009 2023-03-06 12:35:53.000000 voltron-robotics-1.0.3/voltron/util/random.py
--rw-r--r--   0 sidd       (501) staff       (20)    11056 2023-03-07 01:39:00.000000 voltron-robotics-1.0.3/voltron/util/xla_logger.py
-drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-05 12:47:18.917334 voltron-robotics-1.0.3/voltron_robotics.egg-info/
--rw-r--r--   0 sidd       (501) staff       (20)    10757 2023-04-05 12:47:18.000000 voltron-robotics-1.0.3/voltron_robotics.egg-info/PKG-INFO
--rw-r--r--   0 sidd       (501) staff       (20)     1332 2023-04-05 12:47:18.000000 voltron-robotics-1.0.3/voltron_robotics.egg-info/SOURCES.txt
--rw-r--r--   0 sidd       (501) staff       (20)        1 2023-04-05 12:47:18.000000 voltron-robotics-1.0.3/voltron_robotics.egg-info/dependency_links.txt
--rw-r--r--   0 sidd       (501) staff       (20)      201 2023-04-05 12:47:18.000000 voltron-robotics-1.0.3/voltron_robotics.egg-info/requires.txt
--rw-r--r--   0 sidd       (501) staff       (20)       33 2023-04-05 12:47:18.000000 voltron-robotics-1.0.3/voltron_robotics.egg-info/top_level.txt
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.395447 voltron-robotics-1.1.0/
+-rw-r--r--   0 sidd       (501) staff       (20)     1110 2023-02-27 07:13:40.000000 voltron-robotics-1.1.0/LICENSE
+-rw-r--r--   0 sidd       (501) staff       (20)    10815 2023-04-25 08:57:44.394560 voltron-robotics-1.1.0/PKG-INFO
+-rw-r--r--   0 sidd       (501) staff       (20)     8329 2023-04-25 08:54:57.000000 voltron-robotics-1.1.0/README.md
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.358345 voltron-robotics-1.1.0/examples/
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.359406 voltron-robotics-1.1.0/examples/pretrain/
+-rw-r--r--   0 sidd       (501) staff       (20)     3397 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/examples/pretrain/preprocess.py
+-rw-r--r--   0 sidd       (501) staff       (20)    18533 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/examples/pretrain/pretrain.py
+-rw-r--r--   0 sidd       (501) staff       (20)     1856 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/examples/usage.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.359928 voltron-robotics-1.1.0/examples/verification/
+-rw-r--r--   0 sidd       (501) staff       (20)     2795 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/examples/verification/verify.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.360932 voltron-robotics-1.1.0/examples/xla-reference/
+-rw-r--r--   0 sidd       (501) staff       (20)     3472 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/examples/xla-reference/xpreprocess.py
+-rw-r--r--   0 sidd       (501) staff       (20)    38007 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/examples/xla-reference/xpretrain.py
+-rw-r--r--   0 sidd       (501) staff       (20)     2127 2023-04-25 08:51:42.000000 voltron-robotics-1.1.0/pyproject.toml
+-rw-r--r--   0 sidd       (501) staff       (20)       38 2023-04-25 08:57:44.395597 voltron-robotics-1.1.0/setup.cfg
+-rw-r--r--   0 sidd       (501) staff       (20)      187 2023-02-27 07:20:54.000000 voltron-robotics-1.1.0/setup.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.361513 voltron-robotics-1.1.0/voltron/
+-rw-r--r--   0 sidd       (501) staff       (20)      102 2023-02-27 07:21:53.000000 voltron-robotics-1.1.0/voltron/__init__.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.364334 voltron-robotics-1.1.0/voltron/conf/
+-rw-r--r--   0 sidd       (501) staff       (20)      149 2023-03-07 01:39:00.000000 voltron-robotics-1.1.0/voltron/conf/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)     1798 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/conf/accelerators.py
+-rw-r--r--   0 sidd       (501) staff       (20)     3095 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/conf/datasets.py
+-rw-r--r--   0 sidd       (501) staff       (20)    14747 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/conf/models.py
+-rw-r--r--   0 sidd       (501) staff       (20)     1772 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/conf/tracking.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.365213 voltron-robotics-1.1.0/voltron/datasets/
+-rw-r--r--   0 sidd       (501) staff       (20)       35 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/datasets/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)    15867 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/datasets/datasets.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.365951 voltron-robotics-1.1.0/voltron/datasets/v1/
+-rw-r--r--   0 sidd       (501) staff       (20)        0 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/datasets/v1/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)    40177 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/datasets/v1/stream_datasets.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.367296 voltron-robotics-1.1.0/voltron/models/
+-rw-r--r--   0 sidd       (501) staff       (20)       84 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/models/__init__.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.369032 voltron-robotics-1.1.0/voltron/models/core/
+-rw-r--r--   0 sidd       (501) staff       (20)        0 2023-02-27 07:22:17.000000 voltron-robotics-1.1.0/voltron/models/core/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)    22688 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/models/core/vcond.py
+-rw-r--r--   0 sidd       (501) staff       (20)    27404 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/models/core/vdual.py
+-rw-r--r--   0 sidd       (501) staff       (20)    40463 2023-04-25 08:51:25.000000 voltron-robotics-1.1.0/voltron/models/core/vgen.py
+-rw-r--r--   0 sidd       (501) staff       (20)     7301 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/models/instantiate.py
+-rw-r--r--   0 sidd       (501) staff       (20)     5380 2023-04-05 12:45:54.000000 voltron-robotics-1.1.0/voltron/models/materialize.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.371656 voltron-robotics-1.1.0/voltron/models/reproductions/
+-rw-r--r--   0 sidd       (501) staff       (20)        0 2023-02-27 07:24:34.000000 voltron-robotics-1.1.0/voltron/models/reproductions/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)    15788 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/models/reproductions/vmvp.py
+-rw-r--r--   0 sidd       (501) staff       (20)    17436 2023-02-27 07:25:25.000000 voltron-robotics-1.1.0/voltron/models/reproductions/vr3m.py
+-rw-r--r--   0 sidd       (501) staff       (20)    13930 2023-02-27 07:25:25.000000 voltron-robotics-1.1.0/voltron/models/reproductions/vrn3m.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.374392 voltron-robotics-1.1.0/voltron/models/util/
+-rw-r--r--   0 sidd       (501) staff       (20)       46 2023-02-27 07:23:32.000000 voltron-robotics-1.1.0/voltron/models/util/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)     4095 2023-02-27 07:25:25.000000 voltron-robotics-1.1.0/voltron/models/util/extraction.py
+-rw-r--r--   0 sidd       (501) staff       (20)     1994 2023-02-27 07:25:25.000000 voltron-robotics-1.1.0/voltron/models/util/optimization.py
+-rw-r--r--   0 sidd       (501) staff       (20)     8787 2023-02-27 07:25:25.000000 voltron-robotics-1.1.0/voltron/models/util/transformer.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.375958 voltron-robotics-1.1.0/voltron/overwatch/
+-rw-r--r--   0 sidd       (501) staff       (20)       37 2023-03-06 12:35:53.000000 voltron-robotics-1.1.0/voltron/overwatch/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)     2207 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/overwatch/overwatch.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.377536 voltron-robotics-1.1.0/voltron/preprocessing/
+-rw-r--r--   0 sidd       (501) staff       (20)       72 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)    10603 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/core.py
+-rw-r--r--   0 sidd       (501) staff       (20)    12749 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/process.py
+-rw-r--r--   0 sidd       (501) staff       (20)     2944 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/transforms.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.384422 voltron-robotics-1.1.0/voltron/preprocessing/v1/
+-rw-r--r--   0 sidd       (501) staff       (20)      100 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/v1/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)    15156 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/v1/process.py
+-rw-r--r--   0 sidd       (501) staff       (20)     2990 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/v1/transforms.py
+-rw-r--r--   0 sidd       (501) staff       (20)     9083 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/preprocessing/v1/utils.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.387002 voltron-robotics-1.1.0/voltron/util/
+-rw-r--r--   0 sidd       (501) staff       (20)      152 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)     7070 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/checkpointing.py
+-rw-r--r--   0 sidd       (501) staff       (20)    15408 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/metrics.py
+-rw-r--r--   0 sidd       (501) staff       (20)     5698 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/utilities.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.389871 voltron-robotics-1.1.0/voltron/util/v1/
+-rw-r--r--   0 sidd       (501) staff       (20)        0 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/v1/__init__.py
+-rw-r--r--   0 sidd       (501) staff       (20)     4561 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/v1/checkpointing.py
+-rw-r--r--   0 sidd       (501) staff       (20)     3405 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/v1/distributed.py
+-rw-r--r--   0 sidd       (501) staff       (20)     3012 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/v1/random.py
+-rw-r--r--   0 sidd       (501) staff       (20)    11056 2023-04-25 08:50:27.000000 voltron-robotics-1.1.0/voltron/util/v1/xla_logger.py
+drwxr-xr-x   0 sidd       (501) staff       (20)        0 2023-04-25 08:57:44.393433 voltron-robotics-1.1.0/voltron_robotics.egg-info/
+-rw-r--r--   0 sidd       (501) staff       (20)    10815 2023-04-25 08:57:44.000000 voltron-robotics-1.1.0/voltron_robotics.egg-info/PKG-INFO
+-rw-r--r--   0 sidd       (501) staff       (20)     1790 2023-04-25 08:57:44.000000 voltron-robotics-1.1.0/voltron_robotics.egg-info/SOURCES.txt
+-rw-r--r--   0 sidd       (501) staff       (20)        1 2023-04-25 08:57:44.000000 voltron-robotics-1.1.0/voltron_robotics.egg-info/dependency_links.txt
+-rw-r--r--   0 sidd       (501) staff       (20)      217 2023-04-25 08:57:44.000000 voltron-robotics-1.1.0/voltron_robotics.egg-info/requires.txt
+-rw-r--r--   0 sidd       (501) staff       (20)       33 2023-04-25 08:57:44.000000 voltron-robotics-1.1.0/voltron_robotics.egg-info/top_level.txt
```

### Comparing `voltron-robotics-1.0.3/LICENSE` & `voltron-robotics-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/PKG-INFO` & `voltron-robotics-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltron-robotics
-Version: 1.0.3
+Version: 1.1.0
 Summary: Voltron: Language-Driven Representation Learning for Robotics.
 Author-email: Siddharth Karamcheti <skaramcheti@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2021-present, Siddharth Karamcheti and other contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 <div align="center">
     <img src="https://raw.githubusercontent.com/siddk/voltron-robotics/main/docs/assets/voltron-banner.png" alt="Voltron Logo"/>
 </div>
 
 <div align="center">
 
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12766-df2a2a.svg?style=for-the-badge)](https://arxiv.org/abs/2302.12766)
-[![PyTorch](https://img.shields.io/badge/PyTorch-1.12.0-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org/get-started/previous-versions/#v1120)
+[![PyTorch](https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org/get-started/locally/)
 [![Code Style: Black](https://img.shields.io/badge/Code%20Style-Black-000000?style=for-the-badge)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/badge/%E2%9A%A1%EF%B8%8F-Ruff-orange?style=for-the-badge)](https://github.com/charliermarsh/ruff)
 ![License](https://img.shields.io/github/license/siddk/lila?color=blueviolet&style=for-the-badge)
 
 </div>
 
 ---
@@ -73,16 +73,16 @@
 ## Quickstart
 
 This repository is built with PyTorch; while specified as a dependency for the package, we highly recommend that
 you install the desired version (e.g., with accelerator support) for your given hardware and environment
 manager (e.g., `conda`).
 
 PyTorch installation instructions [can be found here](https://pytorch.org/get-started/locally/). This repository
-should work with PyTorch >= 1.12, but has only been thoroughly tested with PyTorch 1.12.0, Torchvision 0.13.0,
-Torchaudio 0.12.0.
+should work with PyTorch >= 1.12. Releases before 1.1.0 have been thoroughly tested with PyTorch 1.12.0,
+Torchvision 0.13.0, and Torchaudio 0.12.0. **Note**: Releases 1.1.0 and after *assume PyTorch 2.0*!
 
 Once PyTorch has been properly installed, you can install this package via PyPI, and you're off!
 
 ```bash
 pip install voltron-robotics
 ```
 
@@ -168,15 +168,15 @@
 language embeddings, or only the image patch embeddings.
 
 **Note:** For the API for the non-Voltron models (e.g., R-MVP, R-R3M), take a look at
 [`examples/verify.py`](examples/verify.py); this file shows how representations from *every* model can be extracted.
 
 ### Adaptation
 
-See [`examples/adapt.py`](examples/adapt.py) and the [`voltron-evaluation`](https://github.com/siddk/voltron-evaluation)
+See [`examples/usage.py`](examples/usage.py) and the [`voltron-evaluation`](https://github.com/siddk/voltron-evaluation)
 repository for more examples on the various ways to adapt/use Voltron representations.
 
 ---
 
 ## Contributing
 
 Before committing to the repository, make sure to set up your dev environment!
```

### Comparing `voltron-robotics-1.0.3/README.md` & `voltron-robotics-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="center">
     <img src="https://raw.githubusercontent.com/siddk/voltron-robotics/main/docs/assets/voltron-banner.png" alt="Voltron Logo"/>
 </div>
 
 <div align="center">
 
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12766-df2a2a.svg?style=for-the-badge)](https://arxiv.org/abs/2302.12766)
-[![PyTorch](https://img.shields.io/badge/PyTorch-1.12.0-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org/get-started/previous-versions/#v1120)
+[![PyTorch](https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org/get-started/locally/)
 [![Code Style: Black](https://img.shields.io/badge/Code%20Style-Black-000000?style=for-the-badge)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/badge/%E2%9A%A1%EF%B8%8F-Ruff-orange?style=for-the-badge)](https://github.com/charliermarsh/ruff)
 ![License](https://img.shields.io/github/license/siddk/lila?color=blueviolet&style=for-the-badge)
 
 </div>
 
 ---
@@ -25,16 +25,16 @@
 ## Quickstart
 
 This repository is built with PyTorch; while specified as a dependency for the package, we highly recommend that
 you install the desired version (e.g., with accelerator support) for your given hardware and environment
 manager (e.g., `conda`).
 
 PyTorch installation instructions [can be found here](https://pytorch.org/get-started/locally/). This repository
-should work with PyTorch >= 1.12, but has only been thoroughly tested with PyTorch 1.12.0, Torchvision 0.13.0,
-Torchaudio 0.12.0.
+should work with PyTorch >= 1.12. Releases before 1.1.0 have been thoroughly tested with PyTorch 1.12.0,
+Torchvision 0.13.0, and Torchaudio 0.12.0. **Note**: Releases 1.1.0 and after *assume PyTorch 2.0*!
 
 Once PyTorch has been properly installed, you can install this package via PyPI, and you're off!
 
 ```bash
 pip install voltron-robotics
 ```
 
@@ -120,15 +120,15 @@
 language embeddings, or only the image patch embeddings.
 
 **Note:** For the API for the non-Voltron models (e.g., R-MVP, R-R3M), take a look at
 [`examples/verify.py`](examples/verify.py); this file shows how representations from *every* model can be extracted.
 
 ### Adaptation
 
-See [`examples/adapt.py`](examples/adapt.py) and the [`voltron-evaluation`](https://github.com/siddk/voltron-evaluation)
+See [`examples/usage.py`](examples/usage.py) and the [`voltron-evaluation`](https://github.com/siddk/voltron-evaluation)
 repository for more examples on the various ways to adapt/use Voltron representations.
 
 ---
 
 ## Contributing
 
 Before committing to the repository, make sure to set up your dev environment!
```

### Comparing `voltron-robotics-1.0.3/examples/adapt.py` & `voltron-robotics-1.1.0/examples/usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
-adapt.py
+usage.py
 
 Example script demonstrating how to load a Voltron model (`V-Cond`) and instantiate a Multiheaded Attention Pooling
 extractor head for downstream tasks.
 
 This is the basic formula/protocol for using Voltron for arbitrary downstream applications.
+
+Run with (from root of repository): `python examples/usage.py`
 """
 import torch
 from torchvision.io import read_image
 
 from voltron import instantiate_extractor, load
 
 
-def adapt() -> None:
-    print("[*] Running `adapt` => Demonstrating Voltron for Various Adaptation Applications")
+def usage() -> None:
+    print("[*] Demonstrating Voltron Usage for Various Adaptation Applications")
 
     # Get `torch.device` for loading model (note -- we'll load weights directly onto device!)
     device = "cuda" if torch.cuda.is_available() else "cpu"
 
     # Load Voltron model --> specify `freeze`, `device` and get model (nn.Module) and preprocessor
     vcond, preprocess = load("v-cond", device=device, freeze=True)
 
@@ -27,17 +29,17 @@
 
     # Get various representations...
     with torch.no_grad():
         multimodal_features = vcond(img, lang, mode="multimodal")  # Fused vision & language features
         visual_features = vcond(img, mode="visual")  # Vision-only features (no language)
 
     # Can instantiate various extractors for downstream applications
-    vector_extractor = instantiate_extractor(vcond, n_latents=1)()
-    seq_extractor = instantiate_extractor(vcond, n_latents=64)()
+    vector_extractor = instantiate_extractor(vcond, n_latents=1, device=device)()
+    seq_extractor = instantiate_extractor(vcond, n_latents=64, device=device)()
 
     # Assertions...
     assert list(vector_extractor(multimodal_features).shape) == [1, vcond.embed_dim], "Should return a dense vector!"
     assert list(seq_extractor(visual_features).shape) == [1, 64, vcond.embed_dim], "Should return a sequence!"
 
 
 if __name__ == "__main__":
-    adapt()
+    usage()
```

### Comparing `voltron-robotics-1.0.3/examples/verify.py` & `voltron-robotics-1.1.0/examples/verification/verify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 verify.py
 
 Example script demonstrating how to load all Voltron models (and reproduced models), take input image(s), and get the
 various (e.g., multimodal, image-only) representations.
 
 Also serves to verify that representation loading is working as advertised.
+
+Run with (from root of repository): `python examples/verification/verify.py`
 """
 import torch
 from torchvision.io import read_image
 
 from voltron import load
 
 # Available Models
 MODELS = ["v-cond", "v-dual", "v-gen", "r-mvp", "r-r3m-vit", "r-r3m-rn50"]
 
 # Sample Inputs
-IMG_A, IMG_B = "examples/img/peel-carrot-initial.png", "examples/img/peel-carrot-final.png"
+IMG_A, IMG_B = "examples/verification/img/peel-carrot-initial.png", "examples/verification/img/peel-carrot-final.png"
 LANGUAGE = "peeling a carrot"
 
 
 def verify() -> None:
     print("[*] Running `verify` =>> Verifying Model Representations!")
 
     # Read both images (we'll use the second image for the dual-frame models)
```

### Comparing `voltron-robotics-1.0.3/examples/xla-reference/xpreprocess.py` & `voltron-robotics-1.1.0/examples/xla-reference/xpreprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 xpreprocess.py
 
 Centralized script for preprocessing Sth-Sth-v2 for TPU/GCP pretraining, using a multi-stage, multiprocessing strategy.
 
-Mean to run as a standalone script, *prior* to calling `xpretrain.py` =>> mostly because we want to preprocess the data
+Run as a standalone script, *prior* to calling `xpretrain.py` =>> mostly because we want to preprocess the data
 once, as a fixed cost.
 """
 import logging
 from dataclasses import dataclass, field
 from typing import Any, Dict, List
 
 import hydra
 from hydra.core.config_store import ConfigStore
 from omegaconf import MISSING
 
 from voltron.conf import DatasetConfig
 from voltron.overwatch import OverwatchRich
-from voltron.preprocessing import index, jsonify_language, preprocess_language, preprocess_videos, unify_batches
-from voltron.util import set_global_seed
+from voltron.preprocessing.v1 import index, jsonify_language, preprocess_language, preprocess_videos, unify_batches
+from voltron.util.v1.random import set_global_seed
 
 # Grab Logger
 overwatch = logging.getLogger(__file__)
 
 
 # Set Defaults (Hydra w/ Structured Configs)
 DEFAULTS = ["_self_", {"dataset": "sth-sth-v2"}, {"override hydra/job_logging": "overwatch_rich"}]
@@ -42,15 +42,15 @@
     # Composable / Structured Arguments
     dataset: DatasetConfig = MISSING                # Dataset(s) for pretraining/preprocessing
     # fmt: on
 
 
 # Hydra Setup :: Retrieve ConfigStore (Singleton) & Register Components
 cs = ConfigStore.instance()
-cs.store(group="hydra/job_logging", name="overwatch_rich", node=OverwatchRich)  # Annoying - configure logger for Hydra
+cs.store(group="hydra/job_logging", name="overwatch_rich", node=OverwatchRich)
 cs.store(name="config", node=PreprocessingConfig)
 
 
 @hydra.main(config_path=None, config_name="config")
 def xpreprocess(cfg: PreprocessingConfig) -> None:
     overwatch.info("Preprocessing :: Running Phases for Frame Extraction, Language Compilation, and Batching...")
```

### Comparing `voltron-robotics-1.0.3/examples/xla-reference/xpretrain.py` & `voltron-robotics-1.1.0/examples/xla-reference/xpretrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 xpretrain.py
 
 (The `x` prefix indicates this is a script geared for XLA/TPU backends *only*)!
 
-Reference script for PyTorch XLA (TPU-based) pretraining on the non-Qualcomm version of Sth-Sth-v2; this is
+Reference script for PyTorch XLA (TPU-based) pretraining on the Something-Something-v2 dataset; this is
 mostly for completeness =>> the hope is that the regular `pretrain.py` script is more general and maintained.
 
 Focuses on multi-TPU (XLA) training --> but also supports single-core TPU training, as the default distributed mp.spawn
 behavior just collapses into a single thread! Loads and preprocesses dataset, instantiates a model, and runs training.
 
-Run with `python xpretrain.py` (will by default use the configuration specified by `DEFAULTS` below).
+Run with `python examples/xla-reference/xpretrain.py` (will use the configuration specified by `DEFAULTS` below).
 """
 import os
 import re
 import time
 from collections import deque
 from dataclasses import dataclass, field
 from datetime import datetime
@@ -30,21 +30,21 @@
 import wandb
 from hydra.core.config_store import ConfigStore
 from omegaconf import MISSING, OmegaConf
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from voltron.conf import AcceleratorConfig, DatasetConfig, ModelConfig, TrackingConfig
+from voltron.datasets.v1.stream_datasets import get_epoch_datasets
 from voltron.models import VMVP, VR3M, VRN3M, VCond, VDual, VGen
 from voltron.overwatch import OverwatchRich
-from voltron.preprocessing.stream_datasets import get_epoch_datasets
-from voltron.util import set_global_seed
-from voltron.util.checkpointing import CheckpointSaver
-from voltron.util.distributed import ResumeableDistributedSampler
-from voltron.util.xla_logger import (
+from voltron.util.v1.checkpointing import XLACheckpointSaver
+from voltron.util.v1.distributed import ResumeableDistributedSampler
+from voltron.util.v1.random import set_global_seed
+from voltron.util.v1.xla_logger import (
     log_epoch_end_update,
     log_vcond_train_update,
     log_vdual_train_update,
     log_vgen_train_update,
     log_vmvp_train_update,
     log_vr3m_train_update,
     log_vrn3m_train_update,
@@ -373,15 +373,15 @@
         # Initialize Weights & Biases
         xm.master_print(f"W&B Resume is {cfg.resume} w/ W&B Resume ID = {wandb_resume_id}!")
         wandb.init(
             project=cfg.tracking.project,
             entity=cfg.tracking.entity,
             config=cfg,
             name=run_id,
-            dir=f"{os.getcwd()}" if cfg.tracking.dir is None else cfg.tracking.dir,
+            dir=f"{os.getcwd()}" if cfg.tracking.directory is None else cfg.tracking.directory,
             tags=tags,
             notes=cfg.tracking.notes,
             resume="allow" if start_checkpoint is not None else False,
             id=wandb_resume_id,
             # Weird line because PT-TPU VMs don't come with a working install of Tensorflow...
             settings=wandb.Settings(_disable_stats=True),
         )
@@ -442,15 +442,15 @@
         reconstruction_losses, lm_losses, lm_ppl = deque(maxlen=128), deque(maxlen=128), deque(maxlen=128)
         zero_reconstruction, k_reconstruction = deque(maxlen=128), deque(maxlen=128)
 
     else:
         raise NotImplementedError(f"Trackers for Model `{cfg.model.arch}` not implemented!")
 
     # 0th Checkpoint - Pull out optimizer state explicitly (`groups` are not serializable & can easily be replicated)
-    saver = CheckpointSaver(cfg.tracking.checkpoint_strategy, run_dir, cfg.accelerator.accelerator)
+    saver = XLACheckpointSaver(cfg.tracking.checkpoint_strategy, run_dir, cfg.accelerator.accelerator)
     if start_checkpoint is None and start_epoch == 0:
         xm.master_print("Saving 0th Epoch Checkpoint...")
         saver.save(
             epoch=0, is_local_step=False, model=model, optimizer=optimizer, duration=0, train_loss=None, val_loss=None
         )
 
     # Run on all processes --> retrieve "0th epoch" dataset!
```

### Comparing `voltron-robotics-1.0.3/pyproject.toml` & `voltron-robotics-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "voltron-robotics"
 authors = [
     {name = "Siddharth Karamcheti", email="skaramcheti@cs.stanford.edu"}
 ]
 description = "Voltron: Language-Driven Representation Learning for Robotics."
-version = "1.0.3"
+version = "1.1.0"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["robotics", "representation learning", "natural language processing", "machine learning"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -25,26 +25,27 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "av",
+    "einops",
     "gdown",
     "google-cloud-storage",
-    "einops",
+    "h5py",
     "hurry.filesize",
-    "hydra-core==1.1.1", # Lock Hydra =>> future versions break...
+    "hydra-core==1.1.1",    # Lock Hydra =>> future versions break!
     "jsonlines",
-    "omegaconf==2.1.2",  # Lock OmegaConf =>> future versions break...
+    "omegaconf==2.1.2",     # Lock OmegaConf =>> future versions break!
     "opencv-python",
+    "pandas",
     "rich",
-    "torch",
-    "torchvision",
-    "torchaudio",
+    "torch>=2.0.0",         # Native PyTorch Code (Release 2.0.0) uses PyTorch 2.0!
+    "torchvision>=0.15.0",
     "transformers",
     "wandb",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
```

### Comparing `voltron-robotics-1.0.3/voltron/conf/accelerators.py` & `voltron-robotics-1.1.0/voltron/conf/accelerators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 accelerator.py
 
 Base Hydra Structured Configs for defining various accelerator schemes. Uses a simple single inheritance structure.
 """
+import os
 from dataclasses import dataclass
 
 from hydra.core.config_store import ConfigStore
 from omegaconf import MISSING
 
+# === Vanilla Accelerators (Deprecated; mostly for XLA code) ===
+
 
 @dataclass
 class AcceleratorConfig:
     accelerator: str = MISSING
     num_accelerators: int = MISSING
     num_workers: int = MISSING
 
@@ -40,13 +43,26 @@
 @dataclass
 class TPUv3EightConfig(AcceleratorConfig):
     accelerator = "tpu"
     num_accelerators = 8
     num_workers = 8
 
 
+# === GPU Default Config --> just set `num_workers`; `torchrun` takes care of the rest! ===
+#   > Note :: Defaults to 1 GPU if WORLD_SIZE not set (e.g., not running with `torchrun`)
+
+
+@dataclass
+class TorchRunDefaultConfig(AcceleratorConfig):
+    accelerator = "gpu"
+    num_accelerators = int(os.environ["WORLD_SIZE"] if "WORLD_SIZE" in os.environ else 1)
+    num_workers = 8
+
+
 # Create a configuration group `accelerator` and populate with the above...
 cs = ConfigStore.instance()
 cs.store(group="accelerator", name="tpu-v2-1", node=TPUv2OneConfig)
 cs.store(group="accelerator", name="tpu-v2-8", node=TPUv2EightConfig)
 cs.store(group="accelerator", name="tpu-v3-1", node=TPUv3OneConfig)
 cs.store(group="accelerator", name="tpu-v3-8", node=TPUv3EightConfig)
+
+cs.store(group="accelerator", name="torchrun", node=TorchRunDefaultConfig)
```

### Comparing `voltron-robotics-1.0.3/voltron/conf/datasets.py` & `voltron-robotics-1.1.0/voltron/conf/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,24 +12,28 @@
 from omegaconf import MISSING
 
 
 @dataclass
 class DatasetConfig:
     name: str = MISSING
     path: str = MISSING
-    artifact_path: str = to_absolute_path("data/processed/sth-sth-v2")
+    artifact_path: str = MISSING
 
     # Streaming Parameters (assumes fully preprocessed dataset lives at `stream_prefix/...`)
+    #   =>> Deprecated as of `v2`
     stream: bool = True
     stream_prefix: str = "data/processed"
 
     # Dataset-Specific Parameters
     resolution: int = 224
     normalization: Tuple[Any, Any] = MISSING
 
+    # For preprocessing --> maximum size of saved frames (assumed square)
+    preprocess_resolution: int = MISSING
+
     # Validation Parameters
     n_val_videos: int = MISSING
 
     # Language Modeling Parameters
     language_model: str = "distilbert-base-uncased"
     hf_cache: str = to_absolute_path("data/hf-cache")
 
@@ -54,21 +58,25 @@
 
 
 @dataclass
 class SthSthv2Config(DatasetConfig):
     # fmt: off
     name: str = "sth-sth-v2"
     path: str = to_absolute_path("data/raw/sth-sth-v2")
+    artifact_path: str = to_absolute_path("data/processed/sth-sth-v2")
 
     # Dataset Specific arguments
     normalization: Tuple[Any, Any] = (                              # Mean & Standard Deviation (default :: ImageNet)
         (0.485, 0.456, 0.406),
         (0.229, 0.224, 0.225),
     )
 
+    # Sth-Sth-v2 Videos have a fixed height of 240; we'll crop to square at this resolution!
+    preprocess_resolution: int = 240
+
     # Validation Parameters
     n_val_videos: int = 1000                                        # Number of Validation Clips (fast evaluation!)
 
     # Epochs for Dataset
     warmup_epochs: int = 20
     max_epochs: int = 400
```

### Comparing `voltron-robotics-1.0.3/voltron/conf/models.py` & `voltron-robotics-1.1.0/voltron/conf/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,20 @@
     # Dataset Modality
     data_modality: str = MISSING
 
     # Default Vision Transformer Configuration
     patch_size: int = 16
     mlp_ratio: float = 4.0
 
+    # Effective batch size --> total number of examples before gradient update
+    effective_bsz: int = MISSING
+
     # Number of examples one can safely fit on an accelerator w/ this model!
-    device_bsz: int = MISSING
+    device_bsz: int = MISSING  # For backwards compatibility, only use device_bsz for XLA/TPU pretraining...
+    native_bsz: int = MISSING  # For backwards compatibility, define a separate `native_bsz`...
 
 
 # @Data-Locked Reproductions --- Encompasses MVP (MAE) + R3M
 
 
 # MVP (Base Masked Autoencoder)
 @dataclass
@@ -52,14 +56,15 @@
     decoder_embed_dim: int = MISSING
     decoder_n_heads: int = MISSING
 
     # MAE Loss/Objective Configuration
     norm_pixel_loss: bool = True
     effective_bsz: int = 1024
     device_bsz: int = MISSING
+    native_bsz: int = MISSING
 
     # Optimization Parameters
     optimizer: str = "adamw"
     schedule: str = "linear-warmup+cosine-decay"
     base_lr: float = 1.5e-4
     min_lr: float = 0.0
     betas: Tuple[float, float] = (0.9, 0.95)
@@ -80,14 +85,15 @@
     decoder_depth = 6
     decoder_embed_dim = 192
     decoder_n_heads = 6
 
     # Number of examples one can safely fit on an accelerator w/ this model!
     #   > TPU-v3: max of 128 per device.
     device_bsz = 128
+    native_bsz = 128
 
 
 # R3M Models --> Just different visual encoders, roughly following the above!
 @dataclass
 class R3MConfig(ModelConfig):
     arch: str = "v-r3m"
     identifier: str = MISSING
@@ -113,14 +119,15 @@
     # Loss/Objective Configuration
     lang_reward_weight: float = 1.0
     tcn_weight: float = 1.0
     l1_weight: float = 1e-5
     l2_weight: float = 1e-5
     n_negatives: int = 3
     device_bsz: int = MISSING
+    native_bsz: int = MISSING
 
     # Optimization Parameters
     optimizer: str = "adam"
     schedule: str = "linear-warmup+cosine-decay"
     lr: float = 1e-4
     min_lr: float = 0.0
 
@@ -134,14 +141,15 @@
     #       > https://github.com/rwightman/pytorch-image-models/blob/master/timm/models/vision_transformer.py#L683
     depth = 12
     embed_dim = 384
     n_heads = 6
 
     # Device Batch Size
     device_bsz = 32
+    native_bsz = 128
 
 
 # R3M -- ResNet50 Encoder (instead of ViT)
 @dataclass
 class ResNet3MConfig(ModelConfig):
     arch: str = "v-rn3m"
     identifier: str = MISSING
@@ -165,28 +173,30 @@
     # Loss/Objective Configuration
     lang_reward_weight: float = 1.0
     tcn_weight: float = 1.0
     l1_weight: float = 1e-5
     l2_weight: float = 1e-5
     n_negatives: int = 3
     device_bsz: int = MISSING
+    native_bsz: int = MISSING
 
     # Optimization Parameters
     optimizer: str = "adam"
     lr: float = 1e-4
 
 
 class RN3M50Config(ResNet3MConfig):
     identifier = "r-r3m-rn50"
 
     # Architecture Parameters
     fc_dim = 2048
 
     # Device Batch Size
     device_bsz = 32
+    native_bsz = 128
 
 
 # @Voltron Models -- VCond, VDual, VGen
 
 
 # VCond -- Single Frame + Language Conditioning
 @dataclass
@@ -212,18 +222,21 @@
     encoder_embed_dim: int = MISSING
     encoder_n_heads: int = MISSING
 
     decoder_depth: int = MISSING
     decoder_embed_dim: int = MISSING
     decoder_n_heads: int = MISSING
 
+    use_cls_token: bool = True
+
     # MAE Loss/Objective Configuration
     norm_pixel_loss: bool = True
     effective_bsz: int = 1024
     device_bsz: int = MISSING
+    native_bsz: int = MISSING
 
     # Optimization Parameters
     optimizer: str = "adamw"
     schedule: str = "linear-warmup+cosine-decay"
     base_lr: float = 1.5e-4
     min_lr: float = 0.0
     betas: Tuple[float, float] = (0.9, 0.95)
@@ -246,15 +259,17 @@
 
     decoder_depth = 6
     decoder_embed_dim = 192
     decoder_n_heads = 6
 
     # Number of examples one can safely fit on an accelerator w/ this model!
     #   > TPU-v3: max of 128 per device
+    #   > GPU w/ 32G of RAM: max of 128 per device!
     device_bsz = 128
+    native_bsz = 128
 
 
 @dataclass
 class VCondBaseConfig(VCondConfig):
     identifier = "v-cond-base"
 
     # No language dropout...
@@ -270,15 +285,17 @@
 
     decoder_depth = 8
     decoder_embed_dim = 512
     decoder_n_heads = 16
 
     # Number of examples one can safely fit on an accelerator w/ this model!
     #   > TPU-v3: max of 128 per device!
+    #   > GPU w/ 32G of RAM: max of 128 per device!
     device_bsz = 128
+    native_bsz = 128
 
 
 # VDual - Dual Frame (0th Frame + Kth frame) + Language Conditioning
 @dataclass
 class VDualConfig(ModelConfig):
     arch: str = "v-dual"
     identifier: str = MISSING
@@ -302,18 +319,21 @@
     encoder_embed_dim: int = MISSING
     encoder_n_heads: int = MISSING
 
     decoder_depth: int = MISSING
     decoder_embed_dim: int = MISSING
     decoder_n_heads: int = MISSING
 
+    use_cls_token: bool = True
+
     # MAE Loss/Objective Configuration -- Cut effective batch size since we see 12-25x contexts per batch example!
     norm_pixel_loss: bool = True
     effective_bsz: int = 1024
     device_bsz: int = MISSING
+    native_bsz: int = MISSING
 
     # Optimization Parameters
     optimizer: str = "adamw"
     schedule: str = "linear-warmup+cosine-decay"
     base_lr: float = 1.5e-4
     min_lr: float = 0.0
     betas: Tuple[float, float] = (0.9, 0.95)
@@ -336,15 +356,43 @@
 
     decoder_depth = 6
     decoder_embed_dim = 192
     decoder_n_heads = 6
 
     # Number of examples one can safely fit on an accelerator w/ this model!
     #   > TPU-v3: max of 128 per device!
+    #   > GPU w/ 32G of RAM: max of 128 per device!
+    device_bsz = 128
+    native_bsz = 128
+
+
+@dataclass
+class VDualBaseConfig(VDualConfig):
+    identifier = "v-dual-base"
+
+    # No language dropout...
+    lang_dropout = 0.0
+
+    # Architecture Parameters -- should match ViT Base Architecture to the letter!
+    #   Note: Base is defined in TIMM & Original MAE Repository:
+    #       > https://github.com/rwightman/pytorch-image-models/blob/master/timm/models/vision_transformer.py#L723
+    #       > https://github.com/facebookresearch/mae/blob/main/models_mae.py#L223
+    encoder_depth = 12
+    encoder_embed_dim = 768
+    encoder_n_heads = 12
+
+    decoder_depth = 8
+    decoder_embed_dim = 512
+    decoder_n_heads = 16
+
+    # Number of examples one can safely fit on an accelerator w/ this model!
+    #   > TPU-v3: max of 128 per device!
+    #   > GPU w/ 32G of RAM: max of 64 per device!
     device_bsz = 128
+    native_bsz = 64
 
 
 # VGen - Dual Frame with Language Conditioning AND Language Generation
 @dataclass
 class VGenConfig(ModelConfig):
     arch: str = "v-gen"
     identifier: str = MISSING
@@ -369,18 +417,21 @@
     encoder_embed_dim: int = MISSING
     encoder_n_heads: int = MISSING
 
     decoder_depth: int = MISSING
     decoder_embed_dim: int = MISSING
     decoder_n_heads: int = MISSING
 
+    use_cls_token: bool = True
+
     # MAE Loss/Objective Configuration -- Cut effective batch size since we see 12-25x contexts per batch example!
     norm_pixel_loss: bool = True
     effective_bsz: int = 1024
     device_bsz: int = MISSING
+    native_bsz: int = MISSING
 
     # Optimization Parameters
     optimizer: str = "adamw"
     schedule: str = "linear-warmup+cosine-decay"
     base_lr: float = 1.5e-4
     min_lr: float = 0.0
     betas: Tuple[float, float] = (0.9, 0.95)
@@ -403,15 +454,43 @@
 
     decoder_depth = 6
     decoder_embed_dim = 192
     decoder_n_heads = 6
 
     # Number of examples one can safely fit on an accelerator w/ this model!
     #   > TPU-v3: max of 64 per device!
+    #   > GPU w/ 32G of RAM: max of 64 per device!
     device_bsz = 64
+    native_bsz = 64
+
+
+@dataclass
+class VGen50BaseConfig(VGenConfig):
+    identifier = "v-gen-base"
+
+    # LM Parameters --> control % of examples that are for "language generation" (no conditioning)
+    gen_ratio = 0.50
+
+    # Architecture Parameters -- should match ViT Base Architecture to the letter!
+    #   Note: Base is defined in TIMM & Original MAE Repository:
+    #       > https://github.com/rwightman/pytorch-image-models/blob/master/timm/models/vision_transformer.py#L723
+    #       > https://github.com/facebookresearch/mae/blob/main/models_mae.py#L223
+    encoder_depth = 12
+    encoder_embed_dim = 768
+    encoder_n_heads = 12
+
+    decoder_depth = 8
+    decoder_embed_dim = 512
+    decoder_n_heads = 16
+
+    # Number of examples one can safely fit on an accelerator w/ this model!
+    #   > TPU-v3: max of 32 per device!
+    #   > GPU w/ 32G of RAM: max of 32 per device!
+    device_bsz = 32
+    native_bsz = 32
 
 
 # Create a configuration group `model` and populate with the above...
 cs = ConfigStore.instance()
 
 # === @Data-Locked Reproductions ===
 
@@ -426,10 +505,12 @@
 
 # VCond Architectures
 cs.store(group="model", name="v-cond", node=VCondSmallConfig)
 cs.store(group="model", name="v-cond-base", node=VCondBaseConfig)
 
 # VDual
 cs.store(group="model", name="v-dual", node=VDualSmallConfig)
+cs.store(group="model", name="v-dual-base", node=VDualBaseConfig)
 
 # VGen
 cs.store(group="model", name="v-gen", node=VGen50SmallConfig)
+cs.store(group="model", name="v-gen-base", node=VGen50BaseConfig)
```

### Comparing `voltron-robotics-1.0.3/voltron/conf/tracking.py` & `voltron-robotics-1.1.0/voltron/conf/tracking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 tracking.py
 
 Base Hydra Structured Config for defining various run & experiment tracking configurations, e.g., via Weights & Biases.
 Uses a simple single inheritance structure.
 """
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List, Optional, Tuple
 
 from hydra.core.config_store import ConfigStore
 from omegaconf import MISSING
 
 
 @dataclass
 class TrackingConfig:
+    # Active Loggers --> List of Loggers
+    active_loggers: List[str] = field(default_factory=lambda: ["jsonl", "wandb"])
+
     # Generic Logging Frequency --> Matters more for XLA/TPUs... set this to be as large as you can stomach!
     log_frequency: int = 100
 
     # Checkpointing Strategy --> Save each epoch, keep most recent `idx[0]` checkpoints & *every* `idx[1]` checkpoints
     #   Additionally, save (locally) a checkpoint every `idx[2]` steps for the current epoch (-1).
     checkpoint_strategy: Tuple[int, int, int] = (1, 1, 1500)
```

### Comparing `voltron-robotics-1.0.3/voltron/models/core/vcond.py` & `voltron-robotics-1.1.0/voltron/models/core/vcond.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         weight_decay: float,
         warmup_epochs: int,
         max_epochs: int,
         mask_ratio: float = 0.75,
         mlp_ratio: float = 4.0,
         in_channels: int = 3,
         norm_pixel_loss: bool = True,
+        use_cls_token: bool = False,
     ) -> None:
         """
         Initialize a VCond model with the requisite architecture parameters.
 
         :param resolution: Base image resolution -- usually 224 (ImageNet size).
         :param patch_size: Height/Width of each patch in pixels -- usually 16.
         :param encoder_depth: Number of Transformer blocks in the encoder -- should be greater than decoder.
@@ -76,37 +77,44 @@
         :param weight_decay: Weight decay for global weight regularization (only applied to non-bias, non-LN layers).
         :param warmup_epochs: Number of epochs to warmup learning rate for linear warmup schedule.
         :param max_epochs: Total number of training epochs to be run.
         :param mask_ratio: Ratio for number of patches to mask out for MAE -- should be fairly high!
         :param mlp_ratio: Ratio for embedding size to Position-wise Feed-Forward MLP (gets shrunk back down).
         :param in_channels: Default number of channels in the base image -- almost always 3.
         :param norm_pixel_loss: Normalize decoder pixel targets for reconstruction (better perf, not interpretable).
+        :param use_cls_token: Add <CLS> token for continued pretraining (NOTE: not used in MAE pretraining/finetuning!)
         """
         super().__init__()
         self.resolution, self.patch_size, self.mask_ratio = resolution, patch_size, mask_ratio
         self.in_channels, self.norm_pixel_loss, self.mlp_ratio = in_channels, norm_pixel_loss, mlp_ratio
         self.optimizer, self.schedule, self.betas, self.weight_decay = optimizer, schedule, betas, weight_decay
         self.lr, self.base_lr, self.min_lr, self.effective_bsz = None, base_lr, min_lr, effective_bsz
         self.warmup_epochs, self.max_epochs = warmup_epochs, max_epochs
+        self.use_cls_token = use_cls_token
         self.language_dim = language_dim
 
         # Encoder/Decoder Parameters
         self.encoder_depth, self.decoder_depth = encoder_depth, decoder_depth
         self.encoder_embed_dim, self.encoder_n_heads = encoder_embed_dim, encoder_n_heads
         self.decoder_embed_dim, self.decoder_n_heads = decoder_embed_dim, decoder_n_heads
 
         # General Parameters (for downstream adaptation)
         self.embed_dim, self.n_heads = self.encoder_embed_dim, self.encoder_n_heads
 
-        # MAE Encoder Parameters --> No CLS Token!
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            self.cls_token = nn.Parameter(torch.zeros(1, 1, self.encoder_embed_dim))
+
+        # MAE Encoder Parameters
         self.patch2embed = PatchEmbed(
             self.resolution, self.patch_size, self.encoder_embed_dim, in_channels=self.in_channels
         )
         self.encoder_pe = nn.Parameter(
-            torch.zeros(1, self.patch2embed.num_patches, self.encoder_embed_dim), requires_grad=False
+            torch.zeros(1, self.patch2embed.num_patches + (1 if self.use_cls_token else 0), self.encoder_embed_dim),
+            requires_grad=False,
         )
         self.encoder_blocks = nn.ModuleList(
             [
                 Block(
                     self.encoder_embed_dim,
                     self.encoder_n_heads,
                     self.mlp_ratio,
@@ -121,18 +129,19 @@
 
         # Projection from Language Embedding to Decoder
         self.lang2encoder = nn.Linear(self.language_dim, self.encoder_embed_dim)
 
         # Projection from Encoder to Decoder
         self.encoder2decoder = nn.Linear(self.encoder_embed_dim, self.decoder_embed_dim)
 
-        # MAE Decoder Parameters -- Remember the MASK Token!
+        # MAE Decoder Parameters -- Remember the CLS Token (if specified)!
         self.mask_token = nn.Parameter(torch.zeros(1, 1, self.decoder_embed_dim))
         self.decoder_pe = nn.Parameter(
-            torch.zeros(1, self.patch2embed.num_patches, self.decoder_embed_dim), requires_grad=False
+            torch.zeros(1, self.patch2embed.num_patches + (1 if self.use_cls_token else 0), self.decoder_embed_dim),
+            requires_grad=False,
         )
         self.decoder_blocks = nn.ModuleList(
             [
                 Block(
                     self.decoder_embed_dim,
                     self.decoder_n_heads,
                     self.mlp_ratio,
@@ -165,26 +174,32 @@
 
         # Freeze the LM
         for _, param in self.lm.named_parameters():
             param.requires_grad = False
 
     def initialize_weights(self) -> None:
         # Position Encoding -- Fixed 2D Sine-Cosine Embeddings
-        enc_pe = get_2D_position_embeddings(self.encoder_embed_dim, int(self.patch2embed.num_patches**0.5))
+        enc_pe = get_2D_position_embeddings(
+            self.encoder_embed_dim, int(self.patch2embed.num_patches**0.5), cls_token=self.use_cls_token
+        )
         self.encoder_pe.data.copy_(torch.from_numpy(enc_pe).float().unsqueeze(0))
-        dec_pe = get_2D_position_embeddings(self.decoder_embed_dim, int(self.patch2embed.num_patches**0.5))
+        dec_pe = get_2D_position_embeddings(
+            self.decoder_embed_dim, int(self.patch2embed.num_patches**0.5), cls_token=self.use_cls_token
+        )
         self.decoder_pe.data.copy_(torch.from_numpy(dec_pe).float().unsqueeze(0))
 
         # Initialize PatchEmbedding as a Linear...
         nn.init.xavier_uniform_(self.patch2embed.proj.weight.data.view([self.patch2embed.proj.weight.data.shape[0], -1]))
 
         # Initialize Mask Token, Img Token, Lang Token w/ Truncated Normal
         nn.init.normal_(self.mask_token, std=0.02)
         nn.init.normal_(self.img_token, std=0.02)
         nn.init.normal_(self.lang_token, std=0.02)
+        if self.use_cls_token:
+            nn.init.normal_(self.cls_token, std=0.02)
 
         # Default Transformer initializer on everything else...
         self.apply(self.transformer_initializer)
 
     @staticmethod
     def transformer_initializer(m: nn.Module) -> None:
         # Use `xavier_uniform` following Jax ViT
@@ -264,16 +279,23 @@
         return representations if mode == "multimodal" else representations[:, : -lang_mask.shape[-1]]
 
     def encode(self, img: torch.Tensor, lang: torch.Tensor, lang_mask: torch.Tensor) -> torch.Tensor:
         """Default representation extraction function, given a batch of images and tokenized language."""
         lang_embeddings = self.encode_language(lang, lang_mask)
         projected_language = self.lang2encoder(lang_embeddings)
 
-        # Patchify + Position Embedding
+        # Patchify
         patches = self.patch2embed(img)
+
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_tokens = self.cls_token.expand(img.shape[0], -1, -1)
+            patches = torch.cat([cls_tokens, patches], dim=1)
+
+        # Position Encoding
         patches_pe = patches + self.encoder_pe
 
         # Add "modality" embeddings to patches & language
         img_embeddings, lang_embeddings = patches_pe + self.img_token, projected_language + self.lang_token
 
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer
         patches_mask = torch.ones_like(img_embeddings[..., -1], dtype=lang_mask.dtype)
@@ -287,61 +309,83 @@
 
         # Return the full sequence of multimodal embeddings...
         return multimodal_embeddings
 
     def forward_encoder(
         self, img: torch.Tensor, lang: torch.Tensor, lang_mask: torch.Tensor, mask_ratio: Optional[float] = None
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        # Patchify + Position Embedding
+        lang_embeddings = self.encode_language(lang, lang_mask)
+        projected_lang = self.lang2encoder(lang_embeddings)
+
+        # Patchify + Position Embedding (without <CLS> Token!)
         patches = self.patch2embed(img)
-        patches_pe = patches + self.encoder_pe
+        patches_pe = patches + (self.encoder_pe if not self.use_cls_token else self.encoder_pe[:, 1:, :])
 
         # Create mask (and go ahead and mask out patches at the same time)
         visible_patches, mask, restore_idxs = self.mask(patches_pe, mask_ratio)
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_token_pe = self.cls_token + self.encoder_pe[:, :1, :]
+            cls_tokens = cls_token_pe.expand(img.shape[0], -1, -1)
+            visible_patches = torch.cat([cls_tokens, visible_patches], dim=1)
+
         # Add "modality" embeddings to patches & language
-        visible_patches, lang = visible_patches + self.img_token, lang + self.lang_token
+        visible_patches, projected_lang = visible_patches + self.img_token, projected_lang + self.lang_token
 
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer
         visible_mask = torch.ones_like(visible_patches[..., -1], dtype=lang_mask.dtype)
-        multimodal_embedding = torch.cat([visible_patches, lang], dim=1)  # Merge on sequence length...
+        multimodal_embedding = torch.cat([visible_patches, projected_lang], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([visible_mask, lang_mask], dim=1)  # Merge on sequence length...
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             multimodal_embedding = block(multimodal_embedding, multimodal_mask)
         multimodal_embedding = self.encoder_norm(multimodal_embedding)
 
-        # Split multimodal embedding, remove language and return only the visible patches!
+        # Split multimodal embedding, remove language and return only the visible patches (+ optional <CLS> token)!
         visible_patches = multimodal_embedding[:, : -lang_mask.shape[-1], ...]
         return visible_patches, mask, restore_idxs
 
     def forward_decoder(self, visible_patches: torch.Tensor, restore_idxs: torch.Tensor) -> torch.Tensor:
         # Project patches into decoder embedding dimension
         projected_patches = self.encoder2decoder(visible_patches)
 
         # Add Mask Tokens to Sequence & Unshuffle
         mask_tokens = self.mask_token.repeat(
-            projected_patches.shape[0], restore_idxs.shape[1] - visible_patches.shape[1], 1
-        )
-        concatenated_patches = torch.cat([projected_patches, mask_tokens], dim=1)
-        unshuffled_patches = torch.gather(
-            concatenated_patches, dim=1, index=restore_idxs[..., None].repeat(1, 1, self.decoder_embed_dim)
+            projected_patches.shape[0],
+            restore_idxs.shape[1] - visible_patches.shape[1] + (1 if self.use_cls_token else 0),
+            1,
         )
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            # Remove & add back CLS Token as part of the "unshuffling"
+            concatenated_patches = torch.cat([projected_patches[:, 1:, :], mask_tokens], dim=1)  # Skip CLS Token
+            no_cls_unshuffled_patches = torch.gather(
+                concatenated_patches, dim=1, index=restore_idxs[..., None].repeat(1, 1, self.decoder_embed_dim)
+            )
+            unshuffled_patches = torch.cat([projected_patches[:, :1, :], no_cls_unshuffled_patches], dim=1)
+        else:
+            concatenated_patches = torch.cat([projected_patches, mask_tokens], dim=1)
+            unshuffled_patches = torch.gather(
+                concatenated_patches, dim=1, index=restore_idxs[..., None].repeat(1, 1, self.decoder_embed_dim)
+            )
+
         # Add Position Embeddings
         decoder_patches = unshuffled_patches + self.decoder_pe
 
         # Apply Transformer Blocks...
         for block in self.decoder_blocks:
             decoder_patches = block(decoder_patches)
         decoder_patches = self.decoder_norm(decoder_patches)
 
-        # Run final projection & return
-        return self.decoder_prediction(decoder_patches)
+        # Run final projection & return --> note <CLS> token handling!
+        decoder_prediction = self.decoder_prediction(decoder_patches)
+        return decoder_prediction if not self.use_cls_token else decoder_prediction[:, 1:, :]
 
     def patchify(self, imgs: torch.Tensor) -> torch.Tensor:
         """Convert a batch of images to their patched equivalents, by naive reshaping"""
         return rearrange(
             imgs,
             "bsz c (height patch_h) (width patch_w) -> bsz (height width) (patch_h patch_w c)",
             patch_h=self.patch_size,
@@ -362,26 +406,21 @@
 
         # Compute mean loss only on *removed* patches and return
         return (avg_loss_per_patch * mask).sum() / mask.sum()
 
     def forward(
         self, img: torch.Tensor, lang: torch.Tensor, lang_mask: torch.Tensor, mask_ratio: Optional[float] = None
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        # First, get precomputed language embeddings & project to encoder_embed_dim; language only used in encoder!
-        lang_embeddings = self.encode_language(lang, lang_mask)
-        projected_language = self.lang2encoder(lang_embeddings)
-
-        # MAE --> does image masking in the body of the model...
-        visible_patches, mask, restore_idxs = self.forward_encoder(img, projected_language, lang_mask, mask_ratio)
+        visible_patches, mask, restore_idxs = self.forward_encoder(img, lang, lang_mask, mask_ratio)
         reconstructions = self.forward_decoder(visible_patches, restore_idxs)
         loss = self.compute_loss(img, reconstructions, mask)
         return loss, reconstructions, mask
 
     def configure_optimizer(self) -> Tuple[torch.optim.Optimizer, Callable[[int, float], float]]:
-        # Short-circuit on valid optimizers
+        # Short-Circuit on Valid Optimizers
         if self.optimizer not in ["adamw"]:
             raise NotImplementedError(f"Optimizer `{self.optimizer}` not supported - try [`adamw`] instead!")
 
         # Create Parameter Groups --> bias terms, normalization layer parameters shouldn't be decayed...
         #   > This is a compact rewrite of `param_groups_weight_decay()` from TIMM because I don't want the dependency
         decay, no_decay = [], []
         for name, param in self.named_parameters():
```

### Comparing `voltron-robotics-1.0.3/voltron/models/core/vdual.py` & `voltron-robotics-1.1.0/voltron/models/core/vdual.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         weight_decay: float,
         warmup_epochs: int,
         max_epochs: int,
         mask_ratio: float = 0.75,
         mlp_ratio: float = 4.0,
         in_channels: int = 3,
         norm_pixel_loss: bool = True,
+        use_cls_token: bool = False,
     ) -> None:
         """
         Initialize a VDual model with the requisite architecture parameters.
 
         :param resolution: Base image resolution -- usually 224 (ImageNet size).
         :param patch_size: Height/Width of each patch in pixels -- usually 16.
         :param encoder_depth: Number of Transformer blocks in the encoder -- should be greater than decoder.
@@ -76,37 +77,44 @@
         :param weight_decay: Weight decay for global weight regularization (only applied to non-bias, non-LN layers).
         :param warmup_epochs: Number of epochs to warmup learning rate for linear warmup schedule.
         :param max_epochs: Total number of training epochs to be run.
         :param mask_ratio: Ratio for number of patches to mask out for MAE -- should be fairly high!
         :param mlp_ratio: Ratio for embedding size to Position-wise FeedForward MLP (gets shrunk back down).
         :param in_channels: Default number of channels in the base image -- almost always 3.
         :param norm_pixel_loss: Normalize decoder pixel targets for reconstruction (better perf, not interpretable).
+        :param use_cls_token: Add <CLS> token for continued pretraining (NOTE: not used in MAE pretraining/finetuning!)
         """
         super().__init__()
         self.resolution, self.patch_size, self.mask_ratio = resolution, patch_size, mask_ratio
         self.in_channels, self.norm_pixel_loss, self.mlp_ratio = in_channels, norm_pixel_loss, mlp_ratio
         self.optimizer, self.schedule, self.betas, self.weight_decay = optimizer, schedule, betas, weight_decay
         self.lr, self.base_lr, self.min_lr, self.effective_bsz = None, base_lr, min_lr, effective_bsz
         self.warmup_epochs, self.max_epochs = warmup_epochs, max_epochs
+        self.use_cls_token = use_cls_token
         self.language_dim = language_dim
 
         # Encoder/Decoder Parameters
         self.encoder_depth, self.decoder_depth = encoder_depth, decoder_depth
         self.encoder_embed_dim, self.encoder_n_heads = encoder_embed_dim, encoder_n_heads
         self.decoder_embed_dim, self.decoder_n_heads = decoder_embed_dim, decoder_n_heads
 
         # General Parameters (for downstream adaptation)
         self.embed_dim, self.n_heads = self.encoder_embed_dim, self.encoder_n_heads
 
-        # MAE Encoder Parameters --> No CLS Token!
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            self.cls_token = nn.Parameter(torch.zeros(1, 1, self.encoder_embed_dim))
+
+        # MAE Encoder Parameters
         self.patch2embed = PatchEmbed(
             self.resolution, self.patch_size, self.encoder_embed_dim, in_channels=self.in_channels
         )
         self.encoder_pe = nn.Parameter(
-            torch.zeros(1, self.patch2embed.num_patches, self.encoder_embed_dim), requires_grad=False
+            torch.zeros(1, self.patch2embed.num_patches + (1 if self.use_cls_token else 0), self.encoder_embed_dim),
+            requires_grad=False,
         )
         self.encoder_blocks = nn.ModuleList(
             [
                 Block(
                     self.encoder_embed_dim,
                     self.encoder_n_heads,
                     self.mlp_ratio,
@@ -121,18 +129,19 @@
 
         # Projection from Language Embedding to Decoder
         self.lang2encoder = nn.Linear(self.language_dim, self.encoder_embed_dim)
 
         # Projection from Encoder to Decoder
         self.encoder2decoder = nn.Linear(self.encoder_embed_dim, self.decoder_embed_dim)
 
-        # MAE Decoder Parameters -- Remember the MASK Token!
+        # MAE Decoder Parameters -- Remember the CLS Token (if specified)!
         self.mask_token = nn.Parameter(torch.zeros(1, 1, 1, self.decoder_embed_dim))
         self.decoder_pe = nn.Parameter(
-            torch.zeros(1, self.patch2embed.num_patches, self.decoder_embed_dim), requires_grad=False
+            torch.zeros(1, self.patch2embed.num_patches + (1 if self.use_cls_token else 0), self.decoder_embed_dim),
+            requires_grad=False,
         )
         self.decoder_blocks = nn.ModuleList(
             [
                 Block(
                     self.decoder_embed_dim,
                     self.decoder_n_heads,
                     self.mlp_ratio,
@@ -171,26 +180,32 @@
 
         # Freeze the LM
         for _, param in self.lm.named_parameters():
             param.requires_grad = False
 
     def initialize_weights(self) -> None:
         # Position Encoding -- Fixed 2D Sine-Cosine Embeddings
-        enc_pe = get_2D_position_embeddings(self.encoder_embed_dim, int(self.patch2embed.num_patches**0.5))
+        enc_pe = get_2D_position_embeddings(
+            self.encoder_embed_dim, int(self.patch2embed.num_patches**0.5), cls_token=self.use_cls_token
+        )
         self.encoder_pe.data.copy_(torch.from_numpy(enc_pe).float().unsqueeze(0))
-        dec_pe = get_2D_position_embeddings(self.decoder_embed_dim, int(self.patch2embed.num_patches**0.5))
+        dec_pe = get_2D_position_embeddings(
+            self.decoder_embed_dim, int(self.patch2embed.num_patches**0.5), cls_token=self.use_cls_token
+        )
         self.decoder_pe.data.copy_(torch.from_numpy(dec_pe).float().unsqueeze(0))
 
         # Initialize PatchEmbedding as a Linear...
         nn.init.xavier_uniform_(self.patch2embed.proj.weight.data.view([self.patch2embed.proj.weight.data.shape[0], -1]))
 
         # Initialize Mask Token, Img Token, Lang Token w/ Truncated Normal
         nn.init.normal_(self.mask_token, std=0.02)
         nn.init.normal_(self.img_token, std=0.02)
         nn.init.normal_(self.lang_token, std=0.02)
+        if self.use_cls_token:
+            nn.init.normal_(self.cls_token, std=0.02)
 
         # Everything else...
         self.apply(self.transformer_initializer)
 
     @staticmethod
     def transformer_initializer(m: nn.Module) -> None:
         if isinstance(m, nn.Linear):
@@ -277,94 +292,137 @@
     def encode(self, imgs: torch.Tensor, lang: torch.Tensor, lang_mask: torch.Tensor) -> torch.Tensor:
         """Default representation extraction function, given a batch of dual-images and tokenized language."""
         lang_embeddings = self.encode_language(lang, lang_mask)
         projected_language = self.lang2encoder(lang_embeddings)
 
         # Patchify, broadcast position embedding ctx_len (0 + K) dimension, unfold, add `ctx_enc_pe` embeddings!
         patches = self.patch2embed(rearrange(imgs, "bsz ctx channels res1 res2 -> (bsz ctx) channels res1 res2"))
-        patches_pe = patches + self.encoder_pe
+        patches_pe = patches + (self.encoder_pe[:, 1:, :] if self.use_cls_token else self.encoder_pe)
         ctx_patches = rearrange(patches_pe, "(bsz ctx) seq embed -> bsz ctx seq embed", ctx=2)
         ctx_patches_pe = ctx_patches + self.ctx_enc_pe[:, :2, ...]
 
         # Add "modality" embeddings to patches & language & flatten out context patches...
         img_ctx_embeddings, lang_embeddings = ctx_patches_pe + self.img_token, projected_language + self.lang_token
         img_embeddings = rearrange(img_ctx_embeddings, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_token_pe = self.cls_token + self.encoder_pe[:, :1, :] + self.img_token[:, 0, :, :]
+            cls_tokens = cls_token_pe.expand(imgs.shape[0], -1, -1)
+            img_embeddings = torch.cat([cls_tokens, img_embeddings], dim=1)
+
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer
         patches_mask = torch.ones_like(img_embeddings[..., -1], dtype=lang_mask.dtype)
         multimodal_embeddings = torch.cat([img_embeddings, lang_embeddings], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([patches_mask, lang_mask], dim=1)  # Merge on sequence length...
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             multimodal_embeddings = block(multimodal_embeddings, multimodal_mask)
         multimodal_embeddings = self.encoder_norm(multimodal_embeddings)
 
-        # Return the full sequence of multimodal embeddings (but ignore 0th frame)...
-        return multimodal_embeddings[:, self.patch2embed.num_patches :]
+        # Return the full sequence of multimodal embeddings (but ignore 0th frame) => the `~` denote what to remove!
+        #   => [CLS] + ~[n_patches x 0th frame]~ + [n_patches x Kth frame] + [max_lang_len language]
+        #   => ~[n_patches x 0th frame]~ + [n_patches x Kth frame] + [max_lang_len language]
+        if self.use_cls_token:
+            return torch.cat(
+                [multimodal_embeddings[:, :1, :], multimodal_embeddings[:, 1 + self.patch2embed.num_patches :, :]], dim=1
+            )
+        else:
+            return multimodal_embeddings[:, self.patch2embed.num_patches :]
 
     def forward_encoder(
         self, img_ctx: torch.Tensor, lang: torch.Tensor, lang_mask: torch.Tensor, mask_ratio: Optional[float] = None
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        lang_embeddings = self.encode_language(lang, lang_mask)
+        projected_lang = self.lang2encoder(lang_embeddings)
+
         # Patchify, broadcast position embedding across ctx_len (0 + K) dimension, unfold, add `ctx_enc_pe` embeddings!
         patches = self.patch2embed(rearrange(img_ctx, "bsz ctx channels res1 res2 -> (bsz ctx) channels res1 res2"))
-        patches_pe = patches + self.encoder_pe
+        patches_pe = patches + (self.encoder_pe if not self.use_cls_token else self.encoder_pe[:, 1:, :])
         ctx_patches = rearrange(patches_pe, "(bsz ctx) seq embed -> bsz ctx seq embed", ctx=2)
         ctx_patches_pe = ctx_patches + self.ctx_enc_pe[:, :2, ...]
 
         # Create mask (and go ahead and mask out patches at the same time)
         visible_ctx_patches, mask, restore_idxs = self.mask(ctx_patches_pe, mask_ratio)
 
         # Add "modality" embeddings to patches & language & flatten out context patches...
-        visible_ctx_patches, lang = visible_ctx_patches + self.img_token, lang + self.lang_token
+        visible_ctx_patches, lang = visible_ctx_patches + self.img_token, projected_lang + self.lang_token
         visible_patches = rearrange(visible_ctx_patches, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_token_pe = self.cls_token + self.encoder_pe[:, :1, :] + self.img_token[:, 0, :, :]
+            cls_tokens = cls_token_pe.expand(img_ctx.shape[0], -1, -1)
+            visible_patches = torch.cat([cls_tokens, visible_patches], dim=1)
+
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer...
         visible_mask = torch.ones_like(visible_patches[..., -1], dtype=lang_mask.dtype)
         multimodal_embedding = torch.cat([visible_patches, lang], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([visible_mask, lang_mask], dim=1)  # Merge on sequence length...
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             multimodal_embedding = block(multimodal_embedding, multimodal_mask)
         multimodal_embedding = self.encoder_norm(multimodal_embedding)
 
-        # Split multimodal embedding, remove language, and return only the visible ctx (0th + Kth frame) patches!
-        visible_ctx_patches = rearrange(
-            multimodal_embedding[:, : -lang_mask.shape[-1], ...], "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2
-        )
-        return visible_ctx_patches, mask, restore_idxs
+        # Split multimodal embedding, remove language, return the visible ctx (0th + Kth frame) patches (+ <CLS>)!
+        visible_patches = multimodal_embedding[:, : -lang_mask.shape[-1], ...]
+        return visible_patches, mask, restore_idxs
 
-    def forward_decoder(self, visible_ctx_patches: torch.Tensor, restore_idxs: torch.Tensor) -> torch.Tensor:
-        # Project patches into decoder embedding dimension (visible_ctx_patches :: [bsz, 2, seq, enc_embed])
-        projected_ctx_patches = self.encoder2decoder(visible_ctx_patches)
+    def forward_decoder(self, visible_patches: torch.Tensor, restore_idxs: torch.Tensor) -> torch.Tensor:
+        # Project patches into decoder embedding dimension (visible_ctx_patches :: [bsz, (CLS) + 2 * seq, enc_embed])
+        projected_patches = self.encoder2decoder(visible_patches)
+        visible_per_frame = (projected_patches.shape[1] - (1 if self.use_cls_token else 0)) // 2
 
         # Add Mask Tokens to Sequence and Unshuffle
-        mask_tokens = self.mask_token.repeat(
-            projected_ctx_patches.shape[0], 2, restore_idxs.shape[1] - visible_ctx_patches.shape[2], 1
-        )
-        concatenated_ctx_patches = torch.cat([projected_ctx_patches, mask_tokens], dim=2)
-        unshuffled_ctx_patches = torch.gather(
-            concatenated_ctx_patches,
-            dim=2,
-            index=restore_idxs[:, None, ..., None].repeat(1, 2, 1, self.decoder_embed_dim),
-        )
+        mask_tokens = self.mask_token.repeat(projected_patches.shape[0], 2, restore_idxs.shape[1] - visible_per_frame, 1)
+
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            # Remove CLS Token as part of "unshuffling"
+            projected_ctx_patches = rearrange(
+                projected_patches[:, 1:, :], "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2
+            )
+            no_cls_concatenated_ctx_patches = torch.cat([projected_ctx_patches, mask_tokens], dim=2)
+            unshuffled_ctx_patches = torch.gather(
+                no_cls_concatenated_ctx_patches,
+                dim=2,
+                index=restore_idxs[:, None, ..., None].repeat(1, 2, 1, self.decoder_embed_dim),
+            )
+        else:
+            projected_ctx_patches = rearrange(projected_patches, "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2)
+            concatenated_ctx_patches = torch.cat([projected_ctx_patches, mask_tokens], dim=2)
+            unshuffled_ctx_patches = torch.gather(
+                concatenated_ctx_patches,
+                dim=2,
+                index=restore_idxs[:, None, ..., None].repeat(1, 2, 1, self.decoder_embed_dim),
+            )
 
         # Add position embeddings, `ctx_dec_pe` embeddings, and flatten patches for Transformer...
-        decoder_ctx_patches_pe = unshuffled_ctx_patches + self.decoder_pe[None, ...]
+        decoder_ctx_patches_pe = unshuffled_ctx_patches + (
+            self.decoder_pe[None, ...] if not self.use_cls_token else self.decoder_pe[None, :, 1:, :]
+        )
         decoder_ctx_patches = decoder_ctx_patches_pe + self.ctx_dec_pe[:, :2, ...]
         decoder_patches = rearrange(decoder_ctx_patches, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            # Add back <CLS> Token from `projected_patches[:, :1, :]`
+            cls_embedding = projected_patches[:, :1, :] + self.decoder_pe[:, :1, :]
+            decoder_patches = torch.cat([cls_embedding, decoder_patches], dim=1)
+
         # Apply Transformer Blocks...
         for block in self.decoder_blocks:
             decoder_patches = block(decoder_patches)
         decoder_patches = self.decoder_norm(decoder_patches)
 
-        # Run final projection & return "unflattened" patches
-        reconstructions = self.decoder_prediction(decoder_patches)
+        # Run final projection & return "unflattened" patches --> note <CLS> token handling!
+        decoder_prediction = self.decoder_prediction(decoder_patches)
+        reconstructions = decoder_prediction if not self.use_cls_token else decoder_prediction[:, 1:, :]
         return rearrange(reconstructions, "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2)
 
     def patchify(self, imgs: torch.Tensor) -> torch.Tensor:
         """Convert a batch of (0th + Kth frame) images to their patched equivalents by naive reshaping."""
         return rearrange(
             imgs,
             "bsz ctx c (height patch_h) (width patch_w) -> bsz ctx (height width) (patch_h patch_w c)",
@@ -404,20 +462,15 @@
         :param lang: A [bsz, seq_len] tensor of language context to condition on.
         :param lang_mask: A [bsz, seq_len] binary mask tensor to indicate padding locations in the lang tensor.
         :param mask_ratio: Optional masking ratio to use instead of the default.
 
         :return Tuple of losses and intermediates, as follows:
             > (combined loss, [reconstruction loss per frame in {0, K}])
         """
-        # First, get precomputed language embeddings & project to encoder_embed_dim; language only used in encoder!
-        lang_embeddings = self.encode_language(lang, lang_mask)
-        projected_language = self.lang2encoder(lang_embeddings)
-
-        # Reshape image context to apply masking *identically*
-        visible_ctx_patches, mask, restore_idxs = self.forward_encoder(imgs, projected_language, lang_mask, mask_ratio)
+        visible_ctx_patches, mask, restore_idxs = self.forward_encoder(imgs, lang, lang_mask, mask_ratio)
         ctx_reconstructions = self.forward_decoder(visible_ctx_patches, restore_idxs)
         zero_loss, k_loss = self.compute_loss(imgs, ctx_reconstructions, mask)
 
         # Return average reconstruction loss, individual losses...
         loss = (zero_loss + k_loss) / 2
         return loss, [zero_loss, k_loss]
```

### Comparing `voltron-robotics-1.0.3/voltron/models/core/vgen.py` & `voltron-robotics-1.1.0/voltron/models/core/vgen.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         weight_decay: float,
         warmup_epochs: int,
         max_epochs: int,
         mask_ratio: float = 0.75,
         mlp_ratio: float = 4.0,
         in_channels: int = 3,
         norm_pixel_loss: bool = True,
+        use_cls_token: bool = False,
         eps: float = 1e-8,
     ) -> None:
         """
         Initialize a VGen model with the requisite architecture parameters.
 
         :param resolution: Base image resolution -- usually 224 (ImageNet size).
         :param patch_size: Height/Width of each patch in pixels -- usually 16.
@@ -89,39 +90,46 @@
         :param weight_decay: Weight decay for global weight regularization (only applied to non-bias, non-LN layers).
         :param warmup_epochs: Number of epochs to warmup learning rate for linear warmup schedule.
         :param max_epochs: Total number of training epochs to be run.
         :param mask_ratio: Ratio for number of patches AND tokens to mask out for M3AE -- should be fairly high!
         :param mlp_ratio: Ratio for embedding size to Position-wise FeedForward MLP (gets shrunk back down).
         :param in_channels: Default number of channels in the base image -- almost always 3.
         :param norm_pixel_loss: Normalize decoder pixel targets for reconstruction (better perf, not interpretable).
+        :param use_cls_token: Add <CLS> token for continued pretraining (NOTE: not used in MAE pretraining/finetuning!)
         :param eps: Epsilon for preventing divide by zero.
         """
         super().__init__()
         self.resolution, self.patch_size, self.mask_ratio, self.eps = resolution, patch_size, mask_ratio, eps
         self.in_channels, self.norm_pixel_loss, self.mlp_ratio = in_channels, norm_pixel_loss, mlp_ratio
         self.optimizer, self.schedule, self.betas, self.weight_decay = optimizer, schedule, betas, weight_decay
         self.lr, self.base_lr, self.min_lr, self.effective_bsz = None, base_lr, min_lr, effective_bsz
         self.mae_weight, self.lm_weight, self.language_dim = mae_weight, lm_weight, language_dim
         self.max_lang_len, self.vocab_size = max_lang_len, vocab_size
+        self.use_cls_token = use_cls_token
         self.warmup_epochs, self.max_epochs = warmup_epochs, max_epochs
 
         # Encoder/Decoder Parameters
         self.encoder_depth, self.decoder_depth = encoder_depth, decoder_depth
         self.encoder_embed_dim, self.encoder_n_heads = encoder_embed_dim, encoder_n_heads
         self.decoder_embed_dim, self.decoder_n_heads = decoder_embed_dim, decoder_n_heads
 
         # General Parameters (for downstream adaptation)
         self.embed_dim, self.n_heads = self.encoder_embed_dim, self.encoder_n_heads
 
-        # MAE Encoder Parameters --> No CLS Token!
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            self.cls_token = nn.Parameter(torch.zeros(1, 1, self.encoder_embed_dim))
+
+        # MAE Encoder Parameters
         self.patch2embed = PatchEmbed(
             self.resolution, self.patch_size, self.encoder_embed_dim, in_channels=self.in_channels
         )
         self.encoder_pe = nn.Parameter(
-            torch.zeros(1, self.patch2embed.num_patches, self.encoder_embed_dim), requires_grad=False
+            torch.zeros(1, self.patch2embed.num_patches + (1 if self.use_cls_token else 0), self.encoder_embed_dim),
+            requires_grad=False,
         )
         self.encoder_blocks = nn.ModuleList(
             [
                 Block(
                     self.encoder_embed_dim,
                     self.encoder_n_heads,
                     self.mlp_ratio,
@@ -137,20 +145,19 @@
         # Projection from Language Embedding to Decoder
         self.lang2encoder = nn.Linear(self.language_dim, self.encoder_embed_dim)
         self.lang2decoder = nn.Linear(self.language_dim, self.decoder_embed_dim)
 
         # Projection from Encoder to Decoder
         self.encoder2decoder = nn.Linear(self.encoder_embed_dim, self.decoder_embed_dim)
 
-        # MAE Decoder Parameters -- Remember the MASK Token!
+        # MAE Decoder Parameters -- Remember the CLS Token (if specified)!
         self.mask_token = nn.Parameter(torch.zeros(1, 1, 1, self.decoder_embed_dim))
-
-        # Decoder PE has to be aware of both patches and language, since injecting new mask tokens...
         self.decoder_pe = nn.Parameter(
-            torch.zeros(1, self.patch2embed.num_patches, self.decoder_embed_dim), requires_grad=False
+            torch.zeros(1, self.patch2embed.num_patches + (1 if self.use_cls_token else 0), self.decoder_embed_dim),
+            requires_grad=False,
         )
         self.decoder_blocks = nn.ModuleList(
             [
                 Block(
                     self.decoder_embed_dim,
                     self.decoder_n_heads,
                     self.mlp_ratio,
@@ -198,26 +205,32 @@
 
         # Freeze the LM
         for _, param in self.lm.named_parameters():
             param.requires_grad = False
 
     def initialize_weights(self) -> None:
         # Position Encoding -- Fixed 2D Sine-Cosine Embeddings
-        enc_pe = get_2D_position_embeddings(self.encoder_embed_dim, int(self.patch2embed.num_patches**0.5))
+        enc_pe = get_2D_position_embeddings(
+            self.encoder_embed_dim, int(self.patch2embed.num_patches**0.5), cls_token=self.use_cls_token
+        )
         self.encoder_pe.data.copy_(torch.from_numpy(enc_pe).float().unsqueeze(0))
-        dec_pe = get_2D_position_embeddings(self.decoder_embed_dim, int(self.patch2embed.num_patches**0.5))
+        dec_pe = get_2D_position_embeddings(
+            self.decoder_embed_dim, int(self.patch2embed.num_patches**0.5), cls_token=self.use_cls_token
+        )
         self.decoder_pe.data.copy_(torch.from_numpy(dec_pe).float().unsqueeze(0))
 
         # Initialize PatchEmbedding as a Linear...
         nn.init.xavier_uniform_(self.patch2embed.proj.weight.data.view([self.patch2embed.proj.weight.data.shape[0], -1]))
 
         # Initialize Mask Token, Img Token, Lang Token w/ Truncated Normal
         nn.init.normal_(self.mask_token, std=0.02)
         nn.init.normal_(self.img_enc_token, std=0.02)
         nn.init.normal_(self.lang_enc_token, std=0.02)
+        if self.use_cls_token:
+            nn.init.normal_(self.cls_token, std=0.02)
 
         # Everything else...
         self.apply(self.transformer_initializer)
 
     @staticmethod
     def transformer_initializer(m: nn.Module) -> None:
         if isinstance(m, nn.Linear):
@@ -312,104 +325,132 @@
     def encode(self, imgs: torch.Tensor, lang: torch.Tensor, lang_mask: torch.Tensor) -> torch.Tensor:
         """Default representation extraction function, given a batch of dual-images and tokenized language."""
         lang_embeddings = self.encode_language(lang, lang_mask)
         projected_language = self.lang2encoder(lang_embeddings)
 
         # Patchify, broadcast position embedding across ctx_len (0 + K) dimension, unfold, add `ctx_enc_pe` embeddings!
         patches = self.patch2embed(rearrange(imgs, "bsz ctx channels res1 res2 -> (bsz ctx) channels res1 res2"))
-        patches_pe = patches + self.encoder_pe
+        patches_pe = patches + (self.encoder_pe[:, 1:, :] if self.use_cls_token else self.encoder_pe)
         ctx_patches = rearrange(patches_pe, "(bsz ctx) seq embed -> bsz ctx seq embed", ctx=2)
         ctx_patches_pe = ctx_patches + self.ctx_enc_pe[:, :2, ...]
 
         # Add "modality" embeddings to patches & language & flatten out context patches...
         img_ctx_embeddings, lang_embeddings = (
             ctx_patches_pe + self.img_enc_token,
             projected_language + self.lang_enc_token,
         )
         img_embeddings = rearrange(img_ctx_embeddings, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_token_pe = self.cls_token + self.encoder_pe[:, :1, :] + self.img_enc_token[:, 0, :, :]
+            cls_tokens = cls_token_pe.expand(imgs.shape[0], -1, -1)
+            img_embeddings = torch.cat([cls_tokens, img_embeddings], dim=1)
+
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer
         patches_mask = torch.ones_like(img_embeddings[..., -1], dtype=lang_mask.dtype)
         multimodal_embeddings = torch.cat([img_embeddings, lang_embeddings], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([patches_mask, lang_mask], dim=1)  # Merge on sequence length...
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             multimodal_embeddings = block(multimodal_embeddings, multimodal_mask)
         multimodal_embeddings = self.encoder_norm(multimodal_embeddings)
 
-        # Return the full sequence of multimodal embeddings (but ignore 0th frame)...
-        return multimodal_embeddings[:, self.patch2embed.num_patches :]
+        # Return the full sequence of multimodal embeddings (but ignore 0th frame) => the `~` denote what to remove!
+        #   => [CLS] + ~[n_patches x 0th frame]~ + [n_patches x Kth frame] + [max_lang_len language]
+        #   => ~[n_patches x 0th frame]~ + [n_patches x Kth frame] + [max_lang_len language]
+        if self.use_cls_token:
+            return torch.cat(
+                [multimodal_embeddings[:, :1, :], multimodal_embeddings[:, 1 + self.patch2embed.num_patches :, :]], dim=1
+            )
+        else:
+            return multimodal_embeddings[:, self.patch2embed.num_patches :]
 
     def score(self, imgs: torch.Tensor, langs: torch.Tensor, lang_masks: torch.Tensor) -> torch.Tensor:
         """
         Given an example 0-K pair and a set of k language instructions, output scores under the generative language
         model for each instruction.
 
         :param imgs: 0-K pairs --> [1, 2, 3, 224, 224]
         :param langs: Tokenized language input --> [1, k, seq]
         :param lang_masks: Language padding masks --> [1, k, seq]
 
         :return: [1, k] Tensor of LM probabilities given imgs.
         """
         # Blank out the "encoder" language --> just [<CLS> = 101, 0 ...]
-        blank_lang, blank_lang_mask = torch.zeros(1, self.max_lang_len, dtype=torch.int64), torch.zeros(
-            1, self.max_lang_len, dtype=torch.int64
-        )
+        blank_lang = torch.zeros(1, self.max_lang_len, dtype=torch.int64, device=imgs.device)
+        blank_lang_mask = torch.zeros(1, self.max_lang_len, dtype=torch.int64, device=imgs.device)
         blank_lang[0][0], blank_lang_mask[0][0] = 101, 1
 
         # === Encoder Forward ===
         lang_embeddings = self.encode_language(blank_lang, blank_lang_mask)
         projected_language = self.lang2encoder(lang_embeddings)
 
         # Patchify, broadcast position embedding across ctx_len (0 + K) dimension, unfold, add `ctx_enc_pe` embeddings!
         patches = self.patch2embed(rearrange(imgs, "bsz ctx channels res1 res2 -> (bsz ctx) channels res1 res2"))
-        patches_pe = patches + self.encoder_pe
+        patches_pe = patches + (self.encoder_pe[:, 1:, :] if self.use_cls_token else self.encoder_pe)
         ctx_patches = rearrange(patches_pe, "(bsz ctx) seq embed -> bsz ctx seq embed", ctx=2)
         ctx_patches_pe = ctx_patches + self.ctx_enc_pe[:, :2, ...]
 
         # Add "modality" embeddings to patches & language & flatten out context patches...
         img_ctx_embeddings, lang_embeddings = (
             ctx_patches_pe + self.img_enc_token,
             projected_language + self.lang_enc_token,
         )
         img_embeddings = rearrange(img_ctx_embeddings, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_token_pe = self.cls_token + self.encoder_pe[:, :1, :] + self.img_enc_token[:, 0, :, :]
+            cls_tokens = cls_token_pe.expand(imgs.shape[0], -1, -1)
+            img_embeddings = torch.cat([cls_tokens, img_embeddings], dim=1)
+
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer
         patches_mask = torch.ones_like(img_embeddings[..., -1], dtype=blank_lang_mask.dtype)
         multimodal_embeddings = torch.cat([img_embeddings, lang_embeddings], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([patches_mask, blank_lang_mask], dim=1)  # Merge on sequence length...
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             multimodal_embeddings = block(multimodal_embeddings, multimodal_mask)
         multimodal_embeddings = self.encoder_norm(multimodal_embeddings)
 
-        # Split multimodal embedding, remove language, and return only the 0th + Kth frame patches
-        enc_ctx_patches = rearrange(
-            multimodal_embeddings[:, : -blank_lang_mask.shape[-1], ...],
-            "bsz (ctx seq) embed -> bsz ctx seq embed",
-            ctx=2,
-        )
+        # Split multimodal embedding, remove language, and return only the (CLS +) 0th + Kth frame patches
+        enc_patches = multimodal_embeddings[:, : -blank_lang_mask.shape[-1], ...]
 
         # === Encoder =>> Decoder Hand-Off ===
-        enc_patches = repeat(enc_ctx_patches, "b ctx seq embed -> (bsz b) ctx seq embed", bsz=langs.size(0))
-
-        # Get token embeddings -- *NOT CONTEXTUAL* -- for the lang_gen tokens...
+        enc_patches = repeat(enc_patches, "b cseq embed -> (bsz b) cseq embed", bsz=langs.size(0))
         lang_gen_embeddings = self.embed_language(langs)
 
         # === Decoder Forward ===
-        projected_ctx_patches = self.encoder2decoder(enc_patches)
+        projected_patches = self.encoder2decoder(enc_patches)
         projected_lang_gen = self.lang2decoder(lang_gen_embeddings)
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            projected_ctx_patches = rearrange(
+                projected_patches[:, 1:, :], "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2
+            )
+        else:
+            projected_ctx_patches = rearrange(projected_patches, "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2)
+
         # Add position embeddings, `ctx_dec_pe` embeddings, and flatten patches for Transformer...
-        decoder_ctx_patches_pe = projected_ctx_patches + self.decoder_pe[None, ...]
+        decoder_ctx_patches_pe = projected_ctx_patches + (
+            self.decoder_pe[None, ...] if not self.use_cls_token else self.decoder_pe[None, :, 1:, :]
+        )
         decoder_ctx_patches = decoder_ctx_patches_pe + self.ctx_dec_pe[:, :2, ...]
         decoder_patches = rearrange(decoder_ctx_patches, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            # Add back <CLS> Token from `projected_patches[:, :1, :]`
+            cls_embedding = projected_patches[:, :1, :] + self.decoder_pe[:, :1, :]
+            decoder_patches = torch.cat([cls_embedding, decoder_patches], dim=1)
+
         # Add language -> create "mask" by multiply padding by self.prefix_mask
         decoder_patches_mask = torch.ones_like(decoder_patches[..., -1], dtype=lang_masks.dtype)
         multimodal_embedding = torch.cat([decoder_patches, projected_lang_gen], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([decoder_patches_mask, lang_masks], dim=1)  # Merge on sequence length...
 
         # Compute prefix_padded_mask
         prefix_padded_mask = rearrange(multimodal_mask, "bsz seq -> bsz 1 seq 1") * self.prefix_mask
@@ -438,86 +479,120 @@
     def forward_encoder(
         self,
         img_ctx: torch.Tensor,
         lang_con: torch.Tensor,
         lang_con_mask: torch.Tensor,
         mask_ratio: Optional[float] = None,
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        lang_embeddings = self.encode_language(lang_con, lang_con_mask)
+        projected_lang = self.lang2encoder(lang_embeddings)
+
+        # Reshape image context to apply masking *identically*
+
         # Patchify, broadcast position embedding across ctx_len (0 + K) dimension, unfold, add `ctx_enc_pe` embeddings!
         patches = self.patch2embed(rearrange(img_ctx, "bsz ctx channels res1 res2 -> (bsz ctx) channels res1 res2"))
-        patches_pe = patches + self.encoder_pe
+        patches_pe = patches + (self.encoder_pe if not self.use_cls_token else self.encoder_pe[:, 1:, :])
         ctx_patches = rearrange(patches_pe, "(bsz ctx) seq embed -> bsz ctx seq embed", ctx=2)
         ctx_patches_pe = ctx_patches + self.ctx_enc_pe[:, :2, ...]
 
         # Create mask (and go ahead and mask out patches at the same time)
         visible_ctx_patches, mask, restore_idxs = self.mask(ctx_patches_pe, mask_ratio)
 
         # Add "modality" embeddings to patches & language & flatten out context patches...
-        visible_ctx_patches, lang = visible_ctx_patches + self.img_enc_token, lang_con + self.lang_enc_token
+        visible_ctx_patches, lang = visible_ctx_patches + self.img_enc_token, projected_lang + self.lang_enc_token
         visible_patches = rearrange(visible_ctx_patches, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            cls_token_pe = self.cls_token + self.encoder_pe[:, :1, :] + self.img_enc_token[:, 0, :, :]
+            cls_tokens = cls_token_pe.expand(img_ctx.shape[0], -1, -1)
+            visible_patches = torch.cat([cls_tokens, visible_patches], dim=1)
+
         # Create "dummy" visible mask, concatenate image patches & language, feed to Transformer...
         visible_mask = torch.ones_like(visible_patches[..., -1], dtype=lang_con_mask.dtype)
         multimodal_embedding = torch.cat([visible_patches, lang], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([visible_mask, lang_con_mask], dim=1)  # Merge on sequence length...
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             multimodal_embedding = block(multimodal_embedding, multimodal_mask)
         multimodal_embedding = self.encoder_norm(multimodal_embedding)
 
-        # Split multimodal embedding, remove language, and return only the visible ctx (0th + Kth frame) patches!
-        visible_ctx_patches = rearrange(
-            multimodal_embedding[:, : -lang_con_mask.shape[-1], ...], "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2
-        )
-        return visible_ctx_patches, mask, restore_idxs
+        # Split multimodal embedding, remove language, return the visible ctx (0th + Kth frame) patches (+ <CLS>)!
+        visible_patches = multimodal_embedding[:, : -lang_con_mask.shape[-1], ...]
+        return visible_patches, mask, restore_idxs
 
     def forward_decoder(
         self,
-        visible_ctx_patches: torch.Tensor,
+        visible_patches: torch.Tensor,
         restore_idxs: torch.Tensor,
         lang_gen: torch.Tensor,
         lang_gen_mask: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
-        # Project patches & lang_gen into decoder embedding dimension (visible_ctx_patches :: [bsz, 2, seq, enc_embed])
-        projected_ctx_patches = self.encoder2decoder(visible_ctx_patches)
+        # Project patches & lang_gen into decoder dimension (visible_patches :: [bsz, (CLS) + 2 * seq, enc_embed])
+        projected_patches = self.encoder2decoder(visible_patches)
         projected_lang_gen = self.lang2decoder(lang_gen)
+        visible_per_frame = (projected_patches.shape[1] - (1 if self.use_cls_token else 0)) // 2
 
         # Add Mask Tokens to Sequence and Unshuffle
-        mask_tokens = self.mask_token.repeat(
-            projected_ctx_patches.shape[0], 2, restore_idxs.shape[1] - visible_ctx_patches.shape[2], 1
-        )
-        concatenated_ctx_patches = torch.cat([projected_ctx_patches, mask_tokens], dim=2)
-        unshuffled_ctx_patches = torch.gather(
-            concatenated_ctx_patches,
-            dim=2,
-            index=restore_idxs[:, None, ..., None].repeat(1, 2, 1, self.decoder_embed_dim),
-        )
+        mask_tokens = self.mask_token.repeat(projected_patches.shape[0], 2, restore_idxs.shape[1] - visible_per_frame, 1)
+
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            # Remove CLS Token as part of "unshuffling"
+            projected_ctx_patches = rearrange(
+                projected_patches[:, 1:, :], "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2
+            )
+            no_cls_concatenated_ctx_patches = torch.cat([projected_ctx_patches, mask_tokens], dim=2)
+            unshuffled_ctx_patches = torch.gather(
+                no_cls_concatenated_ctx_patches,
+                dim=2,
+                index=restore_idxs[:, None, ..., None].repeat(1, 2, 1, self.decoder_embed_dim),
+            )
+        else:
+            projected_ctx_patches = rearrange(projected_patches, "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2)
+            concatenated_ctx_patches = torch.cat([projected_ctx_patches, mask_tokens], dim=2)
+            unshuffled_ctx_patches = torch.gather(
+                concatenated_ctx_patches,
+                dim=2,
+                index=restore_idxs[:, None, ..., None].repeat(1, 2, 1, self.decoder_embed_dim),
+            )
 
         # Add position embeddings, `ctx_dec_pe` embeddings, and flatten patches for Transformer...
-        decoder_ctx_patches_pe = unshuffled_ctx_patches + self.decoder_pe[None, ...]
+        decoder_ctx_patches_pe = unshuffled_ctx_patches + (
+            self.decoder_pe[None, ...] if not self.use_cls_token else self.decoder_pe[None, :, 1:, :]
+        )
         decoder_ctx_patches = decoder_ctx_patches_pe + self.ctx_dec_pe[:, :2, ...]
         decoder_patches = rearrange(decoder_ctx_patches, "bsz ctx seq embed -> bsz (ctx seq) embed")
 
+        # (Optional) <CLS> Token Handling
+        if self.use_cls_token:
+            # Add back <CLS> Token from `projected_patches[:, :1, :]`
+            cls_embedding = projected_patches[:, :1, :] + self.decoder_pe[:, :1, :]
+            decoder_patches = torch.cat([cls_embedding, decoder_patches], dim=1)
+
         # Add language -> create "mask" by multiply padding by self.prefix_mask
         decoder_patches_mask = torch.ones_like(decoder_patches[..., -1], dtype=lang_gen_mask.dtype)
         multimodal_embedding = torch.cat([decoder_patches, projected_lang_gen], dim=1)  # Merge on sequence length...
         multimodal_mask = torch.cat([decoder_patches_mask, lang_gen_mask], dim=1)  # Merge on sequence length...
 
         # Compute prefix_padded_mask
         prefix_padded_mask = rearrange(multimodal_mask, "bsz seq -> bsz 1 seq 1") * self.prefix_mask
 
         # Apply Transformer Blocks...
         for block in self.decoder_blocks:
             multimodal_embedding = block(multimodal_embedding, prefix_padded_mask)
         multimodal_embedding = self.decoder_norm(multimodal_embedding)
 
         # Split multimodal embedding into patches and language...
+        patches_ctx = multimodal_embedding[:, : -lang_gen_mask.shape[-1], ...]
         patches = rearrange(
-            multimodal_embedding[:, : -lang_gen_mask.shape[-1], ...], "bsz (ctx seq) embed -> bsz ctx seq embed", ctx=2
+            patches_ctx if not self.use_cls_token else patches_ctx[:, 1:, :],
+            "bsz (ctx seq) embed -> bsz ctx seq embed",
+            ctx=2,
         )
         lang = multimodal_embedding[:, -lang_gen_mask.shape[-1] :, ...]
 
         # Project each up to the output space...
         reconstructions = self.decoder_patch_prediction(patches)
         generations = self.decoder_lang_prediction(lang)
 
@@ -588,16 +663,15 @@
                 f"k_loss: {k_loss.isnan().any()} -- "
                 f"reconstruction_loss: {reconstruction_loss.isnan().any()} -- "
                 f"ce_loss: {ce_loss.isnan().any()} -- "
                 f"per_token_loss: {per_token_loss.isnan().any()} -- "
                 f"lang_example_loss: {lang_example_loss.isnan().any()} -- "
                 f"lang_loss: {lang_loss.isnan().any()}"
             )
-            import os
-            os._exit(0)
+            exit(1)
             # fmt: on
 
         # Compute weighted loss...
         loss = self.mae_weight * reconstruction_loss + self.lm_weight * lang_loss
         return loss, reconstruction_loss, lang_loss, zero_loss, k_loss
 
     def forward(
@@ -621,22 +695,15 @@
         :param lang_gen_mask: A [bsz, seq_len] binary mask tensor to indicate padding/null in `lang_gen`.
         :param lang_gen_weight: A [bsz] tensor of per-example weights to indicate when to 0 `lm` loss.
         :param mask_ratio: Optional masking ratio to use instead of the default.
 
         :return: Tuple of losses and intermediates, as follows:
             > (combined loss, reconstruction loss, lm loss, [reconstruction loss per frame in {0, K}])
         """
-        # First, get precomputed language embeddings & project to encoder_embed_dim; language only used in encoder!
-        lang_embeddings = self.encode_language(lang_con, lang_con_mask)
-        projected_language = self.lang2encoder(lang_embeddings)
-
-        # Reshape image context to apply masking *identically*
-        visible_ctx_patches, mask, restore_idxs = self.forward_encoder(
-            imgs, projected_language, lang_con_mask, mask_ratio
-        )
+        visible_ctx_patches, mask, restore_idxs = self.forward_encoder(imgs, lang_con, lang_con_mask, mask_ratio)
 
         # Get token embeddings -- *NOT CONTEXTUAL* -- for the lang_gen tokens...
         lang_gen_embeddings = self.embed_language(lang_gen)
 
         # Run patches, and lang_gen through decoder --> note that we need a causal mask on language generation...
         ctx_reconstructions, generated_language = self.forward_decoder(
             visible_ctx_patches, restore_idxs, lang_gen_embeddings, lang_gen_mask
```

### Comparing `voltron-robotics-1.0.3/voltron/models/materialize.py` & `voltron-robotics-1.1.0/voltron/models/materialize.py`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/voltron/models/reproductions/vmvp.py` & `voltron-robotics-1.1.0/voltron/models/reproductions/vmvp.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         """Perform per-sample random masking by shuffling :: uses argsort random noise to identify masked patches"""
         bsz, n_patches, embed_dim = patches.shape
         if mask_ratio is not None:
             n_keep = int(n_patches * (1 - mask_ratio))
         else:
             n_keep = int(n_patches * (1 - self.mask_ratio))
 
-        # Sample some noise of n_patches size, argsort to get shuffled IDs (keep small), argsort again to get "unshuffle"
+        # Sample some noise of n_patches size, argsort to get shuffled IDs (keep small), argsort again to "unshuffle"
         #   > For clarity -- argsort is an invertible transformation (if argsort `restore`, recovers `shuffle`)
         shuffle_idxs = torch.argsort(torch.rand(bsz, n_patches, device=patches.device), dim=1)
         restore_idxs = torch.argsort(shuffle_idxs, dim=1)
 
         # Get "keep" (visible) patches
         visible_patches = torch.gather(patches, dim=1, index=shuffle_idxs[:, :n_keep, None].repeat(1, 1, embed_dim))
 
@@ -183,20 +183,16 @@
 
     def encode(self, img: torch.Tensor) -> torch.Tensor:
         """Run a single image through the MAE and extract patch embeddings."""
 
         # Note: All of this code is taken near-verbatim from the MVP repository...
         #   > Ref: https://github.com/ir413/mvp/blob/master/mvp/backbones/vit.py#L30
         patches = self.patch2embed(img)
-        patches_pe = patches + self.encoder_pe[:, 1:, :]
-
-        # Add CLS Token
-        cls_token = self.cls_token + self.encoder_pe[:, :1, :]
-        cls_tokens = cls_token.expand(img.shape[0], -1, -1)
-        cls_patches = torch.cat([cls_tokens, patches_pe], dim=1)
+        cls_tokens = self.cls_token.expand(img.shape[0], -1, -1)
+        cls_patches = torch.cat([cls_tokens, patches]) + self.encoder_pe
 
         # Apply Transformer Blocks...
         for block in self.encoder_blocks:
             cls_patches = block(cls_patches)
         cls_patches = self.encoder_norm(cls_patches)
         return cls_patches
 
@@ -224,21 +220,21 @@
 
     def forward_decoder(self, visible_patches: torch.Tensor, restore_idxs: torch.Tensor) -> torch.Tensor:
         # Project patches into decoder embedding dimension
         projected_patches = self.encoder2decoder(visible_patches)
 
         # Add Mask Tokens to Sequence
         mask_tokens = self.mask_token.repeat(
-            projected_patches.shape[0], restore_idxs.shape[1] - visible_patches.shape[1], 1
+            projected_patches.shape[0], restore_idxs.shape[1] - visible_patches.shape[1] + 1, 1
         )
 
         # Remove & add back CLS Token as part of the "unshuffling"
         concatenated_patches = torch.cat([projected_patches[:, 1:, :], mask_tokens], dim=1)  # Skip CLS Token
         unshuffled_patches = torch.gather(
-            concatenated_patches, dim=1, index=restore_idxs[..., None].repeat(1, 1, projected_patches.shape[2])
+            concatenated_patches, dim=1, index=restore_idxs[..., None].repeat(1, 1, self.decoder_embed_dim)
         )
         cls_unshuffled_patches = torch.cat([projected_patches[:, :1, :], unshuffled_patches], dim=1)  # Add CLS Token
 
         # Add Position Embeddings
         cls_decoder_patches = cls_unshuffled_patches + self.decoder_pe
 
         # Apply Transformer Blocks...
```

### Comparing `voltron-robotics-1.0.3/voltron/models/reproductions/vr3m.py` & `voltron-robotics-1.1.0/voltron/models/reproductions/vr3m.py`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/voltron/models/reproductions/vrn3m.py` & `voltron-robotics-1.1.0/voltron/models/reproductions/vrn3m.py`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/voltron/models/util/extraction.py` & `voltron-robotics-1.1.0/voltron/models/util/extraction.py`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/voltron/models/util/optimization.py` & `voltron-robotics-1.1.0/voltron/models/util/optimization.py`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/voltron/models/util/transformer.py` & `voltron-robotics-1.1.0/voltron/models/util/transformer.py`

 * *Files identical despite different names*

### Comparing `voltron-robotics-1.0.3/voltron/overwatch/overwatch.py` & `voltron-robotics-1.1.0/voltron/overwatch/overwatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 "class": "logging.FileHandler",
                 "formatter": "simple-file",
                 "filename": "${hydra.job.name}.log",
             },
         }
     )
     root: Dict[str, Any] = field(default_factory=lambda: {"level": "INFO", "handlers": ["console", "file"]})
-    disable_existing_loggers: bool = False
+    disable_existing_loggers: bool = True
 
 
 # Standard Overwatch Variant --> Performant, no bells & whistles
 @dataclass
 class OverwatchStandard:
     version: int = 1
     formatters: Dict[str, Any] = field(default_factory=lambda: {"simple": {"format": FORMATTER, "datefmt": DATEFMT}})
@@ -54,8 +54,8 @@
                 "class": "logging.FileHandler",
                 "formatter": "simple",
                 "filename": "${hydra.job.name}.log",
             },
         }
     )
     root: Dict[str, Any] = field(default_factory=lambda: {"level": "INFO", "handlers": ["console", "file"]})
-    disable_existing_loggers: bool = False
+    disable_existing_loggers: bool = True
```

### Comparing `voltron-robotics-1.0.3/voltron/preprocessing/process.py` & `voltron-robotics-1.1.0/voltron/preprocessing/v1/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 
 Utility functions for serializing datasets in multiple passes, using multiprocessing for efficient parallelization.
 Exposes a three-phase sequence for preprocessing:
     - Phase I: Read in raw videos (and language), serialize *all extracted* frames to a subdirectory for easy retrieval.
     - Phase II: Given image paths and language, assemble language statistics & pre-tokenize for easy batching.
     - Phase III: Given a total number of "conceivable epochs", create data-controlled "epoch" sets for each model.
 
-This script tries to be smart where it can, using multiprocessing.Pool in Phase I to speed-up the serialization
+This script tries to be smart where it can, using multiprocessing.Pool in Phase I to speed up the serialization
 process. It also tries to be somewhat safe & efficient, producing idempotent resumes.
+
+Note :: This code represents the `v1` (initial release) preprocessing flow; this will eventually be deprecated!
 """
 import json
 import logging
 import multiprocessing as mp
 import os
 import shutil
 from functools import partial
 from pathlib import Path
 from typing import Tuple
 
 import torch
 from rich.progress import track
 from transformers import AutoTokenizer
 
-from voltron.preprocessing.transforms import get_pre_transform
-from voltron.preprocessing.utils import do_dry_run, precompute_epoch, process_video
+from voltron.preprocessing.v1.transforms import get_pre_transform
+from voltron.preprocessing.v1.utils import do_dry_run, precompute_epoch, process_video
 
 # Grab Logger
 overwatch = logging.getLogger(__file__)
 
 
 def preprocess_videos(
     name: str,
@@ -44,15 +46,15 @@
     if name == "sth-sth-v2":
         # Overview of Return Values:
         #   `t_registry` and `v_registry` =>> store mappings of "vid_id" -> {metadata}
         #   `t_dir` and `v_dir` =>> store "processed data" (extracted frames)
         t_dir, v_dir = Path(artifact_path) / name / "train", Path(artifact_path) / name / "val"
         t_registry, v_registry = t_dir / "registry.json", v_dir / "registry.json"
 
-        # Short-Circuit / Cache Logic
+        # Short-Circuit / Caching Logic
         if t_registry.exists() and v_registry.exists():
             return t_registry, v_registry, t_dir, v_dir
 
         # Setup / Book-Keeping
         os.makedirs(t_dir, exist_ok=True)
         os.makedirs(v_dir, exist_ok=True)
```

### Comparing `voltron-robotics-1.0.3/voltron/preprocessing/stream_datasets.py` & `voltron-robotics-1.1.0/voltron/datasets/v1/stream_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Core PyTorch Datasets for the various "flavors" of data used by the various models under study. Crucially, each dataset
 loads from the corresponding "batch" serialized files, that define the exact data to use.
 
 Notably, these serialized files control exactly what data is seen by *all* methods **across epochs.** Using them is
 fairly critical to reproducibility & fair comparison.
 
-This specific file contains logic for a "streaming" DataLoader; data is fetched (within the dataloader, by each
+This specific file contains logic for a "streaming" Dataset; data is fetched (within the dataloader, by each
 worker) via an open connection over the network to a GCS bucket, materializing data as raw BytesIO objects fed to
 PIL.Image constructors.
 """
 import json
 import os
 from io import BytesIO
 from pathlib import Path
@@ -25,15 +25,15 @@
 from google.resumable_media._helpers import _LOGGER
 from PIL import Image, UnidentifiedImageError
 from torch.utils.data import Dataset, get_worker_info
 from torchvision.io import read_image
 from torchvision.transforms import Compose
 from torchvision.transforms.functional import pil_to_tensor
 
-from voltron.preprocessing.transforms import get_online_transform
+from voltron.preprocessing.v1.transforms import get_online_transform
 from voltron.util.distributed import get_rank
 
 # NOTE --> IF STREAMING JPEGS, WE NEED TO USE PILLOW TO READ FILES (w/o extracting locally...)
 #   =>> Instead of `read_image(file)` assume we have "fname" and open fileobj (as BytesIO) -- remember to `seek(0)`
 #
 # > from PIL import Image
 # > from torchvision.transforms.functional import pil_to_tensor
```

### Comparing `voltron-robotics-1.0.3/voltron/preprocessing/transforms.py` & `voltron-robotics-1.1.0/voltron/preprocessing/v1/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import cv2
 import numpy as np
 import torch
 from torchvision.transforms import Compose, ConvertImageDtype, Lambda, Normalize
 
 
-# Definitions of Video Transformations (Reference: something-something-v2-baseline)
+# Definitions of Video Transformations (Reference: `something-something-v2-baseline`)
 class ComposeMix:
     def __init__(self, transforms):
         self.transforms = transforms
 
     def __call__(self, imgs):
         for transformation, scope in self.transforms:
             if scope == "img":
@@ -45,14 +45,19 @@
     def __init__(self, size):
         self.size = size
 
     def __call__(self, img):
         return cv2.resize(img, tuple(self.size))
 
 
+def identity(x):
+    """Transform needs to be pickleable for multiprocessing.spawn()."""
+    return x.float()
+
+
 def get_pre_transform(dataset: str, resolution: int, scale_factor: float = 1.1) -> ComposeMix:
     """Defines a `pre` transform to be applied *when serializing the images* (first pass)."""
     if dataset == "sth-sth-v2":
         if scale_factor > 1:
             transform = ComposeMix(
                 [
                     [Scale((int(resolution * scale_factor), int(resolution * scale_factor))), "img"],
@@ -67,19 +72,14 @@
             )
 
         return transform
     else:
         raise NotImplementedError(f"(Pre) transforms for dataset `{dataset}` not yet implemented!")
 
 
-def identity(x):
-    """Transform needs to be pickleable for multiprocessing.spawn()."""
-    return x.float()
-
-
 def get_online_transform(dataset: str, model_arch: str, normalization: Tuple[Any, Any]) -> Compose:
     """Defines an `online` transform to be applied *when batching the images* (during training/validation)."""
     if dataset == "sth-sth-v2":
         # Note: R3M does *not* expect normalized 0-1 (then ImageNet normalized) images --> drop the identity.
         if model_arch in {"v-r3m", "v-rn3m"}:
             return Compose([Lambda(identity)])
         else:
```

### Comparing `voltron-robotics-1.0.3/voltron/preprocessing/utils.py` & `voltron-robotics-1.1.0/voltron/preprocessing/v1/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import av
 import cv2
 import numpy as np
 from hurry.filesize import alternative, size
 from rich.progress import track
 from tqdm import tqdm
 
-from voltron.preprocessing.transforms import ComposeMix
+from voltron.preprocessing.v1.transforms import ComposeMix
 
 # Grab Logger
 overwatch = logging.getLogger(__file__)
 logging.getLogger("libav").setLevel(logging.ERROR)
 
 
 # Videos are saved as `train_dir/{vid}/{vid}_idx={i}.jpg
```

### Comparing `voltron-robotics-1.0.3/voltron/util/checkpointing.py` & `voltron-robotics-1.1.0/voltron/util/v1/checkpointing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 """
 checkpointing.py
 
-Core utility class for handling model/optimizer serialization & checkpointing... including (eventually) resume from
-checkpoint logic.
+XLA-specific utility class for handling model/optimizer serialization & checkpointing.
 
 Support the following strategies:
     - (k, -1, -1) --> Keep only the most recent "k" epoch checkpoints
     - (k, m, -1) --> Keep the most recent "k" epoch checkpoints and *every* m epoch checkpoint
     - (k, m, s = 2500) --> Keep "k" and "m" subject to above, but also keep *s* step checkpoints for current epoch
 """
 import os
 from collections import deque
 from pathlib import Path
 from typing import Any, Optional, Tuple
 
-import wandb
+import torch.nn as nn
+from torch.optim.optimizer import Optimizer
 
 
 class FixedDeck(deque):
-    def __init__(self, maxlen):
+    def __init__(self, maxlen: int) -> None:
         super().__init__(maxlen=maxlen)
 
     def append(self, x: Any) -> Any:
         pop_value = None
         if self.__len__() == self.maxlen:
             pop_value = self.__getitem__(0)
 
         # Perform parent append and return popped value, if any!
         super().append(x)
         return pop_value
 
 
-class CheckpointSaver:
-    def __init__(self, strategy: Tuple[int, int, int], run_dir: str, accelerator: str):
+class XLACheckpointSaver:
+    def __init__(self, strategy: Tuple[int, int, int], run_dir: str) -> None:
         """
-        Create a checkpoint saver with the provided strategy that saves to the given path, with handling for the
-        specific hardware accelerator.
+        Create a checkpoint saver with the provided strategy that saves to the given path, with XLA-specific handling.
 
         :param strategy: Strategy, following the (k, -1, -1) -- (k, m, -1) -- (k, m, s) description above.
         :param run_dir: Path to root of `run_dir`
-        :param accelerator: Hardware accelerator to run on -- TODO :: Only TPUs supported right now!
         """
         import torch_xla.core.xla_model as xm
 
-        (self.k, self.m, self.s), self.run_dir, self.accelerator = strategy, run_dir, accelerator
+        (self.k, self.m, self.s), self.run_dir = strategy, run_dir
         self.recents, self.intervals, self.step_checkpoints = FixedDeck(maxlen=self.k), set(), set()
 
         # If `self.s` is -1 --> disable step_checkpoints
         self.enable_step = self.s != -1
 
         # Create "checkpoints" subdirectory
         self.path = Path(run_dir) / "checkpoints"
@@ -60,16 +58,16 @@
         # Create Saver
         xm.master_print(f"Created Saver w/ `k` = {self.k}, `m` = {self.m}`, `s` = {self.s}!")
 
     def save(
         self,
         epoch: int,
         is_local_step: bool,
-        model: Any,
-        optimizer: Any,
+        model: nn.Module,
+        optimizer: Optimizer,
         duration: int,
         local_step: Optional[int] = None,
         train_loss: Optional[float] = None,
         val_loss: Optional[float] = None,
     ) -> None:
         """Performs the save operation, unlinking existing stale checkpoints, if necessary."""
         import torch_xla.core.xla_model as xm
@@ -105,10 +103,7 @@
                 while len(self.step_checkpoints) > 0:
                     os.remove(self.step_checkpoints.pop())
 
                 # Finally, recency add & unlink/delete if necessary
                 to_remove = self.recents.append(checkpoint)
                 if to_remove is not None and to_remove not in self.intervals:
                     os.remove(to_remove)
-
-                # Extra Redundancy --> Save Model to W&B...
-                wandb.save(str(checkpoint))
```

### Comparing `voltron-robotics-1.0.3/voltron/util/distributed.py` & `voltron-robotics-1.1.0/voltron/util/v1/distributed.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -20,38 +20,14 @@
 import torch
 from torch.utils.data import Dataset
 from torch.utils.data.distributed import DistributedSampler
 
 T_co = TypeVar("T_co", covariant=True)
 
 
-def xla_available() -> bool:
-    try:
-        return find_spec("torch_xla") is not None
-    except ModuleNotFoundError:
-        return False
-
-
-def get_rank() -> int:
-    """Returns the global rank [0, World Size) of the current process."""
-    if xla_available():
-        import torch_xla.core.xla_model as xm
-
-        # By default, if XLA is available, assume we're running under XMP Spawn
-        return xm.get_ordinal()
-
-    # Try to get rank via torch.distributed, but catch error if only single process
-    try:
-        return torch.distributed.get_rank()
-
-    # RuntimeError => not running distributed (single process)
-    except RuntimeError:
-        return 0
-
-
 class ResumeableDistributedSampler(DistributedSampler):
     def __init__(
         self,
         seen_examples: int,
         resume_epoch: int,
         dataset: Dataset,
         num_replicas: int,
@@ -84,7 +60,31 @@
 
     def set_epoch(self, epoch: int) -> None:
         # If epoch != self.resume_epoch --> we're in "regular DistributedSampler" mode (just a wrapper class)
         #   > Intuition: We should *only* truncate examples on the first epoch upon resuming!
         self.epoch = epoch
         if self.epoch != self.resume_epoch:
             self.do_resume = False
+
+
+def xla_available() -> bool:
+    try:
+        return find_spec("torch_xla") is not None
+    except ModuleNotFoundError:
+        return False
+
+
+def get_rank() -> int:
+    """Returns the global rank [0, World Size) of the current process."""
+    if xla_available():
+        import torch_xla.core.xla_model as xm
+
+        # By default, if XLA is available, assume we're running under XMP Spawn
+        return xm.get_ordinal()
+
+    # Try to get rank via torch.distributed, but catch error if only single process
+    try:
+        return torch.distributed.get_rank()
+
+    # RuntimeError => not running distributed (single process)
+    except RuntimeError:
+        return 0
```

### Comparing `voltron-robotics-1.0.3/voltron/util/random.py` & `voltron-robotics-1.1.0/voltron/util/v1/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import random
 from typing import Callable
 
 import numpy as np
 import torch
 
-from voltron.util.distributed import get_rank
+from voltron.util.v1.distributed import get_rank
 
 
 def set_global_seed(seed: int) -> Callable[[int], None]:
     """Sets seed for all randomness libraries (mostly random, numpy, torch) and produces a `worker_init_fn`"""
     assert np.iinfo(np.uint32).min < seed < np.iinfo(np.uint32).max, "Seed outside the np.uint32 bounds!"
 
     # Set Seed as an Environment Variable
```

### Comparing `voltron-robotics-1.0.3/voltron/util/xla_logger.py` & `voltron-robotics-1.1.0/voltron/util/v1/xla_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     average_step_time = np.mean(list(step_times))
 
     # Console Logging --> Just log the aggregated train loss...
     xm.master_print(
         f"Epoch {epoch:03d}, Global Step {global_step:06d} || LR :: {lr:.6f} -- Train Loss :: {train_loss:.4f}"
     )
 
-    # Log ot Weights & Biases + JSONL
+    # Log to Weights & Biases + JSONL
     blob = {
         "Pretrain/Step": global_step,
         "Pretrain/Epoch": epoch,
         "Pretrain/V-MVP Train Loss": train_loss.item(),
         "Pretrain/Reconstruction Loss": reconstruction_loss.item(),
         "Pretrain/Learning Rate": lr,
         "Pretrain/Step Time": average_step_time,
```

### Comparing `voltron-robotics-1.0.3/voltron_robotics.egg-info/PKG-INFO` & `voltron-robotics-1.1.0/voltron_robotics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltron-robotics
-Version: 1.0.3
+Version: 1.1.0
 Summary: Voltron: Language-Driven Representation Learning for Robotics.
 Author-email: Siddharth Karamcheti <skaramcheti@cs.stanford.edu>
 License: MIT License
         
         Copyright (c) 2021-present, Siddharth Karamcheti and other contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,15 +49,15 @@
 <div align="center">
     <img src="https://raw.githubusercontent.com/siddk/voltron-robotics/main/docs/assets/voltron-banner.png" alt="Voltron Logo"/>
 </div>
 
 <div align="center">
 
 [![arXiv](https://img.shields.io/badge/arXiv-2302.12766-df2a2a.svg?style=for-the-badge)](https://arxiv.org/abs/2302.12766)
-[![PyTorch](https://img.shields.io/badge/PyTorch-1.12.0-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org/get-started/previous-versions/#v1120)
+[![PyTorch](https://img.shields.io/badge/PyTorch-2.0.0-EE4C2C.svg?style=for-the-badge&logo=pytorch)](https://pytorch.org/get-started/locally/)
 [![Code Style: Black](https://img.shields.io/badge/Code%20Style-Black-000000?style=for-the-badge)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/badge/%E2%9A%A1%EF%B8%8F-Ruff-orange?style=for-the-badge)](https://github.com/charliermarsh/ruff)
 ![License](https://img.shields.io/github/license/siddk/lila?color=blueviolet&style=for-the-badge)
 
 </div>
 
 ---
@@ -73,16 +73,16 @@
 ## Quickstart
 
 This repository is built with PyTorch; while specified as a dependency for the package, we highly recommend that
 you install the desired version (e.g., with accelerator support) for your given hardware and environment
 manager (e.g., `conda`).
 
 PyTorch installation instructions [can be found here](https://pytorch.org/get-started/locally/). This repository
-should work with PyTorch >= 1.12, but has only been thoroughly tested with PyTorch 1.12.0, Torchvision 0.13.0,
-Torchaudio 0.12.0.
+should work with PyTorch >= 1.12. Releases before 1.1.0 have been thoroughly tested with PyTorch 1.12.0,
+Torchvision 0.13.0, and Torchaudio 0.12.0. **Note**: Releases 1.1.0 and after *assume PyTorch 2.0*!
 
 Once PyTorch has been properly installed, you can install this package via PyPI, and you're off!
 
 ```bash
 pip install voltron-robotics
 ```
 
@@ -168,15 +168,15 @@
 language embeddings, or only the image patch embeddings.
 
 **Note:** For the API for the non-Voltron models (e.g., R-MVP, R-R3M), take a look at
 [`examples/verify.py`](examples/verify.py); this file shows how representations from *every* model can be extracted.
 
 ### Adaptation
 
-See [`examples/adapt.py`](examples/adapt.py) and the [`voltron-evaluation`](https://github.com/siddk/voltron-evaluation)
+See [`examples/usage.py`](examples/usage.py) and the [`voltron-evaluation`](https://github.com/siddk/voltron-evaluation)
 repository for more examples on the various ways to adapt/use Voltron representations.
 
 ---
 
 ## Contributing
 
 Before committing to the repository, make sure to set up your dev environment!
```

### Comparing `voltron-robotics-1.0.3/voltron_robotics.egg-info/SOURCES.txt` & `voltron-robotics-1.1.0/voltron_robotics.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-examples/adapt.py
-examples/verify.py
+examples/usage.py
+examples/pretrain/preprocess.py
+examples/pretrain/pretrain.py
+examples/verification/verify.py
 examples/xla-reference/xpreprocess.py
 examples/xla-reference/xpretrain.py
 voltron/__init__.py
 voltron/conf/__init__.py
 voltron/conf/accelerators.py
 voltron/conf/datasets.py
 voltron/conf/models.py
 voltron/conf/tracking.py
+voltron/datasets/__init__.py
+voltron/datasets/datasets.py
+voltron/datasets/v1/__init__.py
+voltron/datasets/v1/stream_datasets.py
 voltron/models/__init__.py
+voltron/models/instantiate.py
 voltron/models/materialize.py
 voltron/models/core/__init__.py
 voltron/models/core/vcond.py
 voltron/models/core/vdual.py
 voltron/models/core/vgen.py
 voltron/models/reproductions/__init__.py
 voltron/models/reproductions/vmvp.py
@@ -25,21 +32,28 @@
 voltron/models/util/__init__.py
 voltron/models/util/extraction.py
 voltron/models/util/optimization.py
 voltron/models/util/transformer.py
 voltron/overwatch/__init__.py
 voltron/overwatch/overwatch.py
 voltron/preprocessing/__init__.py
+voltron/preprocessing/core.py
 voltron/preprocessing/process.py
-voltron/preprocessing/stream_datasets.py
 voltron/preprocessing/transforms.py
-voltron/preprocessing/utils.py
+voltron/preprocessing/v1/__init__.py
+voltron/preprocessing/v1/process.py
+voltron/preprocessing/v1/transforms.py
+voltron/preprocessing/v1/utils.py
 voltron/util/__init__.py
 voltron/util/checkpointing.py
-voltron/util/distributed.py
-voltron/util/random.py
-voltron/util/xla_logger.py
+voltron/util/metrics.py
+voltron/util/utilities.py
+voltron/util/v1/__init__.py
+voltron/util/v1/checkpointing.py
+voltron/util/v1/distributed.py
+voltron/util/v1/random.py
+voltron/util/v1/xla_logger.py
 voltron_robotics.egg-info/PKG-INFO
 voltron_robotics.egg-info/SOURCES.txt
 voltron_robotics.egg-info/dependency_links.txt
 voltron_robotics.egg-info/requires.txt
 voltron_robotics.egg-info/top_level.txt
```

