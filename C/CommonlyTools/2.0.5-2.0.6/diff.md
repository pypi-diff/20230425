# Comparing `tmp/CommonlyTools-2.0.5.tar.gz` & `tmp/CommonlyTools-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.0.5.tar", last modified: Tue Apr 25 02:28:26 2023, max compression
+gzip compressed data, was "CommonlyTools-2.0.6.tar", last modified: Tue Apr 25 02:46:20 2023, max compression
```

## Comparing `CommonlyTools-2.0.5.tar` & `CommonlyTools-2.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.0.5/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.5/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2827 2023-04-25 02:25:03.000000 CommonlyTools-2.0.5/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      735 2023-04-25 02:25:17.000000 CommonlyTools-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:46:20.056428 CommonlyTools-2.0.6/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:46:20.052428 CommonlyTools-2.0.6/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 02:46:19.000000 CommonlyTools-2.0.6/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-25 02:46:19.000000 CommonlyTools-2.0.6/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 02:46:19.000000 CommonlyTools-2.0.6/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-25 02:46:19.000000 CommonlyTools-2.0.6/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-25 02:46:19.000000 CommonlyTools-2.0.6/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 02:46:20.052428 CommonlyTools-2.0.6/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.0.6/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:46:20.052428 CommonlyTools-2.0.6/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.6/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2829 2023-04-25 02:43:59.000000 CommonlyTools-2.0.6/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 02:46:20.056428 CommonlyTools-2.0.6/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-04-25 02:43:31.000000 CommonlyTools-2.0.6/setup.py
```

### Comparing `CommonlyTools-2.0.5/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.0.6/CommonlyTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.5
+Version: 2.0.6
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.5/LICENSE` & `CommonlyTools-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.5/PKG-INFO` & `CommonlyTools-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.5
+Version: 2.0.6
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.5/README.md` & `CommonlyTools-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.5/commonlytools/discohook.py` & `CommonlyTools-2.0.6/commonlytools/discohook.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     for embed in embeds:
         result={}
         if embed.title != None:
             result["title"]=embed.title
         if embed.description != None:
             result["description"]=embed.description
         result["color"]=embed.colour
-        if embed.field != {}:
-            result["fields"]=embed.field
+        if embed.fields != []:
+            result["fields"]=embed.fields
         if embed.author != {}:
             result["author"]=embed.author
         if embed.footer != {}:
             result["footer"]=embed.footer
         if embed.timestamp:
             result["timestamp"]=embed.timestamp
         if embed.image != {}:
```

### Comparing `CommonlyTools-2.0.5/setup.py` & `CommonlyTools-2.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.0.5",
+    version="2.0.6",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

