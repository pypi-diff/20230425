# Comparing `tmp/CommonlyTools-2.0.4.tar.gz` & `tmp/CommonlyTools-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.0.4.tar", last modified: Tue Apr 25 01:25:03 2023, max compression
+gzip compressed data, was "CommonlyTools-2.0.5.tar", last modified: Tue Apr 25 02:28:26 2023, max compression
```

## Comparing `CommonlyTools-2.0.4.tar` & `CommonlyTools-2.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:24:30.000000 CommonlyTools-2.0.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.4/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2726 2023-04-25 01:19:59.000000 CommonlyTools-2.0.4/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      735 2023-04-25 01:24:41.000000 CommonlyTools-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-25 02:28:26.000000 CommonlyTools-2.0.5/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:35:28.000000 CommonlyTools-2.0.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.5/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2827 2023-04-25 02:25:03.000000 CommonlyTools-2.0.5/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 02:28:26.654048 CommonlyTools-2.0.5/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-04-25 02:25:17.000000 CommonlyTools-2.0.5/setup.py
```

### Comparing `CommonlyTools-2.0.4/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.0.5/CommonlyTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.4
+Version: 2.0.5
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.4/LICENSE` & `CommonlyTools-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.4/PKG-INFO` & `CommonlyTools-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.4
+Version: 2.0.5
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
```

### Comparing `CommonlyTools-2.0.4/README.md` & `CommonlyTools-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.4/commonlytools/discohook.py` & `CommonlyTools-2.0.5/commonlytools/discohook.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,26 +15,34 @@
         self._author={}
         self._footer={}
         self._thumbnail={}
         self._field=[]
         
 
     def author(self, name:str=None, url:str=None, icon_url:str=None):
+        if name == None and url == None and icon_url == None:
+            return self._author
         self._author={"name": name, "url": url, "icon_url": icon_url}
 
 
     def footer(self, text:str=None, icon_url:str=None):
+        if text == None and icon_url == None:
+            return self._footer
         self._footer={"text": text, "icon_url": icon_url}
 
 
-    def image(self, image_url):
+    def image(self, image_url:str=None):
+        if image_url == None:
+            return self._image
         self._image={"url": image_url}
 
 
-    def thumbnail(self, thumbnail_url):
+    def thumbnail(self, thumbnail_url:str=None):
+        if thumbnail_url == None:
+            return self._thumbnail
         self._thumbnail={"url": thumbnail_url}
 
 
     def add_field(self, name:str=None, value:str=None, inline:bool=False):
         self._field.append({"name": name, "value": value, "inline": inline})
 
 
@@ -49,31 +57,15 @@
         return self._colour
 
 
     def timestamp(self):
         return self._timestamp
 
 
-    def image(self):
-        return self._image
-
-
-    def author(self):
-        return self._author
-        
-
-    def footer(self):
-        return self._footer
-
-
-    def thumbnail(self):
-        return self._thumbnail
-
-
-    def field(self):
+    def fields(self):
         return self._field
 
 
 def send(webhook_url:str, username:str=None, avatar_url:str=None, content:str=None, embeds:list=[]):
     embeds_dict=[]
     for embed in embeds:
         result={}
```

### Comparing `CommonlyTools-2.0.4/setup.py` & `CommonlyTools-2.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.0.4",
+    version="2.0.5",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

