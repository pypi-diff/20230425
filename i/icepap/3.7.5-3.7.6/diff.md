# Comparing `tmp/icepap-3.7.5.tar.gz` & `tmp/icepap-3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icepap-3.7.5.tar", last modified: Thu Mar 16 16:36:24 2023, max compression
+gzip compressed data, was "dist/icepap-3.7.6.tar", last modified: Tue Apr 25 12:26:56 2023, max compression
```

## Comparing `icepap-3.7.5.tar` & `icepap-3.7.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     7958 2023-03-16 16:30:32.000000 icepap-3.7.5/CHANGELOG.md
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    35149 2019-07-24 09:07:48.000000 icepap-3.7.5/LICENSE.txt
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      331 2019-07-24 09:07:48.000000 icepap-3.7.5/MANIFEST.in
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      824 2023-03-16 16:36:23.000000 icepap-3.7.5/PKG-INFO
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1292 2023-01-17 18:42:24.000000 icepap-3.7.5/README.md
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/doc/
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/doc/source/
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/doc/source/_static/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    43840 2019-07-24 09:07:48.000000 icepap-3.7.5/doc/source/_static/ALBALogo_WHITE.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)   270686 2019-07-24 09:07:48.000000 icepap-3.7.5/doc/source/_static/IcePAP_3D.png
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      249 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/api.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      257 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/applications.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/axis.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/backups.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      240 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/communication.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8661 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/conf.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      231 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/controller.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      212 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/fwversion.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      634 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/index.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      223 2019-07-24 09:07:48.000000 icepap-3.7.5/doc/source/low_level_methods.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      321 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/programming.rst
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      197 2023-01-17 18:42:24.000000 icepap-3.7.5/doc/source/utils.rst
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap/
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      898 2023-03-16 16:30:58.000000 icepap-3.7.5/icepap/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    47609 2023-03-16 16:30:32.000000 icepap-3.7.5/icepap/axis.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap/cli/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/cli/__init__.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      698 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/cli/__main__.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     9843 2023-03-16 16:30:32.000000 icepap-3.7.5/icepap/cli/cli.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    11305 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/cli/progress_bar.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8332 2023-03-02 11:10:19.000000 icepap-3.7.5/icepap/cli/repl.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     6700 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/cli/tables.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      565 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/cli/utils.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5389 2023-03-16 16:30:32.000000 icepap-3.7.5/icepap/communication.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    24083 2023-03-16 16:30:32.000000 icepap-3.7.5/icepap/controller.py
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     9892 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/fwversion.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     5219 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/group.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     8743 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/tcp.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)    17403 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/utils.py
--rw-r--r--   0 rhoms     (1268) Computing  (1000)     7130 2023-01-17 18:42:24.000000 icepap-3.7.5/icepap/vdatalib.py
-drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      824 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/PKG-INFO
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      914 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/SOURCES.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/dependency_links.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       50 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/entry_points.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)      114 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/requires.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)        7 2023-03-16 16:36:23.000000 icepap-3.7.5/icepap.egg-info/top_level.txt
--rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2023-03-16 16:36:23.000000 icepap-3.7.5/setup.cfg
--rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2116 2023-03-16 16:30:58.000000 icepap-3.7.5/setup.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8011 2023-04-25 12:17:56.000000 icepap-3.7.6/CHANGELOG.md
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    35149 2019-07-24 09:07:48.000000 icepap-3.7.6/LICENSE.txt
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      331 2019-07-24 09:07:48.000000 icepap-3.7.6/MANIFEST.in
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      824 2023-04-25 12:26:56.000000 icepap-3.7.6/PKG-INFO
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     1292 2023-01-17 18:42:24.000000 icepap-3.7.6/README.md
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/doc/
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/doc/source/
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/doc/source/_static/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    43840 2019-07-24 09:07:48.000000 icepap-3.7.6/doc/source/_static/ALBALogo_WHITE.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)   270686 2019-07-24 09:07:48.000000 icepap-3.7.6/doc/source/_static/IcePAP_3D.png
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      249 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/api.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      257 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/applications.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/axis.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      201 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/backups.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      240 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/communication.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     8661 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/conf.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      231 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/controller.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      212 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/fwversion.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      634 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/index.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      223 2019-07-24 09:07:48.000000 icepap-3.7.6/doc/source/low_level_methods.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      321 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/programming.rst
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      197 2023-01-17 18:42:24.000000 icepap-3.7.6/doc/source/utils.rst
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap/
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      898 2023-04-25 12:18:17.000000 icepap-3.7.6/icepap/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    47665 2023-04-25 12:17:56.000000 icepap-3.7.6/icepap/axis.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap/cli/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        0 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/cli/__init__.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)      698 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/cli/__main__.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     9843 2023-03-16 16:30:32.000000 icepap-3.7.6/icepap/cli/cli.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    11305 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/cli/progress_bar.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8332 2023-03-02 11:10:19.000000 icepap-3.7.6/icepap/cli/repl.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     6700 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/cli/tables.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      565 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/cli/utils.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5389 2023-03-16 16:30:32.000000 icepap-3.7.6/icepap/communication.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)    24083 2023-03-16 16:30:32.000000 icepap-3.7.6/icepap/controller.py
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     9892 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/fwversion.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     5219 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/group.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     8743 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/tcp.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)    17403 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/utils.py
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)     7130 2023-01-17 18:42:24.000000 icepap-3.7.6/icepap/vdatalib.py
+drwxr-xr-x   0 rhoms     (1268) Computing  (1000)        0 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      824 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/PKG-INFO
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      914 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/SOURCES.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        1 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/dependency_links.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       50 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/entry_points.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)      114 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/requires.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)        7 2023-04-25 12:26:56.000000 icepap-3.7.6/icepap.egg-info/top_level.txt
+-rw-r--r--   0 rhoms     (1268) Computing  (1000)       38 2023-04-25 12:26:56.000000 icepap-3.7.6/setup.cfg
+-rwxr-xr-x   0 rhoms     (1268) Computing  (1000)     2116 2023-04-25 12:18:17.000000 icepap-3.7.6/setup.py
```

### Comparing `icepap-3.7.5/CHANGELOG.md` & `icepap-3.7.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ### Fixed
  - Movement command does not accept negative values (Issue #77).
  - Update icepapctl animation.
  - Bug on repl when the mode is not the same for all axes.
  - Communication error with multilines answers
  - Fix typo
  - Return names with spaces
+ - Fix bug when hardware does not have serial number
 
 ## [3.6.x] 
 ### Added
  - Add fver property to read only the driver and the system version instead 
    of reading all modules versions.
  - Allow to use IcePAPAxis object as parameter of IcePAPController commands.
```

### Comparing `icepap-3.7.5/LICENSE.txt` & `icepap-3.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/PKG-INFO` & `icepap-3.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: icepap
-Version: 3.7.5
+Version: 3.7.6
 Summary: Python IcePAP Extension
 Home-page: https://github.com/ALBA-Synchrotron/pyIcePAP
 Author: Guifre Cuni et al.
 Author-email: ctbeamlines@cells.es
 License: GPLv3
 Description: Python IcePAP Extension for Win32, Linux, BSD, Jython
 Platform: UNKNOWN
```

### Comparing `icepap-3.7.5/README.md` & `icepap-3.7.6/README.md`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/doc/source/_static/ALBALogo_WHITE.png` & `icepap-3.7.6/doc/source/_static/ALBALogo_WHITE.png`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/doc/source/_static/IcePAP_3D.png` & `icepap-3.7.6/doc/source/_static/IcePAP_3D.png`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/doc/source/conf.py` & `icepap-3.7.6/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/doc/source/index.rst` & `icepap-3.7.6/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/__init__.py` & `icepap-3.7.6/icepap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 from .communication import IcePAPCommunication
 from .controller import IcePAPController
 from .fwversion import *
 from .utils import *
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-version = '3.7.5'
+version = '3.7.6'
```

### Comparing `icepap-3.7.5/icepap/axis.py` & `icepap-3.7.6/icepap/axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,15 +522,17 @@
     def id(self):
         """
         Get hardware ID and the serial number (Icepap user manual pag. 80).
 
         :return: (str HW ID, str SN)
         """
         hw_id = self.send_cmd('?ID HW')[0]
-        sn_id = self.send_cmd('?ID SN')[0]
+        sn_id = self.send_cmd("?ID SN")
+        if sn_id is not None:
+            sn_id = sn_id[0]
         return hw_id, sn_id
 
     @property
     def post(self):
         """
         Get the result of the power-on self test. Zero means there were not
         errors (IcePAP user manual pag. 110).
```

### Comparing `icepap-3.7.5/icepap/cli/__main__.py` & `icepap-3.7.6/icepap/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/cli/cli.py` & `icepap-3.7.6/icepap/cli/cli.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/cli/progress_bar.py` & `icepap-3.7.6/icepap/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/cli/repl.py` & `icepap-3.7.6/icepap/cli/repl.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/cli/tables.py` & `icepap-3.7.6/icepap/cli/tables.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/cli/utils.py` & `icepap-3.7.6/icepap/cli/utils.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/communication.py` & `icepap-3.7.6/icepap/communication.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/controller.py` & `icepap-3.7.6/icepap/controller.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/fwversion.py` & `icepap-3.7.6/icepap/fwversion.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/group.py` & `icepap-3.7.6/icepap/group.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/tcp.py` & `icepap-3.7.6/icepap/tcp.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/utils.py` & `icepap-3.7.6/icepap/utils.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap/vdatalib.py` & `icepap-3.7.6/icepap/vdatalib.py`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/icepap.egg-info/PKG-INFO` & `icepap-3.7.6/icepap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: icepap
-Version: 3.7.5
+Version: 3.7.6
 Summary: Python IcePAP Extension
 Home-page: https://github.com/ALBA-Synchrotron/pyIcePAP
 Author: Guifre Cuni et al.
 Author-email: ctbeamlines@cells.es
 License: GPLv3
 Description: Python IcePAP Extension for Win32, Linux, BSD, Jython
 Platform: UNKNOWN
```

### Comparing `icepap-3.7.5/icepap.egg-info/SOURCES.txt` & `icepap-3.7.6/icepap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icepap-3.7.5/setup.py` & `icepap-3.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setup.py
 import sys
 from setuptools import setup
 from setuptools import find_packages
 
 # The version is updated automatically with bumpversion
 # Do not update manually
-__version = '3.7.5'
+__version = '3.7.6'
 
 # windows installer:
 # python setup.py bdist_wininst
 
 # patch distutils if it can't cope with the "classifiers" or
 # "download_url" keywords
```

