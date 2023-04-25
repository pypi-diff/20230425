# Comparing `tmp/terminally-0.1.3.tar.gz` & `tmp/terminally-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminally-0.1.3.tar", last modified: Tue Apr 25 11:07:40 2023, max compression
+gzip compressed data, was "terminally-0.1.5.tar", last modified: Tue Apr 25 11:15:19 2023, max compression
```

## Comparing `terminally-0.1.3.tar` & `terminally-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:07:40.821874 terminally-0.1.3/
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 11:07:40.821874 terminally-0.1.3/PKG-INFO
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)      601 2023-04-25 11:06:42.000000 terminally-0.1.3/README.md
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       38 2023-04-25 11:07:40.821874 terminally-0.1.3/setup.cfg
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)      300 2023-04-25 11:07:21.000000 terminally-0.1.3/setup.py
-drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:07:40.818540 terminally-0.1.3/terminally/
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       22 2023-04-25 11:04:12.000000 terminally-0.1.3/terminally/__init__.py
--rwxr-xr-x   0 moonsun   (1000) moonsun   (1000)     7413 2023-04-25 10:33:46.000000 terminally-0.1.3/terminally/ally.py
-drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:07:40.821874 terminally-0.1.3/terminally.egg-info/
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 11:07:40.000000 terminally-0.1.3/terminally.egg-info/PKG-INFO
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)      266 2023-04-25 11:07:40.000000 terminally-0.1.3/terminally.egg-info/SOURCES.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)        1 2023-04-25 11:07:40.000000 terminally-0.1.3/terminally.egg-info/dependency_links.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       46 2023-04-25 11:07:40.000000 terminally-0.1.3/terminally.egg-info/entry_points.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       15 2023-04-25 11:07:40.000000 terminally-0.1.3/terminally.egg-info/requires.txt
--rw-r--r--   0 moonsun   (1000) moonsun   (1000)       11 2023-04-25 11:07:40.000000 terminally-0.1.3/terminally.egg-info/top_level.txt
+drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:15:19.693747 terminally-0.1.5/
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 11:15:19.693747 terminally-0.1.5/PKG-INFO
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)      601 2023-04-25 11:06:42.000000 terminally-0.1.5/README.md
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       38 2023-04-25 11:15:19.693747 terminally-0.1.5/setup.cfg
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)      300 2023-04-25 11:15:10.000000 terminally-0.1.5/setup.py
+drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:15:19.693747 terminally-0.1.5/terminally/
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       23 2023-04-25 11:12:41.000000 terminally-0.1.5/terminally/__init__.py
+-rwxr-xr-x   0 moonsun   (1000) moonsun   (1000)     7413 2023-04-25 10:33:46.000000 terminally-0.1.5/terminally/ally.py
+drwxr-xr-x   0 moonsun   (1000) moonsun   (1000)        0 2023-04-25 11:15:19.693747 terminally-0.1.5/terminally.egg-info/
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       54 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/PKG-INFO
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)      266 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/SOURCES.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)        1 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/dependency_links.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       46 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/entry_points.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       15 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/requires.txt
+-rw-r--r--   0 moonsun   (1000) moonsun   (1000)       11 2023-04-25 11:15:19.000000 terminally-0.1.5/terminally.egg-info/top_level.txt
```

### Comparing `terminally-0.1.3/README.md` & `terminally-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `terminally-0.1.3/terminally/ally.py` & `terminally-0.1.5/terminally/ally.py`

 * *Files identical despite different names*

