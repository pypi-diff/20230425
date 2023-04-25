# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202304142234.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202304250944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304142234.tar", last modified: Fri Apr 14 22:34:35 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304250944.tar", last modified: Tue Apr 25 09:44:45 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202304142234.tar` & `hcai-datasets-nightly-0.1.7.dev202304250944.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.017945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.017945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20249 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    22257 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.184566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.188566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22257 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10746 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-25 09:44:45.000000 hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 09:44:45.192566 hcai-datasets-nightly-0.1.7.dev202304250944/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-25 09:44:32.000000 hcai-datasets-nightly-0.1.7.dev202304250944/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304250944/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304142234
+Version: 0.1.7.dev202304250944
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/README.md` & `hcai-datasets-nightly-0.1.7.dev202304250944/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,25 @@
         self.data_streams = data_streams
         self.annotator = annotator
         self.left_context_ms = ndu.parse_time_string_to_ms(left_context)
         self.right_context_ms = ndu.parse_time_string_to_ms(right_context)
         self.frame_size_ms = (
             ndu.parse_time_string_to_ms(frame_size) if frame_size else None
         )
+
+
+        if self.frame_size_ms == 0:
+            print("WARNING: Frame size 0 is invalid. Returning whole session as sample.")
+            self.frame_size_ms = None
+
         self.stride_ms = (
             ndu.parse_time_string_to_ms(stride) if stride else self.frame_size_ms
         )
+
+
         self.start_ms = ndu.parse_time_string_to_ms(start)
         if not self.start_ms:
             self.start_ms = 0
 
         self.end_ms = ndu.parse_time_string_to_ms(end)
         if not self.end_ms:
             self.end_ms = float("inf")
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,47 +300,47 @@
     return seconds_to_frame(sr=sr, time_s=time_ms / 1000)
 
 
 def parse_time_string_to_ms(frame: Union[str, int, float]) -> int:
     # if frame is specified milliseconds as string
     if str(frame).endswith("ms"):
         try:
-            return float(frame[:-2])
+            return int(frame[:-2])
         except ValueError:
             raise ValueError(
                 "Invalid input format for frame in milliseconds: {}".format(frame)
             )
     # if frame is specified in seconds as string
     elif str(frame).endswith("s"):
         try:
             frame_s = float(frame[:-1])
-            return float(frame_s * 1000)
+            return int(frame_s * 1000)
         except ValueError:
             raise ValueError(
                 "Invalid input format for frame in seconds: {}".format(frame)
             )
     # if type is float we assume the input will be seconds
     elif isinstance(frame, float) or "." in str(frame):
         try:
             print(
                 "WARNING: Automatically inferred type for frame {} is float.".format(
                     frame
                 )
             )
-            return float(1000 * float(frame))
+            return int(1000 * float(frame))
         except ValueError:
             raise ValueError("Invalid input format for frame: {}".format(frame))
     # if type is int we assume the input will be milliseconds
     elif isinstance(frame, int) or (isinstance(frame, str) and frame.isdigit()):
         try:
             print(
                 "WARNING: Automatically inferred type for frame {} is int.".format(
                     frame
                 )
             )
-            return float(frame)
+            return int(frame)
         except ValueError:
             raise ValueError("Invalid input format for frame: {}".format(frame))
 
     print(
         f'WARNING: Could  not automatically parse time "{frame}" to seconds. Returning None '
     )
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304142234
+Version: 0.1.7.dev202304250944
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202304250944/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304142234/setup.py` & `hcai-datasets-nightly-0.1.7.dev202304250944/setup.py`

 * *Files identical despite different names*

