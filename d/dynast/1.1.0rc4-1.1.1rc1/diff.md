# Comparing `tmp/dynast-1.1.0rc4.tar.gz` & `tmp/dynast-1.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynast-1.1.0rc4.tar", last modified: Fri Mar  3 08:35:29 2023, max compression
+gzip compressed data, was "dynast-1.1.1rc1.tar", last modified: Mon Apr 24 22:18:48 2023, max compression
```

## Comparing `dynast-1.1.0rc4.tar` & `dynast-1.1.1rc1.tar`

### file list

```diff
@@ -1,80 +1,121 @@
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.184078 dynast-1.1.0rc4/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      581 2023-02-09 17:30:12.000000 dynast-1.1.0rc4/LICENSE.md
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13654 2023-03-03 08:35:29.184078 dynast-1.1.0rc4/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13135 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/README.md
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.084067 dynast-1.1.0rc4/dynast/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.100069 dynast-1.1.0rc4/dynast/analytics/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/analytics/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3114 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/analytics/results.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4442 2023-02-22 21:42:40.000000 dynast-1.1.0rc4/dynast/analytics/visualize.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      749 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/cli.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/common.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-03-01 23:29:58.000000 dynast-1.1.0rc4/dynast/dynast_manager.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.104070 dynast-1.1.0rc4/dynast/measure/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/measure/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/measure/latency.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.108070 dynast-1.1.0rc4/dynast/predictors/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/predictors/__init__.py
--rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6754 2023-02-09 17:30:13.000000 dynast-1.1.0rc4/dynast/predictors/dynamic_predictor.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-02-15 23:55:06.000000 dynast-1.1.0rc4/dynast/predictors/predictor_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/python.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.120071 dynast-1.1.0rc4/dynast/search/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/search/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-02-28 00:09:11.000000 dynast-1.1.0rc4/dynast/search/encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/search/evaluation_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16411 2023-03-01 18:19:31.000000 dynast-1.1.0rc4/dynast/search/evolutionary.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41130 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/dynast/search/search_tactic.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.120071 dynast-1.1.0rc4/dynast/supernetwork/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/supernetwork/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.124072 dynast-1.1.0rc4/dynast/supernetwork/image_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/supernetwork/image_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.128072 dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2236 2023-03-01 18:23:06.000000 dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14312 2023-03-01 18:23:06.000000 dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/ofa_interface.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.140073 dynast-1.1.0rc4/dynast/supernetwork/machine_translation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/supernetwork/machine_translation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-03-02 04:20:04.000000 dynast-1.1.0rc4/dynast/supernetwork/machine_translation/modules_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7753 2023-02-09 17:30:14.000000 dynast-1.1.0rc4/dynast/supernetwork/machine_translation/transformer_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22144 2023-03-01 18:23:06.000000 dynast-1.1.0rc4/dynast/supernetwork/machine_translation/transformer_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43476 2023-03-02 04:22:44.000000 dynast-1.1.0rc4/dynast/supernetwork/machine_translation/transformer_supernetwork.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.144074 dynast-1.1.0rc4/dynast/supernetwork/recommendation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:15.000000 dynast-1.1.0rc4/dynast/supernetwork/recommendation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/dynast/supernetwork/supernetwork_registry.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.152075 dynast-1.1.0rc4/dynast/supernetwork/text_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-03-03 08:34:31.000000 dynast-1.1.0rc4/dynast/supernetwork/text_classification/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/dynast/supernetwork/text_classification/bert_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12532 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/dynast/supernetwork/text_classification/bert_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7283 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/dynast/supernetwork/text_classification/bert_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3599 2023-03-02 00:16:55.000000 dynast-1.1.0rc4/dynast/supernetwork/text_classification/sst2_dataloader.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.164076 dynast-1.1.0rc4/dynast/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-02-28 00:35:26.000000 dynast-1.1.0rc4/dynast/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-02-09 17:30:15.000000 dynast-1.1.0rc4/dynast/utils/cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9665 2023-02-09 17:30:15.000000 dynast-1.1.0rc4/dynast/utils/datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-03-01 18:23:06.000000 dynast-1.1.0rc4/dynast/utils/distributed.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8451 2023-02-16 21:50:11.000000 dynast-1.1.0rc4/dynast/utils/nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6788 2023-02-09 17:30:15.000000 dynast-1.1.0rc4/dynast/utils/reference.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.096069 dynast-1.1.0rc4/dynast.egg-info/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13654 2023-03-03 08:35:29.000000 dynast-1.1.0rc4/dynast.egg-info/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2087 2023-03-03 08:35:29.000000 dynast-1.1.0rc4/dynast.egg-info/SOURCES.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-03-03 08:35:29.000000 dynast-1.1.0rc4/dynast.egg-info/dependency_links.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-03-03 08:35:29.000000 dynast-1.1.0rc4/dynast.egg-info/entry_points.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      399 2023-03-03 08:35:29.000000 dynast-1.1.0rc4/dynast.egg-info/requires.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-03-03 08:35:29.000000 dynast-1.1.0rc4/dynast.egg-info/top_level.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      316 2023-02-09 17:30:15.000000 dynast-1.1.0rc4/pyproject.toml
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-03-03 08:35:29.184078 dynast-1.1.0rc4/setup.cfg
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-03-03 08:34:55.000000 dynast-1.1.0rc4/setup.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.176077 dynast-1.1.0rc4/tests/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-03-03 08:35:29.180077 dynast-1.1.0rc4/tests/checks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/checks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1983 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/checks/check_license.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1155 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/checks/helpers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/functional_reference.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/test_cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1249 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/test_datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-03-01 18:23:06.000000 dynast-1.1.0rc4/tests/test_dynast_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-02-09 17:30:16.000000 dynast-1.1.0rc4/tests/test_nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-02-28 00:35:26.000000 dynast-1.1.0rc4/tests/test_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-03-01 18:23:06.000000 dynast-1.1.0rc4/tests/test_utils_distributed.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.318829 dynast-1.1.1rc1/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/LICENSE.md
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 22:18:48.314829 dynast-1.1.1rc1/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/README.md
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.294724 dynast-1.1.1rc1/dynast/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.406736 dynast-1.1.1rc1/dynast/analytics/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/analytics/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3114 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/analytics/results.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4440 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/analytics/visualize.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4260 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/cli.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/common.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-04-17 18:37:40.000000 dynast-1.1.1rc1/dynast/dynast_manager.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.426738 dynast-1.1.1rc1/dynast/measure/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/measure/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/measure/latency.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.462741 dynast-1.1.1rc1/dynast/predictors/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/predictors/__init__.py
+-rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6754 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/predictors/dynamic_predictor.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-02-15 23:55:06.000000 dynast-1.1.1rc1/dynast/predictors/predictor_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/python.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.518747 dynast-1.1.1rc1/dynast/search/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/search/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-02-28 00:09:11.000000 dynast-1.1.1rc1/dynast/search/encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/search/evaluation_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16411 2023-03-01 18:19:31.000000 dynast-1.1.1rc1/dynast/search/evolutionary.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41232 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/search/search_tactic.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.542750 dynast-1.1.1rc1/dynast/supernetwork/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.554751 dynast-1.1.1rc1/dynast/supernetwork/image_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.586754 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.610756 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.622758 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.662762 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.686764 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.726769 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.790775 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14924 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14562 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12722 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.854782 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8794 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8315 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.902787 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16263 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.998797 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.030800 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6956 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2236 2023-03-01 18:23:06.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15134 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.082805 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-03-02 04:20:04.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7753 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22144 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43476 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.094806 dynast-1.1.1rc1/dynast/supernetwork/recommendation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:15.000000 dynast-1.1.1rc1/dynast/supernetwork/recommendation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/supernetwork_registry.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.142811 dynast-1.1.1rc1/dynast/supernetwork/text_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-04-19 16:16:52.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12532 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7283 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3599 2023-03-02 00:16:55.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/sst2_dataloader.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.198817 dynast-1.1.1rc1/dynast/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-04-13 00:13:03.000000 dynast-1.1.1rc1/dynast/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-02-09 17:30:15.000000 dynast-1.1.1rc1/dynast/utils/cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9665 2023-04-17 23:29:51.000000 dynast-1.1.1rc1/dynast/utils/datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-03-01 18:23:06.000000 dynast-1.1.1rc1/dynast/utils/distributed.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6569 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/utils/nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6722 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/utils/reference.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.374732 dynast-1.1.1rc1/dynast.egg-info/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4906 2023-04-24 22:18:47.000000 dynast-1.1.1rc1/dynast.egg-info/SOURCES.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/dependency_links.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/entry_points.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      354 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/requires.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/top_level.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      316 2023-03-06 23:12:04.000000 dynast-1.1.1rc1/pyproject.toml
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-04-24 22:18:48.322830 dynast-1.1.1rc1/setup.cfg
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-04-24 22:18:44.000000 dynast-1.1.1rc1/setup.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.274825 dynast-1.1.1rc1/tests/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.306828 dynast-1.1.1rc1/tests/checks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/checks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/tests/checks/check_license.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1155 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/checks/helpers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-04-17 23:32:40.000000 dynast-1.1.1rc1/tests/functional_reference.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/test_cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1249 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/test_datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-04-17 18:37:41.000000 dynast-1.1.1rc1/tests/test_dynast_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/test_nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/tests/test_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/tests/test_utils_distributed.py
```

### Comparing `dynast-1.1.0rc4/LICENSE.md` & `dynast-1.1.1rc1/dynast/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# License Agreement
+# Copyright (c) 2022 Intel Corporation
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-Copyright (c) 2022 Intel Corporation
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-  http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+from dynast.python import main as dynast  # noqa: F401
```

### Comparing `dynast-1.1.0rc4/PKG-INFO` & `dynast-1.1.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.1.0rc4
+Version: 1.1.1rc1
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -75,17 +75,19 @@
 
 You can also install DyNAS-T from PyPI:
 
 ```bash
 pip install dynast
 ```
 
+Installing DyNAS-T with `pip` will make a `dynast` command available in your CLI.
+
 
 ## Running DyNAS-T
-The `run_search.py` template provide a starting point for running the NAS process. An evaluation is the process of determining the fitness of an architectural candidate. A *validation* evaluation is the costly process of running the full validation set. A *predictor* evaluation uses a pre-trained performance predictor.
+The `dynast/cli.py` (you can use `dynast` command to invoke this script) template provide a starting point for running the NAS process. An evaluation is the process of determining the fitness of an architectural candidate. A *validation* evaluation is the costly process of running the full validation set. A *predictor* evaluation uses a pre-trained performance predictor.
 
 * `supernet` - Name of the pre-trained super-network. See list of supported super-networks. For a custom super-network, you will have to modify the code including the `dynast_manager.py` and `supernetwork_registry.py` files.
 * `optimization_metrics` - These are the metrics that the NAS process optimizes for. Note that the number of objectives you specify must be compatible with the supporting algorithm.
 * `measurements` - In addition to the optimization metrics, you can specify which measurements you would like to take during an full evaluation.
 * `search_tactic` - `linas` Lightweight iterative NAS (recommended) or `evolutionary` (good for benchmarking and testing new super-networks).
 * `search_algo` - Determines which evolutionary algorithm to run for the `linas` low-fidelity inner loop or the `evolutionary` search tactic.
 * `num_evals` - Number of evaluations (full validation measurements) to take. For example, if 1 validation measurement takes 5 minutes, 120 evaluations would take 10 hours.
@@ -95,84 +97,84 @@
 * `dataset_path` - Location of the dataset used for training the super-network of interest.
 
 ### Single-Objective
 
 *Example 1a.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy using a simple evolutionary genetic algorithm (GA) approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_ga_acc.csv \
     --search_tactic evolutionary \
     --num_evals 250 \
     --search_algo ga
 ```
 
 *Example 1b.* NAS process for the OFA MobileNetV3-w1.2 super-network that optimizes for ImageNet Top-1 accuracy using a LINAS + GA approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.2 \
     --optimization_metrics accuracy_top1 \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w12_linasga_acc.csv \
     --search_tactic linas \
     --num_evals 250 \
     --search_algo ga
 ```
 
 ### Multi-Objective
 
 *Example 2a.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy *and* multiply-and-accumulates (MACs) using a LINAS+NSGA-II approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 macs \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_linasnsga2_acc_macs.csv \
     --search_tactic evolutionary \
     --num_evals 250 \
     --search_algo nsga2
 ```
 
 *Example 2b.* NAS process for the OFA ResNet50 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) using a evolutionary AGE-MOEA approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_resnet50 \
     --optimization_metrics accuracy_top1 params \
     --measurements accuracy_top1 macs params \
     --results_path resnet50_age_acc_params.csv \
     --search_tactic evolutionary \
     --num_evals 500 \
     --search_algo age
 ```
 
 ### Many-Objective
 
 *Example 3a.* NAS process for the OFA ResNet50 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) *and* multiply-and-accumulates (MACs) using a evolutionary unsga3 approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_resnet50 \
     --optimization_metrics accuracy_top1 macs params \
     --measurements accuracy_top1 macs params \
     --results_path resnet50_linasunsga3_acc_macs_params.csv \
     --search_tactic evolutionary \
     --num_evals 500 \
     --search_algo unsga3
 ```
 
 *Example 3b.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) *and* multiply-and-accumulates (MACs) using a linas+unsga3 approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 macs params \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_linasunsga3_acc_macs_params.csv \
     --search_tactic linas \
     --num_evals 500 \
     --search_algo unsga3
@@ -193,15 +195,15 @@
 OMP_NUM_THREADS=28 mpirun \
     --report-bindings \
     -x MASTER_ADDR=127.0.0.1 \
     -x MASTER_PORT=1234 \
     -np 2 \
     -bind-to socket \
     -map-by socket \
-    python run_search.py \
+    dynast \
         --supernet ofa_mbv3_d234_e346_k357_w1.0 \
          --optimization_metrics accuracy_top1 macs \
         --results_path results.csv \
         --search_tactic linas \
         --distributed \
         --population 50 \
         --num_evals 250
```

### Comparing `dynast-1.1.0rc4/README.md` & `dynast-1.1.1rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,19 @@
 
 You can also install DyNAS-T from PyPI:
 
 ```bash
 pip install dynast
 ```
 
+Installing DyNAS-T with `pip` will make a `dynast` command available in your CLI.
+
 
 ## Running DyNAS-T
-The `run_search.py` template provide a starting point for running the NAS process. An evaluation is the process of determining the fitness of an architectural candidate. A *validation* evaluation is the costly process of running the full validation set. A *predictor* evaluation uses a pre-trained performance predictor.
+The `dynast/cli.py` (you can use `dynast` command to invoke this script) template provide a starting point for running the NAS process. An evaluation is the process of determining the fitness of an architectural candidate. A *validation* evaluation is the costly process of running the full validation set. A *predictor* evaluation uses a pre-trained performance predictor.
 
 * `supernet` - Name of the pre-trained super-network. See list of supported super-networks. For a custom super-network, you will have to modify the code including the `dynast_manager.py` and `supernetwork_registry.py` files.
 * `optimization_metrics` - These are the metrics that the NAS process optimizes for. Note that the number of objectives you specify must be compatible with the supporting algorithm.
 * `measurements` - In addition to the optimization metrics, you can specify which measurements you would like to take during an full evaluation.
 * `search_tactic` - `linas` Lightweight iterative NAS (recommended) or `evolutionary` (good for benchmarking and testing new super-networks).
 * `search_algo` - Determines which evolutionary algorithm to run for the `linas` low-fidelity inner loop or the `evolutionary` search tactic.
 * `num_evals` - Number of evaluations (full validation measurements) to take. For example, if 1 validation measurement takes 5 minutes, 120 evaluations would take 10 hours.
@@ -79,84 +81,84 @@
 * `dataset_path` - Location of the dataset used for training the super-network of interest.
 
 ### Single-Objective
 
 *Example 1a.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy using a simple evolutionary genetic algorithm (GA) approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_ga_acc.csv \
     --search_tactic evolutionary \
     --num_evals 250 \
     --search_algo ga
 ```
 
 *Example 1b.* NAS process for the OFA MobileNetV3-w1.2 super-network that optimizes for ImageNet Top-1 accuracy using a LINAS + GA approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.2 \
     --optimization_metrics accuracy_top1 \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w12_linasga_acc.csv \
     --search_tactic linas \
     --num_evals 250 \
     --search_algo ga
 ```
 
 ### Multi-Objective
 
 *Example 2a.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy *and* multiply-and-accumulates (MACs) using a LINAS+NSGA-II approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 macs \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_linasnsga2_acc_macs.csv \
     --search_tactic evolutionary \
     --num_evals 250 \
     --search_algo nsga2
 ```
 
 *Example 2b.* NAS process for the OFA ResNet50 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) using a evolutionary AGE-MOEA approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_resnet50 \
     --optimization_metrics accuracy_top1 params \
     --measurements accuracy_top1 macs params \
     --results_path resnet50_age_acc_params.csv \
     --search_tactic evolutionary \
     --num_evals 500 \
     --search_algo age
 ```
 
 ### Many-Objective
 
 *Example 3a.* NAS process for the OFA ResNet50 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) *and* multiply-and-accumulates (MACs) using a evolutionary unsga3 approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_resnet50 \
     --optimization_metrics accuracy_top1 macs params \
     --measurements accuracy_top1 macs params \
     --results_path resnet50_linasunsga3_acc_macs_params.csv \
     --search_tactic evolutionary \
     --num_evals 500 \
     --search_algo unsga3
 ```
 
 *Example 3b.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) *and* multiply-and-accumulates (MACs) using a linas+unsga3 approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 macs params \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_linasunsga3_acc_macs_params.csv \
     --search_tactic linas \
     --num_evals 500 \
     --search_algo unsga3
@@ -177,15 +179,15 @@
 OMP_NUM_THREADS=28 mpirun \
     --report-bindings \
     -x MASTER_ADDR=127.0.0.1 \
     -x MASTER_PORT=1234 \
     -np 2 \
     -bind-to socket \
     -map-by socket \
-    python run_search.py \
+    dynast \
         --supernet ofa_mbv3_d234_e346_k357_w1.0 \
          --optimization_metrics accuracy_top1 macs \
         --results_path results.csv \
         --search_tactic linas \
         --distributed \
         --population 50 \
         --num_evals 250
```

### Comparing `dynast-1.1.0rc4/dynast/__init__.py` & `dynast-1.1.1rc1/dynast/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dynast.python import main as dynast  # noqa: F401
+
+def get_info(message=''):
+    return 'dynas-\U0001F375 : {}'.format(message)
```

### Comparing `dynast-1.1.0rc4/dynast/analytics/__init__.py` & `dynast-1.1.1rc1/dynast/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/analytics/results.py` & `dynast-1.1.1rc1/dynast/analytics/results.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/analytics/visualize.py` & `dynast-1.1.1rc1/dynast/analytics/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import itertools
 import math
-from turtle import pd
+import pandas as pd
 
 import numpy as np
 from scipy.spatial import Delaunay
 from shapely.geometry import MultiLineString, MultiPoint, mapping
 from shapely.ops import cascaded_union, polygonize
 
 from dynast.utils import log
```

### Comparing `dynast-1.1.0rc4/dynast/cli.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,13 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# This software is subject to the terms and conditions entered into between the parties.
 
-from dynast.common import get_info
+# Once for All: Train One Network and Specialize it for Efficient Deployment
+# Han Cai, Chuang Gan, Tianzhe Wang, Zhekai Zhang, Song Han
+# International Conference on Learning Representations (ICLR), 2020.
 
-
-def main():
-    print(get_info('cli'))
+from .imagenet import *
```

### Comparing `dynast-1.1.0rc4/dynast/common.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,10 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Once for All: Train One Network and Specialize it for Efficient Deployment
+# Han Cai, Chuang Gan, Tianzhe Wang, Zhekai Zhang, Song Han
+# International Conference on Learning Representations (ICLR), 2020.
 
-def get_info(message=''):
-    return 'dynas-\U0001F375 : {}'.format(message)
+from .dynamic_layers import *
+from .dynamic_op import *
```

### Comparing `dynast-1.1.0rc4/dynast/dynast_manager.py` & `dynast-1.1.1rc1/dynast/dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/measure/__init__.py` & `dynast-1.1.1rc1/dynast/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/measure/latency.py` & `dynast-1.1.1rc1/dynast/measure/latency.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/predictors/__init__.py` & `dynast-1.1.1rc1/dynast/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/predictors/dynamic_predictor.py` & `dynast-1.1.1rc1/dynast/predictors/dynamic_predictor.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/predictors/predictor_manager.py` & `dynast-1.1.1rc1/dynast/predictors/predictor_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/python.py` & `dynast-1.1.1rc1/dynast/python.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/search/__init__.py` & `dynast-1.1.1rc1/dynast/search/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/search/encoding.py` & `dynast-1.1.1rc1/dynast/search/encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/search/evaluation_interface.py` & `dynast-1.1.1rc1/dynast/search/evaluation_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/search/evolutionary.py` & `dynast-1.1.1rc1/dynast/search/evolutionary.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/search/search_tactic.py` & `dynast-1.1.1rc1/dynast/search/search_tactic.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         seed: int = 42,
         population: int = 50,
         batch_size: int = 1,
         verbose: bool = False,
         search_algo: str = 'nsga2',
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        valid_size: int = None,
+        test_size: int = None,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         """Params:
 
         - dataset_path - (str) Path to the dataset needed by the supernetwork runner (e.g., ImageNet is used by OFA)
         - supernet - (str) Super-network name
@@ -77,15 +77,15 @@
         self.population = population
         self.batch_size = batch_size
         self.verbose = verbose
         self.search_algo = search_algo
         self.supernet_ckpt_path = supernet_ckpt_path
         self.device = device
         self.dataloader_workers = dataloader_workers
-        self.valid_size = valid_size
+        self.test_size = test_size
 
         self.verify_measurement_types()
         self.format_csv_header()
         self.init_supernet()
 
         if kwargs:
             log.debug('Passed unused parameters: {}'.format(kwargs))
@@ -186,15 +186,16 @@
         ]:
             self.runner_validate = OFARunner(
                 supernet=self.supernet,
                 dataset_path=self.dataset_path,
                 batch_size=self.batch_size,
                 device=self.device,
                 dataloader_workers=self.dataloader_workers,
-                valid_size=self.valid_size,
+                test_size=self.test_size,
+                verbose=self.verbose,
             )
         elif self.supernet == 'transformer_lt_wmt_en_de':
             self.runner_validate = TransformerLTRunner(
                 supernet=self.supernet,
                 dataset_path=self.dataset_path,
                 batch_size=self.batch_size,
                 checkpoint_path=self.supernet_ckpt_path,
@@ -241,15 +242,15 @@
         verbose: bool = False,
         search_algo: str = 'nsga2',
         population: int = 50,
         seed: int = 42,
         batch_size: int = 1,
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        valid_size: int = None,
+        test_size: int = None,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         """Params:
 
         - dataset_path - (str) Path to the dataset needed by the supernetwork runner (e.g., ImageNet is used by OFA)
         - supernet - (str) Super-network name
@@ -272,15 +273,15 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            valid_size=valid_size,
+            test_size=test_size,
             dataloader_workers=dataloader_workers,
         )
 
     def train_predictors(self, results_path: str = None):
         """Handles the training of predictors for the LINAS inner-loop based on the
         user-defined optimization metrics.
 
@@ -342,15 +343,16 @@
                     latency_predictor=self.predictor_dict['latency'],
                     macs_predictor=self.predictor_dict['macs'],
                     params_predictor=self.predictor_dict['params'],
                     acc_predictor=self.predictor_dict['accuracy_top1'],
                     dataset_path=self.dataset_path,
                     device=self.device,
                     dataloader_workers=self.dataloader_workers,
-                    valid_size=self.valid_size,
+                    test_size=self.test_size,
+                    verbose=self.verbose,
                 )
             elif self.supernet == 'transformer_lt_wmt_en_de':
                 runner_predict = TransformerLTRunner(
                     supernet=self.supernet,
                     latency_predictor=self.predictor_dict['latency'],
                     macs_predictor=self.predictor_dict['macs'],
                     params_predictor=self.predictor_dict['params'],
@@ -490,15 +492,15 @@
         results_path,
         seed=42,
         population=50,
         batch_size=1,
         verbose=False,
         search_algo='nsga2',
         supernet_ckpt_path=None,
-        valid_size: int = None,
+        test_size: int = None,
         dataloader_workers: int = 4,
         device: str = 'cpu',
         **kwargs,
     ):
         super().__init__(
             dataset_path=dataset_path,
             supernet=supernet,
@@ -509,15 +511,15 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            valid_size=valid_size,
+            test_size=test_size,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
 
         self._init_search()
 
@@ -628,15 +630,15 @@
         seed=42,
         population=50,
         batch_size=1,
         verbose=False,
         search_algo='nsga2',
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        valid_size: int = None,
+        test_size: int = None,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         super().__init__(
             dataset_path=dataset_path,
             supernet=supernet,
             optimization_metrics=optimization_metrics,
@@ -646,15 +648,15 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            valid_size=valid_size,
+            test_size=test_size,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
 
         self._init_search()
 
@@ -684,15 +686,15 @@
         verbose: bool = False,
         search_algo: str = 'nsga2',
         population: int = 50,
         seed: int = 42,
         batch_size: int = 1,
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        valid_size: int = None,
+        test_size: int = None,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         self.main_results_path = results_path
         LOCAL_RANK, WORLD_RANK, WORLD_SIZE, DIST_METHOD = get_distributed_vars()
         results_path = get_worker_results_path(results_path, WORLD_RANK)
 
@@ -706,15 +708,15 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            valid_size=valid_size,
+            test_size=test_size,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
         """Runs the LINAS search"""
 
         self._init_search()
@@ -778,15 +780,16 @@
                         latency_predictor=self.predictor_dict['latency'],
                         macs_predictor=self.predictor_dict['macs'],
                         params_predictor=self.predictor_dict['params'],
                         acc_predictor=self.predictor_dict['accuracy_top1'],
                         dataset_path=self.dataset_path,
                         device=self.device,
                         dataloader_workers=self.dataloader_workers,
-                        valid_size=self.valid_size,
+                        test_size=self.test_size,
+                        verbose=self.verbose,
                     )
                 elif self.supernet == 'transformer_lt_wmt_en_de':
                     runner_predict = TransformerLTRunner(
                         supernet=self.supernet,
                         latency_predictor=self.predictor_dict['latency'],
                         macs_predictor=self.predictor_dict['macs'],
                         params_predictor=self.predictor_dict['params'],
@@ -923,15 +926,15 @@
         results_path,
         seed=42,
         population=50,
         batch_size=1,
         verbose=False,
         search_algo='nsga2',
         supernet_ckpt_path: str = None,
-        valid_size: int = None,
+        test_size: int = None,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         self.main_results_path = results_path
         LOCAL_RANK, WORLD_RANK, WORLD_SIZE, DIST_METHOD = get_distributed_vars()
         results_path = get_worker_results_path(results_path, WORLD_RANK)
 
@@ -944,15 +947,15 @@
             results_path=results_path,
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
-            valid_size=valid_size,
+            test_size=test_size,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
 
         self._init_search()
```

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/image_classification/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/ofa_encoding.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/image_classification/ofa/ofa_interface.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 
 import copy
 import csv
 import uuid
 from datetime import datetime
 from typing import Tuple
 
-import ofa
 import torch
-from ofa.imagenet_classification.data_providers.imagenet import ImagenetDataProvider
-from ofa.imagenet_classification.run_manager import ImagenetRunConfig, RunManager
-from ofa.tutorial.flops_table import rm_bn_from_net
 
 from dynast.measure.latency import auto_steps
 from dynast.predictors.dynamic_predictor import Predictor
 from dynast.search.evaluation_interface import EvaluationInterface
+from dynast.supernetwork.image_classification.ofa.ofa import model_zoo as ofa_model_zoo
+from dynast.supernetwork.image_classification.ofa.ofa.imagenet_classification.data_providers.imagenet import (
+    ImagenetDataProvider,
+)
+from dynast.supernetwork.image_classification.ofa.ofa.imagenet_classification.run_manager import (
+    ImagenetRunConfig,
+    RunManager,
+)
 from dynast.utils import log
-from dynast.utils.nn import get_macs, get_parameters, measure_latency
+from dynast.utils.datasets import ImageNet
+from dynast.utils.nn import get_macs, get_parameters, measure_latency, validate_classification
 
 
 class OFARunner:
     """The OFARunner class manages the sub-network selection from the OFA super-network and
     the validation measurements of the sub-networks. ResNet50, MobileNetV3 w1.0, and MobileNetV3 w1.2
     are currently supported. Imagenet is required for these super-networks `imagenet-ilsvrc2012`.
     """
@@ -44,30 +49,43 @@
         acc_predictor: Predictor = None,
         macs_predictor: Predictor = None,
         latency_predictor: Predictor = None,
         params_predictor: Predictor = None,
         batch_size: int = 1,
         dataloader_workers: int = 4,
         device: str = 'cpu',
-        valid_size: int = None,
+        test_size: int = None,
+        verbose: bool = False,
     ):
         self.supernet = supernet
         self.acc_predictor = acc_predictor
         self.macs_predictor = macs_predictor
         self.latency_predictor = latency_predictor
         self.params_predictor = params_predictor
         self.batch_size = batch_size
         self.device = device
-        self.test_size = None
+        self.test_size = test_size
+        self.verbose = verbose
+        self.dataset_path = dataset_path
+        self.dataloader_workers = dataloader_workers
         ImagenetDataProvider.DEFAULT_PATH = dataset_path
-        self.ofa_network = ofa.model_zoo.ofa_net(supernet, pretrained=True)
+
+        self.ofa_network = ofa_model_zoo.ofa_net(supernet, pretrained=True)
         self.run_config = ImagenetRunConfig(
             test_batch_size=batch_size,
             n_worker=dataloader_workers,
-            valid_size=valid_size,
+            valid_size=test_size,
+        )
+        self._init_data()
+
+    def _init_data(self):
+        ImageNet.PATH = self.dataset_path
+        self.dataloader = ImageNet.validation_dataloader(
+            batch_size=self.batch_size,
+            num_workers=self.dataloader_workers,
         )
 
     def estimate_accuracy_top1(self, subnet_cfg) -> float:
         top1 = self.acc_predictor.predict(subnet_cfg)
         return top1
 
     def estimate_macs(self, subnet_cfg) -> int:
@@ -83,21 +101,33 @@
         return parameters
 
     def validate_top1(self, subnet_cfg, device=None) -> float:
         device = self.device if not device else device
 
         subnet = self.get_subnet(subnet_cfg)
         folder_name = '/tmp/ofa-tmp-{}'.format(uuid.uuid1().hex)  # TODO(macsz) root directory should be configurable
-        run_manager = RunManager('{}/eval_subnet'.format(folder_name), subnet, self.run_config, init=False)
+        run_manager = RunManager(
+            '{}/eval_subnet'.format(folder_name),
+            subnet,
+            self.run_config,
+            init=False,
+            verbose=self.verbose,
+        )
         run_manager.reset_running_statistics(net=subnet)
 
         # Test sampled subnet
         self.run_config.data_provider.assign_active_img_size(subnet_cfg['r'][0])
-        loss, acc = run_manager.validate(net=subnet, no_logs=True)
-        top1 = acc[0]
+
+        loss, top1, top5 = validate_classification(
+            model=subnet,
+            data_loader=self.dataloader,
+            test_size=self.test_size,
+            device=self.device,
+        )
+
         return top1
 
     def validate_macs_params(self, subnet_cfg: dict, device: str = None) -> Tuple[int, int]:
         """Measure Torch model's FLOPs/MACs as per FVCore calculation
         Args:
             subnet_cfg: sub-network Torch model
             device: Target device. If not provided will use self.device.
```

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/machine_translation/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/machine_translation/modules_supernetwork.py` & `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/machine_translation/transformer_encoding.py` & `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/machine_translation/transformer_interface.py` & `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_interface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -625,17 +625,17 @@
         if self.csv_path:
             with open(self.csv_path, 'a') as f:
                 writer = csv.writer(f)
                 date = str(datetime.now())
                 result = [
                     subnet_sample,
                     date,
+                    individual_results['params'],
                     individual_results['latency'],
                     individual_results['macs'],
-                    individual_results['params'],
                     individual_results['bleu'],
                 ]
                 writer.writerow(result)
 
         # PyMoo only minimizes objectives, thus accuracy needs to be negative
         individual_results['bleu'] = -individual_results['bleu']
         # Return results to pymoo
```

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/machine_translation/transformer_supernetwork.py` & `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/recommendation/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/supernetwork_registry.py` & `dynast-1.1.1rc1/dynast/supernetwork/supernetwork_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 LINAS_INNERLOOP_EVALS = {
     'ofa_resnet50': 5000,
     'ofa_mbv3_d234_e346_k357_w1.0': 20000,
     'ofa_mbv3_d234_e346_k357_w1.2': 20000,
     'ofa_proxyless_d234_e346_k357_w1.3': 20000,
     'transformer_lt_wmt_en_de': 10000,
-    'bert_base_sst2': 10000,
+    'bert_base_sst2': 20000,
 }
 
 SUPERNET_TYPE = {
     'image_classification': [
         'ofa_resnet50',
         'ofa_mbv3_d234_e346_k357_w1.0',
         'ofa_mbv3_d234_e346_k357_w1.2',
```

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/text_classification/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/text_classification/bert_encoding.py` & `dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/text_classification/bert_interface.py` & `dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_interface.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -340,17 +340,17 @@
         if self.csv_path:
             with open(self.csv_path, 'a') as f:
                 writer = csv.writer(f)
                 date = str(datetime.now())
                 result = [
                     subnet_sample,
                     date,
+                    individual_results['params'],
                     individual_results['latency'],
                     individual_results['macs'],
-                    individual_results['params'],
                     individual_results['accuracy_sst2'],
                 ]
                 writer.writerow(result)
 
         # PyMoo only minimizes objectives, thus accuracy needs to be negative
         individual_results['accuracy_sst2'] = -individual_results['accuracy_sst2']
         # Return results to pymoo
```

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/text_classification/bert_supernetwork.py` & `dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/supernetwork/text_classification/sst2_dataloader.py` & `dynast-1.1.1rc1/dynast/supernetwork/text_classification/sst2_dataloader.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/utils/__init__.py` & `dynast-1.1.1rc1/dynast/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/utils/cache.py` & `dynast-1.1.1rc1/dynast/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/utils/datasets.py` & `dynast-1.1.1rc1/dynast/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/utils/distributed.py` & `dynast-1.1.1rc1/dynast/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/dynast/utils/nn.py` & `dynast-1.1.1rc1/dynast/utils/nn.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import time
-from typing import Tuple, Union
+from typing import List, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torchprofile
 
 from dynast.utils import log, measure_time
@@ -44,15 +44,15 @@
     def update(self, val, n=1):
         self.val = val
         self.sum += val * n
         self.count += n
         self.avg = self.sum / self.count
 
 
-def accuracy(output, target, topk=(1,)):
+def accuracy(output, target, topk=(1,)) -> List[float]:
     """Computes the accuracy over the k top predictions for the specified values of k"""
     with torch.no_grad():
         maxk = max(topk)
         batch_size = target.size(0)
 
         _, pred = output.topk(maxk, 1, True, True)
         pred = pred.t()
@@ -65,102 +65,55 @@
         return res
 
 
 @measure_time
 def validate_classification(
     model,
     data_loader,
-    epoch=0,
     test_size=None,
-    is_openvino=False,
-    is_onnx=False,
-    use_mkldnn=False,
     device='cpu',
-    batch_size=128,
 ):
-    # NOTE(macsz): if `use_mkldnn` is set to True and model is an OFA submodel,
-    # please refer to HANDI OFA and follow MKLDNN instructions there.
-
     test_criterion = nn.CrossEntropyLoss()
 
-    if (not is_openvino) and (not is_onnx):
-        if not isinstance(model, nn.DataParallel):
-            model = nn.DataParallel(model)
-        model = model.eval()
+    model = model.eval()
 
     losses = AverageMeter()
     top1 = AverageMeter()
     top5 = AverageMeter()
 
     if test_size is not None:
         total = test_size
     else:
         total = len(data_loader)
 
-    def to_numpy(tensor):
-        return tensor.detach().cpu().numpy() if tensor.requires_grad else tensor.cpu().numpy()
-
     with torch.no_grad():
-        for i, (images, labels) in enumerate(data_loader):
-            epoch += 1
+        for epoch, (images, labels) in enumerate(data_loader):
             log.debug(
                 "Validate #{}/{} {}".format(
-                    epoch,
+                    epoch + 1,
                     total,
                     {
                         "loss": losses.avg,
                         "top1": top1.avg,
                         "top5": top5.avg,
                         "img_size": images.size(2),
                     },
                 )
             )
             images, labels = images.to(device), labels.to(device)
 
-            if use_mkldnn:
-                images = images.to_mkldnn()
-
-            # compute output
-            if is_onnx:
-                output = model.run(
-                    [model.get_outputs()[0].name],
-                    {model.get_inputs()[0].name: to_numpy(images)},
-                )
-                output = torch.from_numpy(output[0]).to(device)
-            elif is_openvino:
-                expected_batch_size = model.inputs["input"].shape[0]
-                img = to_numpy(images)
-                batch_size = len(img)
-
-                # openvino cannot handle dynamic batch sizes, so for
-                # the last batch of dataset, zero pad the batch size
-                if batch_size != expected_batch_size:
-                    assert batch_size < expected_batch_size, "Assert batch_size:{} < expected_batch_size:{}".format(
-                        batch_size, expected_batch_size
-                    )
-                    npad = expected_batch_size - batch_size
-                    img = np.pad(img, ((0, npad), (0, 0), (0, 0), (0, 0)), mode="constant")
-                    img = img.copy()
-
-                output = model.infer(inputs={"input": img})
-                output = torch.Tensor(output["output"])[:batch_size]
-            else:
-                output = model(images)
-
-            if use_mkldnn:
-                output = output.to_dense()
+            output = model(images)
 
             loss = test_criterion(output, labels)
-            # measure accuracy and record loss
             acc1, acc5 = accuracy(output, labels, topk=(1, 5))
 
             losses.update(loss.item(), images.size(0))
             top1.update(acc1, images.size(0))
             top5.update(acc5, images.size(0))
-            if i > total:
+            if epoch + 1 >= total:
                 break
     return losses.avg, top1.avg, top5.avg
 
 
 def get_parameters(
     model: nn.Module,
     device: str = 'cpu',
```

### Comparing `dynast-1.1.0rc4/dynast/utils/reference.py` & `dynast-1.1.1rc1/dynast/utils/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,14 @@
         input_size: int = 224,
         test_size: int = None,
     ) -> Tuple[float, float, float]:
         model = self.model.to(device)
         loss, top1, top5 = validate_classification(
             model=model,
             device=device,
-            is_openvino=False,
-            batch_size=batch_size,
             data_loader=self.dataset.validation_dataloader(
                 batch_size=batch_size,
                 image_size=input_size,
             ),
             test_size=test_size,
         )
         log.info(
```

### Comparing `dynast-1.1.0rc4/dynast.egg-info/PKG-INFO` & `dynast-1.1.1rc1/dynast.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.1.0rc4
+Version: 1.1.1rc1
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -75,17 +75,19 @@
 
 You can also install DyNAS-T from PyPI:
 
 ```bash
 pip install dynast
 ```
 
+Installing DyNAS-T with `pip` will make a `dynast` command available in your CLI.
+
 
 ## Running DyNAS-T
-The `run_search.py` template provide a starting point for running the NAS process. An evaluation is the process of determining the fitness of an architectural candidate. A *validation* evaluation is the costly process of running the full validation set. A *predictor* evaluation uses a pre-trained performance predictor.
+The `dynast/cli.py` (you can use `dynast` command to invoke this script) template provide a starting point for running the NAS process. An evaluation is the process of determining the fitness of an architectural candidate. A *validation* evaluation is the costly process of running the full validation set. A *predictor* evaluation uses a pre-trained performance predictor.
 
 * `supernet` - Name of the pre-trained super-network. See list of supported super-networks. For a custom super-network, you will have to modify the code including the `dynast_manager.py` and `supernetwork_registry.py` files.
 * `optimization_metrics` - These are the metrics that the NAS process optimizes for. Note that the number of objectives you specify must be compatible with the supporting algorithm.
 * `measurements` - In addition to the optimization metrics, you can specify which measurements you would like to take during an full evaluation.
 * `search_tactic` - `linas` Lightweight iterative NAS (recommended) or `evolutionary` (good for benchmarking and testing new super-networks).
 * `search_algo` - Determines which evolutionary algorithm to run for the `linas` low-fidelity inner loop or the `evolutionary` search tactic.
 * `num_evals` - Number of evaluations (full validation measurements) to take. For example, if 1 validation measurement takes 5 minutes, 120 evaluations would take 10 hours.
@@ -95,84 +97,84 @@
 * `dataset_path` - Location of the dataset used for training the super-network of interest.
 
 ### Single-Objective
 
 *Example 1a.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy using a simple evolutionary genetic algorithm (GA) approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_ga_acc.csv \
     --search_tactic evolutionary \
     --num_evals 250 \
     --search_algo ga
 ```
 
 *Example 1b.* NAS process for the OFA MobileNetV3-w1.2 super-network that optimizes for ImageNet Top-1 accuracy using a LINAS + GA approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.2 \
     --optimization_metrics accuracy_top1 \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w12_linasga_acc.csv \
     --search_tactic linas \
     --num_evals 250 \
     --search_algo ga
 ```
 
 ### Multi-Objective
 
 *Example 2a.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy *and* multiply-and-accumulates (MACs) using a LINAS+NSGA-II approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 macs \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_linasnsga2_acc_macs.csv \
     --search_tactic evolutionary \
     --num_evals 250 \
     --search_algo nsga2
 ```
 
 *Example 2b.* NAS process for the OFA ResNet50 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) using a evolutionary AGE-MOEA approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_resnet50 \
     --optimization_metrics accuracy_top1 params \
     --measurements accuracy_top1 macs params \
     --results_path resnet50_age_acc_params.csv \
     --search_tactic evolutionary \
     --num_evals 500 \
     --search_algo age
 ```
 
 ### Many-Objective
 
 *Example 3a.* NAS process for the OFA ResNet50 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) *and* multiply-and-accumulates (MACs) using a evolutionary unsga3 approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_resnet50 \
     --optimization_metrics accuracy_top1 macs params \
     --measurements accuracy_top1 macs params \
     --results_path resnet50_linasunsga3_acc_macs_params.csv \
     --search_tactic evolutionary \
     --num_evals 500 \
     --search_algo unsga3
 ```
 
 *Example 3b.* NAS process for the OFA MobileNetV3-w1.0 super-network that optimizes for ImageNet Top-1 accuracy *and* model size (parameters) *and* multiply-and-accumulates (MACs) using a linas+unsga3 approach.
 
 ```bash
-python run_search.py \
+dynast \
     --supernet ofa_mbv3_d234_e346_k357_w1.0 \
     --optimization_metrics accuracy_top1 macs params \
     --measurements accuracy_top1 macs params \
     --results_path mbnv3w10_linasunsga3_acc_macs_params.csv \
     --search_tactic linas \
     --num_evals 500 \
     --search_algo unsga3
@@ -193,15 +195,15 @@
 OMP_NUM_THREADS=28 mpirun \
     --report-bindings \
     -x MASTER_ADDR=127.0.0.1 \
     -x MASTER_PORT=1234 \
     -np 2 \
     -bind-to socket \
     -map-by socket \
-    python run_search.py \
+    dynast \
         --supernet ofa_mbv3_d234_e346_k357_w1.0 \
          --optimization_metrics accuracy_top1 macs \
         --results_path results.csv \
         --search_tactic linas \
         --distributed \
         --population 50 \
         --num_evals 250
```

### Comparing `dynast-1.1.0rc4/setup.py` & `dynast-1.1.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import datetime
 
 from setuptools import find_packages, setup
 
 
 def get_version():
     # TODO(macsz) Replace with __version__
-    return '1.1.0rc4'
+    return '1.1.1rc1'
 
 
 def get_dependencies():
     deps = []
     with open('requirements.txt') as f:
         lines = f.readlines()
         for line in lines:
```

### Comparing `dynast-1.1.0rc4/tests/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/checks/__init__.py` & `dynast-1.1.1rc1/dynast/supernetwork/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/checks/check_license.py` & `dynast-1.1.1rc1/tests/checks/check_license.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 
     license_path = os.path.join(ROOT_DIR, 'LICENSE.md')
     license_content = ''
     with open(license_path) as f:
         lines = f.readlines()
         for line in lines:
             line = line.strip()
+            if line.startswith('##'):
+                # This will halt on the 3rd party licenses.
+                break
+
             if line and not line.startswith('#'):
                 license_content += line + ' '
     return license_content
 
 
 def get_license_header(path):
     license_content = ''
```

### Comparing `dynast-1.1.0rc4/tests/checks/helpers.py` & `dynast-1.1.1rc1/tests/checks/helpers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/functional_reference.py` & `dynast-1.1.1rc1/tests/functional_reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/test_cache.py` & `dynast-1.1.1rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/test_datasets.py` & `dynast-1.1.1rc1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/test_dynast_manager.py` & `dynast-1.1.1rc1/tests/test_dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/test_nn.py` & `dynast-1.1.1rc1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/test_utils.py` & `dynast-1.1.1rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.0rc4/tests/test_utils_distributed.py` & `dynast-1.1.1rc1/tests/test_utils_distributed.py`

 * *Files identical despite different names*

