# Comparing `tmp/operbot-171.tar.gz` & `tmp/operbot-172.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operbot-171.tar", last modified: Tue Apr 25 08:59:08 2023, max compression
+gzip compressed data, was "operbot-172.tar", last modified: Tue Apr 25 10:55:22 2023, max compression
```

## Comparing `operbot-171.tar` & `operbot-172.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 08:59:08.897756 operbot-171/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-25 07:12:36.000000 operbot-171/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2846 2023-04-25 07:12:36.000000 operbot-171/bin/operbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)      948 2023-04-25 07:12:36.000000 operbot-171/bin/operbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-25 07:12:36.000000 operbot-171/bin/operbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-25 07:12:36.000000 operbot-171/bin/operbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-25 07:12:36.000000 operbot-171/files/operbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/operbot/
--rw-r--r--   0 bart      (1000) bart      (1001)      147 2023-04-25 08:55:43.000000 operbot-171/operbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2834 2023-04-25 08:58:33.000000 operbot-171/operbot/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-25 07:15:29.000000 operbot-171/operbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-25 07:15:29.000000 operbot-171/operbot/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-04-25 07:15:29.000000 operbot-171/operbot/loggers.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/operbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17599 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      918 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7792 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1022 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2657 2023-04-25 07:15:57.000000 operbot-171/operbot/modules/usr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-25 07:15:29.000000 operbot-171/operbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4661 2023-04-25 07:15:29.000000 operbot-171/operbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)      211 2023-04-25 07:19:01.000000 operbot-171/operbot/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-25 07:15:29.000000 operbot-171/operbot/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-25 07:15:29.000000 operbot-171/operbot/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-25 07:15:29.000000 operbot-171/operbot/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/operbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      817 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-25 08:59:08.000000 operbot-171/operbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-25 08:59:08.897756 operbot-171/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-25 07:12:36.000000 operbot-171/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 08:59:08.897756 operbot-171/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-25 07:12:36.000000 operbot-171/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-25 07:12:36.000000 operbot-171/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-25 07:12:36.000000 operbot-171/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-25 07:12:36.000000 operbot-171/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-25 07:12:36.000000 operbot-171/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 10:55:22.805705 operbot-172/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4961 2023-04-25 07:12:36.000000 operbot-172/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2846 2023-04-25 07:12:36.000000 operbot-172/bin/operbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      968 2023-04-25 10:41:31.000000 operbot-172/bin/operbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      223 2023-04-25 07:12:36.000000 operbot-172/bin/operbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1149 2023-04-25 07:12:36.000000 operbot-172/bin/operbotd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      312 2023-04-25 07:12:36.000000 operbot-172/files/operbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/operbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)      147 2023-04-25 08:55:43.000000 operbot-172/operbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2834 2023-04-25 08:58:33.000000 operbot-172/operbot/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-25 07:15:29.000000 operbot-172/operbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6077 2023-04-25 07:15:29.000000 operbot-172/operbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-04-25 07:15:29.000000 operbot-172/operbot/loggers.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/operbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      408 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17599 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      918 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7792 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      340 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1022 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1091 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      313 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2657 2023-04-25 07:15:57.000000 operbot-172/operbot/modules/usr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5596 2023-04-25 07:15:29.000000 operbot-172/operbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4661 2023-04-25 07:15:29.000000 operbot-172/operbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      211 2023-04-25 07:19:01.000000 operbot-172/operbot/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1940 2023-04-25 07:15:29.000000 operbot-172/operbot/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1916 2023-04-25 07:15:29.000000 operbot-172/operbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1041 2023-04-25 07:15:29.000000 operbot-172/operbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/operbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     7498 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      817 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        8 2023-04-25 10:55:22.000000 operbot-172/operbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-25 10:55:22.805705 operbot-172/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1613 2023-04-25 10:42:46.000000 operbot-172/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-25 10:55:22.805705 operbot-172/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      661 2023-04-25 07:12:36.000000 operbot-172/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      356 2023-04-25 07:12:36.000000 operbot-172/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-25 07:12:36.000000 operbot-172/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4588 2023-04-25 07:12:36.000000 operbot-172/test/test_objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1113 2023-04-25 07:12:36.000000 operbot-172/test/test_storage.py
```

### Comparing `operbot-171/PKG-INFO` & `operbot-172/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 171
+Version: 172
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-171/README.rst` & `operbot-172/README.rst`

 * *Files identical despite different names*

### Comparing `operbot-171/bin/operbot` & `operbot-172/bin/operbot`

 * *Files identical despite different names*

### Comparing `operbot-171/bin/operbotcmd` & `operbot-172/bin/operbotcmd`

 * *Files 15% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 sys.path.insert(0, os.getcwd())
 
 
 import operbot.modules
 
 
-from opb.handler import Client, Error
-from opb.handler import command, parse
-from opb.persist import Persist
-from opb.scanner import scanpkg, importer
+from operbot.handler import Client, Error
+from operbot.handler import command, parse
+from operbot.persist import Persist
+from operbot.scanner import scanpkg, importer
 
 
-Persist.workdir = "/var/lib/opb/"
+Persist.workdir = "/var/lib/operbot/"
 
 
 class CLI(Client):
 
     def announce(self, txt):
         pass
```

### Comparing `operbot-171/bin/operbotd` & `operbot-172/bin/operbotd`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/__main__.py` & `operbot-172/operbot/__main__.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/clocked.py` & `operbot-172/operbot/clocked.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/handler.py` & `operbot-172/operbot/handler.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/loggers.py` & `operbot-172/operbot/loggers.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/modules/irc.py` & `operbot-172/operbot/modules/irc.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/modules/log.py` & `operbot-172/operbot/modules/log.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/modules/rss.py` & `operbot-172/operbot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/modules/tdo.py` & `operbot-172/operbot/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/modules/thr.py` & `operbot-172/operbot/modules/thr.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/modules/usr.py` & `operbot-172/operbot/modules/usr.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/objects.py` & `operbot-172/operbot/objects.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/persist.py` & `operbot-172/operbot/persist.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/scanner.py` & `operbot-172/operbot/scanner.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/threads.py` & `operbot-172/operbot/threads.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot/utility.py` & `operbot-172/operbot/utility.py`

 * *Files identical despite different names*

### Comparing `operbot-171/operbot.egg-info/PKG-INFO` & `operbot-172/operbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: operbot
-Version: 171
+Version: 172
 Summary: operator bot
 Home-page: http://github.com/operbot/operbot
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
```

### Comparing `operbot-171/operbot.egg-info/SOURCES.txt` & `operbot-172/operbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `operbot-171/setup.py` & `operbot-172/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 continue
             upl.append(d)
     return upl
 
 
 setup(
     name="operbot",
-    version="171",
+    version="172",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/operbot",
     description="operator bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `operbot-171/test/test_decoder.py` & `operbot-172/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `operbot-171/test/test_inherit.py` & `operbot-172/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `operbot-171/test/test_objects.py` & `operbot-172/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `operbot-171/test/test_storage.py` & `operbot-172/test/test_storage.py`

 * *Files identical despite different names*

