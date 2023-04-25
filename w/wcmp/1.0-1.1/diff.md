# Comparing `tmp/wcmp-1.0.tar.gz` & `tmp/wcmp-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcmp-1.0.tar", last modified: Tue Apr 25 12:31:31 2023, max compression
+gzip compressed data, was "wcmp-1.1.tar", last modified: Tue Apr 25 13:28:13 2023, max compression
```

## Comparing `wcmp-1.0.tar` & `wcmp-1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 12:31:31.119068 wcmp-1.0/
--rw-rw-rw-   0        0        0     1089 2023-04-24 13:47:39.000000 wcmp-1.0/LICENSE
--rw-rw-rw-   0        0        0      801 2023-04-25 12:31:31.114059 wcmp-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-25 12:22:36.000000 wcmp-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 12:31:31.119068 wcmp-1.0/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-04-24 13:44:59.000000 wcmp-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:31:31.103093 wcmp-1.0/wcmp/
--rw-rw-rw-   0        0        0      777 2023-04-25 12:19:32.000000 wcmp-1.0/wcmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:31:31.113066 wcmp-1.0/wcmp.egg-info/
--rw-rw-rw-   0        0        0      801 2023-04-25 12:31:31.000000 wcmp-1.0/wcmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2023-04-25 12:31:31.000000 wcmp-1.0/wcmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:31:31.000000 wcmp-1.0/wcmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 12:31:31.000000 wcmp-1.0/wcmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:28:13.271732 wcmp-1.1/
+-rw-rw-rw-   0        0        0       32 2023-04-25 12:48:57.000000 wcmp-1.1/.gitignore
+-rw-rw-rw-   0        0        0     1089 2023-04-24 13:47:39.000000 wcmp-1.1/LICENSE
+-rw-rw-rw-   0        0        0      907 2023-04-25 13:28:13.271732 wcmp-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-04-25 12:55:34.000000 wcmp-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:28:13.272725 wcmp-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-04-25 13:25:05.000000 wcmp-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:28:13.258764 wcmp-1.1/wcmp/
+-rw-rw-rw-   0        0        0      965 2023-04-25 13:17:25.000000 wcmp-1.1/wcmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:28:13.266741 wcmp-1.1/wcmp.egg-info/
+-rw-rw-rw-   0        0        0      907 2023-04-25 13:28:12.000000 wcmp-1.1/wcmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-04-25 13:28:13.000000 wcmp-1.1/wcmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:28:12.000000 wcmp-1.1/wcmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 13:28:12.000000 wcmp-1.1/wcmp.egg-info/top_level.txt
```

### Comparing `wcmp-1.0/LICENSE` & `wcmp-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wcmp-1.0/PKG-INFO` & `wcmp-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcmp
-Version: 1.0
+Version: 1.1
 Summary: A simple message plus package for notification via wechat.
 Home-page: https://github.com/moshangsang24/wcmp
 Author: moshangsang24
 Author-email: liuyifan731@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,7 +30,11 @@
 ```python
 import wcmp
 # replace the 'X' with your token
 s=wcmp('XXXXXXX')
 s.send('messgaedf')
 ```
 
+## About the Token
+You need to get your personal token from [PushPlush](https://www.pushplus.plus/)
+
+
```

### Comparing `wcmp-1.0/setup.py` & `wcmp-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="wcmp",
-  version="1.0",
+  version="1.1",
   author="moshangsang24",
   author_email="liuyifan731@163.com",
   description="A simple message plus package for notification via wechat.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/moshangsang24/wcmp",
   packages=setuptools.find_packages(),
```

### Comparing `wcmp-1.0/wcmp/__init__.py` & `wcmp-1.1/wcmp/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from urllib.request import urlopen
 from urllib.parse import urlencode
 name = "wcmp"
 
 class wcmp(object):
     def __init__(self,token,base_url='http://www.pushplus.plus/send') -> None:
+        """
+        Args:
+            token: Personal Key Token provided by Pushplus.
+        """
         self.token=token
         self.base_url=base_url
         
     def send(self,content,title=None):
+        """
+        Send Messages.
+        Args:
+            content: Message content (Required)
+            title: Message title (Optional, Bolder font in message)
+        """
         if not isinstance(content,str):
             raise 'The message content must be string!'
         md={'token':self.token,'content':content}
         if title:
             if not isinstance(title,str):
                 raise 'The message title must be string!'
             md['title']=title
         send_url=self.base_url+'?'+urlencode(md)
         urlopen(send_url)
 
 
-if __name__=="__main__":
-    s=wcmp('50a1bcd158c7410dadad532249e02ac0')
-    s.send('messgaedf')
```

### Comparing `wcmp-1.0/wcmp.egg-info/PKG-INFO` & `wcmp-1.1/wcmp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcmp
-Version: 1.0
+Version: 1.1
 Summary: A simple message plus package for notification via wechat.
 Home-page: https://github.com/moshangsang24/wcmp
 Author: moshangsang24
 Author-email: liuyifan731@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,7 +30,11 @@
 ```python
 import wcmp
 # replace the 'X' with your token
 s=wcmp('XXXXXXX')
 s.send('messgaedf')
 ```
 
+## About the Token
+You need to get your personal token from [PushPlush](https://www.pushplus.plus/)
+
+
```

