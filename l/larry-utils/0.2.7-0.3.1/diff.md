# Comparing `tmp/larry_utils-0.2.7.tar.gz` & `tmp/larry_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "larry_utils-0.2.7.tar", last modified: Fri Apr  7 02:57:16 2023, max compression
+gzip compressed data, was "larry_utils-0.3.1.tar", last modified: Tue Apr 25 10:35:02 2023, max compression
```

## Comparing `larry_utils-0.2.7.tar` & `larry_utils-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-07 02:57:16.116927 larry_utils-0.2.7/
--rw-r--r--   0 root         (0) staff       (20)      162 2023-04-07 02:57:16.116799 larry_utils-0.2.7/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-07 02:57:16.116001 larry_utils-0.2.7/larry_utils/
--rw-r--r--   0 root         (0) staff       (20)     4118 2023-04-07 02:56:46.000000 larry_utils-0.2.7/larry_utils/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      530 2023-02-21 04:24:25.000000 larry_utils-0.2.7/larry_utils/create.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-07 02:57:16.116625 larry_utils-0.2.7/larry_utils.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      162 2023-04-07 02:57:16.000000 larry_utils-0.2.7/larry_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      228 2023-04-07 02:57:16.000000 larry_utils-0.2.7/larry_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-07 02:57:16.000000 larry_utils-0.2.7/larry_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-07 02:57:15.000000 larry_utils-0.2.7/larry_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       12 2023-04-07 02:57:16.000000 larry_utils-0.2.7/larry_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-07 02:57:16.116978 larry_utils-0.2.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      369 2023-04-07 02:57:14.000000 larry_utils-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-25 10:35:02.649432 larry_utils-0.3.1/
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-04-25 10:35:02.649193 larry_utils-0.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-25 10:35:02.648161 larry_utils-0.3.1/larry_utils/
+-rw-r--r--   0 root         (0) staff       (20)     3263 2023-04-25 10:34:48.000000 larry_utils-0.3.1/larry_utils/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      530 2023-02-21 04:24:25.000000 larry_utils-0.3.1/larry_utils/create.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-25 10:35:02.648911 larry_utils-0.3.1/larry_utils.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      162 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      228 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       12 2023-04-25 10:35:02.000000 larry_utils-0.3.1/larry_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-25 10:35:02.649510 larry_utils-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      369 2023-04-25 10:34:58.000000 larry_utils-0.3.1/setup.py
```

### Comparing `larry_utils-0.2.7/larry_utils/__init__.py` & `larry_utils-0.3.1/larry_utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,35 +71,14 @@
         with open(savename, 'wb') as f:
             f.write(x)
         return True
     except Exception as e:
         print(e)
         return False
 
-def extrat_tags(line, tags):
-    res = []
-    for t in tags:
-        if t in line:
-            res.append(t)
-    res = sorted(res, key=lambda x: -len(x))
-    new = []
-    for i in res:
-        find = False
-        for j in new:
-            if i in j:
-                find = True 
-                break
-        if not find:
-            new.append(i)
-    if len(new):
-        idx = [line.index(_) for _ in new]
-        new = list(zip(new, idx))
-        new = sorted(new, key=lambda x: -x[1])
-        new = [i[0] for i in new] 
-    return new
 
 
 def read_json(file_path):
     d = open(file_path).read().split('\n')
     res = []
     for line in d:
         try:
@@ -121,32 +100,24 @@
 
 def write_pkl(file_path, d):
     import pickle
     with open(file_path, 'wb') as f:
         f.write(pickle.dumps(d))
 
 
+
 def get_resolution(resolution):
     resolutions = [('16:9', 16./9), ('4:3', 4./3), ('1:1', 1), ('3:4', 3./4), ('9:16', 9./16)]
  
     Bmatch, Bdistance = '', 19
     ratio = resolution[0] / resolution[1]
     if True:
         for match, distance in resolutions:
             if abs(ratio - distance) < Bdistance:
                 Bmatch = match
                 Bdistance = abs(ratio - distance)
     return Bmatch
 
 
-import os
-ddd = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'map.pkl')
-
-en2ch = pickle.loads(open(ddd, 'rb').read())
-def translate_tag(tag):
-    if tag in en2ch:
-        return en2ch[tag]
-    elif tag.replace('_', ' ') in en2ch:
-        return en2ch[tag.replace('_', ' ')]
-    elif tag.replace(' ', '_') in en2ch:
-        return en2ch[tag.replace(' ', '_')]
-    return tag
+def hash(x):
+    import hashlib
+    return hashlib.md5(x).hexdigest()
```

### Comparing `larry_utils-0.2.7/larry_utils/create.py` & `larry_utils-0.3.1/larry_utils/create.py`

 * *Files identical despite different names*

