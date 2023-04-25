# Comparing `tmp/pyctm-0.0.7.tar.gz` & `tmp/pyctm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyctm-0.0.7.tar", last modified: Wed Sep  7 21:15:18 2022, max compression
+gzip compressed data, was "pyctm-0.0.8.tar", last modified: Tue Apr 25 02:07:46 2023, max compression
```

## Comparing `pyctm-0.0.7.tar` & `pyctm-0.0.8.tar`

### file list

```diff
@@ -1,43 +1,64 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.152997 pyctm-0.0.7/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1070 2022-03-23 23:56:36.000000 pyctm-0.0.7/LICENSE
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      224 2022-09-07 21:15:18.152997 pyctm-0.0.7/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       14 2022-03-23 23:56:36.000000 pyctm-0.0.7/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.144997 pyctm-0.0.7/pyctm/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-24 04:12:10.000000 pyctm-0.0.7/pyctm/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.144997 pyctm-0.0.7/pyctm/codelet/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-24 03:47:54.000000 pyctm-0.0.7/pyctm/codelet/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1788 2022-09-07 21:14:27.000000 pyctm-0.0.7/pyctm/codelet/codelet.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1539 2022-04-01 02:29:27.000000 pyctm-0.0.7/pyctm/codelet/codelet_application.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.148997 pyctm-0.0.7/pyctm/memory/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-24 03:47:56.000000 pyctm-0.0.7/pyctm/memory/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      163 2022-03-30 02:30:03.000000 pyctm-0.0.7/pyctm/memory/distributed_memory_type.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5633 2022-04-06 03:13:28.000000 pyctm-0.0.7/pyctm/memory/k_distributed_memory.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.148997 pyctm-0.0.7/pyctm/memory/kafka/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-25 04:19:57.000000 pyctm-0.0.7/pyctm/memory/kafka/__init__.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.152997 pyctm-0.0.7/pyctm/memory/kafka/builder/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-30 01:55:35.000000 pyctm-0.0.7/pyctm/memory/kafka/builder/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2588 2022-04-05 03:45:55.000000 pyctm-0.0.7/pyctm/memory/kafka/builder/k_consumer_builder.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1336 2022-04-05 03:48:58.000000 pyctm-0.0.7/pyctm/memory/kafka/builder/k_producer_builder.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.152997 pyctm-0.0.7/pyctm/memory/kafka/config/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-30 01:56:08.000000 pyctm-0.0.7/pyctm/memory/kafka/config/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      484 2022-04-05 02:16:48.000000 pyctm-0.0.7/pyctm/memory/kafka/config/topic_config.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       93 2022-03-30 03:10:04.000000 pyctm-0.0.7/pyctm/memory/kafka/k_distributed_memory_behavior.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.152997 pyctm-0.0.7/pyctm/memory/kafka/thread/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-30 01:56:38.000000 pyctm-0.0.7/pyctm/memory/kafka/thread/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2007 2022-04-06 03:14:22.000000 pyctm-0.0.7/pyctm/memory/kafka/thread/k_memory_content_publisher_thread.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1005 2022-04-06 03:15:27.000000 pyctm-0.0.7/pyctm/memory/kafka/thread/k_memory_content_receiver_thread.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      892 2022-04-01 02:32:12.000000 pyctm-0.0.7/pyctm/memory/kafka/topic_config_provider.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      410 2022-04-01 00:47:25.000000 pyctm-0.0.7/pyctm/memory/memory.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      889 2022-04-06 02:13:47.000000 pyctm-0.0.7/pyctm/memory/memory_object.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.152997 pyctm-0.0.7/pyctm/tests/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        0 2022-03-24 03:55:02.000000 pyctm-0.0.7/pyctm/tests/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1869 2022-04-06 03:18:18.000000 pyctm-0.0.7/pyctm/tests/k_distributed_memory_test.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1069 2022-04-05 13:01:53.000000 pyctm-0.0.7/pyctm/tests/memory_object_test.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2022-09-07 21:15:18.144997 pyctm-0.0.7/pyctm.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      224 2022-09-07 21:15:17.000000 pyctm-0.0.7/pyctm.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1037 2022-09-07 21:15:18.000000 pyctm-0.0.7/pyctm.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2022-09-07 21:15:17.000000 pyctm-0.0.7/pyctm.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       16 2022-09-07 21:15:17.000000 pyctm-0.0.7/pyctm.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        6 2022-09-07 21:15:17.000000 pyctm-0.0.7/pyctm.egg-info/top_level.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2022-09-07 21:15:18.152997 pyctm-0.0.7/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      420 2022-09-07 21:15:04.000000 pyctm-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.360651 pyctm-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-12-12 22:12:32.000000 pyctm-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-25 02:07:46.360651 pyctm-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       14 2022-12-12 22:12:32.000000 pyctm-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/plan_gui/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 23:28:52.000000 pyctm-0.0.8/plan_gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/plan_gui/gan_model/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 21:23:28.000000 pyctm-0.0.8/plan_gui/gan_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-04-10 20:48:18.000000 pyctm-0.0.8/plan_gui/gan_model/generator.py
+-rw-r--r--   0 root         (0) root         (0)    10493 2023-04-10 20:50:56.000000 pyctm-0.0.8/plan_gui/plan_gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/codelet/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/codelet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/codelet/codelet.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2022-12-20 02:57:57.000000 pyctm-0.0.8/pyctm/codelet/codelet_application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/correction_engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-19 01:18:41.000000 pyctm-0.0.8/pyctm/correction_engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-02-01 17:58:17.000000 pyctm-0.0.8/pyctm/correction_engines/naive_bayes_correction_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/memory/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      163 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/distributed_memory_type.py
+-rw-r--r--   0 root         (0) root         (0)     5633 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/k_distributed_memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/memory/kafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/memory/kafka/builder/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/builder/k_consumer_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/builder/k_producer_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm/memory/kafka/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      484 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/config/topic_config.py
+-rw-r--r--   0 root         (0) root         (0)       93 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/k_distributed_memory_behavior.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.360651 pyctm-0.0.8/pyctm/memory/kafka/thread/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/thread/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/thread/k_memory_content_publisher_thread.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/thread/k_memory_content_receiver_thread.py
+-rw-r--r--   0 root         (0) root         (0)      892 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/kafka/topic_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)      410 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/memory.py
+-rw-r--r--   0 root         (0) root         (0)      889 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/memory/memory_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.360651 pyctm-0.0.8/pyctm/representation/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      242 2023-01-31 03:48:20.000000 pyctm-0.0.8/pyctm/representation/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)      323 2022-12-20 02:55:39.000000 pyctm-0.0.8/pyctm/representation/idea.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2022-12-20 04:31:17.000000 pyctm-0.0.8/pyctm/representation/idea_metadata_values.py
+-rw-r--r--   0 root         (0) root         (0)      310 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/representation/sdr_idea.py
+-rw-r--r--   0 root         (0) root         (0)      242 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/representation/sdr_idea_builder.py
+-rw-r--r--   0 root         (0) root         (0)     8334 2023-02-01 18:44:30.000000 pyctm-0.0.8/pyctm/representation/sdr_idea_deserializer.py
+-rw-r--r--   0 root         (0) root         (0)     9867 2023-03-16 13:00:25.000000 pyctm-0.0.8/pyctm/representation/sdr_idea_serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-01-19 04:41:24.000000 pyctm-0.0.8/pyctm/representation/value_converter.py
+-rw-r--r--   0 root         (0) root         (0)      396 2022-12-20 04:25:35.000000 pyctm-0.0.8/pyctm/representation/value_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.360651 pyctm-0.0.8/pyctm/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/tests/k_distributed_memory_test.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-12-12 22:12:32.000000 pyctm-0.0.8/pyctm/tests/memory_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-02-01 18:44:28.000000 pyctm-0.0.8/pyctm/tests/sdr_idea_serializer_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 02:07:46.356651 pyctm-0.0.8/pyctm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-25 02:07:46.000000 pyctm-0.0.8/pyctm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 02:07:46.000000 pyctm-0.0.8/pyctm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 02:07:46.000000 pyctm-0.0.8/pyctm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-25 02:07:46.000000 pyctm-0.0.8/pyctm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-25 02:07:46.000000 pyctm-0.0.8/pyctm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 02:07:46.360651 pyctm-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-25 02:07:25.000000 pyctm-0.0.8/setup.py
```

### Comparing `pyctm-0.0.7/LICENSE` & `pyctm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/codelet/codelet.py` & `pyctm-0.0.8/pyctm/codelet/codelet.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/codelet/codelet_application.py` & `pyctm-0.0.8/pyctm/codelet/codelet_application.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/k_distributed_memory.py` & `pyctm-0.0.8/pyctm/memory/k_distributed_memory.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/kafka/builder/k_consumer_builder.py` & `pyctm-0.0.8/pyctm/memory/kafka/builder/k_consumer_builder.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/kafka/builder/k_producer_builder.py` & `pyctm-0.0.8/pyctm/memory/kafka/builder/k_producer_builder.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/kafka/thread/k_memory_content_publisher_thread.py` & `pyctm-0.0.8/pyctm/memory/kafka/thread/k_memory_content_publisher_thread.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/kafka/thread/k_memory_content_receiver_thread.py` & `pyctm-0.0.8/pyctm/memory/kafka/thread/k_memory_content_receiver_thread.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/kafka/topic_config_provider.py` & `pyctm-0.0.8/pyctm/memory/kafka/topic_config_provider.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/memory/memory_object.py` & `pyctm-0.0.8/pyctm/memory/memory_object.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/tests/k_distributed_memory_test.py` & `pyctm-0.0.8/pyctm/tests/k_distributed_memory_test.py`

 * *Files identical despite different names*

### Comparing `pyctm-0.0.7/pyctm/tests/memory_object_test.py` & `pyctm-0.0.8/pyctm/tests/memory_object_test.py`

 * *Files identical despite different names*

