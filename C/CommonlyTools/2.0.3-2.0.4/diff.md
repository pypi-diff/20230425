# Comparing `tmp/CommonlyTools-2.0.3.tar.gz` & `tmp/CommonlyTools-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.0.3.tar", last modified: Tue Apr 25 01:22:51 2023, max compression
+gzip compressed data, was "CommonlyTools-2.0.4.tar", last modified: Tue Apr 25 01:25:03 2023, max compression
```

## Comparing `CommonlyTools-2.0.3.tar` & `CommonlyTools-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:22:51.304210 CommonlyTools-2.0.3/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:22:51.300210 CommonlyTools-2.0.3/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1646 2023-04-25 01:22:51.000000 CommonlyTools-2.0.3/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-25 01:22:51.000000 CommonlyTools-2.0.3/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 01:22:51.000000 CommonlyTools-2.0.3/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-25 01:22:51.000000 CommonlyTools-2.0.3/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-25 01:22:51.000000 CommonlyTools-2.0.3/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1646 2023-04-25 01:22:51.300210 CommonlyTools-2.0.3/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      911 2023-04-24 12:32:29.000000 CommonlyTools-2.0.3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:22:51.300210 CommonlyTools-2.0.3/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.3/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2726 2023-04-25 01:19:59.000000 CommonlyTools-2.0.3/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 01:22:51.304210 CommonlyTools-2.0.3/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      735 2023-04-25 01:21:45.000000 CommonlyTools-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-25 01:25:03.000000 CommonlyTools-2.0.4/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1661 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      926 2023-04-25 01:24:30.000000 CommonlyTools-2.0.4/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.4/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2726 2023-04-25 01:19:59.000000 CommonlyTools-2.0.4/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-25 01:25:03.435961 CommonlyTools-2.0.4/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      735 2023-04-25 01:24:41.000000 CommonlyTools-2.0.4/setup.py
```

### Comparing `CommonlyTools-2.0.3/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.0.4/CommonlyTools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.3
+Version: 2.0.4
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
@@ -16,15 +16,15 @@
         
         >commonlytools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
         >>>from commonlytools import discohook
         >>>
-        >>>embed=discohook.Embed(color=..., colour=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
+        >>>embed=discohook.Embed(color=..., colour=..., timestamp=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
         >>>```
         >>
```

### Comparing `CommonlyTools-2.0.3/LICENSE` & `CommonlyTools-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.3/PKG-INFO` & `CommonlyTools-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.3
+Version: 2.0.4
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
@@ -16,15 +16,15 @@
         
         >commonlytools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
         >>>from commonlytools import discohook
         >>>
-        >>>embed=discohook.Embed(color=..., colour=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
+        >>>embed=discohook.Embed(color=..., colour=..., timestamp=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
         >>>```
         >>
```

### Comparing `CommonlyTools-2.0.3/README.md` & `CommonlyTools-2.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 >commonlytools/discohook.py
 >>Discord Webhook Sender
 >>>Step 1(If you do not need to use embed, you can skip this step.)
 >>>```py
 >>>from commonlytools import discohook
 >>>
->>>embed=discohook.Embed(color=..., colour=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
+>>>embed=discohook.Embed(color=..., colour=..., timestamp=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
 >>>embed.author(name="...", url="...", icon_url="...") #author
 >>>embed.footer(text="...", icon_url="...") #footer
 >>>embed.image(image_url="...") #image
 >>>embed.thumbnail(thumbnail_url="...") #thumbnail
 >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
 >>>```
 >>
```

### Comparing `CommonlyTools-2.0.3/commonlytools/discohook.py` & `CommonlyTools-2.0.4/commonlytools/discohook.py`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.3/setup.py` & `CommonlyTools-2.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.0.3",
+    version="2.0.4",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```

