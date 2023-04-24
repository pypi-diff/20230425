# Comparing `tmp/dynast-1.1.1rc1.tar.gz` & `tmp/dynast-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynast-1.1.1rc1.tar", last modified: Mon Apr 24 22:18:48 2023, max compression
+gzip compressed data, was "dynast-1.2.0rc1.tar", last modified: Mon Apr 24 22:52:14 2023, max compression
```

## Comparing `dynast-1.1.1rc1.tar` & `dynast-1.2.0rc1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.318829 dynast-1.1.1rc1/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/LICENSE.md
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 22:18:48.314829 dynast-1.1.1rc1/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/README.md
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.294724 dynast-1.1.1rc1/dynast/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.406736 dynast-1.1.1rc1/dynast/analytics/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/analytics/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3114 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/analytics/results.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4440 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/analytics/visualize.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4260 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/cli.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/common.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-04-17 18:37:40.000000 dynast-1.1.1rc1/dynast/dynast_manager.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.426738 dynast-1.1.1rc1/dynast/measure/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/measure/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/measure/latency.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.462741 dynast-1.1.1rc1/dynast/predictors/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/predictors/__init__.py
--rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6754 2023-02-09 17:30:13.000000 dynast-1.1.1rc1/dynast/predictors/dynamic_predictor.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-02-15 23:55:06.000000 dynast-1.1.1rc1/dynast/predictors/predictor_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/python.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.518747 dynast-1.1.1rc1/dynast/search/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/search/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-02-28 00:09:11.000000 dynast-1.1.1rc1/dynast/search/encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/search/evaluation_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16411 2023-03-01 18:19:31.000000 dynast-1.1.1rc1/dynast/search/evolutionary.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41232 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/search/search_tactic.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.542750 dynast-1.1.1rc1/dynast/supernetwork/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.554751 dynast-1.1.1rc1/dynast/supernetwork/image_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.586754 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.610756 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.622758 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.662762 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.686764 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.726769 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.790775 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14924 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14562 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12722 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.854782 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8794 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8315 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.902787 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16263 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.998797 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.030800 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6956 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2236 2023-03-01 18:23:06.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15134 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.082805 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-03-02 04:20:04.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7753 2023-02-09 17:30:14.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22144 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43476 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.094806 dynast-1.1.1rc1/dynast/supernetwork/recommendation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:15.000000 dynast-1.1.1rc1/dynast/supernetwork/recommendation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/supernetwork/supernetwork_registry.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.142811 dynast-1.1.1rc1/dynast/supernetwork/text_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-04-19 16:16:52.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12532 2023-04-24 21:57:09.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7283 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3599 2023-03-02 00:16:55.000000 dynast-1.1.1rc1/dynast/supernetwork/text_classification/sst2_dataloader.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.198817 dynast-1.1.1rc1/dynast/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-04-13 00:13:03.000000 dynast-1.1.1rc1/dynast/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-02-09 17:30:15.000000 dynast-1.1.1rc1/dynast/utils/cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9665 2023-04-17 23:29:51.000000 dynast-1.1.1rc1/dynast/utils/datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-03-01 18:23:06.000000 dynast-1.1.1rc1/dynast/utils/distributed.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6569 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/utils/nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6722 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/dynast/utils/reference.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:47.374732 dynast-1.1.1rc1/dynast.egg-info/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4906 2023-04-24 22:18:47.000000 dynast-1.1.1rc1/dynast.egg-info/SOURCES.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/dependency_links.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/entry_points.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      354 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/requires.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-04-24 22:18:46.000000 dynast-1.1.1rc1/dynast.egg-info/top_level.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      316 2023-03-06 23:12:04.000000 dynast-1.1.1rc1/pyproject.toml
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-04-24 22:18:48.322830 dynast-1.1.1rc1/setup.cfg
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-04-24 22:18:44.000000 dynast-1.1.1rc1/setup.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.274825 dynast-1.1.1rc1/tests/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:18:48.306828 dynast-1.1.1rc1/tests/checks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/checks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-04-24 21:46:13.000000 dynast-1.1.1rc1/tests/checks/check_license.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1155 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/checks/helpers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-04-17 23:32:40.000000 dynast-1.1.1rc1/tests/functional_reference.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/test_cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1249 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/test_datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-04-17 18:37:41.000000 dynast-1.1.1rc1/tests/test_dynast_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-02-09 17:30:16.000000 dynast-1.1.1rc1/tests/test_nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/tests/test_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-03-06 23:12:11.000000 dynast-1.1.1rc1/tests/test_utils_distributed.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:14.293094 dynast-1.2.0rc1/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/LICENSE.md
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 22:52:14.285093 dynast-1.2.0rc1/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/README.md
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.136975 dynast-1.2.0rc1/dynast/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.268988 dynast-1.2.0rc1/dynast/analytics/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/analytics/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3114 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/analytics/results.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4440 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/analytics/visualize.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4260 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/cli.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/common.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-04-17 18:37:40.000000 dynast-1.2.0rc1/dynast/dynast_manager.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.292991 dynast-1.2.0rc1/dynast/measure/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/measure/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/measure/latency.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.328994 dynast-1.2.0rc1/dynast/predictors/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/predictors/__init__.py
+-rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6754 2023-02-09 17:30:13.000000 dynast-1.2.0rc1/dynast/predictors/dynamic_predictor.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-02-15 23:55:06.000000 dynast-1.2.0rc1/dynast/predictors/predictor_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-02-09 17:30:14.000000 dynast-1.2.0rc1/dynast/python.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.393001 dynast-1.2.0rc1/dynast/search/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.2.0rc1/dynast/search/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-02-28 00:09:11.000000 dynast-1.2.0rc1/dynast/search/encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-02-09 17:30:14.000000 dynast-1.2.0rc1/dynast/search/evaluation_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16411 2023-03-01 18:19:31.000000 dynast-1.2.0rc1/dynast/search/evolutionary.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41232 2023-04-24 21:57:09.000000 dynast-1.2.0rc1/dynast/search/search_tactic.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.417003 dynast-1.2.0rc1/dynast/supernetwork/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc1/dynast/supernetwork/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.429005 dynast-1.2.0rc1/dynast/supernetwork/image_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.469009 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.497012 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.509013 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.553017 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.577020 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.617024 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.669029 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14924 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14562 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12722 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.725035 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8794 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8315 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.765039 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16263 2023-04-24 21:57:09.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.849048 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.893052 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6956 2023-04-24 21:57:09.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2236 2023-03-01 18:23:06.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15134 2023-04-24 21:57:09.000000 dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.961059 dynast-1.2.0rc1/dynast/supernetwork/machine_translation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc1/dynast/supernetwork/machine_translation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-03-02 04:20:04.000000 dynast-1.2.0rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7753 2023-02-09 17:30:14.000000 dynast-1.2.0rc1/dynast/supernetwork/machine_translation/transformer_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22144 2023-04-24 21:57:09.000000 dynast-1.2.0rc1/dynast/supernetwork/machine_translation/transformer_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43476 2023-03-06 23:12:11.000000 dynast-1.2.0rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.977061 dynast-1.2.0rc1/dynast/supernetwork/recommendation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:15.000000 dynast-1.2.0rc1/dynast/supernetwork/recommendation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/supernetwork/supernetwork_registry.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:14.049069 dynast-1.2.0rc1/dynast/supernetwork/text_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc1/dynast/supernetwork/text_classification/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-04-19 16:16:52.000000 dynast-1.2.0rc1/dynast/supernetwork/text_classification/bert_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12532 2023-04-24 21:57:09.000000 dynast-1.2.0rc1/dynast/supernetwork/text_classification/bert_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7283 2023-03-06 23:12:11.000000 dynast-1.2.0rc1/dynast/supernetwork/text_classification/bert_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3599 2023-03-02 00:16:55.000000 dynast-1.2.0rc1/dynast/supernetwork/text_classification/sst2_dataloader.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:14.129077 dynast-1.2.0rc1/dynast/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-04-13 00:13:03.000000 dynast-1.2.0rc1/dynast/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-02-09 17:30:15.000000 dynast-1.2.0rc1/dynast/utils/cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9665 2023-04-17 23:29:51.000000 dynast-1.2.0rc1/dynast/utils/datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-03-01 18:23:06.000000 dynast-1.2.0rc1/dynast/utils/distributed.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6569 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/utils/nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6722 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/dynast/utils/reference.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:13.228984 dynast-1.2.0rc1/dynast.egg-info/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 22:52:12.000000 dynast-1.2.0rc1/dynast.egg-info/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4906 2023-04-24 22:52:12.000000 dynast-1.2.0rc1/dynast.egg-info/SOURCES.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-04-24 22:52:12.000000 dynast-1.2.0rc1/dynast.egg-info/dependency_links.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-04-24 22:52:12.000000 dynast-1.2.0rc1/dynast.egg-info/entry_points.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      354 2023-04-24 22:52:12.000000 dynast-1.2.0rc1/dynast.egg-info/requires.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-04-24 22:52:12.000000 dynast-1.2.0rc1/dynast.egg-info/top_level.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      316 2023-03-06 23:12:04.000000 dynast-1.2.0rc1/pyproject.toml
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-04-24 22:52:14.293094 dynast-1.2.0rc1/setup.cfg
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-04-24 22:51:10.000000 dynast-1.2.0rc1/setup.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:14.233087 dynast-1.2.0rc1/tests/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.2.0rc1/tests/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 22:52:14.273091 dynast-1.2.0rc1/tests/checks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.2.0rc1/tests/checks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-04-24 21:46:13.000000 dynast-1.2.0rc1/tests/checks/check_license.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1155 2023-02-09 17:30:16.000000 dynast-1.2.0rc1/tests/checks/helpers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-04-17 23:32:40.000000 dynast-1.2.0rc1/tests/functional_reference.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-02-09 17:30:16.000000 dynast-1.2.0rc1/tests/test_cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1249 2023-02-09 17:30:16.000000 dynast-1.2.0rc1/tests/test_datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-04-17 18:37:41.000000 dynast-1.2.0rc1/tests/test_dynast_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-02-09 17:30:16.000000 dynast-1.2.0rc1/tests/test_nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-03-06 23:12:11.000000 dynast-1.2.0rc1/tests/test_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-03-06 23:12:11.000000 dynast-1.2.0rc1/tests/test_utils_distributed.py
```

### Comparing `dynast-1.1.1rc1/LICENSE.md` & `dynast-1.2.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/PKG-INFO` & `dynast-1.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.1.1rc1
+Version: 1.2.0rc1
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.1.1rc1/README.md` & `dynast-1.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/__init__.py` & `dynast-1.2.0rc1/dynast/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/analytics/__init__.py` & `dynast-1.2.0rc1/dynast/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/analytics/results.py` & `dynast-1.2.0rc1/dynast/analytics/results.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/analytics/visualize.py` & `dynast-1.2.0rc1/dynast/analytics/visualize.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/cli.py` & `dynast-1.2.0rc1/dynast/cli.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/common.py` & `dynast-1.2.0rc1/dynast/common.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/dynast_manager.py` & `dynast-1.2.0rc1/dynast/dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/measure/__init__.py` & `dynast-1.2.0rc1/dynast/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/measure/latency.py` & `dynast-1.2.0rc1/dynast/measure/latency.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/predictors/__init__.py` & `dynast-1.2.0rc1/dynast/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/predictors/dynamic_predictor.py` & `dynast-1.2.0rc1/dynast/predictors/dynamic_predictor.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/predictors/predictor_manager.py` & `dynast-1.2.0rc1/dynast/predictors/predictor_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/python.py` & `dynast-1.2.0rc1/dynast/python.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/search/__init__.py` & `dynast-1.2.0rc1/dynast/search/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/search/encoding.py` & `dynast-1.2.0rc1/dynast/search/encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/search/evaluation_interface.py` & `dynast-1.2.0rc1/dynast/search/evaluation_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/search/evolutionary.py` & `dynast-1.2.0rc1/dynast/search/evolutionary.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/search/search_tactic.py` & `dynast-1.2.0rc1/dynast/search/search_tactic.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py` & `dynast-1.2.0rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/machine_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py` & `dynast-1.2.0rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_encoding.py` & `dynast-1.2.0rc1/dynast/supernetwork/machine_translation/transformer_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_interface.py` & `dynast-1.2.0rc1/dynast/supernetwork/machine_translation/transformer_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py` & `dynast-1.2.0rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/recommendation/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/supernetwork_registry.py` & `dynast-1.2.0rc1/dynast/supernetwork/supernetwork_registry.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/text_classification/__init__.py` & `dynast-1.2.0rc1/dynast/supernetwork/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_encoding.py` & `dynast-1.2.0rc1/dynast/supernetwork/text_classification/bert_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_interface.py` & `dynast-1.2.0rc1/dynast/supernetwork/text_classification/bert_interface.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/text_classification/bert_supernetwork.py` & `dynast-1.2.0rc1/dynast/supernetwork/text_classification/bert_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/supernetwork/text_classification/sst2_dataloader.py` & `dynast-1.2.0rc1/dynast/supernetwork/text_classification/sst2_dataloader.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/utils/__init__.py` & `dynast-1.2.0rc1/dynast/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/utils/cache.py` & `dynast-1.2.0rc1/dynast/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/utils/datasets.py` & `dynast-1.2.0rc1/dynast/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/utils/distributed.py` & `dynast-1.2.0rc1/dynast/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/utils/nn.py` & `dynast-1.2.0rc1/dynast/utils/nn.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast/utils/reference.py` & `dynast-1.2.0rc1/dynast/utils/reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/dynast.egg-info/PKG-INFO` & `dynast-1.2.0rc1/dynast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.1.1rc1
+Version: 1.2.0rc1
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.1.1rc1/dynast.egg-info/SOURCES.txt` & `dynast-1.2.0rc1/dynast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/setup.py` & `dynast-1.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import datetime
 
 from setuptools import find_packages, setup
 
 
 def get_version():
     # TODO(macsz) Replace with __version__
-    return '1.1.1rc1'
+    return '1.2.0rc1'
 
 
 def get_dependencies():
     deps = []
     with open('requirements.txt') as f:
         lines = f.readlines()
         for line in lines:
```

### Comparing `dynast-1.1.1rc1/tests/__init__.py` & `dynast-1.2.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/checks/__init__.py` & `dynast-1.2.0rc1/tests/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/checks/check_license.py` & `dynast-1.2.0rc1/tests/checks/check_license.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/checks/helpers.py` & `dynast-1.2.0rc1/tests/checks/helpers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/functional_reference.py` & `dynast-1.2.0rc1/tests/functional_reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/test_cache.py` & `dynast-1.2.0rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/test_datasets.py` & `dynast-1.2.0rc1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/test_dynast_manager.py` & `dynast-1.2.0rc1/tests/test_dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/test_nn.py` & `dynast-1.2.0rc1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/test_utils.py` & `dynast-1.2.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.1.1rc1/tests/test_utils_distributed.py` & `dynast-1.2.0rc1/tests/test_utils_distributed.py`

 * *Files identical despite different names*

