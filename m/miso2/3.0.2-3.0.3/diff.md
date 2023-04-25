# Comparing `tmp/miso2-3.0.2.tar.gz` & `tmp/miso2-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miso2-3.0.2.tar", last modified: Tue Apr 25 11:51:30 2023, max compression
+gzip compressed data, was "miso2-3.0.3.tar", last modified: Tue Apr 25 12:01:58 2023, max compression
```

## Comparing `miso2-3.0.2.tar` & `miso2-3.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.682736 miso2-3.0.2/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1054 2023-04-25 06:11:49.000000 miso2-3.0.2/LICENCE.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      817 2023-04-25 11:51:30.682736 miso2-3.0.2/PKG-INFO
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      191 2023-04-25 06:11:49.000000 miso2-3.0.2/README.md
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.674736 miso2-3.0.2/miso/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2205 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/__main__.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.678736 miso2-3.0.2/miso/data/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2760 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1567 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/download.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     7328 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/filenames_dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3133 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/image_dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2574 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/image_loader.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3963 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/image_utils.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     7948 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/tf_generator.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5338 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/training_dataset.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3473 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/data/utils.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.678736 miso2-3.0.2/miso/deploy/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/deploy/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5839 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/deploy/inference.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     6140 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/deploy/model_info.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     8173 2023-04-25 11:03:22.000000 miso2-3.0.2/miso/deploy/saving.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5139 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/deploy/server.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.678736 miso2-3.0.2/miso/layers/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4315 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/_common_blocks.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2072 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/asoftmax.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2841 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/batch_instance_normalisation.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3251 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/cyclic.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     7993 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/group_normalisation.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     2479 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/layers/msoftmax.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.678736 miso2-3.0.2/miso/models/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/models/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4475 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/models/base_cyclic.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5671 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/models/factory.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)       50 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/models/model_zoo.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)    12979 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/models/resnet_cyclic.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4772 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/models/transfer_learning.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.682736 miso2-3.0.2/miso/stats/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1452 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/accuracy.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)    13669 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/confusion_matrix.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     6150 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/embedding.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4861 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/mislabelling.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      882 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/most_representative.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1454 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/projections.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      957 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/stats/training.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.682736 miso2-3.0.2/miso/training/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/training/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     4918 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/training/adaptive_learning_rate.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     3154 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/training/parameters.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5238 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/training/tf_augmentation.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)    24676 2023-04-25 11:49:00.000000 miso2-3.0.2/miso/training/trainer.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1702 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/training/training_result.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.682736 miso2-3.0.2/miso/utils/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/__init__.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     9973 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/flowcam.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      726 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/lock.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      216 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/misc.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1407 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/rolling_buffer.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     5155 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/singleton.py
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     9990 2023-04-25 06:11:49.000000 miso2-3.0.2/miso/utils/wave.py
-drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 11:51:30.682736 miso2-3.0.2/miso2.egg-info/
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      817 2023-04-25 11:51:30.000000 miso2-3.0.2/miso2.egg-info/PKG-INFO
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1491 2023-04-25 11:51:30.000000 miso2-3.0.2/miso2.egg-info/SOURCES.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        1 2023-04-25 11:51:30.000000 miso2-3.0.2/miso2.egg-info/dependency_links.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)      231 2023-04-25 11:51:30.000000 miso2-3.0.2/miso2.egg-info/requires.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)        5 2023-04-25 11:51:30.000000 miso2-3.0.2/miso2.egg-info/top_level.txt
--rw-rw-r--   0 chaos     (1000) chaos     (1000)       38 2023-04-25 11:51:30.682736 miso2-3.0.2/setup.cfg
--rw-rw-r--   0 chaos     (1000) chaos     (1000)     1794 2023-04-25 11:50:22.000000 miso2-3.0.2/setup.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1054 2023-04-25 06:11:49.000000 miso2-3.0.3/LICENCE.txt
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      817 2023-04-25 12:01:58.271395 miso2-3.0.3/PKG-INFO
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      191 2023-04-25 06:11:49.000000 miso2-3.0.3/README.md
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.263395 miso2-3.0.3/miso/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     2205 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/__main__.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/data/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     2760 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/dataset.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1567 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/download.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     7328 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/filenames_dataset.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     3133 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/image_dataset.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     2574 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/image_loader.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     3963 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/image_utils.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     7948 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/tf_generator.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     5338 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/training_dataset.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     3473 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/data/utils.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/deploy/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     5839 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/inference.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     6140 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/model_info.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     8173 2023-04-25 11:03:22.000000 miso2-3.0.3/miso/deploy/saving.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     5139 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/deploy/server.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/layers/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     4315 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/_common_blocks.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     2072 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/asoftmax.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     2841 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/batch_instance_normalisation.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     3251 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/cyclic.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     7993 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/group_normalisation.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     2479 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/layers/msoftmax.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/models/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     4475 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/base_cyclic.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     5671 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/factory.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)       50 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/model_zoo.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)    12979 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/resnet_cyclic.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     4772 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/models/transfer_learning.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.267395 miso2-3.0.3/miso/stats/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1452 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/accuracy.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)    13669 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/confusion_matrix.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     6150 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/embedding.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     4861 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/mislabelling.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      882 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/most_representative.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1454 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/projections.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      957 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/stats/training.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/miso/training/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     4918 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/adaptive_learning_rate.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     3154 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/parameters.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     5238 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/tf_augmentation.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)    24759 2023-04-25 11:59:34.000000 miso2-3.0.3/miso/training/trainer.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1702 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/training/training_result.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/miso/utils/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        0 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/__init__.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     9973 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/flowcam.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      726 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/lock.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      216 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/misc.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1407 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/rolling_buffer.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     5155 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/singleton.py
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     9990 2023-04-25 06:11:49.000000 miso2-3.0.3/miso/utils/wave.py
+drwxrwxr-x   0 chaos     (1000) chaos     (1000)        0 2023-04-25 12:01:58.271395 miso2-3.0.3/miso2.egg-info/
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      817 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/PKG-INFO
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1491 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/SOURCES.txt
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        1 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/dependency_links.txt
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)      231 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/requires.txt
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)        5 2023-04-25 12:01:58.000000 miso2-3.0.3/miso2.egg-info/top_level.txt
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)       38 2023-04-25 12:01:58.271395 miso2-3.0.3/setup.cfg
+-rw-rw-r--   0 chaos     (1000) chaos     (1000)     1794 2023-04-25 12:01:06.000000 miso2-3.0.3/setup.py
```

### Comparing `miso2-3.0.2/LICENCE.txt` & `miso2-3.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/PKG-INFO` & `miso2-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miso2
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python scripts for training CNNs for particle classification
 Home-page: https://github.com/microfossil/particle-classification
 Author: Ross Marchant
 Author-email: ross.g.marchant@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/microfossil/particle-classification
 Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
```

### Comparing `miso2-3.0.2/miso/__main__.py` & `miso2-3.0.3/miso/__main__.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/dataset.py` & `miso2-3.0.3/miso/data/dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/download.py` & `miso2-3.0.3/miso/data/download.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/filenames_dataset.py` & `miso2-3.0.3/miso/data/filenames_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/image_dataset.py` & `miso2-3.0.3/miso/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/image_loader.py` & `miso2-3.0.3/miso/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/image_utils.py` & `miso2-3.0.3/miso/data/image_utils.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/tf_generator.py` & `miso2-3.0.3/miso/data/tf_generator.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/training_dataset.py` & `miso2-3.0.3/miso/data/training_dataset.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/data/utils.py` & `miso2-3.0.3/miso/data/utils.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/deploy/inference.py` & `miso2-3.0.3/miso/deploy/inference.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/deploy/model_info.py` & `miso2-3.0.3/miso/deploy/model_info.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/deploy/saving.py` & `miso2-3.0.3/miso/deploy/saving.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/deploy/server.py` & `miso2-3.0.3/miso/deploy/server.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/layers/_common_blocks.py` & `miso2-3.0.3/miso/layers/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/layers/asoftmax.py` & `miso2-3.0.3/miso/layers/asoftmax.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/layers/batch_instance_normalisation.py` & `miso2-3.0.3/miso/layers/batch_instance_normalisation.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/layers/cyclic.py` & `miso2-3.0.3/miso/layers/cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/layers/group_normalisation.py` & `miso2-3.0.3/miso/layers/group_normalisation.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/layers/msoftmax.py` & `miso2-3.0.3/miso/layers/msoftmax.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/models/base_cyclic.py` & `miso2-3.0.3/miso/models/base_cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/models/factory.py` & `miso2-3.0.3/miso/models/factory.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/models/resnet_cyclic.py` & `miso2-3.0.3/miso/models/resnet_cyclic.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/models/transfer_learning.py` & `miso2-3.0.3/miso/models/transfer_learning.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/accuracy.py` & `miso2-3.0.3/miso/stats/accuracy.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/confusion_matrix.py` & `miso2-3.0.3/miso/stats/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/embedding.py` & `miso2-3.0.3/miso/stats/embedding.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/mislabelling.py` & `miso2-3.0.3/miso/stats/mislabelling.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/most_representative.py` & `miso2-3.0.3/miso/stats/most_representative.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/projections.py` & `miso2-3.0.3/miso/stats/projections.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/stats/training.py` & `miso2-3.0.3/miso/stats/training.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/training/adaptive_learning_rate.py` & `miso2-3.0.3/miso/training/adaptive_learning_rate.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/training/parameters.py` & `miso2-3.0.3/miso/training/parameters.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/training/tf_augmentation.py` & `miso2-3.0.3/miso/training/tf_augmentation.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/training/trainer.py` & `miso2-3.0.3/miso/training/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,16 @@
         os.makedirs(training_examples_dir)
         images, labels = next(iter(train_gen.create()))
         for t_idx, im in enumerate(images):
             im = im.numpy() * 255
             im[im > 255] = 255
             if np.ndim(im) == 2:
                 im = np.repeat(im[:, :, np.newaxis], 3, axis=-1)
+            elif im.shape[-1] == 1:
+                im = np.repeat(im, 3, axis=-1)
             skimage.io.imsave(
                 os.path.join(training_examples_dir, "{:03d}.jpg".format(t_idx)),
                 im.astype(np.uint8),
             )
 
         # Validation generator
         if tf_version == 2:
```

### Comparing `miso2-3.0.2/miso/training/training_result.py` & `miso2-3.0.3/miso/training/training_result.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/utils/flowcam.py` & `miso2-3.0.3/miso/utils/flowcam.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/utils/lock.py` & `miso2-3.0.3/miso/utils/lock.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/utils/rolling_buffer.py` & `miso2-3.0.3/miso/utils/rolling_buffer.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/utils/singleton.py` & `miso2-3.0.3/miso/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso/utils/wave.py` & `miso2-3.0.3/miso/utils/wave.py`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/miso2.egg-info/PKG-INFO` & `miso2-3.0.3/miso2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miso2
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python scripts for training CNNs for particle classification
 Home-page: https://github.com/microfossil/particle-classification
 Author: Ross Marchant
 Author-email: ross.g.marchant@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/microfossil/particle-classification
 Project-URL: Paper, https://jm.copernicus.org/articles/39/183/2020/
```

### Comparing `miso2-3.0.2/miso2.egg-info/SOURCES.txt` & `miso2-3.0.3/miso2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miso2-3.0.2/setup.py` & `miso2-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='miso2',
-    version='3.0.2',
+    version='3.0.3',
     description='Python scripts for training CNNs for particle classification',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ross Marchant',
     author_email='ross.g.marchant@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

