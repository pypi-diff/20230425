# Comparing `tmp/watchmen_indicator_kernel-16.5.0.tar.gz` & `tmp/watchmen_indicator_kernel-16.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_kernel-16.5.0.tar", max compression
+gzip compressed data, was "watchmen_indicator_kernel-16.5.1.tar", max compression
```

## Comparing `watchmen_indicator_kernel-16.5.0.tar` & `watchmen_indicator_kernel-16.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1281 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/__init__.py
--rw-r--r--   0        0        0       86 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/common/__init__.py
--rw-r--r--   0        0        0       49 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/common/exception.py
--rw-r--r--   0        0        0      329 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/common/settings.py
--rw-r--r--   0        0        0      286 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/__init__.py
--rw-r--r--   0        0        0       53 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/data_helper.py
--rw-r--r--   0        0        0     4327 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/inspection_data_service.py
--rw-r--r--   0        0        0    11588 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/subject_base_service.py
--rw-r--r--   0        0        0    19385 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/topic_base_service.py
--rw-r--r--   0        0        0      140 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective/__init__.py
--rw-r--r--   0        0        0      313 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective/data_helper.py
--rw-r--r--   0        0        0    27145 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective/data_service.py
--rw-r--r--   0        0        0       59 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
--rw-r--r--   0        0        0    11941 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
--rw-r--r--   0        0        0    21400 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
--rw-r--r--   0        0        0    10799 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
--rw-r--r--   0        0        0     8341 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
--rw-r--r--   0        0        0      397 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/bucket.py
--rw-r--r--   0        0        0      979 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/derived_objective.py
--rw-r--r--   0        0        0     1051 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/enum.py
--rw-r--r--   0        0        0      284 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/factor.py
--rw-r--r--   0        0        0     1330 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/indicator.py
--rw-r--r--   0        0        0     3110 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/parameter.py
--rw-r--r--   0        0        0      786 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/subject.py
--rw-r--r--   0        0        0    12305 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/time_frame.py
--rw-r--r--   0        0        0     1074 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/topic.py
--rw-r--r--   0        0        0      268 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1762 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/achievement_task_service.py
--rw-r--r--   0        0        0     8647 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/bucket_service.py
--rw-r--r--   0        0        0     4960 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/derived_objective_service.py
--rw-r--r--   0        0        0     6695 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/indicator_service.py
--rw-r--r--   0        0        0     5783 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/objective_service.py
--rw-r--r--   0        0        0       46 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/plugin/__init__.py
--rw-r--r--   0        0        0      678 2023-04-06 09:13:10.388010 watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/plugin/connector.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1281 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/common/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/common/exception.py
+-rw-r--r--   0        0        0      329 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/common/settings.py
+-rw-r--r--   0        0        0      286 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/__init__.py
+-rw-r--r--   0        0        0     1901 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/data_helper.py
+-rw-r--r--   0        0        0     4327 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/inspection_data_service.py
+-rw-r--r--   0        0        0    11588 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/subject_base_service.py
+-rw-r--r--   0        0        0    19385 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/topic_base_service.py
+-rw-r--r--   0        0        0      140 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/data_helper.py
+-rw-r--r--   0        0        0    27145 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/data_service.py
+-rw-r--r--   0        0        0       59 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
+-rw-r--r--   0        0        0    11941 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
+-rw-r--r--   0        0        0    21400 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
+-rw-r--r--   0        0        0    10799 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
+-rw-r--r--   0        0        0     8341 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
+-rw-r--r--   0        0        0      397 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/bucket.py
+-rw-r--r--   0        0        0      979 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/derived_objective.py
+-rw-r--r--   0        0        0     1051 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/enum.py
+-rw-r--r--   0        0        0      284 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/factor.py
+-rw-r--r--   0        0        0     1330 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/indicator.py
+-rw-r--r--   0        0        0     3110 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/parameter.py
+-rw-r--r--   0        0        0      786 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/subject.py
+-rw-r--r--   0        0        0    12305 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/time_frame.py
+-rw-r--r--   0        0        0     1074 2023-04-25 10:52:45.980220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/topic.py
+-rw-r--r--   0        0        0      268 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1762 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/achievement_task_service.py
+-rw-r--r--   0        0        0     8647 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/bucket_service.py
+-rw-r--r--   0        0        0     4960 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/derived_objective_service.py
+-rw-r--r--   0        0        0     6695 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/indicator_service.py
+-rw-r--r--   0        0        0     5783 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/objective_service.py
+-rw-r--r--   0        0        0       46 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/plugin/__init__.py
+-rw-r--r--   0        0        0      678 2023-04-25 10:52:45.984220 watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/plugin/connector.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.5.1/PKG-INFO
```

### Comparing `watchmen_indicator_kernel-16.5.0/pyproject.toml` & `watchmen_indicator_kernel-16.5.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-indicator-kernel"
-version = "16.5.0"
+version = "16.5.1"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.0"
-watchmen-inquiry-trino = { version = "16.5.0", optional = true }
-watchmen-storage-mysql = { version = "16.5.0", optional = true }
-watchmen-storage-oracle = { version = "16.5.0", optional = true }
-watchmen-storage-mongodb = { version = "16.5.0", optional = true }
-watchmen-storage-mssql = { version = "16.5.0", optional = true }
-watchmen-storage-postgresql = { version = "16.5.0", optional = true }
-watchmen-storage-oss = { version = "16.5.0", optional = true }
-watchmen-storage-s3 = { version = "16.5.0", optional = true }
+watchmen-inquiry-kernel = "16.5.1"
+watchmen-inquiry-trino = { version = "16.5.1", optional = true }
+watchmen-storage-mysql = { version = "16.5.1", optional = true }
+watchmen-storage-oracle = { version = "16.5.1", optional = true }
+watchmen-storage-mongodb = { version = "16.5.1", optional = true }
+watchmen-storage-mssql = { version = "16.5.1", optional = true }
+watchmen-storage-postgresql = { version = "16.5.1", optional = true }
+watchmen-storage-oss = { version = "16.5.1", optional = true }
+watchmen-storage-s3 = { version = "16.5.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/data_helper.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/data_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/inspection_data_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/inspection_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/subject_base_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/subject_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/inspection/topic_base_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/inspection/topic_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective/data_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/data_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/bucket.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/bucket.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/derived_objective.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/derived_objective.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/enum.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/enum.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/indicator.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/indicator.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/parameter.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/subject.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/subject.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/time_frame.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/time_frame.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/data/utils/topic.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/data/utils/topic.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/achievement_task_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/achievement_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/bucket_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/bucket_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/derived_objective_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/derived_objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/indicator_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/indicator_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/meta/objective_service.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/meta/objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.0/src/watchmen_indicator_kernel/plugin/connector.py` & `watchmen_indicator_kernel-16.5.1/src/watchmen_indicator_kernel/plugin/connector.py`

 * *Files identical despite different names*

