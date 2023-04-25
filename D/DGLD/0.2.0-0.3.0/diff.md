# Comparing `tmp/DGLD-0.2.0.tar.gz` & `tmp/DGLD-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DGLD-0.2.0.tar", last modified: Tue Apr 25 01:26:20 2023, max compression
+gzip compressed data, was "DGLD-0.3.0.tar", last modified: Tue Apr 25 01:56:06 2023, max compression
```

## Comparing `DGLD-0.2.0.tar` & `DGLD-0.3.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.397150 DGLD-0.2.0/
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.385150 DGLD-0.2.0/DGLD/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/__init__.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.385150 DGLD-0.2.0/DGLD/models/
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.385150 DGLD-0.2.0/DGLD/models/AAGNN/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6840 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AAGNN/AAGNN_batch.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1697 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AAGNN/AAGNN_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       87 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AAGNN/__init__.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.385150 DGLD-0.2.0/DGLD/models/ALARM/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       76 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ALARM/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3772 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ALARM/alarm_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    11141 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ALARM/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.385150 DGLD-0.2.0/DGLD/models/ANEMONE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       79 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ANEMONE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6139 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ANEMONE/anemone_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3533 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ANEMONE/dataset.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    14438 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ANEMONE/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.389150 DGLD-0.2.0/DGLD/models/AdONE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AdONE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    13393 2023-04-24 10:25:49.000000 DGLD-0.2.0/DGLD/models/AdONE/adone_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    10378 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AdONE/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.389150 DGLD-0.2.0/DGLD/models/AnomalyDAE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       85 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AnomalyDAE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     4022 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AnomalyDAE/anomalydae_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    13403 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/AnomalyDAE/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.389150 DGLD-0.2.0/DGLD/models/CONAD/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/CONAD/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9671 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/CONAD/conad_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    15975 2023-04-24 10:25:52.000000 DGLD-0.2.0/DGLD/models/CONAD/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.389150 DGLD-0.2.0/DGLD/models/CoLA/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       70 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/CoLA/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6089 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/CoLA/colautils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3559 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/CoLA/dataset.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    13773 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/CoLA/model.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.389150 DGLD-0.2.0/DGLD/models/ComGA/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ComGA/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     5121 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ComGA/comga_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    15081 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ComGA/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/DOMINANT/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       81 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/DOMINANT/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3461 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/DOMINANT/dominant_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     8588 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/DOMINANT/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/DONE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       73 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/DONE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9542 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/DONE/done_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     8902 2023-04-24 10:25:54.000000 DGLD-0.2.0/DGLD/models/DONE/models.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/GAAN/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       71 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GAAN/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     2365 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GAAN/gaan_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    14682 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GAAN/model.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/GCNAE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       74 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GCNAE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1566 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GCNAE/gcnae_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    10161 2023-04-24 10:25:56.000000 DGLD-0.2.0/DGLD/models/GCNAE/model.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/GUIDE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       73 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GUIDE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6840 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GUIDE/guide_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    16003 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/GUIDE/model.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/MLPAE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       74 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/MLPAE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1567 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/MLPAE/mlpae_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9490 2023-04-24 10:25:59.000000 DGLD-0.2.0/DGLD/models/MLPAE/model.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/ONE/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       70 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ONE/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     8344 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ONE/model.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1933 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/ONE/one_utils.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.393150 DGLD-0.2.0/DGLD/models/SCAN/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       72 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/SCAN/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     4738 2023-04-24 10:26:02.000000 DGLD-0.2.0/DGLD/models/SCAN/model.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      790 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/SCAN/scan_utils.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.397150 DGLD-0.2.0/DGLD/models/SLGAD/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9117 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/SLGAD/SL_GAD_utils.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/SLGAD/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    12520 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/SLGAD/dataset.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    26118 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/SLGAD/model.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      564 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/models/__init__.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.397150 DGLD-0.2.0/DGLD/modules/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/__init__.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.397150 DGLD-0.2.0/DGLD/modules/dglAug/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       57 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/dglAug/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     2773 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/dglAug/augs.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.397150 DGLD-0.2.0/DGLD/modules/dglAug/transforms/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      511 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/dglAug/transforms/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1591 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/dglAug/transforms/feature_dropout.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1099 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/dglAug/transforms/node_shuffle.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1714 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/modules/dglAug/transforms/random_mask.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.397150 DGLD-0.2.0/DGLD/utils/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        4 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/__init__.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6573 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/argparser.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    14585 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/common.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      736 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/common_params.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    15913 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/dataset.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3823 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/early_stopping.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1684 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/evaluation.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3114 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/inject_anomalies.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9233 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/load_data.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3518 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/log.py
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    17203 2023-04-24 10:24:41.000000 DGLD-0.2.0/DGLD/utils/sample.py
-drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:26:20.385150 DGLD-0.2.0/DGLD.egg-info/
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      235 2023-04-25 01:26:20.000000 DGLD-0.2.0/DGLD.egg-info/PKG-INFO
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     2346 2023-04-25 01:26:20.000000 DGLD-0.2.0/DGLD.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        1 2023-04-25 01:26:20.000000 DGLD-0.2.0/DGLD.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        5 2023-04-25 01:26:20.000000 DGLD-0.2.0/DGLD.egg-info/top_level.txt
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      235 2023-04-25 01:26:20.397150 DGLD-0.2.0/PKG-INFO
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       38 2023-04-25 01:26:20.397150 DGLD-0.2.0/setup.cfg
--rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      560 2023-04-24 11:49:25.000000 DGLD-0.2.0/setup.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.048478 DGLD-0.3.0/
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.036478 DGLD-0.3.0/DGLD/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/__init__.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.036478 DGLD-0.3.0/DGLD/models/
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/AAGNN/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6840 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AAGNN/AAGNN_batch.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1697 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AAGNN/AAGNN_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       87 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AAGNN/__init__.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/ALARM/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       76 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ALARM/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3772 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ALARM/alarm_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    11141 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ALARM/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/ANEMONE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       79 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ANEMONE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6139 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ANEMONE/anemone_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3533 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ANEMONE/dataset.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    14438 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ANEMONE/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/AdONE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AdONE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    13393 2023-04-24 10:25:49.000000 DGLD-0.3.0/DGLD/models/AdONE/adone_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    10378 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AdONE/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/AnomalyDAE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       85 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AnomalyDAE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     4022 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AnomalyDAE/anomalydae_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    13403 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/AnomalyDAE/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/CONAD/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/CONAD/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9671 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/CONAD/conad_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    15975 2023-04-24 10:25:52.000000 DGLD-0.3.0/DGLD/models/CONAD/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/CoLA/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       70 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/CoLA/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6089 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/CoLA/colautils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3559 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/CoLA/dataset.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    13773 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/CoLA/model.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/ComGA/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ComGA/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     5121 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ComGA/comga_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    15081 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ComGA/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/DOMINANT/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       81 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/DOMINANT/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3461 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/DOMINANT/dominant_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     8588 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/DOMINANT/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.040478 DGLD-0.3.0/DGLD/models/DONE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       73 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/DONE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9542 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/DONE/done_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     8902 2023-04-24 10:25:54.000000 DGLD-0.3.0/DGLD/models/DONE/models.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/GAAN/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       71 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GAAN/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     2365 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GAAN/gaan_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    14682 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GAAN/model.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/GCNAE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       74 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GCNAE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1566 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GCNAE/gcnae_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    10161 2023-04-24 10:25:56.000000 DGLD-0.3.0/DGLD/models/GCNAE/model.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/GUIDE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       73 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GUIDE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6840 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GUIDE/guide_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    16003 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/GUIDE/model.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/MLPAE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       74 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/MLPAE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1567 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/MLPAE/mlpae_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9490 2023-04-24 10:25:59.000000 DGLD-0.3.0/DGLD/models/MLPAE/model.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/ONE/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       70 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ONE/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     8344 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ONE/model.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1933 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/ONE/one_utils.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/SCAN/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       72 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/SCAN/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     4738 2023-04-24 10:26:02.000000 DGLD-0.3.0/DGLD/models/SCAN/model.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      790 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/SCAN/scan_utils.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/models/SLGAD/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9117 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/SLGAD/SL_GAD_utils.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       75 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/SLGAD/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    12520 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/SLGAD/dataset.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    26118 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/SLGAD/model.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      564 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/models/__init__.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/modules/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/__init__.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/modules/dglAug/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       57 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/dglAug/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     2773 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/dglAug/augs.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.044478 DGLD-0.3.0/DGLD/modules/dglAug/transforms/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      511 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/dglAug/transforms/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1591 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/dglAug/transforms/feature_dropout.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1099 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/dglAug/transforms/node_shuffle.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1714 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/modules/dglAug/transforms/random_mask.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.048478 DGLD-0.3.0/DGLD/utils/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        4 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/__init__.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     6573 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/argparser.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    14585 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/common.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      736 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/common_params.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    15913 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/dataset.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3823 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/early_stopping.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     1684 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/evaluation.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3114 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/inject_anomalies.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     9233 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/load_data.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     3518 2023-04-24 10:24:41.000000 DGLD-0.3.0/DGLD/utils/log.py
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)    17204 2023-04-25 01:39:52.000000 DGLD-0.3.0/DGLD/utils/sample.py
+drwxrwxr-x   0 xuyilun   (1013) xuyilun   (1013)        0 2023-04-25 01:56:06.036478 DGLD-0.3.0/DGLD.egg-info/
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      235 2023-04-25 01:56:05.000000 DGLD-0.3.0/DGLD.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)     2346 2023-04-25 01:56:06.000000 DGLD-0.3.0/DGLD.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        1 2023-04-25 01:56:05.000000 DGLD-0.3.0/DGLD.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)        5 2023-04-25 01:56:05.000000 DGLD-0.3.0/DGLD.egg-info/top_level.txt
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      235 2023-04-25 01:56:06.048478 DGLD-0.3.0/PKG-INFO
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)       38 2023-04-25 01:56:06.048478 DGLD-0.3.0/setup.cfg
+-rw-rw-r--   0 xuyilun   (1013) xuyilun   (1013)      560 2023-04-25 01:55:48.000000 DGLD-0.3.0/setup.py
```

### Comparing `DGLD-0.2.0/DGLD/models/AAGNN/AAGNN_batch.py` & `DGLD-0.3.0/DGLD/models/AAGNN/AAGNN_batch.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/AAGNN/AAGNN_utils.py` & `DGLD-0.3.0/DGLD/models/AAGNN/AAGNN_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ALARM/alarm_utils.py` & `DGLD-0.3.0/DGLD/models/ALARM/alarm_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ALARM/models.py` & `DGLD-0.3.0/DGLD/models/ALARM/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ANEMONE/anemone_utils.py` & `DGLD-0.3.0/DGLD/models/ANEMONE/anemone_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ANEMONE/dataset.py` & `DGLD-0.3.0/DGLD/models/ANEMONE/dataset.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ANEMONE/models.py` & `DGLD-0.3.0/DGLD/models/ANEMONE/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/AdONE/adone_utils.py` & `DGLD-0.3.0/DGLD/models/AdONE/adone_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/AdONE/models.py` & `DGLD-0.3.0/DGLD/models/AdONE/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/AnomalyDAE/anomalydae_utils.py` & `DGLD-0.3.0/DGLD/models/AnomalyDAE/anomalydae_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/AnomalyDAE/models.py` & `DGLD-0.3.0/DGLD/models/AnomalyDAE/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/CONAD/conad_utils.py` & `DGLD-0.3.0/DGLD/models/CONAD/conad_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/CONAD/models.py` & `DGLD-0.3.0/DGLD/models/CONAD/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/CoLA/colautils.py` & `DGLD-0.3.0/DGLD/models/CoLA/colautils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/CoLA/dataset.py` & `DGLD-0.3.0/DGLD/models/CoLA/dataset.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/CoLA/model.py` & `DGLD-0.3.0/DGLD/models/CoLA/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ComGA/comga_utils.py` & `DGLD-0.3.0/DGLD/models/ComGA/comga_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ComGA/models.py` & `DGLD-0.3.0/DGLD/models/ComGA/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/DOMINANT/dominant_utils.py` & `DGLD-0.3.0/DGLD/models/DOMINANT/dominant_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/DOMINANT/models.py` & `DGLD-0.3.0/DGLD/models/DOMINANT/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/DONE/done_utils.py` & `DGLD-0.3.0/DGLD/models/DONE/done_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/DONE/models.py` & `DGLD-0.3.0/DGLD/models/DONE/models.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/GAAN/gaan_utils.py` & `DGLD-0.3.0/DGLD/models/GAAN/gaan_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/GAAN/model.py` & `DGLD-0.3.0/DGLD/models/GAAN/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/GCNAE/gcnae_utils.py` & `DGLD-0.3.0/DGLD/models/GCNAE/gcnae_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/GCNAE/model.py` & `DGLD-0.3.0/DGLD/models/GCNAE/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/GUIDE/guide_utils.py` & `DGLD-0.3.0/DGLD/models/GUIDE/guide_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/GUIDE/model.py` & `DGLD-0.3.0/DGLD/models/GUIDE/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/MLPAE/mlpae_utils.py` & `DGLD-0.3.0/DGLD/models/MLPAE/mlpae_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/MLPAE/model.py` & `DGLD-0.3.0/DGLD/models/MLPAE/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ONE/model.py` & `DGLD-0.3.0/DGLD/models/ONE/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/ONE/one_utils.py` & `DGLD-0.3.0/DGLD/models/ONE/one_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/SCAN/model.py` & `DGLD-0.3.0/DGLD/models/SCAN/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/SCAN/scan_utils.py` & `DGLD-0.3.0/DGLD/models/SCAN/scan_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/SLGAD/SL_GAD_utils.py` & `DGLD-0.3.0/DGLD/models/SLGAD/SL_GAD_utils.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/SLGAD/dataset.py` & `DGLD-0.3.0/DGLD/models/SLGAD/dataset.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/SLGAD/model.py` & `DGLD-0.3.0/DGLD/models/SLGAD/model.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/models/__init__.py` & `DGLD-0.3.0/DGLD/models/__init__.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/modules/dglAug/augs.py` & `DGLD-0.3.0/DGLD/modules/dglAug/augs.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/modules/dglAug/transforms/feature_dropout.py` & `DGLD-0.3.0/DGLD/modules/dglAug/transforms/feature_dropout.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/modules/dglAug/transforms/node_shuffle.py` & `DGLD-0.3.0/DGLD/modules/dglAug/transforms/node_shuffle.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/modules/dglAug/transforms/random_mask.py` & `DGLD-0.3.0/DGLD/modules/dglAug/transforms/random_mask.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/argparser.py` & `DGLD-0.3.0/DGLD/utils/argparser.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/common.py` & `DGLD-0.3.0/DGLD/utils/common.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/common_params.py` & `DGLD-0.3.0/DGLD/utils/common_params.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/dataset.py` & `DGLD-0.3.0/DGLD/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/early_stopping.py` & `DGLD-0.3.0/DGLD/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/evaluation.py` & `DGLD-0.3.0/DGLD/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/inject_anomalies.py` & `DGLD-0.3.0/DGLD/utils/inject_anomalies.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/load_data.py` & `DGLD-0.3.0/DGLD/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/log.py` & `DGLD-0.3.0/DGLD/utils/log.py`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/DGLD/utils/sample.py` & `DGLD-0.3.0/DGLD/utils/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         rwl: List[List]
             the list of subgraph generated
         """
         # newg = dgl.remove_self_loop(g)
         # newg = dgl.add_self_loop(newg)
         # length is Very influential to the effect of the model, maybe caused "remote" neighbor is
         # not "friendly" to Rebuild Properties.
-        paces = dgl.sampling.random_walk(g, start_nodes, length=self.length * 3, restart_prob=0)[0]
+        paces = dgl.sampling.random_walk(g, start_nodes, length=self.length * 3, restart_prob=0.)[0]
         rwl = []
         for start, pace in zip(start_nodes, paces):
             pace = pace.unique().numpy()
             np.random.shuffle(pace)
             pace = pace[: self.length].tolist()
             pace = move_start_node_fisrt(pace, start)
             pace += [pace[0]] * max(0, self.length - len(pace))
```

### Comparing `DGLD-0.2.0/DGLD.egg-info/SOURCES.txt` & `DGLD-0.3.0/DGLD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DGLD-0.2.0/setup.py` & `DGLD-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
 setup(name='DGLD', #注意一定不要和pypi官网上之前出现过的模块名重复，不然报错
-      version='0.2.0',
+      version='0.3.0',
       description='A Deep Graph Anomaly Detection Library based on DGL',
       author='miziha-zp;zhoushengisnoob;GavinYGM;fmc123653;cfuser;Xinstein-rx',
       author_email='arlenjing@gmail.com', #这里务必填写正确的email格式
       packages=find_packages(),  # 表示你要封装的包，find_packages用于系统自动从当前目录开始找包
       license="apache 3.0"
       )
```

