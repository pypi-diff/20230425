# Comparing `tmp/plex-nfs-watchdog-0.0.3.tar.gz` & `tmp/plex-nfs-watchdog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-nfs-watchdog-0.0.3.tar", last modified: Fri Apr 21 13:49:04 2023, max compression
+gzip compressed data, was "plex-nfs-watchdog-0.0.4.tar", last modified: Tue Apr 25 13:01:11 2023, max compression
```

## Comparing `plex-nfs-watchdog-0.0.3.tar` & `plex-nfs-watchdog-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.435566 plex-nfs-watchdog-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.439566 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/config/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/plex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/plex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/plex/plex_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-21 13:48:53.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/plex_nfs_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:49:04.443566 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-21 13:49:04.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-21 13:49:04.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:49:04.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 13:49:04.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 13:49:04.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 13:49:04.000000 plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.335427 plex-nfs-watchdog-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/config/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/plex_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-25 13:01:00.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/plex_nfs_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:01:11.339427 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 13:01:11.000000 plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/top_level.txt
```

### Comparing `plex-nfs-watchdog-0.0.3/LICENSE` & `plex-nfs-watchdog-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.3/PKG-INFO` & `plex-nfs-watchdog-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.3 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.4 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.3/README.md` & `plex-nfs-watchdog-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.3/setup.cfg` & `plex-nfs-watchdog-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/modules/plex/plex_agent.py` & `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/modules/plex/plex_agent.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog/plex_nfs_watchdog.py` & `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog/plex_nfs_watchdog.py`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/PKG-INFO` & `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.3 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.4 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.3/src/plex_nfs_watchdog.egg-info/SOURCES.txt` & `plex-nfs-watchdog-0.0.4/src/plex_nfs_watchdog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

