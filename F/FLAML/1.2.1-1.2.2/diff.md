# Comparing `tmp/FLAML-1.2.1.tar.gz` & `tmp/FLAML-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-1.2.1.tar", last modified: Mon Apr 17 17:43:38 2023, max compression
+gzip compressed data, was "FLAML-1.2.2.tar", last modified: Tue Apr 25 03:33:14 2023, max compression
```

## Comparing `FLAML-1.2.1.tar` & `FLAML-1.2.2.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.746997 FLAML-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 17:42:30.000000 FLAML-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-17 17:42:30.000000 FLAML-1.2.1/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-17 17:43:38.746997 FLAML-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-17 17:42:30.000000 FLAML-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/code_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37202 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/oai/completion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129453 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)   105105 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    37129 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:43:38.746997 FLAML-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-17 17:42:30.000000 FLAML-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.746997 FLAML-1.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-25 03:32:17.000000 FLAML-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-25 03:32:17.000000 FLAML-1.2.2/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-25 03:33:14.070906 FLAML-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-25 03:32:17.000000 FLAML-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37502 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/oai/completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129453 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37129 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 03:33:14.070906 FLAML-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-25 03:32:17.000000 FLAML-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_version.py
```

### Comparing `FLAML-1.2.1/FLAML.egg-info/PKG-INFO` & `FLAML-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,14 @@
-Metadata-Version: 2.1
-Name: FLAML
-Version: 1.2.1
-Summary: A fast library for automated machine learning and tuning
-Home-page: https://github.com/microsoft/FLAML
-Author: Microsoft Corporation
-Author-email: hpo@microsoft.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: notebook
-Provides-Extra: spark
-Provides-Extra: test
-Provides-Extra: catboost
-Provides-Extra: blendsearch
-Provides-Extra: ray
-Provides-Extra: azureml
-Provides-Extra: nni
-Provides-Extra: vw
-Provides-Extra: hf
-Provides-Extra: nlp
-Provides-Extra: ts_forecast
-Provides-Extra: forecast
-Provides-Extra: benchmark
-Provides-Extra: openai
-Provides-Extra: synapse
-License-File: LICENSE
-License-File: NOTICE.md
-
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
 ![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
 [![Downloads](https://pepy.tech/badge/flaml)](https://pepy.tech/project/flaml)
-[![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![](https://img.shields.io/discord/1025786666260111483?logo=discord&style=flat)](https://discord.gg/Cppx2vSPVP)
+<!-- [![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 
 
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
@@ -144,19 +113,17 @@
 
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
-- [Talks](https://www.youtube.com/channel/UCfU0zfFXHXdAd5x-WvFBk5A) and [tutorials](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) about FLAML.
-
 - Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
 
-- FAQ [here](https://microsoft.github.io/FLAML/docs/FAQ).
+- Discord [here](https://discord.gg/Cppx2vSPVP).
 
 - Contributing guide [here](https://microsoft.github.io/FLAML/docs/Contribute).
 
 - ML.NET documentation and tutorials for [Model Builder](https://learn.microsoft.com/dotnet/machine-learning/tutorials/predict-prices-with-model-builder), [ML.NET CLI](https://learn.microsoft.com/dotnet/machine-learning/tutorials/sentiment-analysis-cli), and [AutoML API](https://learn.microsoft.com/dotnet/machine-learning/how-to-guides/how-to-use-the-automl-api).
 
 ## Contributing
```

### Comparing `FLAML-1.2.1/FLAML.egg-info/SOURCES.txt` & `FLAML-1.2.2/FLAML.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 flaml/data.py
 flaml/ml.py
 flaml/model.py
 flaml/version.py
 flaml/autogen/__init__.py
 flaml/autogen/code_utils.py
 flaml/autogen/math_utils.py
+flaml/autogen/extensions/__init__.py
 flaml/autogen/oai/__init__.py
 flaml/autogen/oai/completion.py
 flaml/automl/__init__.py
 flaml/automl/automl.py
 flaml/automl/data.py
 flaml/automl/logger.py
 flaml/automl/ml.py
```

### Comparing `FLAML-1.2.1/FLAML.egg-info/requires.txt` & `FLAML-1.2.2/FLAML.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 NumPy>=1.17.0rc1
 lightgbm>=2.3.1
 xgboost>=0.90
 scipy>=1.4.1
 pandas>=1.1.4
 scikit-learn>=0.24
 
+[autogen]
+openai==0.27.4
+diskcache
+docker
+
 [azureml]
 azureml-mlflow
 
 [benchmark]
 catboost>=0.26
 psutil==5.8.0
 xgboost==1.3.3
@@ -47,15 +52,14 @@
 jupyter
 matplotlib
 openml==0.10.2
 
 [openai]
 openai==0.27.4
 diskcache
-optuna==2.8.0
 
 [ray]
 ray[tune]~=1.13
 
 [spark]
 pyspark>=3.2.0
 joblibspark>=0.5.0
```

### Comparing `FLAML-1.2.1/LICENSE` & `FLAML-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/NOTICE.md` & `FLAML-1.2.2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/PKG-INFO` & `FLAML-1.2.2/FLAML.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.1
+Version: 1.2.2
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,25 +21,26 @@
 Provides-Extra: vw
 Provides-Extra: hf
 Provides-Extra: nlp
 Provides-Extra: ts_forecast
 Provides-Extra: forecast
 Provides-Extra: benchmark
 Provides-Extra: openai
+Provides-Extra: autogen
 Provides-Extra: synapse
 License-File: LICENSE
 License-File: NOTICE.md
 
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
 ![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
 [![Downloads](https://pepy.tech/badge/flaml)](https://pepy.tech/project/flaml)
-[![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![](https://img.shields.io/discord/1025786666260111483?logo=discord&style=flat)](https://discord.gg/Cppx2vSPVP)
+<!-- [![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 
 
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
@@ -144,19 +145,17 @@
 
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
-- [Talks](https://www.youtube.com/channel/UCfU0zfFXHXdAd5x-WvFBk5A) and [tutorials](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) about FLAML.
-
 - Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
 
-- FAQ [here](https://microsoft.github.io/FLAML/docs/FAQ).
+- Discord [here](https://discord.gg/Cppx2vSPVP).
 
 - Contributing guide [here](https://microsoft.github.io/FLAML/docs/Contribute).
 
 - ML.NET documentation and tutorials for [Model Builder](https://learn.microsoft.com/dotnet/machine-learning/tutorials/predict-prices-with-model-builder), [ML.NET CLI](https://learn.microsoft.com/dotnet/machine-learning/tutorials/sentiment-analysis-cli), and [AutoML API](https://learn.microsoft.com/dotnet/machine-learning/how-to-guides/how-to-use-the-automl-api).
 
 ## Contributing
```

### Comparing `FLAML-1.2.1/README.md` & `FLAML-1.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,46 @@
+Metadata-Version: 2.1
+Name: FLAML
+Version: 1.2.2
+Summary: A fast library for automated machine learning and tuning
+Home-page: https://github.com/microsoft/FLAML
+Author: Microsoft Corporation
+Author-email: hpo@microsoft.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: notebook
+Provides-Extra: spark
+Provides-Extra: test
+Provides-Extra: catboost
+Provides-Extra: blendsearch
+Provides-Extra: ray
+Provides-Extra: azureml
+Provides-Extra: nni
+Provides-Extra: vw
+Provides-Extra: hf
+Provides-Extra: nlp
+Provides-Extra: ts_forecast
+Provides-Extra: forecast
+Provides-Extra: benchmark
+Provides-Extra: openai
+Provides-Extra: autogen
+Provides-Extra: synapse
+License-File: LICENSE
+License-File: NOTICE.md
+
 [![PyPI version](https://badge.fury.io/py/FLAML.svg)](https://badge.fury.io/py/FLAML)
 ![Conda version](https://img.shields.io/conda/vn/conda-forge/flaml)
 [![Build](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml/badge.svg)](https://github.com/microsoft/FLAML/actions/workflows/python-package.yml)
 ![Python Version](https://img.shields.io/badge/3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)
 [![Downloads](https://pepy.tech/badge/flaml)](https://pepy.tech/project/flaml)
-[![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![](https://img.shields.io/discord/1025786666260111483?logo=discord&style=flat)](https://discord.gg/Cppx2vSPVP)
+<!-- [![Join the chat at https://gitter.im/FLAMLer/community](https://badges.gitter.im/FLAMLer/community.svg)](https://gitter.im/FLAMLer/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) -->
 
 
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
@@ -113,19 +145,17 @@
 
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
-- [Talks](https://www.youtube.com/channel/UCfU0zfFXHXdAd5x-WvFBk5A) and [tutorials](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) about FLAML.
-
 - Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
 
-- FAQ [here](https://microsoft.github.io/FLAML/docs/FAQ).
+- Discord [here](https://discord.gg/Cppx2vSPVP).
 
 - Contributing guide [here](https://microsoft.github.io/FLAML/docs/Contribute).
 
 - ML.NET documentation and tutorials for [Model Builder](https://learn.microsoft.com/dotnet/machine-learning/tutorials/predict-prices-with-model-builder), [ML.NET CLI](https://learn.microsoft.com/dotnet/machine-learning/tutorials/sentiment-analysis-cli), and [AutoML API](https://learn.microsoft.com/dotnet/machine-learning/how-to-guides/how-to-use-the-automl-api).
 
 ## Contributing
```

### Comparing `FLAML-1.2.1/flaml/autogen/math_utils.py` & `FLAML-1.2.2/flaml/autogen/math_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,32 @@
 from typing import Optional
+from flaml.autogen import oai, DEFAULT_MODEL
+
+_MATH_PROMPT = "{problem} Solve the problem carefully. Simplify your answer as much as possible. Put the final answer in \\boxed{{}}."
+_MATH_CONFIG = {
+    "model": DEFAULT_MODEL,
+    "prompt": _MATH_PROMPT,
+}
+
+
+def solve_problem(problem: str, **config) -> str:
+    """(work in progress) Solve the math problem.
+
+    Args:
+        problem (str): The problem statement.
+        config (Optional, dict): The configuration for the API call.
+
+    Returns:
+        str: The solution to the problem.
+    """
+    params = {**_MATH_CONFIG, **config}
+    response = oai.Completion.create({"problem": problem}, **params)
+    cost = oai.Completion.cost(params["model"], response)
+    results = eval_math_responses(oai.Completion.extract_text(response))
+    return results.get("voted_answer"), cost
 
 
 def remove_boxed(string: str) -> Optional[str]:
     """Source: https://github.com/hendrycks/math
     Extract the text within a \\boxed{...} environment.
     Example:
     >>> remove_boxed(\\boxed{\\frac{2}{3}})
```

### Comparing `FLAML-1.2.1/flaml/autogen/oai/completion.py` & `FLAML-1.2.2/flaml/autogen/oai/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,17 +141,18 @@
                 # print("using cached response")
                 return response
         openai_completion = openai.ChatCompletion if config["model"] in cls.chat_models else openai.Completion
         start_time = time.time()
         request_timeout = cls.request_timeout
         while True:
             try:
-                response = openai_completion.create(request_timeout=request_timeout, **config)
-                cls._cache.set(key, response)
-                return response
+                if "request_timeout" in config:
+                    response = openai_completion.create(**config)
+                else:
+                    response = openai_completion.create(request_timeout=request_timeout, **config)
             except (
                 ServiceUnavailableError,
                 APIError,
                 APIConnectionError,
             ):
                 # transient error
                 logger.warning(f"retrying in {cls.retry_time} seconds...", exc_info=1)
@@ -166,29 +167,36 @@
                 ):
                     logger.info(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 elif eval_only:
                     raise
                 else:
                     break
                 if isinstance(e, Timeout):
+                    if "request_timeout" in config:
+                        raise
                     request_timeout <<= 1
                 request_timeout = min(request_timeout, time_left)
                 sleep(cls.retry_time)
             except InvalidRequestError:
                 if "azure" == openai.api_type and "model" in config:
                     # azure api uses "engine" instead of "model"
                     config = config.copy()
                     config["engine"] = config.pop("model").replace("gpt-3.5-turbo", "gpt-35-turbo")
                 else:
                     raise
+            else:
+                if use_cache:
+                    cls._cache.set(key, response)
+                return response
         logger.warning(
             f"Failed to get response from openai api due to getting RateLimitError or Timeout for {cls.retry_timeout} seconds."
         )
         response = -1
-        cls._cache.set(key, response)
+        if use_cache:
+            cls._cache.set(key, response)
         return response
 
     @classmethod
     def _get_max_valid_n(cls, key, max_tokens):
         # find the max value in max_valid_n_per_max_tokens
         # whose key is equal or larger than max_tokens
         return max(
```

### Comparing `FLAML-1.2.1/flaml/automl/automl.py` & `FLAML-1.2.2/flaml/automl/automl.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/data.py` & `FLAML-1.2.2/flaml/automl/data.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/ml.py` & `FLAML-1.2.2/flaml/automl/ml.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/model.py` & `FLAML-1.2.2/flaml/automl/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1132,16 +1132,15 @@
 
         new_trainer = self._init_model_for_predict()
         try:
             predictions = new_trainer.predict(test_dataset).predictions
         except ZeroDivisionError:
             logger.warning("Zero division error appeared in HuggingFace Transformers.")
             predictions = np.array([-0.05] * len(test_dataset))
-        else:
-            return predictions
+        return predictions
 
     def score(self, X_val: DataFrame, y_val: Series, **kwargs):
         import transformers
 
         transformers.logging.set_verbosity_error()
 
         self._metric = kwargs["metric"]
@@ -1165,22 +1164,21 @@
         X_test, _ = self._tokenize_text(X, **self._kwargs)
         test_dataset = Dataset.from_pandas(X_test)
 
         new_trainer = self._init_model_for_predict()
 
         kwargs = {} if self._task not in NLG_TASKS else {"metric_key_prefix": "predict"}
         try:
-            predictions = new_trainer.predict(test_dataset, **kwargs)
+            predictions = new_trainer.predict(test_dataset, **kwargs).predictions
         except ZeroDivisionError:
             logger.warning("Zero division error appeared in HuggingFace Transformers.")
             predictions = np.array([0] * len(test_dataset))
-
         post_y_pred, _ = postprocess_prediction_and_true(
             task=self._task,
-            y_pred=predictions.predictions,
+            y_pred=predictions,
             tokenizer=self.tokenizer,
             hf_args=self._training_args,
             X=X,
         )
         return post_y_pred
 
     def config2params(self, config: dict) -> dict:
```

### Comparing `FLAML-1.2.1/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-1.2.2/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-1.2.2/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-1.2.2/flaml/automl/nlp/huggingface/training_args.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/nlp/huggingface/utils.py` & `FLAML-1.2.2/flaml/automl/nlp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/nlp/utils.py` & `FLAML-1.2.2/flaml/automl/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/spark/configs.py` & `FLAML-1.2.2/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/spark/metrics.py` & `FLAML-1.2.2/flaml/automl/spark/metrics.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/spark/utils.py` & `FLAML-1.2.2/flaml/automl/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/state.py` & `FLAML-1.2.2/flaml/automl/state.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/task/generic_task.py` & `FLAML-1.2.2/flaml/automl/task/generic_task.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/task/task.py` & `FLAML-1.2.2/flaml/automl/task/task.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/training_log.py` & `FLAML-1.2.2/flaml/automl/training_log.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/automl/utils.py` & `FLAML-1.2.2/flaml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/all/binary.json` & `FLAML-1.2.2/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/all/multiclass.json` & `FLAML-1.2.2/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/all/regression.json` & `FLAML-1.2.2/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/estimator.py` & `FLAML-1.2.2/flaml/default/estimator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/extra_tree/binary.json` & `FLAML-1.2.2/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/extra_tree/multiclass.json` & `FLAML-1.2.2/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/extra_tree/regression.json` & `FLAML-1.2.2/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/greedy.py` & `FLAML-1.2.2/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/lgbm/binary.json` & `FLAML-1.2.2/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/lgbm/multiclass.json` & `FLAML-1.2.2/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/lgbm/regression.json` & `FLAML-1.2.2/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/portfolio.py` & `FLAML-1.2.2/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/regret.py` & `FLAML-1.2.2/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/rf/binary.json` & `FLAML-1.2.2/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/rf/multiclass.json` & `FLAML-1.2.2/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/rf/regression.json` & `FLAML-1.2.2/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/suggest.py` & `FLAML-1.2.2/flaml/default/suggest.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/xgb_limitdepth/binary.json` & `FLAML-1.2.2/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-1.2.2/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/xgb_limitdepth/regression.json` & `FLAML-1.2.2/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/xgboost/binary.json` & `FLAML-1.2.2/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/xgboost/multiclass.json` & `FLAML-1.2.2/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/default/xgboost/regression.json` & `FLAML-1.2.2/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/onlineml/autovw.py` & `FLAML-1.2.2/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/onlineml/trial.py` & `FLAML-1.2.2/flaml/onlineml/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/onlineml/trial_runner.py` & `FLAML-1.2.2/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/__init__.py` & `FLAML-1.2.2/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/analysis.py` & `FLAML-1.2.2/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/result.py` & `FLAML-1.2.2/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/sample.py` & `FLAML-1.2.2/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/scheduler/online_scheduler.py` & `FLAML-1.2.2/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-1.2.2/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/blendsearch.py` & `FLAML-1.2.2/flaml/tune/searcher/blendsearch.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/cfo_cat.py` & `FLAML-1.2.2/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/flow2.py` & `FLAML-1.2.2/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/online_searcher.py` & `FLAML-1.2.2/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/search_thread.py` & `FLAML-1.2.2/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/suggestion.py` & `FLAML-1.2.2/flaml/tune/searcher/suggestion.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/searcher/variant_generator.py` & `FLAML-1.2.2/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/space.py` & `FLAML-1.2.2/flaml/tune/space.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/spark/utils.py` & `FLAML-1.2.2/flaml/tune/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/trial.py` & `FLAML-1.2.2/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/trial_runner.py` & `FLAML-1.2.2/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/tune.py` & `FLAML-1.2.2/flaml/tune/tune.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/flaml/tune/utils.py` & `FLAML-1.2.2/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/setup.py` & `FLAML-1.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,15 +116,16 @@
             "holidays<0.14",  # to prevent installation error for prophet
             "prophet>=1.0.1",
             "statsmodels>=0.12.2",
             "hcrystalball==0.1.10",
             "pytorch-forecasting>=0.9.0",
         ],
         "benchmark": ["catboost>=0.26", "psutil==5.8.0", "xgboost==1.3.3"],
-        "openai": ["openai==0.27.4", "diskcache", "optuna==2.8.0"],
+        "openai": ["openai==0.27.4", "diskcache"],
+        "autogen": ["openai==0.27.4", "diskcache", "docker"],
         "synapse": ["joblibspark>=0.5.0", "optuna==2.8.0", "pyspark>=3.2.0"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `FLAML-1.2.1/test/test_autovw.py` & `FLAML-1.2.2/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/test/test_conda_distribution.py` & `FLAML-1.2.2/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/test/test_gpu.py` & `FLAML-1.2.2/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.1/test/test_model.py` & `FLAML-1.2.2/test/test_model.py`

 * *Files identical despite different names*

