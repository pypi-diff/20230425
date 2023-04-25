# Comparing `tmp/mynotiontools-0.0.8.2.tar.gz` & `tmp/mynotiontools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mynotiontools-0.0.8.2.tar", last modified: Thu Dec  1 08:01:57 2022, max compression
+gzip compressed data, was "dist/mynotiontools-0.0.9.tar", last modified: Thu Dec  1 08:41:34 2022, max compression
```

## Comparing `mynotiontools-0.0.8.2.tar` & `mynotiontools-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       38 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/setup.cfg
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     3770 2022-12-01 08:01:44.000000 mynotiontools-0.0.8.2/setup.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      608 2022-11-28 10:27:36.000000 mynotiontools-0.0.8.2/README.md
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1049 2022-11-27 17:38:00.000000 mynotiontools-0.0.8.2/LICENSE
-drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools.egg-info/
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        1 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools.egg-info/dependency_links.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       14 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools.egg-info/top_level.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        9 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools.egg-info/requires.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      321 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools.egg-info/SOURCES.txt
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1266 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools.egg-info/PKG-INFO
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.0.8.2/MANIFEST.in
-drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/mynotiontools/
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)    11316 2022-12-01 08:01:32.000000 mynotiontools-0.0.8.2/mynotiontools/__init__.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      352 2022-11-28 03:39:39.000000 mynotiontools-0.0.8.2/mynotiontools/__version__.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       40 2022-11-28 06:39:58.000000 mynotiontools-0.0.8.2/mynotiontools/main.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.0.8.2/mynotiontools/core.py
--rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1266 2022-12-01 08:01:57.000000 mynotiontools-0.0.8.2/PKG-INFO
+drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       38 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/setup.cfg
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     3767 2022-12-01 08:41:27.000000 mynotiontools-0.0.9/setup.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      608 2022-11-28 10:27:36.000000 mynotiontools-0.0.9/README.md
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1049 2022-11-27 17:38:00.000000 mynotiontools-0.0.9/LICENSE
+drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        1 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/dependency_links.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       14 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/top_level.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)        9 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/requires.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      321 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/SOURCES.txt
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1264 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools.egg-info/PKG-INFO
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.0.9/MANIFEST.in
+drwxrwxr-x   0 suyelu    (1000) suyelu    (1000)        0 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/mynotiontools/
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)    11452 2022-12-01 08:41:08.000000 mynotiontools-0.0.9/mynotiontools/__init__.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)      352 2022-11-28 03:39:39.000000 mynotiontools-0.0.9/mynotiontools/__version__.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       40 2022-11-28 06:39:58.000000 mynotiontools-0.0.9/mynotiontools/main.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)       26 2022-11-27 17:34:02.000000 mynotiontools-0.0.9/mynotiontools/core.py
+-rw-rw-r--   0 suyelu    (1000) suyelu    (1000)     1264 2022-12-01 08:41:34.000000 mynotiontools-0.0.9/PKG-INFO
```

### Comparing `mynotiontools-0.0.8.2/setup.py` & `mynotiontools-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'mynotiontools'
 DESCRIPTION = 'Some tools for notion, Just for fun.'
 URL = 'https://github.com/suyelu/mynotion'
 EMAIL = 'suyelu@hotmail.com'
 AUTHOR = 'Vincent Su'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.8.02'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests'
 ]
 
 # What packages are optional?
```

### Comparing `mynotiontools-0.0.8.2/README.md` & `mynotiontools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mynotiontools-0.0.8.2/LICENSE` & `mynotiontools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mynotiontools-0.0.8.2/mynotiontools.egg-info/PKG-INFO` & `mynotiontools-0.0.9/mynotiontools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mynotiontools
-Version: 0.0.8.2
+Version: 0.0.9
 Summary: Some tools for notion, Just for fun.
 Home-page: https://github.com/suyelu/mynotion
 Author: Vincent Su
 Author-email: suyelu@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mynotiontools-0.0.8.2/mynotiontools/__init__.py` & `mynotiontools-0.0.9/mynotiontools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,35 +9,39 @@
 
 class NotionHelper:
     def __init__(self, secrets = None):
         if secrets == None:
             self.secrets = os.environ.get('NOTION_SECRETS')
         else:
             self.secrets = secrets
+        if self.secrets == None:
+            print('NOTION_SECRETS not set')
+            return
         self.headers = {
             "accept": "application/json",
             "Notion-Version": "2022-06-28",
             "content-type": "application/json",
             "Authorization" : self.secrets
         }
         self.payload = {
-            "page_size" : 10000,
-            "filter": None
+            "page_size" : 10000
         }
         self.base_url = "https://api.notion.com/v1/databases/"
         self.keys = []
         self.rela = {}
 
     def get_keys(self, database_id):
         page_size_old = self.payload['page_size']
         self.payload['page_size'] = 1
         response = requests.request("POST", self.base_url + database_id + "/query", json = self.payload, headers = self.headers)
         res = json.loads(response.text)
+        print(response, res, self.headers)
         self.keys = list(res['results'][0]['properties'].keys())
         self.payload['page_size'] = page_size_old
+        return self.keys
 
     def get_rela_name(self, name, rela_id):
             if rela_id == 0:
                 return "None"
             if name not in self.rela:
                 self.rela[name] = {}
             if rela_id in self.rela[name]:
```

### Comparing `mynotiontools-0.0.8.2/PKG-INFO` & `mynotiontools-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mynotiontools
-Version: 0.0.8.2
+Version: 0.0.9
 Summary: Some tools for notion, Just for fun.
 Home-page: https://github.com/suyelu/mynotion
 Author: Vincent Su
 Author-email: suyelu@hotmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

