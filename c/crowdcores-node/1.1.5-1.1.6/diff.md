# Comparing `tmp/crowdcores-node-1.1.5.tar.gz` & `tmp/crowdcores-node-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-node-1.1.5.tar", last modified: Mon Apr 24 02:13:47 2023, max compression
+gzip compressed data, was "crowdcores-node-1.1.6.tar", last modified: Tue Apr 25 01:12:24 2023, max compression
```

## Comparing `crowdcores-node-1.1.5.tar` & `crowdcores-node-1.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:13:47.191743 crowdcores-node-1.1.5/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-24 02:13:47.191743 crowdcores-node-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-21 16:43:57.000000 crowdcores-node-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:13:47.187743 crowdcores-node-1.1.5/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.5/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-04-24 02:02:23.000000 crowdcores-node-1.1.5/crowdcores_node/crowdcores_node.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-04-23 00:44:23.000000 crowdcores-node-1.1.5/crowdcores_node/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:13:47.191743 crowdcores-node-1.1.5/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-24 02:13:47.000000 crowdcores-node-1.1.5/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-24 02:13:47.000000 crowdcores-node-1.1.5/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:13:47.000000 crowdcores-node-1.1.5/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-24 02:13:47.000000 crowdcores-node-1.1.5/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 02:13:47.000000 crowdcores-node-1.1.5/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-24 02:13:47.000000 crowdcores-node-1.1.5/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 02:13:47.191743 crowdcores-node-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-24 02:05:25.000000 crowdcores-node-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:12:24.857795 crowdcores-node-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-25 01:12:24.857795 crowdcores-node-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-21 16:43:57.000000 crowdcores-node-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:12:24.853795 crowdcores-node-1.1.6/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.6/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9322 2023-04-25 01:09:09.000000 crowdcores-node-1.1.6/crowdcores_node/crowdcores_node.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-04-23 00:44:23.000000 crowdcores-node-1.1.6/crowdcores_node/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:12:24.857795 crowdcores-node-1.1.6/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-25 01:12:24.000000 crowdcores-node-1.1.6/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-25 01:12:24.000000 crowdcores-node-1.1.6/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 01:12:24.000000 crowdcores-node-1.1.6/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-25 01:12:24.000000 crowdcores-node-1.1.6/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-25 01:12:24.000000 crowdcores-node-1.1.6/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-25 01:12:24.000000 crowdcores-node-1.1.6/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 01:12:24.857795 crowdcores-node-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-25 01:09:26.000000 crowdcores-node-1.1.6/setup.py
```

### Comparing `crowdcores-node-1.1.5/LICENSE.txt` & `crowdcores-node-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.1.5/README.md` & `crowdcores-node-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.1.5/crowdcores_node/manager.py` & `crowdcores-node-1.1.6/crowdcores_node/manager.py`

 * *Files identical despite different names*

