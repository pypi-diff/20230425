# Comparing `tmp/netin-1.0.5.7.tar.gz` & `tmp/netin-1.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.7.tar", last modified: Sun Apr 23 15:08:11 2023, max compression
+gzip compressed data, was "netin-1.0.5.8.tar", last modified: Tue Apr 25 12:30:42 2023, max compression
```

## Comparing `netin-1.0.5.7.tar` & `netin-1.0.5.8.tar`

### file list

```diff
@@ -1,66 +1,77 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.7/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.7/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 15:08:11.201018 netin-1.0.5.7/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2502 2023-04-23 08:16:29.000000 netin-1.0.5.7/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.7/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.7/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.7/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/notebooks/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2947 2023-04-19 11:08:57.000000 netin-1.0.5.7/examples/notebooks/deleteme.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.7/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.7/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.7/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.7/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-23 14:55:29.000000 netin-1.0.5.7/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.7/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      440 2023-04-23 11:31:23.000000 netin-1.0.5.7/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5060 2023-04-23 14:19:48.000000 netin-1.0.5.7/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13472 2023-04-23 14:19:40.000000 netin-1.0.5.7/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3074 2023-04-23 14:19:52.000000 netin-1.0.5.7/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4701 2023-04-23 14:19:44.000000 netin-1.0.5.7/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    21657 2023-04-23 14:52:02.000000 netin-1.0.5.7/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8232 2023-04-23 12:41:52.000000 netin-1.0.5.7/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2483 2023-04-23 14:23:52.000000 netin-1.0.5.7/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5943 2023-04-23 14:23:15.000000 netin-1.0.5.7/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6103 2023-04-23 14:24:14.000000 netin-1.0.5.7/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     5818 2023-04-23 14:52:52.000000 netin-1.0.5.7/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.7/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.7/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.7/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.7/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.7/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.7/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     8828 2023-04-23 14:52:43.000000 netin-1.0.5.7/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.7/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2271 2023-04-23 06:45:06.000000 netin-1.0.5.7/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.7/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.7/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.7/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.7/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.7/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.7/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    26872 2023-04-19 13:08:56.000000 netin-1.0.5.7/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.197018 netin-1.0.5.7/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3774 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1290 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.7/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-23 15:08:11.000000 netin-1.0.5.7/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-23 15:08:11.201018 netin-1.0.5.7/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.7/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.7/requirements/docs.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.7/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-23 15:08:11.201018 netin-1.0.5.7/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.7/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.8/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.8/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3858 2023-04-25 12:30:42.038736 netin-1.0.5.8/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2586 2023-04-24 11:45:43.000000 netin-1.0.5.8/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.8/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.8/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.8/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/examples/notebooks/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2956 2023-04-24 13:06:53.000000 netin-1.0.5.8/examples/notebooks/deleteme.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.8/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.8/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.8/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.8/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      421 2023-04-25 11:03:04.000000 netin-1.0.5.8/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-24 23:49:22.000000 netin-1.0.5.8/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/netin/algorithms/sampling/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      244 2023-04-24 23:49:57.000000 netin-1.0.5.8/netin/algorithms/sampling/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-24 22:21:58.000000 netin-1.0.5.8/netin/algorithms/sampling/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2814 2023-04-25 10:52:24.000000 netin-1.0.5.8/netin/algorithms/sampling/degree_group_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2414 2023-04-25 10:52:21.000000 netin-1.0.5.8/netin/algorithms/sampling/degree_rank.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3963 2023-04-25 10:52:17.000000 netin-1.0.5.8/netin/algorithms/sampling/partial_crawls.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1901 2023-04-25 10:52:13.000000 netin-1.0.5.8/netin/algorithms/sampling/random_edges.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2092 2023-04-25 10:52:10.000000 netin-1.0.5.8/netin/algorithms/sampling/random_neighbor.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1684 2023-04-25 10:52:06.000000 netin-1.0.5.8/netin/algorithms/sampling/random_nodes.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5762 2023-04-25 10:48:43.000000 netin-1.0.5.8/netin/algorithms/sampling/sampling.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      296 2023-04-24 23:15:30.000000 netin-1.0.5.8/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5521 2023-04-24 18:03:30.000000 netin-1.0.5.8/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13472 2023-04-24 16:34:00.000000 netin-1.0.5.8/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3434 2023-04-24 18:05:02.000000 netin-1.0.5.8/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5344 2023-04-24 18:36:49.000000 netin-1.0.5.8/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    22097 2023-04-24 18:20:20.000000 netin-1.0.5.8/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8241 2023-04-24 13:06:53.000000 netin-1.0.5.8/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2747 2023-04-24 18:05:16.000000 netin-1.0.5.8/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6308 2023-04-24 18:05:38.000000 netin-1.0.5.8/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6805 2023-04-25 11:41:22.000000 netin-1.0.5.8/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6216 2023-04-24 18:05:57.000000 netin-1.0.5.8/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8299 2023-04-23 12:35:51.000000 netin-1.0.5.8/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.8/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.8/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.8/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.8/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.8/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     8828 2023-04-23 14:52:43.000000 netin-1.0.5.8/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      495 2023-04-24 13:42:57.000000 netin-1.0.5.8/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4994 2023-04-24 10:24:13.000000 netin-1.0.5.8/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2954 2023-04-24 18:16:58.000000 netin-1.0.5.8/netin/stats/networks.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     5682 2023-04-24 10:42:53.000000 netin-1.0.5.8/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.8/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1194 2023-04-24 11:51:14.000000 netin-1.0.5.8/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1872 2023-04-24 15:05:46.000000 netin-1.0.5.8/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.8/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.8/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    26716 2023-04-25 11:02:20.000000 netin-1.0.5.8/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.034736 netin-1.0.5.8/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3858 2023-04-25 12:30:41.000000 netin-1.0.5.8/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1690 2023-04-25 12:30:42.000000 netin-1.0.5.8/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-25 12:30:41.000000 netin-1.0.5.8/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.8/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-25 12:30:41.000000 netin-1.0.5.8/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-25 12:30:41.000000 netin-1.0.5.8/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-25 12:30:42.038736 netin-1.0.5.8/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.8/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       60 2023-04-23 06:45:06.000000 netin-1.0.5.8/requirements/docs.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.8/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-25 12:30:42.038736 netin-1.0.5.8/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4256 2023-04-25 10:29:59.000000 netin-1.0.5.8/setup.py
```

### Comparing `netin-1.0.5.7/LICENSE` & `netin-1.0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/PKG-INFO` & `netin-1.0.5.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.7
+Version: 1.0.5.8
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
@@ -28,14 +28,19 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: default
 Provides-Extra: test
 License-File: LICENSE
 
 NetIn
 ========
+
+.. image:: docs/source/netin-logo.png
+    :width: 200
+    :alt: NetworkInequality
+
 NetIn is a python package for network inference.
 It is based on the NetworkX package and provides a set of methods to study network inequalities.
 The package is currently under development and will be updated regularly.
 
 .. image:: https://github.com/CSHVienna/NetworkInequalities/actions/workflows/python-app.yml/badge.svg
   :target: https://github.com/CSHVienna/NetworkInequalities/actions/workflows/python-app.yml
```

### Comparing `netin-1.0.5.7/README.rst` & `netin-1.0.5.8/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 NetIn
 ========
+
+.. image:: docs/source/netin-logo.png
+    :width: 200
+    :alt: NetworkInequality
+
 NetIn is a python package for network inference.
 It is based on the NetworkX package and provides a set of methods to study network inequalities.
 The package is currently under development and will be updated regularly.
 
 .. image:: https://github.com/CSHVienna/NetworkInequalities/actions/workflows/python-app.yml/badge.svg
   :target: https://github.com/CSHVienna/NetworkInequalities/actions/workflows/python-app.yml
```

### Comparing `netin-1.0.5.7/examples/notebooks/deleteme.py` & `netin-1.0.5.8/examples/notebooks/deleteme.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     fig, ax = plt.subplots(1, 1, figsize=figsize, layout='constrained')
     multiplier = 0
 
     x = None
     groups = None
     maxy = 0
     for g in data:
-        etc = g.count_edges_types()
+        etc = g.calculate_edge_type_counts()
         name = update_name_homophily(g)
 
         groups = list(etc.keys()) if groups is None else groups
         x = np.arange(len(groups)) if x is None else x
         y = [etc[i] for i in groups]
         maxy = max(max(y), maxy)
```

### Comparing `netin-1.0.5.7/netin/generators/dh.py` & `netin-1.0.5.8/netin/generators/dh.py`

 * *Files 7% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         from sympy import symbols
         from sympy import Eq
         from sympy import solve
 
         f_m = self.calculate_fraction_of_minority()
         f_M = 1 - f_m
 
-        e = self.count_edges_types()
+        e = self.calculate_edge_type_counts()
         e_MM = e['MM']
         e_mm = e['mm']
         e_Mm = e['Mm']
         e_mM = e['mM']
 
         p_MM = e_MM / (e_MM + e_Mm)
         p_mm = e_mm / (e_mm + e_mM)
@@ -161,7 +161,20 @@
 
         eq3 = Eq((f_M * hMM) / ((f_M * hMM) + (f_m * hMm)), p_MM)
         eq4 = Eq(hMM + hMm, 1)
 
         solution = solve((eq1, eq2, eq3, eq4), (hmm, hmM, hMM, hMm))
         h_MM, h_mm = solution[hMM], solution[hmm]
         return h_MM, h_mm
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              d=self.d,
+                              f_m=self.f_m,
+                              plo_M=self.plo_M,
+                              plo_m=self.plo_m,
+                              h_MM=self.h_MM,
+                              h_mm=self.h_mm,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.7/netin/generators/directed.py` & `netin-1.0.5.8/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/generators/dpa.py` & `netin-1.0.5.8/netin/generators/dpa.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,7 +100,18 @@
         -------
         np.array
             array of probabilities for each target node.
         """
         probs = np.array([self.get_in_degree(n) + const.EPSILON for n in target_set])
         probs /= probs.sum()
         return probs
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              d=self.d,
+                              f_m=self.f_m,
+                              plo_M=self.plo_M,
+                              plo_m=self.plo_m,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.7/netin/generators/dpah.py` & `netin-1.0.5.8/netin/generators/dpah.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
 
-from netin.utils import constants as const
 from netin.generators.h import Homophily
+from netin.utils import constants as const
 from .dpa import DPA
 
 
 class DPAH(DPA, Homophily):
-
     """Creates a new DPAH instance. A directed graph with preferential attachment and homophily.
 
     Parameters
     ----------
     n: int
         number of nodes (minimum=2)
 
@@ -138,7 +137,24 @@
         Returns
         -------
         Tuple[float, float]
             homophily within the majority and minority groups
         """
         h_MM, h_mm = None, None
         return h_MM, h_mm
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        obj = self.__class__(n=self.n,
+                              d=self.d,
+                              f_m=self.f_m,
+                              plo_M=self.plo_M,
+                              plo_m=self.plo_m,
+                              h_MM=self.h_MM,
+                              h_mm=self.h_mm,
+                              seed=self.seed)
+        obj._initialize(class_attribute=self.class_attribute,
+                        class_values=self.class_values,
+                        class_labels=self.class_labels)
+        return obj
```

### Comparing `netin-1.0.5.7/netin/generators/graph.py` & `netin-1.0.5.8/netin/generators/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from typing import Union, Set, List
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from pqdm.threads import pqdm
 
+import netin
 from netin.utils import constants as const
 from netin.utils import validator as val
+from netin.stats import networks as net
 
 
 class Graph(nx.Graph):
     """Bi-populated network (base graph model)
 
     Parameters
     ----------
@@ -102,18 +104,18 @@
         class_values: list
             list of class values
 
         class_labels: list
             list of class labels
         """
         if class_labels is None:
-            class_labels = [const.MAJORITY_LABEL, const.MINORITY_LABEL]
+            class_labels = const.CLASS_LABELS
         if class_values is None:
-            class_values = [0, 1]
-        self.set_class_attribute(class_attribute)
+            class_values = const.CLASS_VALUES
+        self.set_class_attribute(const.CLASS_ATTRIBUTE)
         self.set_class_values(class_values)
         self.set_class_labels(class_labels)
 
     def get_metadata_as_dict(self) -> dict:
         """
         Returns metadata for a graph as a dictionary.
         It includes the model name, class attribute, class values, class labels, number of nodes,
@@ -180,15 +182,15 @@
         Returns
         -------
         float
             fraction of minorities
         """
         return self.f_m
 
-    def set_seed(self, seed = None):
+    def set_seed(self, seed=None):
         """
         Sets the random seed.
 
         Parameters
         ----------
         seed
             random seed
@@ -400,15 +402,15 @@
             list of class values
 
         class_labels: list
             list of class labels
         """
         self._infer_model_name()
         self._set_class_info(class_attribute, class_values, class_labels)
-        self.graph = self.get_metadata_as_dict()
+        self.graph.update(self.get_metadata_as_dict())
 
     def _init_nodes(self):
         """
         Initializes the list of nodes with their respective labels.
         """
         self.node_list = np.arange(self.n)
         self.n_M = int(round(self.n * (1 - self.f_m)))
@@ -534,25 +536,25 @@
 
         print("=== Computed ===")
         print(f'- is directed: {self.is_directed()}')
         print(f'- number of nodes: {self.number_of_nodes()}')
         print(f'- number of edges: {self.number_of_edges()}')
         print(f'- minimum degree: {self.calculate_minimum_degree()}')
         print(f'- fraction of minority: {self.calculate_fraction_of_minority()}')
-        print(f'- edge-type counts: {self.count_edges_types()}')
+        print(f'- edge-type counts: {self.calculate_edge_type_counts()}')
         print(f"- density: {nx.density(self)}")
         try:
             print(f"- diameter: {nx.diameter(self)}")
         except Exception as ex:
             print(f"- diameter: <{ex}>")
         try:
             print(f"- average shortest path length: {nx.average_shortest_path_length(self)}")
         except Exception as ex:
             print(f"- average shortest path length: <{ex}>")
-        print(f"- average degree: {sum([d for n, d in self.degree]) / self.number_of_nodes()}")
+        print(f"- average degree: {net.get_average_degree(self)}")
         print(f"- degree assortativity: {nx.degree_assortativity_coefficient(self)}")
         print(f"- attribute assortativity ({self.class_attribute}): "
               f"{nx.attribute_assortativity_coefficient(self, self.class_attribute)}")
         print(f"- transitivity: {nx.transitivity(self)}")
         print(f"- average clustering: {nx.average_clustering(self)}")
         self.info_computed()
 
@@ -561,40 +563,37 @@
         Returns the minimum degree of the graph.
 
         Returns
         -------
         int
             minimum degree
         """
-        return min([d for n, d in self.degree])
+        return net.get_min_degree(self)
 
     def calculate_fraction_of_minority(self) -> float:
         """
         Returns the fraction of minority nodes in the graph (based on class attribute).
 
         Returns
         -------
         float
             fraction of minority nodes
         """
-        return sum([1 for n, obj in self.nodes(data=True) if obj[self.class_attribute] == self.class_values[
-            self.class_labels.index(const.MINORITY_LABEL)]]) / self.number_of_nodes()
+        return net.get_minority_fraction(self)
 
-    def count_edges_types(self) -> Counter:
+    def calculate_edge_type_counts(self) -> Counter:
         """
-        Returns the number of edges of each type, e.g., Mm (between majoriy and minority), mm, etc.
+        Returns the number of edges of each type, e.g., Mm (between majority and minority), mm, etc.
 
         Returns
         -------
         Counter
             counter of edges types
         """
-        return Counter([f"{self.class_labels[self.nodes[e[0]][self.class_attribute]]}"
-                        f"{self.class_labels[self.nodes[e[1]][self.class_attribute]]}"
-                        for e in self.edges])
+        return net.get_edge_type_counts(self)
 
     ############################################################
     # Metadata
     ############################################################
 
     def compute_node_stats(self, metric: str, **kwargs) -> List[Union[int, float]]:
         """
@@ -680,7 +679,31 @@
 
         # add ranking values
         for metric in const.VALID_METRICS:
             ncol = f'{metric}_rank'
             df.loc[:, ncol] = df.loc[:, metric].rank(ascending=False, pct=True, method='dense')
 
         return df
+
+    def _makecopy(self):
+        pass
+
+    def copy(self) -> Union[nx.Graph, nx.DiGraph]:
+        """
+        Makes a copy of the current object.
+        Returns
+        -------
+        netin.Graph
+            copy of the current object
+        """
+        g = self._makecopy()
+        g._init_graph(class_attribute=self.class_attribute,
+                      class_values=self.class_values,
+                      class_labels=self.class_labels)
+        g.graph.update(self.graph)
+        g.add_nodes_from((n, d.copy()) for n, d in self._node.items())
+        g.add_edges_from(
+            (u, v, datadict.copy())
+            for u, nbrs in self._adj.items()
+            for v, datadict in nbrs.items()
+        )
+        return g
```

### Comparing `netin-1.0.5.7/netin/generators/h.py` & `netin-1.0.5.8/netin/generators/h.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         h_MM: float
             homophily within majority group
 
         h_mm: float
             homophily within minority group
         """
 
-        e = self.count_edges_types()
+        e = self.calculate_edge_type_counts()
         if self.is_directed():
             h_MM = e['MM'] / (e['MM'] + e['Mm'])
             h_mm = e['mm'] / (e['mm'] + e['mM'])
         else:
             h_MM = e['MM'] / (e['MM'] + e['Mm'] + e['mM'])
             h_mm = e['mm'] / (e['mm'] + e['mM'] + e['Mm'])
```

### Comparing `netin-1.0.5.7/netin/generators/pa.py` & `netin-1.0.5.8/netin/generators/pa.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,7 +75,16 @@
 
         target_set: set
             set of target nodes (ids)
         """
         probs = np.array([(self.degree(target) + const.EPSILON) for target in target_set])
         probs /= probs.sum()
         return probs, target_set
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              k=self.k,
+                              f_m=self.f_m,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.7/netin/generators/pah.py` & `netin-1.0.5.8/netin/generators/pah.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         Notes
         -----
         See derivations in [Karimi2018]_.
         """
         f_m = self.calculate_fraction_of_minority()
         f_M = 1 - f_m
 
-        e = self.count_edges_types()
+        e = self.calculate_edge_type_counts()
         e_MM = e['MM']
         e_mm = e['mm']
         M = e['MM'] + e['mm'] + e['Mm'] + e['mM']
 
         p_MM = e_MM / M
         p_mm = e_mm / M
 
@@ -181,7 +181,18 @@
 
         eq3 = Eq((f_M * f_M * hMM * (1 - b_m)) / ((f_M * hMM * (1 - b_m)) + (f_m * hMm * (1 - b_M))), p_MM)
         eq4 = Eq(hMM + hMm, 1)
 
         solution = solve((eq1, eq2, eq3, eq4), (hmm, hmM, hMM, hMm))
         h_MM, h_mm = solution[hMM], solution[hmm]
         return h_MM, h_mm
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              k=self.k,
+                              f_m=self.f_m,
+                              h_MM=self.h_MM,
+                              h_mm=self.h_mm,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.7/netin/generators/patc.py` & `netin-1.0.5.8/netin/generators/patc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 from typing import Union, Set, Tuple
 
 import numpy as np
+import networkx as nx
 
 from netin.utils import constants as const
 from netin.generators.tc import TriadicClosure
 from .pa import PA
 
 
 class PATC(PA, TriadicClosure):
+    """Creates a new PATC instance. An undirected graph with preferential attachment and triadic closure.
+
+    Parameters
+    ----------
+    n: int
+        number of nodes (minimum=2)
+
+    k: int
+        minimum degree of nodes (minimum=1)
+
+    f_m: float
+        fraction of minorities (minimum=1/n, maximum=(n-1)/n)
+
+    tc: float
+        probability of a new edge to close a triad (minimum=0, maximum=1.)
+
+    seed: object
+        seed for random number generator
+
+    Notes
+    -----
+    The initialization is an undirected with n nodes and no edges.
+    Then, everytime a node is selected as source, it gets connected to k target nodes.
+    Target nodes are selected via preferential attachment `in-degree` [BarabasiAlbert1999]_, or
+    triadic closure `tc` [HolmeKim2002]_.
+    """
 
     ############################################################
     # Constructor
     ############################################################
 
     def __init__(self, n: int, k: int, f_m: float, tc: float, seed: object = None):
-        """Creates a new PATC instance. An undirected graph with preferential attachment and triadic closure.
-
-        Parameters
-        ----------
-        n: int
-            number of nodes (minimum=2)
-
-        k: int
-            minimum degree of nodes (minimum=1)
-
-        f_m: float
-            fraction of minorities (minimum=1/n, maximum=(n-1)/n)
-
-        tc: float
-            probability of a new edge to close a triad (minimum=0, maximum=1.)
-
-        seed: object
-            seed for random number generator
-
-        Notes
-        -----
-        The initialization is an undirected with n nodes and no edges.
-        Then, everytime a node is selected as source, it gets connected to k target nodes.
-        Target nodes are selected via preferential attachment `in-degree` [BarabasiAlbert1999]_, or
-        triadic closure `tc` [HolmeKim2002]_.
-        """
         PA.__init__(self, n=n, k=k, f_m=f_m, seed=seed)
         TriadicClosure.__init__(self, n=n, f_m=f_m, tc=tc, seed=seed)
 
     ############################################################
     # Init
     ############################################################
 
@@ -191,7 +192,33 @@
 
         See Also
         --------
         :func:`netin.TC.update_special_targets`
 
         """
         return TriadicClosure.update_special_targets(self, idx_target, source, target, targets, special_targets)
+
+    ############################################################
+    # Calculations
+    ############################################################
+
+    def infer_triadic_closure(self) -> float:
+        """
+        Approximates analytically the triadic closure value of the graph.
+
+        Returns
+        -------
+        float
+            triadic closure probability of the graph
+        """
+        tc = nx.average_clustering(self)
+        return tc
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              k=self.k,
+                              f_m=self.f_m,
+                              tc=self.tc,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.7/netin/generators/patch.py` & `netin-1.0.5.8/netin/generators/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,7 +185,19 @@
         Returns
         -------
         float
             triadic closure probability of the graph
         """
         tc = None
         return tc
+
+    def _makecopy(self):
+        """
+        Makes a copy of the current object.
+        """
+        return self.__class__(n=self.n,
+                              k=self.k,
+                              f_m=self.f_m,
+                              tc=self.tc,
+                              h_MM=self.h_MM,
+                              h_mm=self.h_mm,
+                              seed=self.seed)
```

### Comparing `netin-1.0.5.7/netin/generators/tc.py` & `netin-1.0.5.8/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/generators/tests/test_directed.py` & `netin-1.0.5.8/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/generators/tests/test_dpah.py` & `netin-1.0.5.8/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/generators/tests/test_patch.py` & `netin-1.0.5.8/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/generators/tests/test_undirected.py` & `netin-1.0.5.8/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/generators/undirected.py` & `netin-1.0.5.8/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.7/netin/utils/constants.py` & `netin-1.0.5.8/netin/utils/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 EMPTY = [None, np.nan]
 
 # GRAPHS
 
 NO_HOMOPHILY = [0.5, None, np.nan]
 NO_TRIADIC_CLOSURE = [0, None, np.nan]
 
+CLASS_ATTRIBUTE = 'm'
+
 MAJORITY_LABEL = 'M'
 MINORITY_LABEL = 'm'
+CLASS_LABELS = [MAJORITY_LABEL, MINORITY_LABEL]
 
 MAJORITY_VALUE = 0
 MINORITY_VALUE = 1
+CLASS_VALUES = [MAJORITY_VALUE, MINORITY_VALUE]
 
 # GENERATIVE MODELS
 
 EPSILON = 0.00001
 MAX_TRIES_EDGE = 100
 
 H_MODEL_NAME = 'Homophily'
```

### Comparing `netin-1.0.5.7/netin/viz/handlers.py` & `netin-1.0.5.8/netin/viz/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 import logging
-from typing import Set
 from typing import List
+from typing import Set
 from typing import Union
 
 import matplotlib
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
-from matplotlib import rc
 import networkx as nx
 import numpy as np
 import pandas as pd
 import seaborn as sns
+from matplotlib import rc
 
-from netin.utils import constants as const
-from netin.viz.constants import *
 from netin.generators.graph import Graph
 from netin.stats.distributions import fit_power_law
+from netin.stats.distributions import get_disparity
 from netin.stats.distributions import get_fraction_of_minority
 from netin.stats.distributions import get_gini_coefficient
-from netin.stats.distributions import get_disparity
+from netin.utils import constants as const
+from netin.viz.constants import *
 
 
 def reset_style():
     """
     Resets the style of the plots to the default style.
-    Returns
-    -------
 
     """
-
     sns.reset_orig()
 
 
 def set_paper_style(font_scale: float = 1.0):
     """
     Sets the style of the plots to the paper style.
     Font family serif, and allows to adjust the font scale.
 
     Parameters
     ----------
     font_scale: float
         A scale factor for the font size.
 
-    Returns
-    -------
-
     """
-
     sns.set_context("paper", font_scale=font_scale)
     rc('font', family='serif')
     rc('lines', linewidth=1.0)
     rc('axes', linewidth=0.5)
     rc('xtick.major', width=0.5)
     rc('ytick.major', width=0.5)
 
@@ -113,35 +106,45 @@
     """
     Saves the figure to a file, shows it and closes the figure.
 
     Parameters
     ----------
     fig: matplotlib.figure.Figure
         figure to save
+
     fn: str
         filename to save the figure
+
     kwargs: dict
-        additional arguments for the `subplots_adjust` function of the figure.
-        - left: float
+        Additional arguments for the ``subplots_adjust`` function of the figure.
+
+        left: float
             left margin
-        - right: float
+
+        right: float
             right margin
-        - bottom: float
+
+        bottom: float
             bottom margin
-        - top: float
+
+        top: float
             top margin
-        - wspace: float
+
+        wspace: float
             width space between subplots
-        - hspace: float
+
+        hspace: float
             height space between subplots
 
-        Additional arguments for the `savefig` function of the figure.
-        - dpi: int
+        Additional arguments for the ``savefig`` function of the figure.
+
+        dpi: int
             dpi of the figure
-        - bbox_inches: str
+
+        bbox_inches: str
             bounding box of the figure
 
     Returns
     -------
 
     """
     dpi = kwargs.pop('dpi', DPI)
@@ -189,71 +192,78 @@
 def _add_class_legend(fig: matplotlib.figure.Figure, **kwargs):
     """
     Shows the legend of the figure using the "class_label" values of the nodes/graph.
 
     Parameters
     ----------
     fig: matplotlib.figure.Figure
-        figure to add the legend
+        Figure to add the legend
+
     kwargs: dict
-        additional arguments for the `legend` function of the figure.
-            - bbox: tuple
-                bounding box of the legend
-            - loc: str
-                location of the legend
+        Additional arguments for the ``legend`` function of the figure.
 
-    Returns
-    -------
+        bbox: tuple
+            bounding box of the legend
 
+        loc: str
+            location of the legend
     """
     maj_patch = mpatches.Patch(color=COLOR_MAJORITY, label='majority')
     min_patch = mpatches.Patch(color=COLOR_MINORITY, label='minority')
     bbox = kwargs.pop('bbox', (1.04, 1))
     loc = kwargs.pop('loc', "upper left")
     fig.legend(handles=[maj_patch, min_patch], bbox_to_anchor=bbox, loc=loc)
 
 
-def plot_graph(data: Union[Graph, Set[Graph], List[Graph]], share_pos: bool = False, fn : str = None, **kwargs):
+def plot_graph(data: Union[Graph, Set[Graph], List[Graph]], share_pos: bool = False, fn: str = None, **kwargs):
     """
     Plots one or multiple (netin.Graph) graphs as matplotlib figures.
 
     Parameters
     ----------
     data: Union[netin.Graph, Set[netin.Graph]]
         graph or set of graphs to plot
+
     share_pos: bool
         if True, the positions of the nodes are shared between the graphs
+
     fn: str
         filename to save the figure
+
     kwargs: dict
-        additional arguments for the `subplots` function of the figure.
-            - cell_size: float
-                size of the cell in inches
-            - nc: int
-                number of columns
-            - node_size: int
-                size of the nodes
-            - node_shape: str
-                shape of the nodes e.g, 'o' for circle, 's' for square
-            - edge_width: float
-                width of the edges
-            - edge_style: str
-                style of the edges e.g., 'solid', 'dashed'
-            - edge_arrows: bool
-                if True, the edges are plotted with arrows
-            - arrow_style: str
-                style of the arrows e.g., '-|>' for filled arrow
-            - arrow_size: int
-                size of the arrows
+        Additional arguments for the ``subplots`` function of the figure.
 
-        additional arguments for the `subplots_adjust` and `savefig` functions of the figure.
+        cell_size: float
+            size of the cell in inches
 
-    Returns
-    -------
+        nc: int
+            number of columns
+
+        node_size: int
+            size of the nodes
+
+        node_shape: str
+            shape of the nodes e.g, 'o' for circle, 's' for square
+
+        edge_width: float
+            width of the edges
+
+        edge_style: str
+            style of the edges e.g., 'solid', 'dashed'
+
+        edge_arrows: bool
+            if True, the edges are plotted with arrows
 
+        arrow_style: str
+            style of the arrows e.g., '-\|>' for filled arrow
+
+        arrow_size: int
+            size of the arrows
+
+        Additional arguments for the ``subplots_adjust`` and ``savefig`` functions of the figure.
     """
     iter_graph = [data] if isinstance(data, Graph) else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_graph), nc=nc)
     cell_size = kwargs.pop('cell_size', DEFAULT_CELL_SIZE)
 
     fig, axes = plt.subplots(nr, nc, figsize=(nc * cell_size, nr * cell_size), sharex=False, sharey=False)
@@ -262,111 +272,132 @@
     edge_width = kwargs.get('edge_width', 0.02)
     edge_style = kwargs.get('edge_style', 'solid')
     edge_arrows = kwargs.get('edge_arrows', True)
     arrow_style = kwargs.get('arrow_style', '-|>')
     arrow_size = kwargs.get('arrow_size', 2)
 
     pos = None
-    same_n = len(set([g.number_of_nodes() for g in iter_graph])) == 1
-    for cell, g in enumerate(iter_graph):
+    # same_n = len(set([g.number_of_nodes() for g in iter_graph])) == 1
+    for cell in np.arange(nc * nr):
         row = cell // nc
         col = cell % nc
-
         ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
 
-        pos = nx.spring_layout(g) if pos is None or not share_pos or not same_n else pos
+        if cell < len(iter_graph):
+            g = iter_graph[cell]
+
+            pos = nx.spring_layout(g) if pos is None or not share_pos else pos # or not same_n
 
-        # nodes
-        maj = g.graph['class_values'][g.graph['class_labels'].index("M")]
-        nodes, node_colors = zip(
-            *[(node, COLOR_MAJORITY if data[g.graph['class_attribute']] == maj else COLOR_MINORITY)
-              for node, data in g.nodes(data=True)])
-        nx.draw_networkx_nodes(g, pos, nodelist=nodes, node_size=node_size, node_color=node_colors,
-                               node_shape=node_shape, ax=ax)
-
-        # edges
-        edges = g.edges()
-        edges, edge_colors = zip(*[((s, t), _get_edge_color(s, t, g)) for s, t in edges])
-        nx.draw_networkx_edges(g, pos, ax=ax, edgelist=edges, edge_color=edge_colors,
-                               width=edge_width, style=edge_style, arrows=edge_arrows, arrowstyle=arrow_style,
-                               arrowsize=arrow_size)
+            # title
+            ax.set_title(g.get_model_name())
+
+            # nodes
+            maj = g.graph['class_values'][g.graph['class_labels'].index("M")]
+            nodes, node_colors = zip(
+                *[(node, COLOR_MAJORITY if data[g.graph['class_attribute']] == maj else COLOR_MINORITY)
+                  for node, data in g.nodes(data=True)])
+            nx.draw_networkx_nodes(g, pos, nodelist=nodes, node_size=node_size, node_color=node_colors,
+                                   node_shape=node_shape, ax=ax)
+
+            # edges
+            edges = g.edges()
+            edges, edge_colors = zip(*[((s, t), _get_edge_color(s, t, g)) for s, t in edges])
+            nx.draw_networkx_edges(g, pos, ax=ax, edgelist=edges, edge_color=edge_colors,
+                                   width=edge_width, style=edge_style, arrows=edge_arrows, arrowstyle=arrow_style,
+                                   arrowsize=arrow_size)
 
         # final touch
         ax.set_axis_off()
-        ax.set_title(g.get_model_name())
 
     # legend
     _add_class_legend(fig, **kwargs)
     _save_plot(fig, fn, **kwargs)
 
 
-def plot_distribution(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List],
+def plot_distribution(data: Union[pd.DataFrame, List[pd.DataFrame]],
+                      col_name: Union[str, List],
                       get_x_y_from_df_fnc: callable, fn=None, **kwargs):
     """
     Plots a distribution of the values of a column of a dataframe.
 
     Parameters
     ----------
     data: Union[pandas.DataFrame, List[pandas.DataFrame]]
-        dataframe or list of dataframes to plot including.
-        A column of this dataframe is used to plot the distribution.
+        Dataframe or list of dataframes to plot including. A column of this dataframe is used to plot the distribution.
+
     col_name: str
         name of the column to plot
+
     get_x_y_from_df_fnc: callable
-        function to get the x and y values from the dataframe
+        Function to get the x and y values from the dataframe
+
     fn: str
-        filename to save the figure
+        Filename to save the figure
+
     kwargs: dict
-        additional arguments
-        - nc: int
+        Additional arguments
+
+        nc: int
             number of columns to show in the grid
-        - cell_size: float or tuple(float, float)
-            size of the cell in inches.
-            If a tuple is given, the first value is the width and the second value is the height.
-        - scatter: bool
+
+        cell_size: float or tuple(float, float)
+            size of the cell in inches. If a tuple is given, the first value is the width and the second value is the height.
+
+        scatter: bool
             if True, the distribution is plotted as a scatter plot
-        - sharex: bool
+
+        sharex: bool
             if True, the x-axis is shared between the subplots
-        - sharey: bool
+
+        sharey: bool
             if True, the y-axis is shared between the subplots
-        - ylabel: str
+
+        ylabel: str
             label of the y-axis if not set, the name of the function get_x_y_from_df_fnc is used
-        - xlabel: str
+
+        xlabel: str
             label of the x-axis.
-        - xlim, ylim: tuple
+
+        xlim, ylim: tuple
             limits of the x and y-axis
-        - hue: str
+
+        hue: str
             name of the column to use for grouping the data
-        - common_norm: bool
-            if True, the y-axis is normalized to the same value (sum of all values).
-            Otherwise, the y-axis is normalized per class (hue)
-        - log_scale: tuple(bool, bool)
-            if True, the x and y-axis are plotted in log scale
-        - hline_fnc: callable
+
+        common_norm: bool
+            If True, the y-axis is normalized to the same value (sum of all values). Otherwise, the y-axis is normalized per class (hue)
+
+        log_scale: tuple(bool, bool)
+            If True, the x and y-axis are plotted in log scale
+
+        hline_fnc: callable
             function to plot a horizontal line
-        - vline_fnc: callable
+
+        vline_fnc: callable
             function to plot a vertical line
-        - suptitle: str
+
+        suptitle: str
             title of the whole plot
-        - cuts: list
+
+        cuts: list
             list of cuts to plot (vertical lines)
-        - gini_fnc: callable
+
+        gini_fnc: callable
             function to plot the gini coefficient in ranking (inequality)
-        - me_fnc: callable
+
+        me_fnc: callable
             function to plot the mean error in ranking (inequity)
-        - beta: float
-            beta value for smoothing the inequity areas (over, under, and fair representation of minority nodes)
-        - class_label_legend: bool
-            if True, the legend of the class labels is plotted
 
-        additional arguments sent to `ax.scatter` or `ax.plot` from matplotlib
+        beta: float
+            beta value for smoothing the inequity areas (over, under, and fair representation of minority nodes)
 
-    Returns
-    -------
+        class_label_legend: bool
+            if True, the legend of the class labels is plotted
 
+        And additional arguments sent to ``ax.scatter`` or ``ax.plot`` from matplotlib
     """
     iter_data = [data] if type(data) == pd.DataFrame else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_data), nc=nc)
     cell_size = kwargs.pop('cell_size', DEFAULT_CELL_SIZE)
     iter_column = [col_name] * (nc * nr) if type(col_name) == str else col_name
 
@@ -462,31 +493,29 @@
 
 def _show_beta(axline, data):
     axline(const.INEQUITY_BETA, ls='--', color='grey', alpha=0.5)
     axline(-const.INEQUITY_BETA, ls='--', color='grey', alpha=0.5)
 
 
 def plot_disparity(data: Union[pd.DataFrame, List[pd.DataFrame]], col_name: Union[str, List], fn: str = None, **kwargs):
-    """
-    Plots the disparity of the ranking of the minority group.
+    """Plots the disparity of the ranking of the minority group.
 
     Parameters
     ----------
     data: pd.DataFrame or List[pd.DataFrame]
         Metadata of nodes (each column is a property, e.g., degree)
+
     col_name: str
         Name of the column to plot (property of node)
+
     fn: str
         File name to save the plot
-    kwargs: dict
-        Additional arguments to pass to the `plot_distribution` function
-
-    Returns
-    -------
 
+    kwargs: dict
+        Additional arguments to pass to the ``plot_distribution`` function
     """
     gap = 0.04
     kwargs['class_label_legend'] = False
     kwargs['xlabel'] = INEQUITY_AXIS_LABEL
     kwargs['ylabel'] = INEQUALITY_AXIS_LABEL
     kwargs['ylim'] = (0.0 - gap, 1.0 + gap)
     kwargs['xlim'] = (-1.0 - gap, 1.0 + gap)
@@ -505,25 +534,25 @@
     """
     Plots the Gini coefficient of the ranking of the minority group.
 
     Parameters
     ----------
     data: pd.DataFrame or List[pd.DataFrame]
         Metadata of nodes (each column is a property, e.g., degree)
+
     col_name: str or List[str]
         Name of the column to plot (property of node)
+
     fn: str
         File name to save the plot
-    kwargs: dict
-        Additional arguments to pass to the `plot_distribution` function
-
-    Returns
-    -------
 
+    kwargs: dict
+        Additional arguments to pass to the ``plot_distribution`` function
     """
+
     def show_gini(ax, ys, cuts):
         gini, x, y, va, ha, color = get_gini_label(ys, cuts)
         ax.text(s=gini,
                 x=x, y=y,
                 color=color,
                 transform=ax.transAxes,
                 ha=ha, va=va)
@@ -564,24 +593,23 @@
     """
     Plots the fraction of minority nodes in each top-k of the rank.
 
     Parameters
     ----------
     data: pd.DataFrame or List[pd.DataFrame]
         Metadata of nodes (each column is a property, e.g., degree)
+
     col_name: str or List
         Name of the column to plot (property of node)
+
     fn: str:
         File name to save the plot
-    kwargs: dict
-        Additional arguments to pass to the `plot_distribution` function
-
-    Returns
-    -------
 
+    kwargs: dict
+        Additional arguments to pass to the ``plot_distribution`` function
     """
     gap = 0.02
 
     def show_me(ax, f_m, ys, beta):
         me, x, y, va, ha, color = get_me_label(f_m, ys, beta)
         ax.text(s=me,
                 x=x, y=y,
@@ -688,17 +716,14 @@
             The four values represent (left, bottom, right, top) in figure coordinates.
         - loc: str
             Location of the legend. One of "best", "upper right", "upper left", "lower left", "lower right",
             "right", "center left", "center right", "lower center", "upper center", "center"
 
         Additional parameters to pass to the plot of each subplot (pdf, cdf, ccdf)
 
-    Returns
-    -------
-
     """
 
     if kind not in TYPE_OF_DISTRIBUTION:
         raise ValueError(f"kind must be one of {TYPE_OF_DISTRIBUTION}")
 
     iter_data = [data] if type(data) == pd.DataFrame else data
     nc = kwargs.pop('nc', None)
@@ -707,15 +732,16 @@
     iter_column = [col_name] * (nc * nr) if type(col_name) == str else col_name
 
     # whole plot
     sharex = kwargs.pop('sharex', False)
     sharey = kwargs.pop('sharey', False)
     log_scale = kwargs.pop('log_scale', (False, False))
     xlabel = kwargs.pop('xlabel', None)
-    ylabel = kwargs.pop('ylabel', "p(X≥x)" if kind == "ccdf" else "p(X<x)" if kind == 'cdf' else "p(X=x)" if kind == 'pdf' else None)
+    ylabel = kwargs.pop('ylabel',
+                        "p(X≥x)" if kind == "ccdf" else "p(X<x)" if kind == 'cdf' else "p(X=x)" if kind == 'pdf' else None)
     verbose = kwargs.pop('verbose', False)
     wspace = kwargs.pop('wspace', None)
     hspace = kwargs.pop('hspace', None)
     suptitle = kwargs.pop('suptitle', None)
 
     # outer legend
     hue = kwargs.pop('hue', None)
```

### Comparing `netin-1.0.5.7/netin.egg-info/PKG-INFO` & `netin-1.0.5.8/netin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.7
+Version: 1.0.5.8
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
@@ -28,14 +28,19 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: default
 Provides-Extra: test
 License-File: LICENSE
 
 NetIn
 ========
+
+.. image:: docs/source/netin-logo.png
+    :width: 200
+    :alt: NetworkInequality
+
 NetIn is a python package for network inference.
 It is based on the NetworkX package and provides a set of methods to study network inequalities.
 The package is currently under development and will be updated regularly.
 
 .. image:: https://github.com/CSHVienna/NetworkInequalities/actions/workflows/python-app.yml/badge.svg
   :target: https://github.com/CSHVienna/NetworkInequalities/actions/workflows/python-app.yml
```

### Comparing `netin-1.0.5.7/netin.egg-info/SOURCES.txt` & `netin-1.0.5.8/netin.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 netin.egg-info/PKG-INFO
 netin.egg-info/SOURCES.txt
 netin.egg-info/dependency_links.txt
 netin.egg-info/not-zip-safe
 netin.egg-info/requires.txt
 netin.egg-info/top_level.txt
 netin/algorithms/__init__.py
+netin/algorithms/sampling/__init__.py
+netin/algorithms/sampling/constants.py
+netin/algorithms/sampling/degree_group_rank.py
+netin/algorithms/sampling/degree_rank.py
+netin/algorithms/sampling/partial_crawls.py
+netin/algorithms/sampling/random_edges.py
+netin/algorithms/sampling/random_neighbor.py
+netin/algorithms/sampling/random_nodes.py
+netin/algorithms/sampling/sampling.py
 netin/generators/__init__.py
 netin/generators/dh.py
 netin/generators/directed.py
 netin/generators/dpa.py
 netin/generators/dpah.py
 netin/generators/graph.py
 netin/generators/h.py
@@ -35,14 +44,15 @@
 netin/generators/tests/__init__.py
 netin/generators/tests/test_directed.py
 netin/generators/tests/test_dpah.py
 netin/generators/tests/test_patch.py
 netin/generators/tests/test_undirected.py
 netin/stats/__init__.py
 netin/stats/distributions.py
+netin/stats/networks.py
 netin/stats/ranking.py
 netin/utils/__init__.py
 netin/utils/constants.py
 netin/utils/validator.py
 netin/viz/__init__.py
 netin/viz/constants.py
 netin/viz/handlers.py
```

### Comparing `netin-1.0.5.7/setup.py` & `netin-1.0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 packages = [
     "netin",
-    "netin.algorithms",
+    "netin.algorithms.sampling",
     "netin.generators",
     "netin.utils",
     "netin.stats",
     "netin.viz",
     "netin.generators.tests",
 ]
```

