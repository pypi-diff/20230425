# Comparing `tmp/waffle_hub-0.1.8.tar.gz` & `tmp/waffle_hub-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.1.8.tar", last modified: Mon Apr 17 23:08:26 2023, max compression
+gzip compressed data, was "waffle_hub-0.1.9.tar", last modified: Tue Apr 25 08:44:29 2023, max compression
```

## Comparing `waffle_hub-0.1.8.tar` & `waffle_hub-0.1.9.tar`

### file list

```diff
@@ -1,68 +1,76 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.8/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.8/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.8/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3721 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7085 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3844 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      102 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2715 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4566 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    20015 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-13 02:15:00.000000 waffle_hub-0.1.8/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1793 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8318 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10931 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    23011 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6296 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      806 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1257 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/data.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13649 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1341 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6827 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2581 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/image.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5480 2023-04-12 07:56:27.000000 waffle_hub-0.1.8/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3385 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2330 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/utils/draw.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1597 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.9/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.9/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      881 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      380 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8355 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9259 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3687 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      168 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2715 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4917 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/huggingface.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4566 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    36845 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10682 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7848 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/hugging_face/train_input_helper.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3203 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9150 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10726 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    32379 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6296 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      806 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1653 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      230 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13649 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1341 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6827 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2581 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      496 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.9/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3573 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5650 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2330 2023-04-25 04:16:04.000000 waffle_hub-0.1.9/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2712 2023-04-25 08:43:33.000000 waffle_hub-0.1.9/waffle_hub/utils/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-25 08:44:29.734405 waffle_hub-0.1.9/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1962 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1888 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      301 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-25 08:44:29.000000 waffle_hub-0.1.9/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.1.8/LICENSE` & `waffle_hub-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/PKG-INFO` & `waffle_hub-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.1.8
+Version: 0.1.9
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
@@ -32,8 +32,8 @@
   </p>
 </div>
 
 Waffle is a framework that lets you use lots of different deep learning tools through just one interface. When it comes to MLOps (machine learning operations), you need to be able to keep up with all the new ideas in deep learning as quickly as possible. But it's hard to do that if you have to write all the code yourself. That's why we started a project to bring together different tools into one framework.
 
 Experience the power of multiple deep learning frameworks at your fingertips with Waffle's seamless integration, unlocking limitless possibilities for your machine learning projects.
 
-See our [documentation](https://snuailab.github.io/waffle_hub/) for more information!
+See our [documentation](https://snuailab.github.io/waffle/) for more information!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.8 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.9 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -19,8 +19,8 @@
 through just one interface. When it comes to MLOps (machine learning
 operations), you need to be able to keep up with all the new ideas in deep
 learning as quickly as possible. But it's hard to do that if you have to write
 all the code yourself. That's why we started a project to bring together
 different tools into one framework. Experience the power of multiple deep
 learning frameworks at your fingertips with Waffle's seamless integration,
 unlocking limitless possibilities for your machine learning projects. See our
-[documentation](https://snuailab.github.io/waffle_hub/) for more information!
+[documentation](https://snuailab.github.io/waffle/) for more information!
```

### Comparing `waffle_hub-0.1.8/README.md` & `waffle_hub-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
   </p>
 </div>
 
 Waffle is a framework that lets you use lots of different deep learning tools through just one interface. When it comes to MLOps (machine learning operations), you need to be able to keep up with all the new ideas in deep learning as quickly as possible. But it's hard to do that if you have to write all the code yourself. That's why we started a project to bring together different tools into one framework.
 
 Experience the power of multiple deep learning frameworks at your fingertips with Waffle's seamless integration, unlocking limitless possibilities for your machine learning projects.
 
-See our [documentation](https://snuailab.github.io/waffle_hub/) for more information!
+See our [documentation](https://snuailab.github.io/waffle/) for more information!
```

#### html2text {}

```diff
@@ -4,8 +4,8 @@
 through just one interface. When it comes to MLOps (machine learning
 operations), you need to be able to keep up with all the new ideas in deep
 learning as quickly as possible. But it's hard to do that if you have to write
 all the code yourself. That's why we started a project to bring together
 different tools into one framework. Experience the power of multiple deep
 learning frameworks at your fingertips with Waffle's seamless integration,
 unlocking limitless possibilities for your machine learning projects. See our
-[documentation](https://snuailab.github.io/waffle_hub/) for more information!
+[documentation](https://snuailab.github.io/waffle/) for more information!
```

### Comparing `waffle_hub-0.1.8/setup.py` & `waffle_hub-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/__init__.py` & `waffle_hub-0.1.9/waffle_hub/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
+import enum
 import importlib
 import warnings
 import enum
 from collections import OrderedDict
 
 from tabulate import tabulate
 
@@ -17,26 +18,26 @@
             f"""
             torch {torch.__version__} has not been tested.
             We recommend you to use one of {pytorch_versions}
             """
         )
 except ModuleNotFoundError as e:
     # TODO: Generalize install strings
-    strings = [
-        "  - conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch",
-        "  - pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113",
-        "  - pip install torch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1",
-    ]
+    strings = []
 
     e.msg = "Need to install torch\n" + "\n".join(strings)
     raise e
 
 # backend supports
 _backends = OrderedDict(
-    {"ultralytics": ["8.0.72"], "autocare_tx_model": ["0.2.0"]}
+    {
+        "ultralytics": ["8.0.87"],
+        "autocare_tx_model": ["0.2.0"],
+        "transformers": ["4.27.4"],
+    }
 )
 
 
 def get_backends() -> dict:
     return _backends
 
 
@@ -59,17 +60,15 @@
                 We recommend you to use one of {versions}
                 """
             )
         return module.__version__
 
     except ModuleNotFoundError as e:
 
-        install_queries = "\n".join(
-            [f"- pip install {backend}=={version}" for version in versions]
-        )
+        install_queries = "\n".join([f"- pip install {backend}=={version}" for version in versions])
 
         e.msg = f"""
             Need to install {backend}.
             Tested versions:
             {install_queries}
             """
         raise e
@@ -93,18 +92,19 @@
     return table
 
 class CustomEnumMeta(enum.EnumMeta):
     def __contains__(cls, item):
         if isinstance(item, str):
             return item.upper() in cls._member_names_
         return super().__contains__(item)
-    
+
     def __upper__(self):
         return self.name.upper()
 
+
 class BaseEnum(enum.Enum, metaclass=CustomEnumMeta):
     """Base class for Enum
 
     Example:
         >>> class Color(BaseEnum):
         >>>     RED = 1
         >>>     GREEN = 2
@@ -131,19 +131,25 @@
         return self.name.upper()
 
     def __repr__(self):
         return self.name.upper()
 
 
 class DataType(BaseEnum):
+    # TODO: map to same value
+
     YOLO = enum.auto()
-    ULTRALYTICS = YOLO
+    ULTRALYTICS = enum.auto()
 
     COCO = enum.auto()
-    TX_MODEL = COCO
+    TX_MODEL = enum.auto()
+    AUTOCARE_TX_MODEL = enum.auto()
+
+    HUGGINGFACE = enum.auto()
+    TRANSFORMERS = enum.auto()
 
 
 class TaskType(BaseEnum):
     CLASSIFICATION = enum.auto()
     OBJECT_DETECTION = enum.auto()
     SEGMENTATION = enum.auto()
     KEYPOINT_DETECTION = enum.auto()
```

### Comparing `waffle_hub-0.1.8/waffle_hub/dataset/adapter/coco.py` & `waffle_hub-0.1.9/waffle_hub/dataset/adapter/coco.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.1.9/waffle_hub/dataset/adapter/yolo.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.1.9/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/experimental/serve.py` & `waffle_hub-0.1.9/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,62 @@
-
 def get_data_config(
-    data_type: str, 
-    image_size: list[int], 
-    batch_size: int, 
+    data_type: str,
+    image_size: list[int],
+    batch_size: int,
     workers: int,
     train_coco: str,
     train_root: str,
     val_coco: str,
     val_root: str,
     test_coco: str,
     test_root: str,
-    unlabeled_coco: str = None,
-    unlabeled_root: str = None,
 ):
     config = {
         "data": {
             "workers_per_gpu": workers,
             "batch_size_per_gpu": batch_size,
             "img_size": image_size,
             "train": {
                 "type": data_type,
                 "data_root": train_root,
                 "ann": train_coco,
                 "augmentation": {
-                    "ColorJitter":{
+                    "ColorJitter": {
                         "brightness": 0.125,
                         "contrast": 0.5,
                         "saturation": 0.5,
-                        "hue": 0.1
+                        "hue": 0.1,
                     },
                     "Affine": {
                         "scale": [0.5, 1.5],
-                        "translate_percent": [-0.1, 0.1], 
+                        "translate_percent": [-0.1, 0.1],
                         "always_apply": True,
                     },
-                    "HorizontalFlip": {
-                        "p": 0.5
-                    },
+                    "HorizontalFlip": {"p": 0.5},
                     "Cutout": {
                         "p": 0.5,
                         "num_holes": 8,
                         "max_h_size": 32,
                         "max_w_size": 32,
-                        "fill_value": 0
+                        "fill_value": 0,
                     },
-                    "ImageNormalization": {
-                        "type": "base"
-                    }
-                }
+                    "ImageNormalization": {"type": "base"},
+                },
             },
             "val": {
                 "type": data_type,
                 "data_root": val_root,
                 "ann": val_coco,
-                "augmentation": {
-                    "ImageNormalization": {
-                        "type": "base"
-                    }
-                }
+                "augmentation": {"ImageNormalization": {"type": "base"}},
             },
             "test": {
                 "type": data_type,
                 "data_root": test_root,
                 "ann": test_coco,
-                "augmentation": {
-                    "ImageNormalization": {
-                        "type": "base"
-                    }
-                }
+                "augmentation": {"ImageNormalization": {"type": "base"}},
             },
             "cache": False,
-            "single_cls": False
-        }
-    } 
-
-    if unlabeled_coco is not None:
-        config["data"]["unlabeled"] = {
-            "type": "UnlabeledDataset",
-            "data_root": unlabeled_root,
-            "ann": unlabeled_coco,
-            "augmentation": {
-                "ImageNormalization": {
-                    "type": "base"
-                }
-            }
+            "single_cls": False,
         }
+    }
 
-    return config
+    return config
```

### Comparing `waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.1.9/waffle_hub/hub/adapter/tx_model/tx_model_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-!!! DEPRECATED !!!
 Tx Model Hub
+See BaseHub documentation for more details about usage.
 """
 
 from waffle_hub import get_installed_backend_version
 
 BACKEND_NAME = "autocare_tx_model"
 BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
 
@@ -20,43 +20,49 @@
 from torchvision import transforms as T
 from waffle_utils.file import io
 
 from waffle_hub.hub.adapter.tx_model.configs import (
     get_data_config,
     get_model_config,
 )
-from waffle_hub.hub.base_hub import BaseHub, TrainContext
-from waffle_hub.hub.model.wrapper import ModelWrapper, ResultParser
+from waffle_hub.hub.base_hub import BaseHub
+from waffle_hub.hub.model.wrapper import ModelWrapper
+from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 
 
 class TxModelHub(BaseHub):
 
     # Common
     MODEL_TYPES = {
         "object_detection": {"YOLOv5": list("sml")},
-        # "classification": {
-        #     "resnet": list("sml"),
-        #     "swin": list("sml")
-        # },
+        "classification": {"Classifier": list("sml")},
     }
 
     # Backend Specifics
     DATA_TYPE_MAP = {
         "object_detection": "COCODetectionDataset",
+        "classification": "COCOClassificationDataset",
     }
 
     WEIGHT_PATH = {
         "object_detection": {
             "YOLOv5": {
                 "s": "temp/autocare_tx_model/detectors/small/model.pth",
                 "m": "temp/autocare_tx_model/detectors/medium/model.pth",
                 "l": "temp/autocare_tx_model/detectors/large/model.pth",
             }
         },
+        "classification": {
+            "Classifier": {
+                "s": "temp/autocare_tx_model/classifiers/small/model.pth",
+                "m": "temp/autocare_tx_model/classifiers/medium/model.pth",
+                "l": "temp/autocare_tx_model/classifiers/large/model.pth",
+            }
+        },
     }
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
@@ -65,17 +71,15 @@
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
         """Create Tx Model Hub Class. Do not use this class directly. Use TxModelHub.new() instead."""
 
         if backend is not None and backend != BACKEND_NAME:
-            raise ValueError(
-                f"you've loaded {backend}. backend must be {BACKEND_NAME}"
-            )
+            raise ValueError(f"you've loaded {backend}. backend must be {BACKEND_NAME}")
 
         if version is not None and version != BACKEND_VERSION:
             warnings.warn(
                 f"you've loaded a {BACKEND_NAME}=={version} version while {BACKEND_NAME}=={BACKEND_VERSION} version is installed."
                 "It will cause unexpected results."
             )
 
@@ -124,21 +128,37 @@
 
         if task == "object_detection":
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
                 return normalize(x)
 
+        elif task == "classification":
+            normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
+
+            def preprocess(x, *args, **kwargs):
+                return normalize(x)
+
         return preprocess
 
     def get_postprocess(self, task: str, *args, **kwargs):
 
         if task == "object_detection":
 
             def inner(x: torch.Tensor, *args, **kwargs):
+                xyxy = x[0]
+                scores = x[1]
+                class_ids = x[2]
+
+                return xyxy, scores, class_ids
+
+        elif task == "classification":
+
+            def inner(x: torch.Tensor, *args, **kwargs):
+                x = [t.squeeze() for t in x]
                 return x
 
         return inner
 
     def get_metrics(self) -> list[dict]:
         """Get metrics from tensorboard log directory.
         Args:
@@ -157,81 +177,80 @@
         # Make a list of dictionaries of tag and value.
         if df.empty:
             return []
 
         metrics = (
             df.sort_values("step")
             .groupby("step")
-            .apply(
-                lambda x: [
-                    {"tag": s, "value": v} for s, v in zip(x.tag, x.value)
-                ]
-            )
+            .apply(lambda x: [{"tag": s, "value": v} for s, v in zip(x.tag, x.value)])
             .to_list()
         )
 
         return metrics
 
     # Train Hook
-    def on_train_start(self, ctx: TrainContext):
+    def on_train_start(self, cfg: TrainConfig):
         # set data
-        ctx.dataset_path: Path = Path(ctx.dataset_path)
-
+        cfg.dataset_path: Path = Path(cfg.dataset_path)
         data_config = get_data_config(
             self.DATA_TYPE_MAP[self.task],
-            [ctx.image_size, ctx.image_size],
-            ctx.batch_size,
-            ctx.workers,
-            str(ctx.dataset_path / "train.json"),
-            str(ctx.dataset_path / "images"),
-            str(ctx.dataset_path / "val.json"),
-            str(ctx.dataset_path / "images"),
-            str(ctx.dataset_path / "test.json"),
-            str(ctx.dataset_path / "images"),
+            [cfg.image_size, cfg.image_size],
+            cfg.batch_size,
+            cfg.workers,
+            str(cfg.dataset_path / "train.json"),
+            str(cfg.dataset_path / "images"),
+            str(cfg.dataset_path / "val.json"),
+            str(cfg.dataset_path / "images"),
+            str(cfg.dataset_path / "test.json"),
+            str(cfg.dataset_path / "images"),
         )
-        ctx.data_config = self.artifact_dir / "data.json"
-        io.save_json(data_config, ctx.data_config, create_directory=True)
+
+        cfg.data_config = self.artifact_dir / "data.json"
+        io.save_json(data_config, cfg.data_config, create_directory=True)
 
         model_config = get_model_config(
             self.model_type,
             self.model_size,
             [x["name"] for x in self.categories],
-            ctx.seed,
-            ctx.letter_box,
-            ctx.epochs,
+            cfg.seed,
+            cfg.learning_rate,
+            cfg.letter_box,
+            cfg.epochs,
         )
-        ctx.model_config = self.artifact_dir / "model.json"
-        io.save_json(model_config, ctx.model_config, create_directory=True)
+
+        cfg.model_config = self.artifact_dir / "model.json"
+        io.save_json(model_config, cfg.model_config, create_directory=True)
 
         # pretrained model
-        ctx.pretrained_model = (
-            ctx.pretrained_model
-            if ctx.pretrained_model is not None
+        cfg.pretrained_model = (
+            cfg.pretrained_model
+            if cfg.pretrained_model is not None
             else self.WEIGHT_PATH[self.task][self.model_type][self.model_size]
         )
-        if not Path(ctx.pretrained_model).exists():
-            ctx.pretrained_model = None
-            warnings.warn(
-                f"{ctx.pretrained_model} does not exists. Train from scratch."
-            )
+        if not Path(cfg.pretrained_model).exists():
+            cfg.pretrained_model = None
+            warnings.warn(f"{cfg.pretrained_model} does not exists. Train from scratch.")
 
-    def training(self, ctx: TrainContext, callback: TrainCallback):
+        cfg.dataset_path = str(cfg.dataset_path.absolute())
 
+    def training(self, cfg: TrainConfig, callback: TrainCallback):
         results = train.run(
             exp_name="train",
-            model_cfg=str(ctx.model_config),
-            data_cfg=str(ctx.data_config),
-            gpus="-1" if ctx.device == "cpu" else str(ctx.device),
+            model_cfg=str(cfg.model_config),
+            data_cfg=str(cfg.data_config),
+            gpus="-1" if cfg.device == "cpu" else str(cfg.device),
             output_dir=str(self.artifact_dir),
-            ckpt=ctx.pretrained_model,
+            ckpt=cfg.pretrained_model,
             overwrite=True,
         )
+        if results is None:
+            raise RuntimeError("Training failed")
         del results
 
-    def on_train_end(self, ctx: TrainContext):
+    def on_train_end(self, cfg: TrainConfig):
         io.copy_file(
             self.artifact_dir / "train" / "best_ckpt.pth",
             self.best_ckpt_file,
             create_directory=True,
         )
         io.copy_file(
             self.artifact_dir / "train" / "last_epoch_ckpt.pth",
@@ -251,18 +270,17 @@
         # get adapt functions
         preprocess = self.get_preprocess(self.task)
         postprocess = self.get_postprocess(self.task)
 
         # get model
         categories = [x["name"] for x in self.categories]
         cfg = io.load_json(self.artifact_dir / "model.json")
-        cfg["model"]["head"]["num_categories"] = len(categories)
         cfg["ckpt"] = str(self.best_ckpt_file)
-        cfg["categories"] = categories
-        cfg["num_categories"] = (len(categories),)
+        cfg["model"]["head"]["num_classes"] = len(categories)
+        cfg["num_classes"] = len(categories)
         model, categories = build_model(AttrDict(cfg), strict=True)
 
         model = ModelWrapper(
             model=model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
         )
```

### Comparing `waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.1.9/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 Ultralytics Hub
+See BaseHub documentation for more details about usage.
 """
 
 from waffle_hub import get_installed_backend_version
 
 BACKEND_NAME = "ultralytics"
 BACKEND_VERSION = get_installed_backend_version(BACKEND_NAME)
 
@@ -72,17 +73,15 @@
         root_dir: str = None,
         backend: str = None,
         version: str = None,
     ):
         """Create Ultralytics Hub Class. Do not use this class directly. Use UltralyticsHub.new() instead."""
 
         if backend is not None and backend != BACKEND_NAME:
-            raise ValueError(
-                f"you've loaded {backend}. backend must be {BACKEND_NAME}"
-            )
+            raise ValueError(f"you've loaded {backend}. backend must be {BACKEND_NAME}")
 
         if version is not None and version != BACKEND_VERSION:
             warnings.warn(
                 f"you've loaded a {BACKEND_NAME}=={version} version while {BACKEND_NAME}=={BACKEND_VERSION} version is installed."
                 "It will cause unexpected results."
             )
 
@@ -153,17 +152,15 @@
         if task == "classification":
 
             def inner(x: torch.Tensor, *args, **kwargs):
                 return [x]
 
         elif task == "object_detection":
 
-            def inner(
-                x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs
-            ):
+            def inner(x: torch.Tensor, image_size: tuple[int, int], *args, **kwargs):
                 x = x[0]  # x[0]: prediction, x[1]: TODO: what is this...?
                 x = x.transpose(1, 2)
 
                 cxcywh = x[:, :, :4]
                 cx, cy, w, h = torch.unbind(cxcywh, dim=-1)
                 x1 = cx - w / 2
                 y1 = cy - h / 2
@@ -223,46 +220,39 @@
         cfg.dataset_path: Path = Path(cfg.dataset_path)
         if self.backend_task_name in ["detect", "segment"]:
             if cfg.dataset_path.suffix not in [".yml", ".yaml"]:
                 yaml_files = list(cfg.dataset_path.glob("*.yaml")) + list(
                     cfg.dataset_path.glob("*.yml")
                 )
                 if len(yaml_files) != 1:
-                    raise FileNotFoundError(
-                        f"Ambiguous data file. Detected files: {yaml_files}"
-                    )
+                    raise FileNotFoundError(f"Ambiguous data file. Detected files: {yaml_files}")
                 cfg.dataset_path = Path(yaml_files[0]).absolute()
             else:
                 cfg.dataset_path = cfg.dataset_path.absolute()
         elif self.backend_task_name == "classify":
 
             from torchvision.datasets.folder import ImageFolder
 
             def find_categories(_, directory: str):
-                return directory, {
-                    v["name"]: i for i, v in enumerate(self.categories)
-                }
+                return directory, {v["name"]: i for i, v in enumerate(self.categories)}
 
             ImageFolder.find_categories = find_categories
 
             if not cfg.dataset_path.is_dir():
                 raise ValueError(
                     f"Classification dataset should be directory. Not {cfg.dataset_path}"
                 )
             cfg.dataset_path = cfg.dataset_path.absolute()
         cfg.dataset_path = str(cfg.dataset_path)
 
         # pretrained model
         cfg.pretrained_model = (
             cfg.pretrained_model
             if cfg.pretrained_model
-            else self.model_type
-            + self.model_size
-            + self.TASK_SUFFIX[self.backend_task_name]
-            + ".pt"
+            else self.model_type + self.model_size + self.TASK_SUFFIX[self.backend_task_name] + ".pt"
         )
 
         # overwrite train config with default config
         for k, v in cfg.to_dict().items():
             if v is None:
                 setattr(cfg, k, self.DEFAULT_PARAMAS[self.task][k])
 
@@ -315,11 +305,7 @@
         model = ModelWrapper(
             model=YOLO(self.best_ckpt_file).model.eval(),
             preprocess=preprocess,
             postprocess=postprocess,
         )
 
         return model
-
-    # Evaluate Hook
-    def evaluating(self):
-        raise NotImplementedError
```

### Comparing `waffle_hub-0.1.8/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.1.9/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/run.py` & `waffle_hub-0.1.9/waffle_hub/run.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/base_schema.py` & `waffle_hub-0.1.9/waffle_hub/schema/base_schema.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/configs.py` & `waffle_hub-0.1.9/waffle_hub/schema/configs.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,30 @@
     device: str = None
     workers: int = None
     seed: int = None
     verbose: bool = None
 
 
 @dataclass
+class EvaluateConfig(BaseSchema):
+    dataset_name: str = None
+    set_name: str = None
+    batch_size: int = None
+    image_size: Union[int, list[int]] = None
+    letter_box: bool = None
+    confidence_threshold: float = None
+    iou_threshold: float = None
+    half: bool = None
+    workers: int = None
+    device: str = None
+    draw: bool = None
+    dataset_root_dir: str = None
+
+
+@dataclass
 class InferenceConfig(BaseSchema):
     source: str = None
     batch_size: int = None
     recursive: bool = None
     image_size: Union[int, list[int]] = None
     letter_box: bool = None
     confidence_threshold: float = None
```

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/data.py` & `waffle_hub-0.1.9/waffle_hub/schema/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.1.9/waffle_hub/schema/fields/annotation.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.1.9/waffle_hub/schema/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/fields/category.py` & `waffle_hub-0.1.9/waffle_hub/schema/fields/category.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/schema/fields/image.py` & `waffle_hub-0.1.9/waffle_hub/schema/fields/image.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub/utils/draw.py` & `waffle_hub-0.1.9/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.8/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.1.9/waffle_hub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.1.8
+Version: 0.1.9
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
@@ -32,8 +32,8 @@
   </p>
 </div>
 
 Waffle is a framework that lets you use lots of different deep learning tools through just one interface. When it comes to MLOps (machine learning operations), you need to be able to keep up with all the new ideas in deep learning as quickly as possible. But it's hard to do that if you have to write all the code yourself. That's why we started a project to bring together different tools into one framework.
 
 Experience the power of multiple deep learning frameworks at your fingertips with Waffle's seamless integration, unlocking limitless possibilities for your machine learning projects.
 
-See our [documentation](https://snuailab.github.io/waffle_hub/) for more information!
+See our [documentation](https://snuailab.github.io/waffle/) for more information!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.8 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.9 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -19,8 +19,8 @@
 through just one interface. When it comes to MLOps (machine learning
 operations), you need to be able to keep up with all the new ideas in deep
 learning as quickly as possible. But it's hard to do that if you have to write
 all the code yourself. That's why we started a project to bring together
 different tools into one framework. Experience the power of multiple deep
 learning frameworks at your fingertips with Waffle's seamless integration,
 unlocking limitless possibilities for your machine learning projects. See our
-[documentation](https://snuailab.github.io/waffle_hub/) for more information!
+[documentation](https://snuailab.github.io/waffle/) for more information!
```

### Comparing `waffle_hub-0.1.8/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.1.9/waffle_hub.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,37 +13,44 @@
 waffle_hub.egg-info/entry_points.txt
 waffle_hub.egg-info/requires.txt
 waffle_hub.egg-info/top_level.txt
 waffle_hub/dataset/__init__.py
 waffle_hub/dataset/dataset.py
 waffle_hub/dataset/adapter/__init__.py
 waffle_hub/dataset/adapter/coco.py
+waffle_hub/dataset/adapter/huggingface.py
 waffle_hub/dataset/adapter/yolo.py
 waffle_hub/experimental/__init__.py
 waffle_hub/experimental/serve.py
 waffle_hub/experimental/auto_label/__init__.py
 waffle_hub/experimental/auto_label/grounding_dino.py
 waffle_hub/hub/__init__.py
 waffle_hub/hub/base_hub.py
 waffle_hub/hub/adapter/__init__.py
+waffle_hub/hub/adapter/hugging_face/__init__.py
+waffle_hub/hub/adapter/hugging_face/hugging_face_hub.py
+waffle_hub/hub/adapter/hugging_face/train_input_helper.py
 waffle_hub/hub/adapter/tx_model/__init__.py
 waffle_hub/hub/adapter/tx_model/tx_model_hub.py
 waffle_hub/hub/adapter/tx_model/configs/__init__.py
 waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
 waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
 waffle_hub/hub/adapter/ultralytics/__init__.py
 waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
 waffle_hub/hub/model/__init__.py
 waffle_hub/hub/model/wrapper.py
 waffle_hub/schema/__init__.py
 waffle_hub/schema/base_schema.py
 waffle_hub/schema/configs.py
 waffle_hub/schema/data.py
+waffle_hub/schema/evaluate.py
+waffle_hub/schema/result.py
 waffle_hub/schema/fields/__init__.py
 waffle_hub/schema/fields/annotation.py
 waffle_hub/schema/fields/base_field.py
 waffle_hub/schema/fields/category.py
 waffle_hub/schema/fields/image.py
 waffle_hub/utils/__init__.py
 waffle_hub/utils/callback.py
 waffle_hub/utils/data.py
-waffle_hub/utils/draw.py
+waffle_hub/utils/draw.py
+waffle_hub/utils/evaluate.py
```

