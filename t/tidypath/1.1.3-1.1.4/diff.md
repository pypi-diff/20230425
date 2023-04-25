# Comparing `tmp/tidypath-1.1.3.tar.gz` & `tmp/tidypath-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.1.3.tar", last modified: Tue Apr 11 21:39:48 2023, max compression
+gzip compressed data, was "tidypath-1.1.4.tar", last modified: Tue Apr 25 10:39:25 2023, max compression
```

## Comparing `tidypath-1.1.3.tar` & `tidypath-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 21:39:48.498314 tidypath-1.1.3/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2022-11-08 08:37:56.000000 tidypath-1.1.3/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 21:39:48.498314 tidypath-1.1.3/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     2804 2023-01-17 19:01:52.000000 tidypath-1.1.3/README.md
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-04-11 21:39:48.498314 tidypath-1.1.3/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1161 2023-04-11 21:39:36.000000 tidypath-1.1.3/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 21:39:48.498314 tidypath-1.1.3/tidypath/
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1629 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5054 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/config.py
--rw-r--r--   0 userx     (1000) wheel      (998)    11478 2023-04-11 21:39:01.000000 tidypath-1.1.3/tidypath/decorators.py
--rw-r--r--   0 userx     (1000) wheel      (998)     6075 2023-04-11 21:32:52.000000 tidypath-1.1.3/tidypath/fmt.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5197 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/inspection.py
--rw-r--r--   0 userx     (1000) wheel      (998)    13081 2023-04-11 21:38:10.000000 tidypath-1.1.3/tidypath/paths.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9844 2023-01-17 19:01:52.000000 tidypath-1.1.3/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 21:39:48.498314 tidypath-1.1.3/tidypath.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      358 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)       63 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        9 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 10:39:25.789180 tidypath-1.1.4/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-07 11:08:19.000000 tidypath-1.1.4/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2023-04-25 10:39:25.789180 tidypath-1.1.4/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2804 2022-11-25 17:30:15.000000 tidypath-1.1.4/README.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-04-25 10:39:25.793180 tidypath-1.1.4/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1161 2023-04-25 10:39:19.000000 tidypath-1.1.4/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 10:39:25.765179 tidypath-1.1.4/tidypath/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2022-11-07 12:11:16.000000 tidypath-1.1.4/tidypath/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1629 2022-11-07 17:52:31.000000 tidypath-1.1.4/tidypath/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5054 2022-11-07 17:57:44.000000 tidypath-1.1.4/tidypath/config.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    11570 2023-04-25 10:36:09.000000 tidypath-1.1.4/tidypath/decorators.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     6075 2023-04-25 10:34:17.000000 tidypath-1.1.4/tidypath/fmt.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5197 2022-11-07 17:56:37.000000 tidypath-1.1.4/tidypath/inspection.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    13081 2023-04-25 10:34:17.000000 tidypath-1.1.4/tidypath/paths.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9844 2022-11-08 08:59:29.000000 tidypath-1.1.4/tidypath/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-04-25 10:39:25.785180 tidypath-1.1.4/tidypath.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2023-04-25 10:39:25.000000 tidypath-1.1.4/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.1.3/LICENSE.md` & `tidypath-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/PKG-INFO` & `tidypath-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.1.3/README.md` & `tidypath-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/setup.py` & `tidypath-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.1.3',
+    version='1.1.4',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.1.3/tidypath/_helper.py` & `tidypath-1.1.4/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/tidypath/config.py` & `tidypath-1.1.4/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/tidypath/decorators.py` & `tidypath-1.1.4/tidypath/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,26 +84,28 @@
     def _savedata(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, funcname_in_filename=funcname_in_filename, **kwargs):
             key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
             save_keys = merge_nested_dict(key_opts, keys, key_default="all")
             saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
 
-            if len(saving_path) > max_str_length:
+            filename_too_long = len(saving_path) > max_str_length
+            if filename_too_long:
                 saving_path = hash_path(saving_path)
-                warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
 
             if Path(saving_path).exists() and not overwrite:
                 try:
                     result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
                 except EOFError:
                     warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
                     result = func(*args, **kwargs)
                     getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
             else:
+                if filename_too_long:
+                    warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
                 result = func(*args, **kwargs)
                 getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
             return result
 
         wrapper.__signature__ = merge_wrapper_signatures(wrapper, ["overwrite", "keys", "save", "funcname_in_filename"])
         wrapper.__out__ = "data"
         return wrapper
```

### Comparing `tidypath-1.1.3/tidypath/fmt.py` & `tidypath-1.1.4/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/tidypath/inspection.py` & `tidypath-1.1.4/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/tidypath/paths.py` & `tidypath-1.1.4/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/tidypath/storage.py` & `tidypath-1.1.4/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.3/tidypath.egg-info/PKG-INFO` & `tidypath-1.1.4/tidypath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.3
+Version: 1.1.4
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

