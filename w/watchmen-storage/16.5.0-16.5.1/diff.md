# Comparing `tmp/watchmen_storage-16.5.0.tar.gz` & `tmp/watchmen_storage-16.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.0.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.1.tar", max compression
```

## Comparing `watchmen_storage-16.5.0.tar` & `watchmen_storage-16.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1061 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/LICENSE
--rw-r--r--   0        0        0      472 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/pyproject.toml
--rw-r--r--   0        0        0     2196 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1685 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0      988 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0     7259 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5884 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4645 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-04-06 09:13:10.428011 watchmen_storage-16.5.0/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 watchmen_storage-16.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/LICENSE
+-rw-r--r--   0        0        0      472 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2196 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1685 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0      988 2023-04-25 10:52:46.028224 watchmen_storage-16.5.1/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0     7259 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     5884 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4645 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-04-25 10:52:46.032224 watchmen_storage-16.5.1/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 watchmen_storage-16.5.1/PKG-INFO
```

### Comparing `watchmen_storage-16.5.0/LICENSE` & `watchmen_storage-16.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.1/src/watchmen_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.1/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.1/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.1/src/watchmen_storage/free_storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.1/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.1/src/watchmen_storage/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.1/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.1/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.1/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.1/src/watchmen_storage/storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.1/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.1/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.0/PKG-INFO` & `watchmen_storage-16.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage
-Version: 16.5.0
+Version: 16.5.1
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.24.20,<2.0.0)
-Requires-Dist: watchmen-model (==16.5.0)
+Requires-Dist: watchmen-model (==16.5.1)
```

