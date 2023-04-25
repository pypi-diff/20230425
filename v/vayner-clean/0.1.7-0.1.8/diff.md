# Comparing `tmp/vayner_clean-0.1.7.tar.gz` & `tmp/vayner_clean-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vayner_clean-0.1.7.tar", last modified: Thu Apr 20 07:25:50 2023, max compression
+gzip compressed data, was "vayner_clean-0.1.8.tar", last modified: Tue Apr 25 09:50:37 2023, max compression
```

## Comparing `vayner_clean-0.1.7.tar` & `vayner_clean-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-20 07:25:50.200290 vayner_clean-0.1.7/
--rw-r--r--   0 willbutler   (502) staff       (20)     1379 2023-04-20 07:25:50.200063 vayner_clean-0.1.7/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      703 2023-03-14 11:27:46.000000 vayner_clean-0.1.7/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-04-20 07:25:50.200365 vayner_clean-0.1.7/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1314 2023-04-20 07:25:39.000000 vayner_clean-0.1.7/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-20 07:25:50.199292 vayner_clean-0.1.7/vayner_clean.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     1379 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      251 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       27 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-04-20 07:25:50.000000 vayner_clean-0.1.7/vayner_clean.egg-info/top_level.txt
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-20 07:25:50.199559 vayner_clean-0.1.7/vee_clean/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-23 14:12:51.000000 vayner_clean-0.1.7/vee_clean/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    15754 2023-04-20 07:20:21.000000 vayner_clean-0.1.7/vee_clean/cleaning_functions.py
+drwxr-xr-x   0 achilleasdrakou   (502) staff       (20)        0 2023-04-25 09:50:37.230348 vayner_clean-0.1.8/
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)     1379 2023-04-25 09:50:37.230149 vayner_clean-0.1.8/PKG-INFO
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)      703 2023-04-25 09:39:33.000000 vayner_clean-0.1.8/README.md
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)       38 2023-04-25 09:50:37.230413 vayner_clean-0.1.8/setup.cfg
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)     1314 2023-04-25 09:47:52.000000 vayner_clean-0.1.8/setup.py
+drwxr-xr-x   0 achilleasdrakou   (502) staff       (20)        0 2023-04-25 09:50:37.229461 vayner_clean-0.1.8/vayner_clean.egg-info/
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)     1379 2023-04-25 09:50:37.000000 vayner_clean-0.1.8/vayner_clean.egg-info/PKG-INFO
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)      251 2023-04-25 09:50:37.000000 vayner_clean-0.1.8/vayner_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)        1 2023-04-25 09:50:37.000000 vayner_clean-0.1.8/vayner_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)       27 2023-04-25 09:50:37.000000 vayner_clean-0.1.8/vayner_clean.egg-info/requires.txt
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)       10 2023-04-25 09:50:37.000000 vayner_clean-0.1.8/vayner_clean.egg-info/top_level.txt
+drwxr-xr-x   0 achilleasdrakou   (502) staff       (20)        0 2023-04-25 09:50:37.229740 vayner_clean-0.1.8/vee_clean/
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)        0 2023-02-16 10:40:13.000000 vayner_clean-0.1.8/vee_clean/__init__.py
+-rw-r--r--   0 achilleasdrakou   (502) staff       (20)    15763 2023-04-25 09:47:56.000000 vayner_clean-0.1.8/vee_clean/cleaning_functions.py
```

### Comparing `vayner_clean-0.1.7/PKG-INFO` & `vayner_clean-0.1.8/vayner_clean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vayner_clean
-Version: 0.1.7
+Name: vayner-clean
+Version: 0.1.8
 Summary: Library for cleaning advertising data from Tracer
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vayner_clean-0.1.7/README.md` & `vayner_clean-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `vayner_clean-0.1.7/setup.py` & `vayner_clean-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="vayner_clean",
-    version="0.1.7",
+    version="0.1.8",
     description="Library for cleaning advertising data from Tracer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Will Butler",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `vayner_clean-0.1.7/vayner_clean.egg-info/PKG-INFO` & `vayner_clean-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vayner-clean
-Version: 0.1.7
+Name: vayner_clean
+Version: 0.1.8
 Summary: Library for cleaning advertising data from Tracer
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vayner_clean-0.1.7/vee_clean/cleaning_functions.py` & `vayner_clean-0.1.8/vee_clean/cleaning_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                            u"\U0001F600-\U0001F64F"  # emoticons
                            u"\U0001F300-\U0001F5FF"  # symbols & pictographs
                            u"\U0001F680-\U0001F6FF"  # transport & map symbols
                            u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
                            "]+", flags=re.UNICODE)
 
 def clean_column_names(df, hardcode_col_dict = {},errors= 'ignore',cols_no_change = ['spend', 'date', 'currency', 
-                            'cohort', 'creative_name', 'group_id', 'engagements', 'created',
+                            'cohort', 'creative_name', 'group_id', 'engagements', 'created', 'ad_id',
                             'plays', 'saved', 'post_hastags', 'content_type', 'linked_content', 'post_id',
                             'video_duration', 'average_time_watched', 'total_time_watched',
                             'adset_targeting', 'completion_rate', 'targeting', 'cohort_new',
                             'video_completions', 'post_hashtags']):
 
     """Cleans the column names of an advertisement performance (organic or paid) dataset, commonly from
     Tracer but could also be from Sprout social. The column names will be standardized so
```

