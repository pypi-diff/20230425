# Comparing `tmp/biopsykit-0.8.1.tar.gz` & `tmp/biopsykit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biopsykit-0.8.1.tar", max compression
+gzip compressed data, was "biopsykit-0.9.0.tar", max compression
```

## Comparing `biopsykit-0.8.1.tar` & `biopsykit-0.9.0.tar`

### file list

```diff
@@ -1,102 +1,96 @@
--rw-r--r--   0        0        0     1166 2023-04-04 21:04:43.747661 biopsykit-0.8.1/LICENSE
--rw-r--r--   0        0        0    14361 2023-04-04 21:04:43.747661 biopsykit-0.8.1/README.md
--rw-r--r--   0        0        0     3339 2023-04-04 21:04:44.291669 biopsykit-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1893 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/__init__.py
--rw-r--r--   0        0        0      414 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/carwatch_logs/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/carwatch_logs/log_actions.py
--rw-r--r--   0        0        0    17104 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/carwatch_logs/log_data.py
--rw-r--r--   0        0        0      849 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/carwatch_logs/log_extras.py
--rw-r--r--   0        0        0     7640 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/carwatch_logs/log_statistics.py
--rw-r--r--   0        0        0     6983 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/carwatch_logs/widgets.py
--rw-r--r--   0        0        0      186 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/__init__.py
--rw-r--r--   0        0        0      408 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/analysis/__init__.py
--rw-r--r--   0        0        0    12555 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/analysis/_analysis.py
--rw-r--r--   0        0        0      174 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/metrics/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/metrics/_metrics.py
--rw-r--r--   0        0        0      343 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/model_selection/__init__.py
--rw-r--r--   0        0        0     9393 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/model_selection/nested_cv.py
--rw-r--r--   0        0        0    38929 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/model_selection/sklearn_pipeline_permuter.py
--rw-r--r--   0        0        0     7731 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/classification/utils.py
--rw-r--r--   0        0        0    21392 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/example_data.py
--rw-r--r--   0        0        0      894 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/__init__.py
--rw-r--r--   0        0        0    10135 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/biopac.py
--rw-r--r--   0        0        0    10777 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/carwatch_logs.py
--rw-r--r--   0        0        0    15695 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/ecg.py
--rw-r--r--   0        0        0     5639 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/eeg.py
--rw-r--r--   0        0        0    32199 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/io.py
--rw-r--r--   0        0        0    21241 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/nilspod.py
--rw-r--r--   0        0        0    11285 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/psg.py
--rw-r--r--   0        0        0    16122 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/saliva.py
--rw-r--r--   0        0        0     1387 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/sleep.py
--rw-r--r--   0        0        0    14480 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/io/sleep_analyzer.py
--rw-r--r--   0        0        0      168 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/metadata/__init__.py
--rw-r--r--   0        0        0     5862 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/metadata/metadata.py
--rw-r--r--   0        0        0      343 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/plotting/__init__.py
--rw-r--r--   0        0        0    29267 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/plotting/plotting.py
--rw-r--r--   0        0        0      399 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/protocols/__init__.py
--rw-r--r--   0        0        0     2765 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/protocols/_utils.py
--rw-r--r--   0        0        0    64732 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/protocols/base.py
--rw-r--r--   0        0        0     2824 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/protocols/car.py
--rw-r--r--   0        0        0    37634 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/protocols/cft.py
--rw-r--r--   0        0        0     6466 2023-04-04 21:04:44.291669 biopsykit-0.8.1/src/biopsykit/protocols/mist.py
--rw-r--r--   0        0        0    45401 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/protocols/plotting.py
--rw-r--r--   0        0        0     4061 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/protocols/tsst.py
--rw-r--r--   0        0        0     1868 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/questionnaires/__init__.py
--rw-r--r--   0        0        0   230208 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/questionnaires/questionnaires.py
--rw-r--r--   0        0        0    28249 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/questionnaires/utils.py
--rw-r--r--   0        0        0      377 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/saliva/__init__.py
--rw-r--r--   0        0        0    26176 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/saliva/saliva.py
--rw-r--r--   0        0        0    16615 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/saliva/utils.py
--rw-r--r--   0        0        0      148 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/__init__.py
--rw-r--r--   0        0        0     1735 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/_base.py
--rw-r--r--   0        0        0      188 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/ecg/__init__.py
--rw-r--r--   0        0        0    67983 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/ecg/ecg.py
--rw-r--r--   0        0        0    33242 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/ecg/plotting.py
--rw-r--r--   0        0        0      133 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/eeg/__init__.py
--rw-r--r--   0        0        0     5189 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/eeg/eeg.py
--rw-r--r--   0        0        0      504 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/__init__.py
--rw-r--r--   0        0        0     5948 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/activity_counts.py
--rw-r--r--   0        0        0      193 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/feature_extraction/__init__.py
--rw-r--r--   0        0        0     6044 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/feature_extraction/static_moments.py
--rw-r--r--   0        0        0     6233 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/imu.py
--rw-r--r--   0        0        0     5678 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/rest_periods.py
--rw-r--r--   0        0        0    12299 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/static_moment_detection.py
--rw-r--r--   0        0        0     7282 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/imu/wear_detection.py
--rw-r--r--   0        0        0      141 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/rsp/__init__.py
--rw-r--r--   0        0        0     6732 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/signals/rsp/rsp.py
--rw-r--r--   0        0        0      344 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/__init__.py
--rw-r--r--   0        0        0    14323 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/plotting.py
--rw-r--r--   0        0        0       73 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/psg/__init__.py
--rw-r--r--   0        0        0      275 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_endpoints/__init__.py
--rw-r--r--   0        0        0     7362 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_endpoints/sleep_endpoints.py
--rw-r--r--   0        0        0      301 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_processing_pipeline/__init__.py
--rw-r--r--   0        0        0     5617 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_processing_pipeline/sleep_processing_pipeline.py
--rw-r--r--   0        0        0      287 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/__init__.py
--rw-r--r--   0        0        0      178 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/_base.py
--rw-r--r--   0        0        0     4819 2023-04-04 21:04:44.295669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke.py
--rw-r--r--   0        0        0     3897 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke_old.py
--rw-r--r--   0        0        0     3678 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/sadeh.py
--rw-r--r--   0        0        0     3635 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/sazonov.py
--rw-r--r--   0        0        0     4695 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/scripps_clinic.py
--rw-r--r--   0        0        0     4196 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/webster.py
--rw-r--r--   0        0        0     3415 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/sleep_wake_detection.py
--rw-r--r--   0        0        0     3552 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/utils.py
--rw-r--r--   0        0        0     2837 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/sleep/utils.py
--rw-r--r--   0        0        0      176 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/stats/__init__.py
--rw-r--r--   0        0        0      970 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/stats/multicoll.py
--rw-r--r--   0        0        0     1891 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/stats/regression.py
--rw-r--r--   0        0        0    57248 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/stats/stats.py
--rw-r--r--   0        0        0      491 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/__init__.py
--rw-r--r--   0        0        0    23062 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0      578 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/_types.py
--rw-r--r--   0        0        0    22228 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/array_handling.py
--rw-r--r--   0        0        0    28841 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/data_processing.py
--rw-r--r--   0        0        0    15651 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/dataframe_handling.py
--rw-r--r--   0        0        0    54944 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/datatype_helper.py
--rw-r--r--   0        0        0      882 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/exceptions.py
--rw-r--r--   0        0        0     5338 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/file_handling.py
--rw-r--r--   0        0        0      900 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/functions.py
--rw-r--r--   0        0        0     1521 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/legacy_helper.py
--rw-r--r--   0        0        0     5022 2023-04-04 21:04:44.299669 biopsykit-0.8.1/src/biopsykit/utils/time.py
--rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 biopsykit-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-25 09:23:42.744886 biopsykit-0.9.0/LICENSE
+-rw-r--r--   0        0        0    14361 2023-04-25 09:23:42.744886 biopsykit-0.9.0/README.md
+-rw-r--r--   0        0        0     3332 2023-04-25 09:23:43.281129 biopsykit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1323 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/__init__.py
+-rw-r--r--   0        0        0      408 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/analysis/__init__.py
+-rw-r--r--   0        0        0    12569 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/analysis/_analysis.py
+-rw-r--r--   0        0        0      174 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/metrics/__init__.py
+-rw-r--r--   0        0        0     2238 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/metrics/_metrics.py
+-rw-r--r--   0        0        0      343 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/model_selection/__init__.py
+-rw-r--r--   0        0        0     9384 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/model_selection/nested_cv.py
+-rw-r--r--   0        0        0    39705 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/model_selection/sklearn_pipeline_permuter.py
+-rw-r--r--   0        0        0     7692 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/classification/utils.py
+-rw-r--r--   0        0        0    18554 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/example_data.py
+-rw-r--r--   0        0        0      894 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/io/__init__.py
+-rw-r--r--   0        0        0    10131 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/io/biopac.py
+-rw-r--r--   0        0        0    10717 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/io/carwatch_logs.py
+-rw-r--r--   0        0        0    15502 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/io/ecg.py
+-rw-r--r--   0        0        0     5638 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/io/eeg.py
+-rw-r--r--   0        0        0    32206 2023-04-25 09:23:43.281129 biopsykit-0.9.0/src/biopsykit/io/io.py
+-rw-r--r--   0        0        0    21160 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/io/nilspod.py
+-rw-r--r--   0        0        0    11275 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/io/psg.py
+-rw-r--r--   0        0        0    16089 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/io/saliva.py
+-rw-r--r--   0        0        0     1386 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/io/sleep.py
+-rw-r--r--   0        0        0    14017 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/io/sleep_analyzer.py
+-rw-r--r--   0        0        0      168 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/metadata/__init__.py
+-rw-r--r--   0        0        0     5861 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/metadata/metadata.py
+-rw-r--r--   0        0        0      343 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/plotting/__init__.py
+-rw-r--r--   0        0        0    29145 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/plotting/plotting.py
+-rw-r--r--   0        0        0      399 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/__init__.py
+-rw-r--r--   0        0        0     2764 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/_utils.py
+-rw-r--r--   0        0        0    64731 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/base.py
+-rw-r--r--   0        0        0     2823 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/car.py
+-rw-r--r--   0        0        0    37578 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/cft.py
+-rw-r--r--   0        0        0     6463 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/mist.py
+-rw-r--r--   0        0        0    45300 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/plotting.py
+-rw-r--r--   0        0        0     4057 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/protocols/tsst.py
+-rw-r--r--   0        0        0     1868 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/questionnaires/__init__.py
+-rw-r--r--   0        0        0   229540 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/questionnaires/questionnaires.py
+-rw-r--r--   0        0        0    28254 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/questionnaires/utils.py
+-rw-r--r--   0        0        0      377 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/saliva/__init__.py
+-rw-r--r--   0        0        0    26125 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/saliva/saliva.py
+-rw-r--r--   0        0        0    16579 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/saliva/utils.py
+-rw-r--r--   0        0        0      148 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/__init__.py
+-rw-r--r--   0        0        0     1734 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/_base.py
+-rw-r--r--   0        0        0      188 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/ecg/__init__.py
+-rw-r--r--   0        0        0    67811 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/ecg/ecg.py
+-rw-r--r--   0        0        0    33160 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/ecg/plotting.py
+-rw-r--r--   0        0        0      133 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/eeg/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/eeg/eeg.py
+-rw-r--r--   0        0        0      504 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/__init__.py
+-rw-r--r--   0        0        0     5945 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/activity_counts.py
+-rw-r--r--   0        0        0      193 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/feature_extraction/__init__.py
+-rw-r--r--   0        0        0     5995 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/feature_extraction/static_moments.py
+-rw-r--r--   0        0        0     6232 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/imu.py
+-rw-r--r--   0        0        0     5634 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/rest_periods.py
+-rw-r--r--   0        0        0    12225 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/static_moment_detection.py
+-rw-r--r--   0        0        0     7846 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/imu/wear_detection.py
+-rw-r--r--   0        0        0      141 2023-04-25 09:23:43.285129 biopsykit-0.9.0/src/biopsykit/signals/rsp/__init__.py
+-rw-r--r--   0        0        0     6729 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/signals/rsp/rsp.py
+-rw-r--r--   0        0        0      344 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/__init__.py
+-rw-r--r--   0        0        0    14249 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/plotting.py
+-rw-r--r--   0        0        0       73 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/psg/__init__.py
+-rw-r--r--   0        0        0      275 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_endpoints/__init__.py
+-rw-r--r--   0        0        0     7394 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_endpoints/sleep_endpoints.py
+-rw-r--r--   0        0        0      301 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_processing_pipeline/__init__.py
+-rw-r--r--   0        0        0     5616 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_processing_pipeline/sleep_processing_pipeline.py
+-rw-r--r--   0        0        0      287 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/__init__.py
+-rw-r--r--   0        0        0      178 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/_base.py
+-rw-r--r--   0        0        0     4832 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke.py
+-rw-r--r--   0        0        0     3926 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke_old.py
+-rw-r--r--   0        0        0     3693 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/sadeh.py
+-rw-r--r--   0        0        0     3650 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/sazonov.py
+-rw-r--r--   0        0        0     4710 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/scripps_clinic.py
+-rw-r--r--   0        0        0     4211 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/webster.py
+-rw-r--r--   0        0        0     3403 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/sleep_wake_detection.py
+-rw-r--r--   0        0        0     3423 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/utils.py
+-rw-r--r--   0        0        0     2836 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/sleep/utils.py
+-rw-r--r--   0        0        0      176 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/stats/__init__.py
+-rw-r--r--   0        0        0      970 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/stats/multicoll.py
+-rw-r--r--   0        0        0     1891 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/stats/regression.py
+-rw-r--r--   0        0        0    56911 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/stats/stats.py
+-rw-r--r--   0        0        0      491 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/__init__.py
+-rw-r--r--   0        0        0    22823 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0      578 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/_types.py
+-rw-r--r--   0        0        0    22045 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/array_handling.py
+-rw-r--r--   0        0        0    28628 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/data_processing.py
+-rw-r--r--   0        0        0    15659 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/dataframe_handling.py
+-rw-r--r--   0        0        0    54935 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/datatype_helper.py
+-rw-r--r--   0        0        0      882 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/exceptions.py
+-rw-r--r--   0        0        0     5337 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/file_handling.py
+-rw-r--r--   0        0        0      900 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/functions.py
+-rw-r--r--   0        0        0     1521 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/legacy_helper.py
+-rw-r--r--   0        0        0     5021 2023-04-25 09:23:43.289129 biopsykit-0.9.0/src/biopsykit/utils/time.py
+-rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 biopsykit-0.9.0/PKG-INFO
```

### Comparing `biopsykit-0.8.1/LICENSE` & `biopsykit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/README.md` & `biopsykit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/pyproject.toml` & `biopsykit-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biopsykit"
-version = "0.8.1"
+version = "0.9.0"
 description = "A Python package for the analysis of biopsychological data."
 authors = [
     "Robert Richer <robert.richer@fau.de>",
     "Arne Küderle <arne.kuederle@fau.de>",
     "Rebecca Lennartz <rebecca.lennartz@fau.de>",
     "Daniel Krauß <daniel.k.krauss@fau.de>",
     "Victoria Müller <victoria.m.mueller@fau.de>",
@@ -42,36 +42,32 @@
 ipympl = {version = "^0.9", optional = true}
 
 [tool.poetry.extras]
 mne = ["mne"]
 jupyter = ["IPython", "ipympl", "ipywidgets"]
 
 [tool.poetry.dev-dependencies]
+black = { version="^22", extras=["jupyter", "d"] }
+poethepoet = "^0.10.0"
 pytest = "^6"
 pytest-cov = "^2"
-prospector = "^1"
-black = { version="^22", extras=["jupyter", "d"] }
-coverage = "^4"
 ipykernel = "^6"
-mypy = "^0.790"
-pytest-xdist = "^2.2.0"
+ruff = "^0.0.261"
 # Doc dependencies. They also need to be updated in ./docs/requirements.txt
 sphinx = "^4"
 numpydoc = "^1"
 sphinx-gallery = "^0.10.0"
 sphinx_issues = "^1.2.0"
 pydata-sphinx-theme = "^0.6.2"
 recommonmark = "^0.6.0"
 toml = "^0.10.1"
 memory_profiler = "^0.57.0"
 coverage-badge = "^1.0.1"
-isort = "^5"
 sphinx-copybutton = "^0.4.0"
 nbsphinx = "^0.8.7"
-poethepoet = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -99,22 +95,20 @@
 profile = "black"
 multi_line_output = 3
 line_length = 120
 skip_gitignore = true
 
 
 [tool.poe.tasks]
-_black = "black ."
-_black_check = "black . --check"
-_isort = "isort **/*.py"
-_isort_check = "isort **/*.py --check-only"
-
-# Reformat all files using black and sort import
+_format_black = "black ."
+_format_ruff = "ruff . --fix-only"
+format = { sequence = ["_format_black", "_format_ruff"], help = "Format all files." }
+lint = { cmd = "ruff src --fix", help = "Lint all files with ruff." }
+_lint_ci = "ruff src --format=github"
+_check_black = "black . --check"
+ci_check = { sequence = ["_check_black", "_lint_ci"], help = "Check all potential format and linting issues." }
+test = {cmd = "pytest --cov=biopsykit -cov-report=term-missing --cov-report=xml", help = "Run Pytest with coverage." }
 docs = {"script" = "_tasks:task_docs"}
-format = { sequence = ["_black", "_isort"], help = "Format all files." }
-format_check = ["_black_check", "_isort_check"]
-lint = {cmd = "prospector", help = "Lint all files with Prospector." }
-test = {cmd = "pytest --cov=biopsykit --cov-report=xml", help = "Run Pytest with coverage." }
 update_version = {"script" = "_tasks:task_update_version"}
 register_ipykernel = { cmd = "python -m ipykernel install --user --name biopsykit --display-name biopsykit", help = "Add a new jupyter kernel for the project." }
 remove_ipykernel = { cmd = "jupyter kernelspec uninstall biopsykit", help = "Remove the project specific jupyter kernel."}
 default = {sequence = ["format", "lint", "test"], help = "Run the default pipeline, consisting of formatting, linting, and testing."}
```

### Comparing `biopsykit-0.8.1/src/biopsykit/classification/analysis/_analysis.py` & `biopsykit-0.9.0/src/biopsykit/classification/analysis/_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Functions to analyze classification results."""
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
+from biopsykit.classification.model_selection import SklearnPipelinePermuter
+from biopsykit.classification.utils import prepare_df_sklearn
 from fau_colors import cmaps
 from matplotlib import pyplot as plt
 from matplotlib.cm import register_cmap
 from matplotlib.colors import ListedColormap
 from sklearn.metrics import ConfusionMatrixDisplay
 
-from biopsykit.classification.model_selection import SklearnPipelinePermuter
-from biopsykit.classification.utils import prepare_df_sklearn
-
 pipeline_step_map = {
     "pipeline_scaler": "Scaler",
     "pipeline_reduce_dim": r"\makecell[lc]{Feature\\ Selection}",
     "pipeline_clf": "Classifier",
 }
 
 metric_map = {
@@ -132,18 +131,18 @@
 
     label_order = best_pipeline[0].classes_
 
     predict_proba_results = []
     predict_proba_labels = []
 
     for i, test_idx in enumerate(test_indices):
-        test_idx = list(test_idx)
+        test_idx_list = list(test_idx)
         pipeline_fold = best_pipeline[i]
-        predict_proba_results.append(pipeline_fold.predict_proba(x[test_idx]))
-        predict_proba_labels.append(y[test_idx])
+        predict_proba_results.append(pipeline_fold.predict_proba(x[test_idx_list]))
+        predict_proba_labels.append(y[test_idx_list])
 
     results_proba = pd.DataFrame(
         np.concatenate(predict_proba_results),
         columns=label_order,
         index=data.index[test_indices_flat],
     )
     if column_names is not None:
```

### Comparing `biopsykit-0.8.1/src/biopsykit/classification/metrics/_metrics.py` & `biopsykit-0.9.0/src/biopsykit/classification/metrics/_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Metrics for classification tasks."""
 from inspect import getmembers
 
 import numpy as np
 import pandas as pd
 import sklearn.metrics
-
 from biopsykit.utils._types import str_t
 
 
 def _apply_score(row: pd.Series, score_func, pos_label: str):
     true_labels_folds = row[0]
     predicted_labels_folds = row[1]
     scores = [
@@ -40,23 +39,23 @@
 
     for metric in metrics:
         score_funcs = dict(getmembers(sklearn.metrics))
         if metric in score_funcs:
             score_func = score_funcs[f"{metric}"]
         elif f"{metric}_score" in score_funcs:
             score_func = score_funcs[f"{metric}_score"]
-            metric = f"{metric}_score"
+            metric = f"{metric}_score"  # noqa: PLW2901
         else:
             raise ValueError(f"Metric '{metric}' not found.")
         metric_out[metric] = metric_slice.apply(_apply_score, args=(score_func, pos_label), axis=1)
     metric_out = pd.concat(metric_out, names=["score", "folds"], axis=1)
 
     metric_out = metric_out.stack(["score", "folds"])
     metric_out = metric_out.groupby(metric_out.index.names[:-1]).agg(
-        [("mean", lambda x: np.mean), ("std", lambda x: np.std(x))]  # pylint:disable=unnecessary-lambda
+        [("mean", lambda x: np.mean), ("std", lambda x: np.std(x))]  # noqa: ARG005
     )
 
     metric_out = metric_out.unstack("score").sort_index(axis=1, level="score")
     metric_out.columns = metric_out.columns.map("_test_".join)
     metric_summary = metric_summary.join(metric_out)
 
     return metric_summary
```

### Comparing `biopsykit-0.8.1/src/biopsykit/classification/model_selection/nested_cv.py` & `biopsykit-0.9.0/src/biopsykit/classification/model_selection/nested_cv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Module with functions for model selection using "nested" cross-validation."""
 import warnings
 from typing import Any, Dict, Optional
 
 import numpy as np
+from biopsykit.classification.utils import split_train_test
 from sklearn.metrics import confusion_matrix, get_scorer
 from sklearn.model_selection import BaseCrossValidator, GridSearchCV, RandomizedSearchCV
 from sklearn.pipeline import Pipeline
 from tqdm.auto import tqdm
 
-from biopsykit.classification.utils import split_train_test
-
 __all__ = ["nested_cv_param_search"]
 
 
 def nested_cv_param_search(  # pylint:disable=invalid-name # pylint:disable=too-many-branches
-    X: np.ndarray,  # pylint:disable=invalid-name
+    X: np.ndarray,  # pylint:disable=invalid-name  # noqa: N803
     y: np.ndarray,
     param_dict: Dict[str, Any],
     pipeline: Pipeline,
     outer_cv: BaseCrossValidator,
     inner_cv: BaseCrossValidator,
     groups: Optional[np.ndarray] = None,
     hyper_search_params: Optional[Dict[str, Any]] = None,
@@ -131,17 +130,15 @@
                 _,
             ) = split_train_test(X, y, train, test, groups)
 
         cv_obj = _fit_cv_obj_one_fold(cv_obj, x_train, y_train, groups_train)
 
         results_dict["param_search"].append(cv_obj)
         for scorer in scoring_dict:
-            results_dict["test_{}".format(scorer)].append(
-                get_scorer(scorer)._score_func(y_test, cv_obj.predict(x_test))
-            )
+            results_dict[f"test_{scorer}"].append(get_scorer(scorer)._score_func(y_test, cv_obj.predict(x_test)))
         results_dict["train_indices"].append(train)
         results_dict["test_indices"].append(test)
         results_dict["predicted_labels"].append(cv_obj.predict(x_test))
         results_dict["true_labels"].append(y_test)
         results_dict["cv_results"].append(cv_obj.cv_results_)
         results_dict["best_estimator"].append(cv_obj.best_estimator_)
         try:
@@ -177,15 +174,15 @@
                 "Error when attempting to fit estimator. "
                 "It seems that you are trying to fit a regression model, "
                 "but specified metrics for classification. "
                 "Please check your code and provide other evaluation metrics if necessary!"
             ) from e
         if "An empty dict was passed." in e.args[0]:
             raise ValueError("No scoring metric was specified for the estimator!") from e
-        raise e
+        raise ValueError from e
     return cv_obj
 
 
 def _get_param_search_cv_object(
     pipeline: Pipeline,
     param_dict: Dict[str, Any],
     inner_cv: BaseCrossValidator,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/classification/model_selection/sklearn_pipeline_permuter.py` & `biopsykit-0.9.0/src/biopsykit/classification/model_selection/sklearn_pipeline_permuter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Module for systematically evaluating different combinations of sklearn pipelines."""
 import functools
 import pickle
 import re
 from copy import deepcopy
-from inspect import getmembers
+from inspect import getmembers, signature
 from itertools import product
 from pathlib import Path
 from shutil import rmtree
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import sklearn.metrics
+from biopsykit.classification.model_selection import nested_cv_param_search
+from biopsykit.classification.utils import _PipelineWrapper, merge_nested_dicts
+from biopsykit.utils._datatype_validation_helper import _assert_file_extension
+from biopsykit.utils._types import T, path_t, str_t
 from joblib import Memory
 from numpy.random import RandomState
 from sklearn.base import BaseEstimator, clone
 from sklearn.model_selection import BaseCrossValidator
 from sklearn.pipeline import Pipeline
 from tqdm.auto import tqdm
 
-from biopsykit.classification.model_selection import nested_cv_param_search
-from biopsykit.classification.utils import _PipelineWrapper, merge_nested_dicts
-from biopsykit.utils._datatype_validation_helper import _assert_file_extension
-from biopsykit.utils._types import T, path_t, str_t
-
 __all__ = ["SklearnPipelinePermuter"]
 
 pipeline_step_map = {
     "pipeline_scaler": "Scaler",
     "pipeline_reduce_dim": r"\makecell[lc]{Feature\\ Selection}",
     "pipeline_clf": "Classifier",
 }
@@ -273,17 +272,17 @@
         # assert pathlib
         file_path = Path(file_path)
         _assert_file_extension(file_path, ".csv")
         score_summary = pd.read_csv(file_path)
         score_summary = score_summary.set_index(list(score_summary.columns)[: num_pipeline_steps + 2])
         return cls(score_summary=score_summary)
 
-    def fit(  # pylint:disable=invalid-name
+    def fit(
         self,
-        X: np.ndarray,  # noqa
+        X: np.ndarray,  # noqa: N803
         y: np.ndarray,
         outer_cv: BaseCrossValidator,
         inner_cv: BaseCrossValidator,
         scoring: Optional[str_t] = None,
         use_cache: Optional[bool] = True,
         **kwargs,
     ):
@@ -385,15 +384,15 @@
             print("")
 
         if use_cache:
             # Delete the temporary cache before exiting
             memory.clear(warn=False)
             rmtree(location)
 
-    @functools.lru_cache(maxsize=5)
+    @functools.lru_cache(maxsize=5)  # noqa: B019
     def pipeline_score_results(self) -> pd.DataFrame:
         """Return parameter search results for each pipeline combination.
 
         Returns
         -------
         :class:`~pandas.DataFrame`
             dataframe with parameter search results for each pipeline combination
@@ -445,15 +444,15 @@
             file path to export
 
         """
         file_path = Path(file_path)
         _assert_file_extension(file_path, ".csv")
         self.results.to_csv(file_path)
 
-    @functools.lru_cache(maxsize=5)
+    @functools.lru_cache(maxsize=5)  # noqa: B019
     def mean_pipeline_score_results(self) -> pd.DataFrame:
         """Compute mean score results for each pipeline combination.
 
         Returns
         -------
         :class:`~pandas.DataFrame`
             dataframe with mean score results for each pipeline combination and each parameter combination,
@@ -547,16 +546,14 @@
 
             df_metric = df_metric.set_index(list(df_metric.columns)[: len(param_dict)])
             list_metric_summary.append(df_metric)
 
         metric_summary = pd.concat(list_metric_summary)
 
         if additional_metrics is not None:
-            if pos_label is None:
-                raise ValueError("pos_label must be specified if additional_metrics are computed!")
             metric_summary = self.compute_additional_metrics(
                 metric_summary, metrics=additional_metrics, pos_label=pos_label
             )
 
         return metric_summary
 
     def export_metric_summary(self, file_path: path_t) -> None:
@@ -687,24 +684,15 @@
         if isinstance(metric_summary_export.index, pd.MultiIndex):
             metric_summary_export.index = metric_summary_export.index.rename(pipeline_step_map)
         metric_summary_export = metric_summary_export.rename(columns=metric_map)
 
         kwargs.setdefault("column_format", self._format_latex_column_format(metric_summary_export))
 
         styler = metric_summary_export.style
-        if isinstance(highlight_best, str):
-            max_metric = metric_summary[f"mean_test_{highlight_best}"].idxmax()
-            # get index of max metric
-            max_metric = metric_summary_export.index.get_loc(max_metric)
-            styler = styler.highlight_max(subset=metric_map[highlight_best], props="bfseries: ;")
-            # get maximum of metric_summary
-            # make index bold
-            styler = styler.apply_index(lambda x: np.where(x.index == max_metric, "bfseries: ;", ""))
-        elif isinstance(highlight_best, bool) and highlight_best:
-            styler = styler.highlight_max(props="bfseries: ;")
+        styler = self._highlight_best(metric_summary, styler, highlight_best, metric_summary_export)
 
         metric_summary_tex = styler.to_latex(**kwargs)
         metric_summary_tex = self._apply_latex_code_correction(metric_summary_tex, si_table_format)
         return metric_summary_tex
 
     @staticmethod
     def _format_latex_column_format(data: pd.DataFrame):
@@ -732,36 +720,35 @@
         ----------
         file_path : :class:`~pathlib.Path` or str
             file path to export
 
         """
         file_path = Path(file_path)
         _assert_file_extension(file_path, ".pkl")
-        with open(file_path, "wb") as f:
+        with file_path.open(mode="wb") as f:
             pickle.dump(self, f)
 
     @staticmethod
     def from_pickle(file_path: path_t) -> "SklearnPipelinePermuter":
-        """Import a :class:`~biopsykit.classification.model_selection.SklearnPipelinePermuter` \
-        instance from a pickle file.
+        """Import a ``SklearnPipelinePermuter`` instance from a pickle file.
 
         Parameters
         ----------
         file_path : :class:`~pathlib.Path` or str
             file path to import
 
         Returns
         -------
         :class:`~biopsykit.classification.model_selection.SklearnPipelinePermuter`
             ``SklearnPipelinePermuter` instance
 
         """
         file_path = Path(file_path)
         _assert_file_extension(file_path, ".pkl")
-        with open(file_path, "rb") as f:
+        with file_path.open(mode="rb") as f:
             return pickle.load(f)
 
     def merge_permuter_instances(self, permuter: "SklearnPipelinePermuter") -> "SklearnPipelinePermuter":
         """Merge two :class:`~biopsykit.classification.model_selection.SklearnPipelinePermuter` instances.
 
         This function first performs a deep copy of the current instance and then merges all attributes of the given
         ``permuter`` instance with the copy. The ``permuter`` instance passed to this function is not modified.
@@ -800,30 +787,38 @@
         permuter_copy.param_searches = merge_nested_dicts(permuter_copy.param_searches, permuter.param_searches)
         permuter_copy.params = merge_nested_dicts(permuter_copy.params, permuter.params)
 
         # merge results dataframes
         results_concat = pd.concat([permuter_copy.results, permuter.results], axis=0)
         param_cols = list(results_concat.filter(like="param_").columns)
         # drop duplicate parameter combinations in results
-        results_concat = results_concat.reset_index("outer_fold").drop_duplicates(subset=["outer_fold"] + param_cols)
+        results_concat = results_concat.reset_index("outer_fold").drop_duplicates(subset=["outer_fold", *param_cols])
         results_concat = results_concat.set_index("outer_fold", append=True)
         permuter_copy.results = results_concat
 
         # merge model combinations
         permuter_copy.model_combinations += permuter.model_combinations
         permuter_copy.model_combinations = list(set(permuter_copy.model_combinations))
 
         return permuter_copy
 
     @staticmethod
     def _apply_score(row: pd.Series, score_func, pos_label: str):
         true_labels_folds = row[0]
         predicted_labels_folds = row[1]
+
+        kwargs = {}
+        params = signature(score_func).parameters
+        if "pos_label" in params:
+            kwargs["pos_label"] = pos_label
+        if "zero_division" in params:
+            kwargs["zero_division"] = 0
+
         scores = [
-            score_func(true_labels, predicted_labels, pos_label=pos_label)
+            score_func(true_labels, predicted_labels, **kwargs)
             for true_labels, predicted_labels in zip(true_labels_folds, predicted_labels_folds)
         ]
         return pd.Series(scores)
 
     def compute_additional_metrics(self, metric_summary: pd.DataFrame, metrics: str_t, pos_label: str) -> pd.DataFrame:
         """Compute additional classification metrics.
 
@@ -842,38 +837,64 @@
             metric summary with additional metrics computed
 
         """
         if isinstance(metrics, str):
             metrics = [metrics]
         metric_slice = metric_summary[["true_labels_folds", "predicted_labels_folds"]].copy()
         metric_out = {}
+        score_funcs = dict(getmembers(sklearn.metrics))
         for metric in metrics:
-            score_funcs = dict(getmembers(sklearn.metrics))
-            if metric in score_funcs:
-                score_func = score_funcs[f"{metric}"]
-                metric = metric.replace("_score", "")
-            elif f"{metric}_score" in score_funcs:
-                score_func = score_funcs[f"{metric}_score"]
+            if metric.endswith("_score"):
+                score_name = metric
+                # strip '_score' suffix from metric name for column name
+                metric = metric.replace("_score", "")  # noqa: PLW2901
+            else:
+                # name for calling sklearn metric function
+                score_name = metric + "_score"
+
+            if score_name in score_funcs:
+                score_func = score_funcs[score_name]
             else:
                 raise ValueError(f"Metric '{metric}' not found.")
+
             metric_out[metric] = metric_slice.apply(self._apply_score, args=(score_func, pos_label), axis=1)
         metric_out = pd.concat(metric_out, names=["score", "folds"], axis=1)
 
         metric_out = metric_out.stack(["score", "folds"])
         metric_out = metric_out.groupby(metric_out.index.names[:-1]).agg(
             [("mean", lambda x: np.mean(x)), ("std", lambda x: np.std(x))]
         )
 
         metric_out = metric_out.unstack("score").sort_index(axis=1, level="score")
         metric_out.columns = metric_out.columns.map("_test_".join)
         metric_summary = metric_summary.join(metric_out)
+
+        # resort columns so that all "mean_test_*" and "std_test_*" columns are at the end
+        cols = list(metric_summary.filter(regex="^(?!mean_test_|std_test_).*$").columns)
+        cols += list(metric_summary.filter(regex="^(mean_test_|std_test_).*$").columns)
+        metric_summary = metric_summary[cols]
+
         return metric_summary
 
     def _initialize_models(self, model_dict: Dict[str, Dict[str, Any]]) -> Dict[str, Dict[str, Any]]:
         if self.random_state is None:
             return model_dict
-        for k, v in model_dict.items():
+        for _k, v in model_dict.items():
             # add fixed random state to each estimator if it has a random_state parameter
             for estimator in v.values():
                 if hasattr(estimator, "random_state"):
                     estimator.random_state = self.random_state
         return model_dict
+
+    @staticmethod
+    def _highlight_best(metric_summary, styler, highlight_best, metric_summary_export):
+        if isinstance(highlight_best, str):
+            max_metric = metric_summary[f"mean_test_{highlight_best}"].idxmax()
+            # get index of max metric
+            max_metric = metric_summary_export.index.get_loc(max_metric)
+            styler = styler.highlight_max(subset=metric_map[highlight_best], props="bfseries: ;")
+            # get maximum of metric_summary
+            # make index bold
+            styler = styler.apply_index(lambda x: np.where(x.index == max_metric, "bfseries: ;", ""))
+        elif isinstance(highlight_best, bool) and highlight_best:
+            styler = styler.highlight_max(props="bfseries: ;")
+        return styler
```

### Comparing `biopsykit-0.8.1/src/biopsykit/classification/utils.py` & `biopsykit-0.9.0/src/biopsykit/classification/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,16 @@
                 x_data.shape, y_data.shape, len(group_keys), np.unique(y_data, return_counts=True)[1]
             )
         )
 
     return x_data, y_data, groups, group_keys
 
 
-def split_train_test(  # pylint:disable=invalid-name
-    X: np.ndarray,  # noqa
+def split_train_test(
+    X: np.ndarray,  # noqa: N803
     y: np.ndarray,
     train: np.ndarray,
     test: np.ndarray,
     groups: Optional[np.ndarray] = None,
 ) -> Tuple[np.ndarray, ...]:
     """Split data into train and test set.
 
@@ -195,15 +195,15 @@
         Targets of test data
     group_train: :class:`~numpy.ndarray`
         Group labels of training data (only available if ``groups`` is not ``None``)
     group_test: :class:`~numpy.ndarray`
         Group labels of test data (only available if ``groups`` is not ``None``)
 
     """
-    X_train, X_test = X[train], X[test]  # noqa
+    X_train, X_test = X[train], X[test]  # noqa: N806
     y_train, y_test = y[train], y[test]
 
     if groups is None:
         return X_train, X_test, y_train, y_test
 
     groups_train = groups[train]
     groups_test = groups[test]
@@ -233,11 +233,10 @@
 def _merge_nested_dicts(dict1: Dict, dict2: Dict) -> Dict:
     for key, value in dict2.items():
         if isinstance(value, dict) and key in dict1:
             _merge_nested_dicts(dict1[key], value)
             # check if value is list
         elif isinstance(value, list) and key in dict1:
             dict1[key] = value if key not in dict1 else dict1[key] + value
-        else:
-            if key not in dict1:
-                dict1[key] = value
+        elif key not in dict1:
+            dict1[key] = value
     return dict1
```

### Comparing `biopsykit-0.8.1/src/biopsykit/example_data.py` & `biopsykit-0.9.0/src/biopsykit/example_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 downloaded into the local user folder.
 """
 from pathlib import Path
 from typing import Dict, Optional, Sequence, Tuple, Union
 from urllib.request import urlretrieve
 
 import pandas as pd
-from tqdm.auto import tqdm
-
 from biopsykit.io import (
     load_long_format_csv,
     load_pandas_dict_excel,
     load_questionnaire_data,
     load_subject_condition_list,
     load_time_log,
 )
-from biopsykit.io.carwatch_logs import load_log_one_subject
 from biopsykit.io.ecg import load_hr_phase_dict
 from biopsykit.io.eeg import MuseDataset
 from biopsykit.io.nilspod import load_dataset_nilspod
 from biopsykit.io.saliva import load_saliva_plate, load_saliva_wide_format
 from biopsykit.io.sleep_analyzer import (
     WITHINGS_RAW_DATA_SOURCES,
     load_withings_sleep_analyzer_raw_file,
@@ -36,14 +33,15 @@
     SalivaRawDataFrame,
     SleepEndpointDataFrame,
     SubjectConditionDataFrame,
     _SalivaMeanSeDataFrame,
     is_saliva_mean_se_dataframe,
 )
 from biopsykit.utils.file_handling import mkdirs
+from tqdm.auto import tqdm
 
 _EXAMPLE_DATA_PATH_LOCAL = Path(__file__).parent.parent.parent.joinpath("example_data")
 _EXAMPLE_DATA_PATH_HOME = Path.home().joinpath(".biopsykit_data")
 _REMOTE_DATA_PATH = "https://raw.githubusercontent.com/mad-lab-fau/BioPsyKit/main/example_data/"
 
 __all__ = [
     "get_condition_list_example",
@@ -61,18 +59,14 @@
     "get_ecg_example_02",
     "get_eeg_example",
     "get_sleep_analyzer_raw_file_unformatted",
     "get_sleep_analyzer_raw_file",
     "get_sleep_analyzer_raw_example",
     "get_sleep_analyzer_summary_example",
     "get_sleep_imu_example",
-    "get_car_watch_log_path_example",
-    "get_car_watch_log_data_zip_path_example",
-    "get_car_watch_log_path_all_subjects_example",
-    "get_car_watch_log_data_example",
     "get_time_log_example",
     "get_questionnaire_example",
     "get_questionnaire_example_wrong_range",
     "get_stats_example",
 ]
 
 # TODO add SHA256 check to assert whether remote example data was changed and should be re-downloaded.
@@ -252,16 +246,15 @@
     for subject_id in subject_ids:
         file_path = _get_data(f"ecg_results/hr_result_{subject_id}.xlsx")
         study_data_dict_hr[subject_id] = pd.read_excel(file_path, sheet_name=None, index_col="time")
     return study_data_dict_hr
 
 
 def get_hr_subject_data_dict_tuple_example() -> HeartRateSubjectDataDict:
-    """Return heart rate example data in the form of a \
-    :obj:`~biopsykit.utils.datatype_helper.HeartRateSubjectDataDict`, but with tuples as keys instead of strings.
+    """Return HR example data as a ``HeartRateSubjectDataDict``, but with tuples as keys instead of strings.
 
     Returns
     -------
     :obj:`~biopsykit.utils.datatype_helper.HeartRateSubjectDataDict`
         dictionary with heart rate time-series, each containing data from different phases.
 
     """
@@ -510,100 +503,14 @@
     sampling_rate : float
         sampling rate of recorded data
 
     """
     return MuseDataset.from_csv_file(_get_data("eeg_muse_example.csv"), tz="Europe/Berlin")
 
 
-def get_car_watch_log_path_example() -> path_t:
-    """Return folder path to *CARWatch App* log files from *one* subject.
-
-    Returns
-    -------
-    :class:`~pathlib.Path` or str
-        path to folder with *CARWatch App* log files.
-
-    """
-    # ensure that folder exists and data in folder is available
-    file_list = [
-        "carwatch_de34f_20191205.csv",
-        "carwatch_de34f_20191206.csv",
-        "carwatch_de34f_20191207.csv",
-        "carwatch_de34f_20191208.csv",
-    ]
-    file_path = None
-    for file in file_list:
-        file_path = _get_data(f"log_data/DE34F/{file}")
-    # get parent directory
-    return file_path.parent
-
-
-def get_car_watch_log_data_zip_path_example() -> path_t:
-    """Return path to *CARWatch App* example log data as zip file from *one* subject.
-
-    Returns
-    -------
-    :class:`~pathlib.Path` or str
-        path to *CARWatch App* example log data as zip file
-
-    """
-    return _get_data("log_data/logs_AB12C.zip")
-
-
-def get_car_watch_log_data_example() -> pd.DataFrame:
-    """Return *CARWatch App* example log data from folder from *one* subject.
-
-    Returns
-    -------
-    data : :class:`~pandas.DataFrame`
-        dataframe with example log data from the *CARWatch* app
-
-    """
-    # ensure that all files are available
-    file_list = [
-        "carwatch_de34f_20191205.csv",
-        "carwatch_de34f_20191206.csv",
-        "carwatch_de34f_20191207.csv",
-        "carwatch_de34f_20191208.csv",
-    ]
-    file_path = None
-    for file in file_list:
-        file_path = _get_data(f"log_data/DE34F/{file}")
-    # get parent directory
-    file_path = file_path.parent
-    return load_log_one_subject(file_path)
-
-
-def get_car_watch_log_path_all_subjects_example() -> path_t:
-    """Return folder path to *CARWatch App* log files for *multiple* subjects.
-
-    Returns
-    -------
-    :class:`~pathlib.Path` or str
-        path to folder with *CARWatch App* log files.
-
-    """
-    # ensure that folder exists and data in folder is available
-    file_list = [
-        "DE34F/carwatch_de34f_20191205.csv",
-        "DE34F/carwatch_de34f_20191206.csv",
-        "DE34F/carwatch_de34f_20191207.csv",
-        "DE34F/carwatch_de34f_20191208.csv",
-        "GH56I/carwatch_gh56i_20191205.csv",
-        "GH56I/carwatch_gh56i_20191206.csv",
-        "GH56I/carwatch_gh56i_20191207.csv",
-        "GH56I/carwatch_gh56i_20191208.csv",
-    ]
-    file_path = None
-    for file in file_list:
-        file_path = _get_data(f"log_data/{file}")
-    # get parent directory
-    return file_path.parent.parent
-
-
 def get_time_log_example() -> pd.DataFrame:
     """Return time log example data.
 
     Returns
     -------
     data : :class:`~pandas.DataFrame`
         dataframe with example time log information. The time log match the data from the two ECG data example
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/__init__.py` & `biopsykit-0.9.0/src/biopsykit/io/__init__.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/io/biopac.py` & `biopsykit-0.9.0/src/biopsykit/io/biopac.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 except ImportError as e:
     raise ImportError(
         "The 'bioread' package is required to read Biopac data files. "
         "Please install it using 'pip install bioread' or 'poetry add bioread'."
     ) from e
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension
 from biopsykit.utils._types import path_t, str_t
 
 __all__ = ["BiopacDataset"]
 
 
 class BiopacDataset:
@@ -154,15 +153,15 @@
             from the recording or to overwrite the start time extracted from the recording.
 
         """
         # sanitize datastreams input
         datastreams = self._sanitize_datastreams_input(datastreams)
 
         # assert that all datastreams have the same sampling rate
-        sampling_rates = set(self._sampling_rate[datastream] for datastream in datastreams)
+        sampling_rates = {self._sampling_rate[datastream] for datastream in datastreams}
         if len(sampling_rates) > 1:
             raise ValueError("All datastreams must have the same sampling rate for combining it into one DataFrame!")
 
         # get datastreams from dict
         data = [self._data[datastream] for datastream in datastreams]
         data = pd.concat(data, axis=1)
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/carwatch_logs.py` & `biopsykit-0.9.0/src/biopsykit/io/carwatch_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import re
 import warnings
 import zipfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Optional, Sequence, Union
 
 import pandas as pd
-from tqdm.auto import tqdm
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension
 from biopsykit.utils._types import path_t
 from biopsykit.utils.time import tz, utc
+from tqdm.auto import tqdm
 
 if TYPE_CHECKING:
     from biopsykit.carwatch_logs import LogData
 
 LOG_FILENAME_PATTERN = "logs_(.*?)"
 
 
@@ -60,20 +59,20 @@
     base_folder = Path(base_folder)
 
     if has_subject_folders:
         folder_list = [p for p in sorted(base_folder.glob("*")) if p.is_dir() and not p.name.startswith(".")]
         dict_log_files = _load_log_file_folder(folder_list)
     else:
         # first, look for available csv files
-        file_list = list(sorted(base_folder.glob("*.csv")))
+        file_list = sorted(base_folder.glob("*.csv"))
         if len(file_list) > 0:
             dict_log_files = _load_log_file_list_csv(file_list, log_filename_pattern)
         else:
             # fallback: look for zip files
-            file_list = list(sorted(base_folder.glob("*.zip")))
+            file_list = sorted(base_folder.glob("*.zip"))
             dict_log_files = _load_log_file_zip(file_list, log_filename_pattern)
 
     if return_df:
         return pd.concat(dict_log_files, names=["subject_id"])
     return dict_log_files
 
 
@@ -90,15 +89,15 @@
     dict_log_files = {}
     if log_filename_pattern is None:
         log_filename_pattern = LOG_FILENAME_PATTERN + ".csv"
     for file in tqdm(file_list):
         subject_id = re.search(log_filename_pattern, file.name).group(1)
         df = pd.read_csv(file, sep=";")
         df["time"] = pd.to_datetime(df["time"])
-        df.set_index("time", inplace=True)
+        df = df.set_index("time")
         dict_log_files[subject_id] = df
     return dict_log_files
 
 
 def _load_log_file_zip(file_list: Sequence[Path], log_filename_pattern: str) -> Dict[str, pd.DataFrame]:
     dict_log_files = {}
     if log_filename_pattern is None:
@@ -173,15 +172,15 @@
 
     Returns
     -------
     :class:`~pandas.DataFrame`
         dataframe with log data for one subject
 
     """
-    file_list = list(sorted(folder_path.glob("*.csv")))
+    file_list = sorted(folder_path.glob("*.csv"))
     return pd.concat([_load_log_file_csv(file) for file in file_list])
 
 
 def _load_log_file_csv(file_path: path_t) -> pd.DataFrame:
     df = pd.read_csv(file_path, sep=";", header=None, names=["time", "action", "extras"])
 
     df["time"] = pd.to_datetime(df["time"], unit="ms")
@@ -237,20 +236,19 @@
             log_data.to_csv(path, sep=";")
             return
         log_data = LogData(log_data)
 
     if subject_id is None:
         subject_id = log_data.subject_id
 
-    export_path = path.joinpath("logs_{}.csv".format(subject_id))
+    export_path = path.joinpath(f"logs_{subject_id}.csv")
     if not export_path.exists() or overwrite:
         log_data.data.to_csv(export_path, sep=";")
-    else:
-        if show_skipped:
-            print("Skipping subject {}. Already exported.".format(subject_id))
+    elif show_skipped:
+        print(f"Skipping subject {subject_id}. Already exported.")
 
 
 def _parse_date(row: pd.Series) -> pd.Series:
     """Parse date in "timestamp" and "timestamp_hidden" columns of a pandas series.
 
     Parameters
     ----------
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/ecg.py` & `biopsykit-0.9.0/src/biopsykit/io/ecg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """I/O functions for files related to ECG processing."""
 import re
 import warnings
 from pathlib import Path
 from typing import Optional, Sequence
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_is_dir
 from biopsykit.utils._types import path_t
 from biopsykit.utils.datatype_helper import HeartRatePhaseDict, HeartRateSubjectDataDict, is_hr_phase_dict
 from biopsykit.utils.file_handling import get_subject_dirs, is_excel_file
 from biopsykit.utils.time import tz
 
 __all__ = [
@@ -70,16 +69,15 @@
     dict_hr = {k: v.tz_localize(tz) for k, v in dict_hr.items()}
     return dict_hr
 
 
 def load_hr_phase_dict_folder(
     base_path: path_t, filename_pattern: str, subfolder_pattern: Optional[str] = None
 ) -> HeartRateSubjectDataDict:
-    """Load a folder with multiple :obj:`~biopsykit.utils.datatype_helper.HeartRatePhaseDict` and concatenate them \
-    into a :obj:`~biopsykit.utils.datatype_helper.HeartRateSubjectDataDict`.
+    r"""Load a folder with multiple ``HeartRatePhaseDict`` and concatenate them  into a ``HeartRateSubjectDataDict``.
 
     This functions looks for all files that match the ``file_pattern`` in the folder specified by ``base_path``
     and loads the files that are all expected to be :obj:`~biopsykit.utils.datatype_helper.HeartRatePhaseDict`.
 
     Subject IDs are extracted from the file name. Hence, ``file_pattern`` needs to be a regex
     including a capture group, e.g. "ecg_results_(\\w+).xlsx".
 
@@ -152,20 +150,18 @@
 
     """
     # ensure pathlib
     base_path = Path(base_path)
 
     dict_hr_subjects = {}
     if subfolder_pattern is None:
-        file_list = list(sorted(base_path.glob("*")))
+        file_list = sorted(base_path.glob("*"))
         file_list = [f for f in file_list if re.search(filename_pattern, f.name)]
         if len(file_list) == 0:
-            raise FileNotFoundError(
-                "No files matching the pattern '{}' found in {}.".format(filename_pattern, base_path)
-            )
+            raise FileNotFoundError(f"No files matching the pattern '{filename_pattern}' found in {base_path}.")
         for file in file_list:
             subject_id = re.findall(filename_pattern, file.name)[0]
             dict_hr_subjects[subject_id] = load_hr_phase_dict(file)
     else:
         subject_dirs = get_subject_dirs(base_path, subfolder_pattern)
 
         for subject_dir in subject_dirs:
@@ -178,15 +174,15 @@
 
 
 def _load_hr_phase_dict_single_subject(subject_dir: Path, filename_pattern: str) -> Optional[HeartRatePhaseDict]:
     subject_id = subject_dir.name
     # first try to search for files with glob (assuming that a regex string without capture group was passed),
     # then try to search via regex search (assuming that a regex string with capture group was passed,
     # which should actually not be done if subfolder_pattern is passed)
-    file_list = list(sorted(subject_dir.glob(filename_pattern)))
+    file_list = sorted(subject_dir.glob(filename_pattern))
     if len(file_list) == 0:
         file_list = sorted(subject_dir.glob("*"))
         # then extract the ones that match
         file_list = [f for f in file_list if re.search(filename_pattern, f.name)]
 
     if len(file_list) == 1:
         return load_hr_phase_dict(file_list[0])
@@ -196,15 +192,15 @@
             "Trying to merge these files into one HeartRatePhaseDict".format(filename_pattern, subject_dir)
         )
         dict_hr = {}
         for file in file_list:
             dict_hr.update(load_hr_phase_dict(file))
         return dict_hr
 
-    print("No Heart Rate data for subject {}".format(subject_id))
+    print(f"No Heart Rate data for subject {subject_id}")
     return None
 
 
 def write_hr_phase_dict(hr_phase_dict: HeartRatePhaseDict, file_path: path_t):
     """Write :obj:`~biopsykit.utils.datatype_helper.HeartRatePhaseDict` to an Excel file.
 
     The :obj:`~biopsykit.utils.datatype_helper.HeartRatePhaseDict` is a dictionary with heart rate time
@@ -292,16 +288,15 @@
 
 def load_hr_phase_dict_csv(
     folder_path: path_t,
     file_pattern: path_t,
     phase_order: Optional[Sequence[str]] = None,
     assert_format: Optional[bool] = True,
 ) -> HeartRatePhaseDict:
-    """Load csv file containing time series heart rate data of one subject from folder and combine it into a \
-    :obj:`~biopsykit.utils.datatype_helper.HeartRatePhaseDict`.
+    """Load csv file with time series HR data of one subject from folder and combine it into a ``HeartRatePhaseDict``.
 
     The returned dictionary will be a :obj:`~biopsykit.utils.datatype_helper.HeartRatePhaseDict`,
     i.e., a dict with heart rate data from one subject split into phases (as exported by :func:`write_hr_phase_dict`).
 
     Parameters
     ----------
     folder_path : :class:`~pathlib.Path` or str
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/eeg.py` & `biopsykit-0.9.0/src/biopsykit/io/eeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """I/O functions for files related to EEG processing."""
 import warnings
 from typing import Optional, Tuple
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_has_columns
 from biopsykit.utils._types import path_t
 
 __all__ = ["load_eeg_raw_muse", "MuseDataset"]
 
 
 class MuseDataset:
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/io.py` & `biopsykit-0.9.0/src/biopsykit/io/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import datetime
 from pathlib import Path
 from typing import Dict, Literal, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pytz
-from nilspodlib import Dataset
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_has_columns, _assert_is_dtype
 from biopsykit.utils._types import path_t
 from biopsykit.utils.dataframe_handling import convert_nan
 from biopsykit.utils.datatype_helper import (
     CodebookDataFrame,
     SubjectConditionDataFrame,
     SubjectConditionDict,
@@ -21,14 +19,15 @@
     is_codebook_dataframe,
     is_subject_condition_dataframe,
     is_subject_condition_dict,
 )
 from biopsykit.utils.exceptions import ValidationError
 from biopsykit.utils.file_handling import is_excel_file
 from biopsykit.utils.time import tz
+from nilspodlib import Dataset
 
 __all__ = [
     "load_long_format_csv",
     "load_time_log",
     "load_subject_condition_list",
     "load_questionnaire_data",
     "load_pandas_dict_excel",
@@ -168,15 +167,15 @@
     data = _apply_index_cols(data, index_cols=index_cols)
     data = _apply_phase_cols(data, phase_cols=phase_cols)
     data.columns.name = "phase"
 
     if not continuous_time:
         data = _parse_time_log_not_continuous(data, index_cols)
 
-    for val in data.values.flatten():
+    for val in data.to_numpy().flatten():
         if val is np.nan:
             continue
         _assert_is_dtype(val, str)
 
     return data
 
 
@@ -229,15 +228,15 @@
     date = _extract_date(dataset, df, date)
 
     if timezone is None:
         timezone = tz
     if isinstance(timezone, str):
         timezone = pytz.timezone(timezone)
 
-    if isinstance(time_log.values.flatten()[0], str):
+    if isinstance(time_log.to_numpy().flatten()[0], str):
         # convert time strings into datetime.time object
         time_log = time_log.applymap(pd.to_datetime)
         time_log = time_log.applymap(lambda val: val.time())
 
     time_log = time_log.applymap(lambda x: timezone.localize(datetime.datetime.combine(date, x)))
     return time_log
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/nilspod.py` & `biopsykit-0.9.0/src/biopsykit/io/nilspod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Module for importing data recorded by NilsPod sensors."""
 import datetime
 import re
 import warnings
 from pathlib import Path
-from typing import Dict, Optional, Sequence, Tuple, Union
+from typing import Dict, Literal, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from nilspodlib import Dataset, SyncedSession
-from typing_extensions import Literal
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_is_dir, _assert_is_dtype
 from biopsykit.utils._types import path_t
 from biopsykit.utils.time import tz
+from nilspodlib import Dataset, SyncedSession
 
 COUNTER_INCONSISTENCY_HANDLING = Literal["raise", "warn", "ignore"]
 """Available behavior types when dealing with NilsPod counter inconsistencies."""
 
 __all__ = [
     "load_dataset_nilspod",
     "load_synced_session_nilspod",
@@ -200,21 +198,21 @@
     :func:`~biopsykit.io.nilspod.load_dataset_nilspod`
         load a single NilsPod dataset
 
     """
     # ensure pathlib
     folder_path = Path(folder_path)
 
-    nilspod_files = list(sorted(folder_path.glob("*.bin")))
+    nilspod_files = sorted(folder_path.glob("*.bin"))
     if len(nilspod_files) == 0:
         raise ValueError("No NilsPod files found in directory!")
 
     kwargs.setdefault("tz", kwargs.pop("timezone", tz))
     session = SyncedSession.from_folder_path(folder_path, **kwargs)
-    session.align_to_syncregion(inplace=True)
+    session = session.align_to_syncregion()
 
     _handle_counter_inconsistencies_session(session, handle_counter_inconsistency)
     if isinstance(datastreams, str):
         datastreams = [datastreams]
 
     # convert dataset to dataframe and localize timestamp
     df = session.data_as_df(datastreams, index="local_datetime", concat_df=True)
@@ -229,15 +227,15 @@
 
 def _handle_counter_inconsistencies_dataset(
     dataset: Dataset, handle_counter_inconsistency: COUNTER_INCONSISTENCY_HANDLING
 ):
     idxs_corrupted = np.where(np.diff(dataset.counter) < 1)[0]
     # edge case: check if only last sample is corrupted. if yes, cut last sample
     if len(idxs_corrupted) == 1 and (idxs_corrupted == len(dataset.counter) - 2):
-        dataset.cut(start=0, stop=idxs_corrupted[0], inplace=True)
+        dataset = dataset.cut(start=0, stop=idxs_corrupted[0])
     elif len(idxs_corrupted) > 1:
         if handle_counter_inconsistency == "raise":
             raise ValueError("Error loading dataset. Counter not monotonously increasing!")
         if handle_counter_inconsistency == "warn":
             warnings.warn(
                 "Counter not monotonously increasing. This might indicate that the dataset is corrupted or "
                 "that the dataset was recorded as part of a synchronized session and might need to be loaded "
@@ -248,15 +246,15 @@
 
 def _handle_counter_inconsistencies_session(
     session: SyncedSession, handle_counter_inconsistency: COUNTER_INCONSISTENCY_HANDLING
 ):
     idxs_corrupted = np.where(np.diff(session.counter) < 1)[0]
     # edge case: check if only last sample is corrupted. if yes, cut last sample
     if len(idxs_corrupted) == 1 and (idxs_corrupted == len(session.counter) - 2):
-        session.cut(start=0, stop=idxs_corrupted[0], inplace=True)
+        session = session.cut(start=0, stop=idxs_corrupted[0])
     elif len(idxs_corrupted) > 1:
         if handle_counter_inconsistency == "raise":
             raise ValueError("Error loading session. Counter not monotonously increasing!")
         if handle_counter_inconsistency == "warn":
             warnings.warn(
                 "Counter not monotonously increasing. This might indicate that the session is corrupted. "
                 "Check the counter of the DataFrame manually!"
@@ -415,15 +413,15 @@
 
     """
     # ensure pathlib
     folder_path = Path(folder_path)
     _assert_is_dir(folder_path)
 
     # look for all NilsPod binary files in the folder
-    dataset_list = list(sorted(folder_path.glob("*.bin")))
+    dataset_list = sorted(folder_path.glob("*.bin"))
     if len(dataset_list) == 0:
         raise ValueError(f"No NilsPod files found in folder {folder_path}!")
     if phase_names is None:
         phase_names = [f"Part{i}" for i in range(len(dataset_list))]
 
     if len(phase_names) != len(dataset_list):
         raise ValueError(
@@ -497,18 +495,15 @@
     nilspod_file_pattern = r"NilsPodX-\w{4}_(.*?).bin"
     # ensure pathlib
     file_path = Path(file_path)
 
     keys = ["name", "percent_corrupt", "condition"]
     dict_res = dict.fromkeys(keys)
     re_groups = re.search(nilspod_file_pattern, file_path.name)
-    if re_groups is not None:
-        name = re_groups.group(1)
-    else:
-        name = file_path.name
+    name = re_groups.group(1) if re_groups is not None else file_path.name
     dict_res["name"] = name
     if not check_nilspod_dataset_corrupted(dataset):
         dict_res["condition"] = "fine"
         dict_res["percent_corrupt"] = 0.0
         return dict_res
 
     idx_diff = np.diff(dataset.counter)
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/psg.py` & `biopsykit-0.9.0/src/biopsykit/io/psg.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 except ImportError as e:
     raise ImportError(
         "The 'mne' package is required to read edf data files. "
         "Please install it using 'pip install mne' or 'poetry add mne'."
     ) from e
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_is_dir
 from biopsykit.utils._types import path_t
 
 __all__ = ["PSGDataset"]
 
 
 class PSGDataset:
@@ -32,15 +31,15 @@
         start_time: Optional[pd.Timestamp] = None,
         tz: Optional[str] = None,
     ):
 
         self._data = data_dict
         for name, data in data_dict.items():
             setattr(self, name, data)
-        for name, sampling_rate in sampling_rate_dict.items():
+        for _, sampling_rate in sampling_rate_dict.items():
             setattr(self, "sampling_rate", sampling_rate)
         setattr(self, "channels", list(self._data.keys()))
         self._sampling_rate = sampling_rate_dict
         self._start_time_datetime = pd.Timestamp(start_time)
         self._start_time_unix = int(time.mktime(start_time.timetuple()))
         self._tz = tz
 
@@ -170,15 +169,15 @@
         FileNotFoundError: if no .edf file is found in the folder
         ValueError: if more than one .edf file is found in the folder
 
         """
         _assert_is_dir(folder_path)
 
         # look for all PSG .edf files in the folder
-        dataset_list = list(sorted(folder_path.glob("*.edf")))
+        dataset_list = sorted(folder_path.glob("*.edf"))
         if len(dataset_list) == 0:
             raise FileNotFoundError(f"No PSG files found in folder {folder_path}!")
         if len(dataset_list) > 1:
             raise ValueError(
                 f"More than one PSG files found in folder {folder_path}!"
                 f"This function only supports one recording per folder!"
             )
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/saliva.py` & `biopsykit-0.9.0/src/biopsykit/io/saliva.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module containing different I/O functions for saliva data."""
 from pathlib import Path
 from typing import Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.io.io import _apply_index_cols
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_has_columns
 from biopsykit.utils._types import path_t
 from biopsykit.utils.datatype_helper import (
     SalivaRawDataFrame,
     SubjectConditionDataFrame,
     _SalivaRawDataFrame,
@@ -284,15 +283,15 @@
     is_saliva_raw_dataframe(data, saliva_type)
 
     return _SalivaRawDataFrame(data)
 
 
 def _get_index_cols(condition_col: str, index_cols: Sequence[str], additional_index_cols: Sequence[str]):
     if condition_col is not None:
-        index_cols = [condition_col] + index_cols
+        index_cols = [condition_col, *index_cols]
 
     if additional_index_cols is None:
         additional_index_cols = []
     if isinstance(additional_index_cols, str):
         additional_index_cols = [additional_index_cols]
 
     return index_cols + additional_index_cols
@@ -391,21 +390,20 @@
 
 
 def _get_id_columns(id_col_names: Sequence[str], extracted_cols: pd.DataFrame):
     if id_col_names is None:
         id_col_names = ["subject", "sample"]
         if len(extracted_cols.columns) == 3:
             id_col_names = ["subject", "day", "sample"]
-    else:
-        if len(id_col_names) != len(extracted_cols.columns):
-            raise ValueError(
-                "Number of 'id_col_names' must match length of extracted index columns! Expected {}, got {}.".format(
-                    len(extracted_cols), len(id_col_names)
-                )
+    elif len(id_col_names) != len(extracted_cols.columns):
+        raise ValueError(
+            "Number of 'id_col_names' must match length of extracted index columns! Expected {}, got {}.".format(
+                len(extracted_cols), len(id_col_names)
             )
+        )
 
     return id_col_names
 
 
 def _get_condition_col(data: pd.DataFrame, condition_col: str) -> Tuple[pd.DataFrame, str]:
     if condition_col is None:
         if "condition" in data.columns:
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/sleep.py` & `biopsykit-0.9.0/src/biopsykit/io/sleep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Module containing different I/O functions to load and save sleep data."""
 from pathlib import Path
 from typing import Dict, Union
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension
 from biopsykit.utils._types import path_t
 from biopsykit.utils.datatype_helper import is_sleep_endpoint_dataframe, is_sleep_endpoint_dict
 
 __all__ = ["save_sleep_endpoints"]
```

### Comparing `biopsykit-0.8.1/src/biopsykit/io/sleep_analyzer.py` & `biopsykit-0.9.0/src/biopsykit/io/sleep_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 from ast import literal_eval
 from pathlib import Path
 from typing import Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.sleep.utils import split_nights
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_has_columns, _assert_is_dir
 from biopsykit.utils._types import path_t
 from biopsykit.utils.datatype_helper import SleepEndpointDataFrame, is_sleep_endpoint_dataframe
 from biopsykit.utils.time import tz
 
 __all__ = [
@@ -84,17 +83,17 @@
 
     """
     # ensure pathlib
     folder_path = Path(folder_path)
 
     _assert_is_dir(folder_path)
 
-    raw_files = list(sorted(folder_path.glob("raw_sleep-monitor_*.csv")))
+    raw_files = sorted(folder_path.glob("raw_sleep-monitor_*.csv"))
     if len(raw_files) == 0:
-        raise ValueError("No sleep analyzer raw files found in {}!".format(folder_path))
+        raise ValueError(f"No sleep analyzer raw files found in {folder_path}!")
     data_sources = [re.findall(r"raw_sleep-monitor_(\S*).csv", s.name)[0] for s in raw_files]
 
     list_data = [
         load_withings_sleep_analyzer_raw_file(
             file_path,
             data_source=WITHINGS_RAW_DATA_SOURCES[data_source],
             timezone=timezone,
@@ -189,15 +188,14 @@
     data["value"] = data["value"].apply(literal_eval)
 
     # rename index
     data.index.name = "time"
     # explode data and apply timestamp explosion to groups
     data_explode = data.apply(pd.Series.explode)
     data_explode = data_explode.groupby("time", group_keys=False).apply(_explode_timestamp)
-    data_explode.index = data_explode.index.tz_localize("UTC").tz_convert(timezone)
     # rename the value column
     data_explode.columns = [data_source]
     # convert dtypes from object into numerical values
     data_explode = data_explode.astype(int)
     # drop duplicate index values
     data_explode = data_explode.loc[~data_explode.index.duplicated()]
 
@@ -269,15 +267,15 @@
     # total duration in seconds
     data["total_duration"] = [int(td.total_seconds()) for td in data["bis"] - data["von"]]
     data["date"] = data["von"]
     data["date"] = data["date"].apply(
         lambda date: ((date - pd.Timedelta("1d")) if date.hour < 12 else date).normalize()
     )
 
-    data.rename(
+    data = data.rename(
         {
             "von": "recording_start",
             "bis": "recording_end",
             "leicht (s)": "total_time_light_sleep",
             "tief (s)": "total_time_deep_sleep",
             "rem (s)": "total_time_rem_sleep",
             "wach (s)": "total_time_awake",
@@ -287,15 +285,14 @@
             "Snoring episodes": "count_snoring_episodes",
             "Snoring (s)": "total_time_snoring",
             "Average heart rate": "heart_rate_avg",
             "Heart rate (min)": "heart_rate_min",
             "Heart rate (max)": "heart_rate_max",
         },
         axis="columns",
-        inplace=True,
     )
 
     data["sleep_onset"] = data["recording_start"] + pd.to_timedelta(data["sleep_onset_latency"], unit="seconds")
     # Wake after Sleep Onset (WASO): total time awake after sleep onset
     data["wake_after_sleep_onset"] = data["total_time_awake"] - data["sleep_onset_latency"] - data["getup_latency"]
     data["wake_onset"] = data["recording_end"] - pd.to_timedelta(data["getup_latency"], unit="seconds")
     # compute total sleep duration
@@ -340,22 +337,17 @@
 
 
 def _explode_timestamp(df: pd.DataFrame) -> pd.DataFrame:
     # sum up the time durations and subtract the first value from it (so that we start from 0)
     # dur_sum then looks like this: [0, 60, 120, 180, ...]
     dur_sum = df["duration"].cumsum() - df["duration"].iloc[0]
     # Add these time durations to the index timestamps.
-    # For that, we need to convert the datetime objects from the pandas DatetimeIndex into a float
-    # and add the time onto it (we first need to multiply it with 10^9 because the time in the index
-    # is stored in nanoseconds)
-    index_sum = df.index.values.astype(float) + 1e9 * dur_sum
-    # convert the float values back into a DatetimeIndex
-    df["time"] = pd.to_datetime(index_sum)
+    df["time"] = df.index + pd.to_timedelta(dur_sum, unit="s")
     # set this as index
-    df.set_index("time", inplace=True)
+    df = df.set_index("time")
     # we don't need the duration column anymore so we can drop it
-    df.drop(columns="duration", inplace=True)
+    df = df.drop(columns="duration")
     return df
 
 
 def _reindex_datetime_index(df: pd.DataFrame) -> pd.DataFrame:
     return df.reindex(df.resample("1min").bfill().index)
```

### Comparing `biopsykit-0.8.1/src/biopsykit/metadata/metadata.py` & `biopsykit-0.9.0/src/biopsykit/metadata/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 If ``data`` is a dataframe that contains more than the required two columns, e.g., if the complete dataframe
 is passed, the required columns can be sliced by specifying them in the ``columns`` parameter.
 
 """
 from typing import Optional, Sequence, Union
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import (
     _assert_has_columns,
     _assert_has_index_levels,
     _assert_len_list,
     _assert_value_range,
 )
```

### Comparing `biopsykit-0.8.1/src/biopsykit/plotting/plotting.py` & `biopsykit-0.9.0/src/biopsykit/plotting/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Module containing several advanced plotting functions."""
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from statannot import add_stat_annotation
-
 from biopsykit.utils.functions import se
+from statannot import add_stat_annotation
 
 _PVALUE_THRESHOLDS = [[1e-3, "***"], [1e-2, "**"], [0.05, "*"]]
 
 
 def lineplot(
     data: pd.DataFrame, x: str, y: str, hue: Optional[str] = None, style: Optional[str] = None, **kwargs
 ) -> Tuple[plt.Figure, plt.Axes]:
@@ -108,18 +107,15 @@
     fig, ax = _plot_get_fig_ax(**kwargs)
 
     kwargs.setdefault("ax", ax)
     kwargs.setdefault("err_kws", {"capsize": 5})
 
     marker, linestyle = _get_styles(data, style, hue, marker, linestyle)
 
-    if hue is not None:
-        grouped = {key: val for key, val in data.groupby(hue)}  # pylint:disable=unnecessary-comprehension
-    else:
-        grouped = {y: data}
+    grouped = dict(tuple(data.groupby(hue))) if hue is not None else {y: data}
 
     if hue_order is not None:
         # reorder group dictionary
         grouped = {key: grouped[key] for key in hue_order}
 
     # generate x axis
     x_vals = data[x].unique()
@@ -372,17 +368,16 @@
             labels,
             rect=rect,
             legend_loc=legend_loc,
             legend_fontsize=legend_fontsize,
             legend_orientation=legend_orientation,
             legend_title=legend_title,
         )
-    else:
-        if kwargs.pop("tight_layout", True):
-            fig.tight_layout()
+    elif kwargs.pop("tight_layout", True):
+        fig.tight_layout()
     return fig, ax
 
 
 def _feature_boxplot_sanitize_stats_kwargs(stats_kwargs: Dict[str, Any]) -> Dict[str, Any]:
     boxplot_pvals = stats_kwargs.get("pvalues", {})
     if len(stats_kwargs) > 0:
         stats_kwargs["comparisons_correction"] = stats_kwargs.get("comparisons_correction", None)
@@ -483,14 +478,15 @@
     legend_fontsize = kwargs.pop("legend_fontsize", None)
     legend_title = kwargs.pop("legend_title", None)
     legend_loc = kwargs.pop("legend_loc", "upper right")
     legend_orientation = kwargs.pop("legend_orientation", "vertical")
     alpha = kwargs.pop("alpha", 1.0)
     kwargs.setdefault("saturation", 1.0)
     rect = kwargs.pop("rect", (0, 0, 0.825, 1.0) if legend_orientation == "vertical" else (0, 0, 1, 0.925))
+    tight_layout = kwargs.pop("tight_layout", True)
 
     if isinstance(features, list):
         features = {f: [f] if isinstance(f, str) else f for f in features}
 
     axs: List[plt.Axes] = kwargs.pop("axs", kwargs.pop("ax", None))
     fig, axs = _plot_get_fig_ax_list(features, axs, **kwargs)
 
@@ -539,15 +535,15 @@
             labels,
             rect=rect,
             legend_loc=legend_loc,
             legend_fontsize=legend_fontsize,
             legend_orientation=legend_orientation,
             legend_title=legend_title,
         )
-    if kwargs.pop("tight_layout", True):
+    if tight_layout:
         fig.tight_layout(rect=rect)
     return fig, axs
 
 
 def _multi_feature_boxplot_get_order(order: Union[Dict[str, Sequence[str]], Sequence[str]], key: str):
     if isinstance(order, dict):
         return order[key]
@@ -598,19 +594,16 @@
     return sns.pairplot(data=data.reset_index(), **kwargs)
 
 
 def _get_df_lineplot(data: pd.DataFrame, x: str, y: str, hue: str, order: Sequence[str]) -> pd.DataFrame:
     if "mean" in data.columns and "se" in data.columns:
         m_se = data
     else:
-        if hue is None:
-            group_cols = [x]
-        else:
-            group_cols = [x, hue]
-        m_se = data[group_cols + [y]].groupby(group_cols).agg([np.mean, se])[y]
+        group_cols = [x] if hue is None else [x, hue]
+        m_se = data[[*group_cols, y]].groupby(group_cols).agg([np.mean, se])[y]
     if order is not None:
         m_se = m_se.reindex(order, level=0)
     return m_se
 
 
 def _set_legend_errorbar(**kwargs):
     legend_fontsize = kwargs.get("legend_fontsize", "small")
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/_utils.py` & `biopsykit-0.9.0/src/biopsykit/protocols/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Utility functions for the ``biopsykit.protocols`` module."""
 from typing import Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
-from pandas._libs.lib import is_timedelta_or_timedelta64_array
-
 from biopsykit.utils._datatype_validation_helper import _assert_len_list
 from biopsykit.utils.datatype_helper import SalivaMeanSeDataFrame
 from biopsykit.utils.exceptions import ValidationError
+from pandas._libs.lib import is_timedelta_or_timedelta64_array
 
 
 def _get_sample_times(
     saliva_data: Union[Dict[str, SalivaMeanSeDataFrame], SalivaMeanSeDataFrame],
     sample_times: Union[Sequence[int], Dict[str, Sequence[int]]],
     test_times: Sequence[int],
     sample_times_absolute: Optional[bool] = False,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/base.py` & `biopsykit-0.9.0/src/biopsykit/protocols/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Module implementing a base class to represent psychological protocols."""
 import json
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Iterable, Optional, Sequence, Tuple, Type, Union
 
+import biopsykit.protocols.plotting as plot
 import matplotlib.pyplot as plt
 import pandas as pd
-from tqdm.auto import tqdm
-
-import biopsykit.protocols.plotting as plot
 from biopsykit.io import write_pandas_dict_excel
 from biopsykit.protocols._utils import _check_sample_times_match, _get_sample_times
 from biopsykit.signals.ecg import EcgProcessor
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_is_dtype
 from biopsykit.utils._types import T, path_t
 from biopsykit.utils.data_processing import (
     add_subject_conditions,
@@ -34,14 +32,15 @@
     SubjectDataDict,
     is_hr_subject_data_dict,
     is_saliva_mean_se_dataframe,
     is_saliva_raw_dataframe,
     is_subject_data_dict,
 )
 from biopsykit.utils.exceptions import ValidationError
+from tqdm.auto import tqdm
 
 
 class BaseProtocol:  # pylint:disable=too-many-public-methods
     """Base class representing a psychological protocol and data collected within a study."""
 
     def __init__(
         self,
@@ -307,15 +306,15 @@
         """
         # ensure pathlib
         file_path = Path(file_path)
         _assert_file_extension(file_path, ".json")
 
         to_export = ["name", "structure", "test_times"]
         json_dict = {key: self.__dict__[key] for key in to_export}
-        with open(file_path, "w+", encoding="utf-8") as fp:
+        with file_path.open(mode="w+", encoding="utf-8") as fp:
             json.dump(json_dict, fp)
 
     @classmethod
     def from_file(cls: Type[T], file_path: path_t) -> T:
         """Load serialized ``Protocol`` object from file.
 
         Parameters
@@ -328,15 +327,15 @@
         instance of :class:`~biopsykit.protocols.BaseProtocol`
             ``Protocol`` instance
 
         """
         file_path = Path(file_path)
         _assert_file_extension(file_path, ".json")
 
-        with open(file_path, encoding="utf-8") as fp:
+        with file_path.open(encoding="utf-8") as fp:
             json_dict = json.load(fp)
             return cls(**json_dict)
 
     def add_saliva_data(
         self,
         saliva_data: Union[SalivaRawDataFrame, Dict[str, SalivaRawDataFrame]],
         saliva_type: Optional[Union[str, Sequence[str]]] = None,
@@ -539,15 +538,15 @@
             data_dict = BaseProtocol._reindex_df(data_dict, param)
 
         self.hr_results[result_id] = data_dict
 
     @staticmethod
     def _reindex_df(data: pd.DataFrame, param: Dict[str, Any]) -> pd.DataFrame:
         if not isinstance(param, dict):
-            raise ValueError(
+            raise TypeError(
                 "If 'reindex' is 'True', a dictionary with dataframe levels as keys "
                 "and new index orders as values is expected!"
             )
         for level, index_values in param.items():
             data = data.reindex(index_values, level=level)
         return data
 
@@ -941,16 +940,16 @@
                 hrv_columns = hrv_baseline.columns
             hrv_baseline = hrv_baseline[hrv_columns]
 
             for phase, dict_hrv_phase in hrv_data_dict.items():
                 if isinstance(dict_hrv_phase, dict):
                     dict_hrv_subphases = {}
                     for subphase, df_hrv in dict_hrv_phase.items():
-                        df_hrv = df_hrv[hrv_columns]
-                        hrv_above_bl = (df_hrv > hrv_baseline.mean()).sum() / len(df_hrv) * 100
+                        df_hrv_slice = df_hrv[hrv_columns]
+                        hrv_above_bl = (df_hrv_slice > hrv_baseline.mean()).sum() / len(df_hrv_slice) * 100
                         dict_hrv_subphases[subphase] = hrv_above_bl
                     dict_hrv[phase] = pd.concat(dict_hrv_subphases, names=["subphase"])
                 else:
                     hrv_above_bl = (dict_hrv_phase > hrv_baseline.mean()).sum() / len(dict_hrv_phase) * 100
                     dict_hrv[phase] = hrv_above_bl
 
             result_dict[subject_id] = pd.concat(dict_hrv, names=["phase"])
@@ -1073,26 +1072,26 @@
         # ensure pathlib
         base_path = Path(base_path)
         if not base_path.is_dir():
             raise ValueError("'base_path' must be a directory!")
         if prefix is None:
             prefix = self.name.lower().replace(" ", "_")
         for key, data in result_dict.items():
-            file_name = "{}_{}.csv".format(prefix, key)
+            file_name = f"{prefix}_{key}.csv"
             data.to_csv(base_path.joinpath(file_name))
 
     def _export_ensemble(self, base_path: path_t, prefix: str, result_dict: Dict[str, Dict[str, pd.DataFrame]]):
         # ensure pathlib
         base_path = Path(base_path)
         if not base_path.is_dir():
             raise ValueError("'base_path' must be a directory!")
         if prefix is None:
             prefix = self.name.lower().replace(" ", "_")
         for key, data in result_dict.items():
-            file_name = "{}_{}.xlsx".format(prefix, key)
+            file_name = f"{prefix}_{key}.xlsx"
             write_pandas_dict_excel(data, base_path.joinpath(file_name))
 
     def get_hrv_results(self, result_id: str) -> pd.DataFrame:
         """Return heart rate variability processing ensemble.
 
         Heart rate variability ensemble can be computed by calling
         :meth:`~biopsykit.protocols.BaseProtocol.compute_hrv_results`.
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/car.py` & `biopsykit-0.9.0/src/biopsykit/protocols/car.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Module representing the Cortisol Awakening Response (CAR) protocol."""
 from typing import Optional, Tuple
 
 import matplotlib.pyplot as plt
-
 from biopsykit.plotting import lineplot
 from biopsykit.protocols import BaseProtocol
 from biopsykit.utils.datatype_helper import is_saliva_raw_dataframe
 
 
 class CAR(BaseProtocol):
     """Class representing psychological protocols for assessing the cortisol awakening response (CAR)."""
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/cft.py` & `biopsykit-0.9.0/src/biopsykit/protocols/cft.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from typing import Any, Dict, Optional, Tuple, Union
 
 import matplotlib.patches as mpatch
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from fau_colors import colors_all
-
 from biopsykit.protocols import BaseProtocol
 from biopsykit.signals.ecg.plotting import hr_plot
 from biopsykit.utils.exceptions import FeatureComputationError
+from fau_colors import colors_all
 
 
 class CFT(BaseProtocol):
     """Class representing the Cold Face Test (CFT) and data collected while conducting the CFT."""
 
     def __init__(
         self,
@@ -475,15 +474,15 @@
         # get time points in seconds
         # TODO check index type
         idx_s = df_hr_cft.index.view(np.int64) / 1e9
         idx_s = idx_s - idx_s[0]
 
         # apply a 2nd degree polynomial fit
         poly = np.polyfit(idx_s, np.squeeze(df_hr_cft.values), deg=2)
-        return {"poly_fit_a{}".format(i): p for i, p in enumerate(reversed(poly))}
+        return {f"poly_fit_a{i}": p for i, p in enumerate(reversed(poly))}
 
     def _sanitize_cft_input(
         self,
         data: pd.DataFrame,
         is_cft_interval: Optional[bool] = False,
         compute_baseline: Optional[bool] = True,
         hr_baseline: Optional[float] = None,
@@ -491,15 +490,15 @@
         """Sanitize CFT input.
 
         Most functions for computing CFT parameter expect multiple possible combinations of input parameter:
 
         * Either data over the whole duration of the CFT procedure (Baseline, CFT, Recovery):
           Then, the CFT Interval will be extracted and Baseline heart rate will be computed based on the
           ``cft_start`` and ``cft_duration`` parameters of the ``CFT`` object
-          (``compute_baseline`` must then be set to ``True`` – the default)
+          (``compute_baseline`` must then be set to ``True`` - the default)
         * Or only data during the CFT interval (``is_cft_interval`` must be set to ``True``).
           Then, the Baseline heart rate muse be explicitly provided via ``hr_baseline`` parameter and
           ``compute_baseline`` must be set to ``False``
 
         This function sanitizes the input and, independent from the input, always returns a tuple with the data cut
         to the CFT Interval and the mean heart rate during the Baseline Interval.
 
@@ -520,29 +519,26 @@
 
         Returns
         -------
         data_cft : :class:`~pandas.DataFrame`
             heart rate data during CFT Interval
 
         """
-        if is_cft_interval:
-            data_cft = data
-        else:
-            # extract CFT interval
-            data_cft = self.extract_cft_interval(data)
+        # extract CFT interval if whole data is passed
+        data_cft = data if is_cft_interval else self.extract_cft_interval(data)
 
         if compute_baseline:
             if is_cft_interval:
                 raise ValueError(
                     "`compute_baseline` must be set to False and `baseline_hr` be supplied "
                     "when only CFT data is passed (`is_cft_interval` is `True`)"
                 )
             hr_baseline = self.baseline_hr(data)
         else:
-            if hr_baseline is None:
+            if hr_baseline is None:  # noqa: PLR5501
                 raise ValueError("`baseline_hr` must be supplied as parameter when `compute_baseline` is set to False!")
 
         return data_cft, hr_baseline
 
     def cft_plot(
         self,
         data: pd.DataFrame,
@@ -598,19 +594,19 @@
 
         if not kwargs.get("plot_datetime_index", False):
             data.index = (data.index - data.index[0]).view(np.int64) / 1e9
 
         times_dict = self._cft_plot_get_cft_times(data, time_baseline, time_recovery)
         df_plot = self._cft_plot_extract_plot_interval(data, times_dict)
 
-        bbox = dict(
-            fc=(1, 1, 1, plt.rcParams["legend.framealpha"]),
-            ec=plt.rcParams["legend.edgecolor"],
-            boxstyle="round",
-        )
+        bbox = {
+            "fc": (1, 1, 1, plt.rcParams["legend.framealpha"]),
+            "ec": plt.rcParams["legend.edgecolor"],
+            "boxstyle": "round",
+        }
 
         hr_plot(heart_rate=df_plot, ax=ax, plot_mean=False)
         self._cft_plot_add_phase_annotations(ax, times_dict, **kwargs)
         self._cft_plot_add_param_annotations(data, cft_params, times_dict, ax, bbox, **kwargs)
 
         self._cft_plot_style_axis(data, ax, **kwargs)
 
@@ -753,18 +749,15 @@
             brady_y,
             color=color,
             marker="o",
             markersize=7,
         )
 
         # Peak Bradycardia hline
-        if isinstance(data.index, pd.DatetimeIndex):
-            xmax = brady_x + pd.Timedelta(seconds=20)
-        else:
-            xmax = brady_x + 20
+        xmax = brady_x + pd.Timedelta(seconds=20) if isinstance(data.index, pd.DatetimeIndex) else brady_x + 20
 
         ax.hlines(
             y=brady_y,
             xmin=brady_x,
             xmax=xmax,
             ls="--",
             lw=2,
@@ -778,21 +771,21 @@
         else:
             brady_x_offset = brady_x + 10
 
         ax.annotate(
             "",
             xy=(brady_x_offset, brady_y),
             xytext=(brady_x_offset, hr_baseline),
-            arrowprops=dict(
-                arrowstyle="<->",
-                lw=2,
-                color=color_adjust,
-                shrinkA=0.0,
-                shrinkB=0.0,
-            ),
+            arrowprops={
+                "arrowstyle": "<->",
+                "lw": 2,
+                "color": color_adjust,
+                "shrinkA": 0.0,
+                "shrinkB": 0.0,
+            },
         )
 
         # Peak Bradycardia Text
         ax.annotate(
             "$Peak_{CFT}$: " + "{:.1f} %".format(cft_params["peak_brady_percent"]),
             xy=(brady_x_offset, brady_y),
             xytext=(10, -5),
@@ -803,21 +796,21 @@
         )
 
         # Peak Bradycardia Latency arrow
         ax.annotate(
             "",
             xy=(cft_start, max_hr_cft),
             xytext=(brady_x, max_hr_cft),
-            arrowprops=dict(
-                arrowstyle="<->",
-                lw=2,
-                color=color,
-                shrinkA=0.0,
-                shrinkB=0.0,
-            ),
+            arrowprops={
+                "arrowstyle": "<->",
+                "lw": 2,
+                "color": color,
+                "shrinkA": 0.0,
+                "shrinkB": 0.0,
+            },
         )
 
         # Peak Bradycardia Latency Text
         ax.annotate(
             "$Latency_{CFT}$: " + "{:.1f} s".format(cft_params["peak_brady_latency"]),
             xy=(brady_x, max_hr_cft),
             xytext=(-7.5, 10),
@@ -867,31 +860,28 @@
             xmax=cft_end,
             ls="--",
             lw=2,
             color=getattr(colors_all, color_key),
             alpha=0.6,
         )
 
-        if isinstance(data.index, pd.DatetimeIndex):
-            x_offset = cft_end - pd.Timedelta(seconds=5)
-        else:
-            x_offset = cft_end - 5
+        x_offset = cft_end - pd.Timedelta(seconds=5) if isinstance(data.index, pd.DatetimeIndex) else cft_end - 5
 
         # Mean Bradycardia arrow
         ax.annotate(
             "",
             xy=(x_offset, mean_hr),
             xytext=(x_offset, cft_params["baseline_hr"]),
-            arrowprops=dict(
-                arrowstyle="<->",
-                lw=2,
-                color=getattr(colors_all, f"{color_key}_dark"),
-                shrinkA=0.0,
-                shrinkB=0.0,
-            ),
+            arrowprops={
+                "arrowstyle": "<->",
+                "lw": 2,
+                "color": getattr(colors_all, f"{color_key}_dark"),
+                "shrinkA": 0.0,
+                "shrinkB": 0.0,
+            },
         )
 
         # Mean Bradycardia Text
         ax.annotate(
             "$Mean_{CFT}$: " + "{:.1f} %".format(cft_params["mean_brady_percent"]),
             xy=(x_offset, mean_hr),
             xytext=(-5, -5),
@@ -935,21 +925,21 @@
         )
 
         # CFT Onset arrow
         ax.annotate(
             "",
             xy=(onset_x, onset_y),
             xytext=(cft_times["cft_start"], onset_y),
-            arrowprops=dict(
-                arrowstyle="<->",
-                lw=2,
-                color=color,
-                shrinkA=0.0,
-                shrinkB=0.0,
-            ),
+            arrowprops={
+                "arrowstyle": "<->",
+                "lw": 2,
+                "color": color,
+                "shrinkA": 0.0,
+                "shrinkB": 0.0,
+            },
         )
 
         # CFT Onset Text
         ax.annotate(
             "$Onset_{CFT}$: " + "{:.1f} s".format(cft_params["onset_latency"]),
             xy=(onset_x, onset_y),
             xytext=(-10, -10),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/mist.py` & `biopsykit-0.9.0/src/biopsykit/protocols/mist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Module representing the Montreal Imaging Stress Task (MIST) protocol."""
 from typing import Dict, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
-
 from biopsykit.protocols import BaseProtocol
 
 
 class MIST(BaseProtocol):
     """Class representing the Montreal Imaging Stress Task (MIST) protocol and data collected within a MIST study."""
 
     def __init__(
@@ -74,15 +73,15 @@
         >>> MIST(name="MIST", structure=structure)
 
 
         References
         ----------
         Dedovic, K., Renwick, R., Mahani, N. K., Engert, V., Lupien, S. J., & Pruessner, J. C. (2005).
         The Montreal Imaging Stress Task: Using functional imaging to investigate the effects of perceiving and
-        processing psychosocial stress in the human brain. *Journal of Psychiatry and Neuroscience*, 30(5), 319–325.
+        processing psychosocial stress in the human brain. *Journal of Psychiatry and Neuroscience*, 30(5), 319-325.
 
         """
         if name is None:
             name = "MIST"
 
         if structure is None:
             structure = {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/plotting.py` & `biopsykit-0.9.0/src/biopsykit/protocols/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 import matplotlib.patches as mpatch
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticks
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from fau_colors import cmaps, colors_all
-from matplotlib.legend_handler import HandlerTuple
-
 from biopsykit.plotting import feature_boxplot, lineplot, multi_feature_boxplot
 from biopsykit.protocols._utils import _get_sample_times
 from biopsykit.saliva.utils import _remove_s0
 from biopsykit.utils.data_processing import get_subphase_durations
 from biopsykit.utils.datatype_helper import (
     MeanSeDataFrame,
     MergedStudyDataDict,
@@ -23,14 +20,16 @@
     SalivaRawDataFrame,
     is_mean_se_dataframe,
     is_saliva_feature_dataframe,
     is_saliva_mean_se_dataframe,
     is_saliva_raw_dataframe,
 )
 from biopsykit.utils.exceptions import ValidationError
+from fau_colors import cmaps, colors_all
+from matplotlib.legend_handler import HandlerTuple
 
 _hr_ensemble_plot_params = {
     "linestyle": ["solid", "dashed", "dotted", "dashdot"],
     "ensemble_alpha": 0.4,
     "background_base_color": "#e0e0e0",
     "background_color": None,
     "background_alpha": 0.1,
@@ -312,15 +311,15 @@
         text=end_phase_text.format(phase),
         xy=(len(data), 0.85 - 0.075 * i),
         xytext=(-5, 0),
         xycoords=ax.get_xaxis_transform(),
         textcoords="offset points",
         ha="right",
         fontsize="small",
-        bbox=dict(facecolor="#e0e0e0", alpha=0.7, boxstyle="round"),
+        bbox={"facecolor": "#e0e0e0", "alpha": 0.7, "boxstyle": "round"},
         zorder=5,
     )
 
 
 def _hr_ensemble_plot_subphase_vspans(
     ax: plt.Axes, data: Dict[str, pd.DataFrame], subphases: Dict[str, Dict[str, int]], **kwargs
 ):
@@ -462,15 +461,15 @@
 
     # build x axis, axis limits and limits for phase spans
     dist = np.mean(np.ediff1d(x_vals))
     x_lims = np.append(x_vals, x_vals[-1] + dist)
     x_lims = x_lims - 0.5 * np.ediff1d(x_lims, to_end=dist)
 
     if "condition" in data.index.names:
-        data_grp = {key: df for key, df in data.groupby("condition")}  # pylint:disable=unnecessary-comprehension
+        data_grp = dict(tuple(data.groupby("condition")))
         order = kwargs.get("order", list(data_grp.keys()))
         data_grp = {key: data_grp[key] for key in order}
 
         for i, (key, df) in enumerate(data_grp.items()):
             _hr_mean_plot(df, x_vals, key, index=i, **kwargs)
     else:
         _hr_mean_plot(data, x_vals, "Data", index=0, **kwargs)
@@ -640,25 +639,22 @@
         lw=0,
     )
     ax.add_patch(p)
 
 
 def _hr_mean_get_x_spans(num_phases: int, num_subphases: Sequence[int]):
     if sum(num_subphases) == 0:
-        x_spans = list(zip([0] + list(range(0, num_phases)), list(range(0, num_phases))))
+        x_spans = list(zip([0, *list(range(0, num_phases))], list(range(0, num_phases))))
     else:
-        x_spans = list(zip([0] + list(np.cumsum(num_subphases)), list(np.cumsum(num_subphases))))
+        x_spans = list(zip([0, *list(np.cumsum(num_subphases))], list(np.cumsum(num_subphases))))
     return x_spans
 
 
 def _hr_mean_get_x_vals(num_phases: int, num_subphases: Sequence[int]):
-    if sum(num_subphases) == 0:
-        x_vals = np.linspace(0, 10, num_phases)
-    else:
-        x_vals = np.linspace(0, 10, sum(num_subphases))
+    x_vals = np.linspace(0, 10, num_phases) if sum(num_subphases) == 0 else np.linspace(0, 10, sum(num_subphases))
     return x_vals
 
 
 def _hr_mean_get_phases_subphases(data: pd.DataFrame) -> Dict[str, Sequence[str]]:
     if "condition" in data.index.names:
         data = [value for key, value in data.groupby("condition")][0]
 
@@ -919,18 +915,15 @@
     ret = is_saliva_raw_dataframe(data, saliva_type, raise_exception=False)
     ret = ret or is_saliva_mean_se_dataframe(data, raise_exception=False)
     if not ret:
         raise ValidationError("'data' is expected to be either a SalivaRawDataFrame or a SalivaMeanSeDataFrame!")
 
 
 def _saliva_plot_get_plot_param(param: Union[Dict[str, str], str], key: str):
-    if isinstance(param, dict):
-        p = param[key]
-    else:
-        p = param
+    p = param[key] if isinstance(param, dict) else param
     return p
 
 
 def _saliva_plot_style_xaxis(xticks: Sequence[str], xaxis_tick_locator: mticks.Locator, ax: plt.Axes):
     if xticks is not None and xaxis_tick_locator is not None:
         ax.xaxis.set_major_locator(xaxis_tick_locator)
         ax.xaxis.set_ticks(xticks)
@@ -979,16 +972,16 @@
             prop={"size": legend_size},
         )
     else:
         handles = [ax.get_legend_handles_labels()[0] for ax in fig.get_axes()]
         handles = [h[0] for handle in handles for h in handle]
         labels = [ax.get_legend_handles_labels()[1] for ax in fig.get_axes()]
         labels = [
-            "{}: {}".format(_saliva_plot_params.get("legend_title")[b], " - ".join(l))
-            for b, l in zip(saliva_types, labels)
+            "{}: {}".format(_saliva_plot_params.get("legend_title")[b], " - ".join(label))
+            for b, label in zip(saliva_types, labels)
         ]
         ncol = len(handles)
 
         fig.legend(
             list(zip(handles[::2], handles[1::2])),
             labels,
             loc=legend_loc,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/protocols/tsst.py` & `biopsykit-0.9.0/src/biopsykit/protocols/tsst.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
         >>>     "Post": None
         >>> }
         >>> TSST(name="TSST", structure=structure)
 
 
         References
         ----------
-        Kirschbaum, C., Pirke, K.-M., & Hellhammer, D. H. (1993). The “Trier Social Stress Test” – A Tool for
-        Investigating Psychobiological Stress Responses in a Laboratory Setting. *Neuropsychobiology*, 28, 76–81.
+        Kirschbaum, C., Pirke, K.-M., & Hellhammer, D. H. (1993). The “Trier Social Stress Test” - A Tool for
+        Investigating Psychobiological Stress Responses in a Laboratory Setting. *Neuropsychobiology*, 28, 76-81.
         https://doi.org/10.1159/000119004
 
         """
         if name is None:
             name = "TSST"
         if structure is None:
             structure = {"Part1": None, "TSST": {"Preparation": 300, "Talk": 300, "Math": 300}, "Part2": None}
```

### Comparing `biopsykit-0.8.1/src/biopsykit/questionnaires/__init__.py` & `biopsykit-0.9.0/src/biopsykit/questionnaires/__init__.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/questionnaires/questionnaires.py` & `biopsykit-0.9.0/src/biopsykit/questionnaires/questionnaires.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 (as list of ints) can be passed to the ``subscales`` parameter.
 
 .. warning::
     Column indices in ``subscales`` are assumed to start at 1 (instead of 0) to avoid confusion with
     questionnaire item columns, which typically also start with index 1!
 
 """
-from typing import Dict, Optional, Sequence, Union
+from typing import Dict, Literal, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
-from typing_extensions import Literal
-
 from biopsykit.questionnaires.utils import (
     _compute_questionnaire_subscales,
     _invert_subscales,
     bin_scale,
     invert,
     to_idx,
 )
@@ -95,15 +93,15 @@
 
     # Sleep Duration: Question 4
     sd = data.filter(regex="04").iloc[:, 0]
 
     # Sleep Latency: Question 2
     sl = data.filter(regex="02").iloc[:, 0]
     # Bin scale: 0-15 = 0, 16-30 = 1, 31-60 = 2, >=61 = 3
-    bin_scale(sl, bins=[0, 15, 30, 60], last_max=True, inplace=True)
+    sl = bin_scale(sl, bins=[0, 15, 30, 60], last_max=True, inplace=False)
 
     data = data.drop(columns=data.filter(regex="0[1234]"))
     data = data.drop(columns=data.filter(regex="05j_text"))
 
     _assert_value_range(data, score_range)
 
     # Subjective Sleep Quality
@@ -189,15 +187,15 @@
     :exc:`~biopsykit.utils.exceptions.ValueRangeError`
         if values are not within the required score range
 
 
     References
     ----------
     Appels, A., Höppener, P., & Mulder, P. (1987). A questionnaire to assess premonitory symptoms of myocardial
-    infarction. *International Journal of Cardiology*, 17(1), 15–24. https://doi.org/10.1016/0167-5273(87)90029-5
+    infarction. *International Journal of Cardiology*, 17(1), 15-24. https://doi.org/10.1016/0167-5273(87)90029-5
 
     """
     score_name = "MVES"
     score_range = [0, 2]
 
     # create copy of data
     data = data.copy()
@@ -517,15 +515,15 @@
 
     _assert_value_range(data, score_range)
 
     # Reverse scores 4, 5, 7, 8
     data = invert(data, cols=to_idx([4, 5, 7, 8]), score_range=score_range)
 
     pss_data = _compute_questionnaire_subscales(data, score_name, subscales)
-    pss_data["{}_Total".format(score_name)] = data.sum(axis=1)
+    pss_data[f"{score_name}_Total"] = data.sum(axis=1)
 
     return pd.DataFrame(pss_data, index=data.index)
 
 
 def cesd(data: pd.DataFrame, columns: Optional[Union[Sequence[str], pd.Index]] = None) -> pd.DataFrame:
     """Compute the **Center for Epidemiological Studies Depression Scale (CES-D)**.
 
@@ -562,15 +560,15 @@
     :exc:`~biopsykit.utils.exceptions.ValueRangeError`
         if values are not within the required score range
 
 
     References
     ----------
     Radloff, L. S. (1977). The CES-D Scale: A Self-Report Depression Scale for Research in the General Population.
-    Applied Psychological Measurement, 1(3), 385–401. https://doi.org/10.1177/014662167700100306
+    Applied Psychological Measurement, 1(3), 385-401. https://doi.org/10.1177/014662167700100306
 
     """
     score_name = "CESD"
     score_range = [0, 3]
 
     # create copy of data
     data = data.copy()
@@ -585,15 +583,15 @@
 
     # Reverse scores 4, 8, 12, 16
     data = invert(data, cols=to_idx([4, 8, 12, 16]), score_range=score_range)
     return pd.DataFrame(data.sum(axis=1), columns=[score_name])
 
 
 def ads_l(data: pd.DataFrame, columns: Optional[Union[Sequence[str], pd.Index]] = None) -> pd.DataFrame:
-    """Compute the **Allgemeine Depressionsskala - Langform (ADS-L)** (General Depression Scale – Long Version).
+    """Compute the **Allgemeine Depressionsskala - Langform (ADS-L)** (General Depression Scale - Long Version).
 
     The General Depression Scale (ADS) is a self-report instrument that can be used to assess the impairment caused by
     depressive symptoms within the last week. Emotional, motivational, cognitive, somatic as well as motor symptoms are
     assessed, motivational, cognitive, somatic, and motor/interactional complaints.
 
     .. note::
         This implementation assumes a score range of [0, 4].
@@ -1397,15 +1395,15 @@
         subscales = ["Partner", "Parent", "Child"]
 
     if isinstance(subscales, str):
         subscales = [subscales]
 
     _assert_value_range(data, score_range)
 
-    lsq_data = {"{}_{}".format(score_name, subscale): data.filter(like=subscale).sum(axis=1) for subscale in subscales}
+    lsq_data = {f"{score_name}_{subscale}": data.filter(like=subscale).sum(axis=1) for subscale in subscales}
 
     return pd.DataFrame(lsq_data, index=data.index)
 
 
 def ctq(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
@@ -1418,15 +1416,15 @@
     * ``PhysicalAbuse``: [9, 11, 12, 15, 17]
     * ``SexualAbuse``: [20, 21, 23, 24, 27]
     * ``EmotionalNeglect``: [5, 7, 13, 19, 28]
     * ``PhysicalNeglect``: [1, 2, 4, 6, 26]
     * ``EmotionalAbuse``: [3, 8, 14, 18, 25]
 
     Additionally, three items assess the validity of the responses (high scores on these items could be grounds for
-    exclusion of a given participants’ responses):
+    exclusion of a given participants` responses):
 
     * ``Validity``: [10, 16, 22]
 
     .. note::
         This implementation assumes a score range of [1, 5].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
@@ -1573,15 +1571,15 @@
 
     return pd.DataFrame(data.sum(axis=1), columns=[score_name])
 
 
 def purpose_life(data: pd.DataFrame, columns: Optional[Union[Sequence[str], pd.Index]] = None) -> pd.DataFrame:
     """Compute the **Purpose in Life** questionnaire.
 
-    Purpose in life refers to the psychological tendency to derive meaning from life’s experiences
+    Purpose in life refers to the psychological tendency to derive meaning from life`s experiences
     and to possess a sense of intentionality and goal directedness that guides behavior.
     Higher scores indicate greater purpose in life.
 
     .. note::
         This implementation assumes a score range of [0, 4].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
@@ -1684,17 +1682,17 @@
 def besaa(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[Union[int, str]]]] = None,
 ) -> pd.DataFrame:
     """Compute the **Body-Esteem Scale for Adolescents and Adults (BESAA)**.
 
-    Body Esteem refers to self-evaluations of one’s body or appearance. The BESAA is based on
-    the idea that feelings about one’s weight can be differentiated from feelings about one’s general appearance,
-    and that one’s own opinions may be differentiated from the opinions attributed to others.
+    Body Esteem refers to self-evaluations of one`s body or appearance. The BESAA is based on
+    the idea that feelings about one`s weight can be differentiated from feelings about one`s general appearance,
+    and that one`s own opinions may be differentiated from the opinions attributed to others.
     Higher scores indicate higher body esteem.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
     * ``Appearance``: [1, 6, 9, 7, 11, 13, 15, 17, 21, 23]
     * ``Weight``: [3, 4, 8, 10, 16, 18, 19, 22]
     * ``Attribution``: [2, 5, 12, 14, 20]
@@ -1969,15 +1967,15 @@
         ) / 2
 
     if all(s in subscales for s in ["SelfConcept", "ControlExp"]):
         pasa_data[score_name + "_Secondary"] = (
             pasa_data[score_name + "_SelfConcept"] + pasa_data[score_name + "_ControlExp"]
         ) / 2
 
-    if all("{}_{}".format(score_name, s) in pasa_data for s in ["Primary", "Secondary"]):
+    if all(f"{score_name}_{s}" in pasa_data for s in ["Primary", "Secondary"]):
         pasa_data[score_name + "_StressComposite"] = (
             pasa_data[score_name + "_Primary"] - pasa_data[score_name + "_Secondary"]
         )
 
     return pd.DataFrame(pasa_data, index=data.index)
 
 
@@ -2138,15 +2136,15 @@
     # create copy of data
     data = data.copy()
 
     if language is None:
         language = "english"
 
     if language not in supported_versions:
-        raise ValueError("questionnaire_version must be one of {}, not {}.".format(supported_versions, language))
+        raise ValueError(f"questionnaire_version must be one of {supported_versions}, not {language}.")
 
     if columns is not None:
         # if columns parameter is supplied: slice columns from dataframe
         _assert_has_columns(data, [columns])
         data = data.loc[:, columns]
 
     _assert_num_columns(data, 20)
@@ -2303,22 +2301,22 @@
         "1": [2, 3, 6, 8, 10],
         "3": [2, 4, 5, 7, 9],
         "5": [3, 4, 5, 9, 10],
         "7": [1, 5, 6, 7, 9],
     }
     idx_kov = {key: np.array(val) for key, val in idx_kov.items()}
     idx_vig = {key: np.setdiff1d(np.arange(1, 11), np.array(val), assume_unique=True) for key, val in idx_kov.items()}
-    abi_kov, abi_vig = [
+    abi_kov, abi_vig = (
         pd.concat(
             [abi_raw.loc[:, key].iloc[:, idx[key] - 1] for key in idx],
             axis=1,
             keys=idx_kov.keys(),
         )
         for idx in [idx_kov, idx_vig]
-    ]
+    )
 
     abi_data = {
         score_name + "_KOV_T": abi_kov.sum(axis=1),
         score_name + "_VIG_T": abi_vig.sum(axis=1),
         score_name + "_KOV_P": abi_kov.loc[:, ["2", "4", "6", "8"]].sum(axis=1),
         score_name + "_VIG_P": abi_vig.loc[:, ["2", "4", "6", "8"]].sum(axis=1),
         score_name + "_KOV_E": abi_kov.loc[:, ["1", "3", "5", "7"]].sum(axis=1),
@@ -2345,15 +2343,15 @@
     enduring tendency to experience anxiety and depression.
 
     The STADI can either be computed only for state, only for trait, or for state and trait.
 
     The state and trait scales both consist of the subscales with the item indices
     (count-by-one, i.e., the first question has the index 1!):
 
-    * Emotionality (Aufgeregtheit - affektive Komponente – ``AU``): [1, 5, 9, 13, 17]
+    * Emotionality (Aufgeregtheit - affektive Komponente - ``AU``): [1, 5, 9, 13, 17]
     * Worry (Besorgnis - kognitive Komponente - ``BE``): [2, 6, 10, 14, 18]
     * Anhedonia (Euthymie - positive Stimmung - ``EU``): [3, 7, 11, 15, 19]
     * Dysthymia (Dysthymie - depressive Stimmung - ``DY``): [4, 8, 12, 16, 20]
 
     .. note::
         This implementation assumes a score range of [1, 4].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
@@ -2433,56 +2431,52 @@
 
     # split into n subitems (either "State", "Trait" or "State and Trait")
     items = np.split(data, len(stadi_type), axis=1)
     data = pd.concat(items, keys=stadi_type, axis=1)
 
     stadi_data = {}
     for st in stadi_type:
-        stadi_data.update(_compute_questionnaire_subscales(data[st], "{}_{}".format(score_name, st), subscales))
-        if all("{}_{}_{}".format(score_name, st, subtype) in stadi_data for subtype in ["AU", "BE"]):
+        stadi_data.update(_compute_questionnaire_subscales(data[st], f"{score_name}_{st}", subscales))
+        if all(f"{score_name}_{st}_{subtype}" in stadi_data for subtype in ["AU", "BE"]):
             stadi_data.update(
                 {
-                    "{}_{}_Anxiety".format(score_name, st): stadi_data["{}_{}_AU".format(score_name, st)]
-                    + stadi_data["{}_{}_BE".format(score_name, st)]
+                    f"{score_name}_{st}_Anxiety": stadi_data[f"{score_name}_{st}_AU"]
+                    + stadi_data[f"{score_name}_{st}_BE"]
                 }
             )
 
-        if all("{}_{}_{}".format(score_name, st, subtype) in stadi_data for subtype in ["EU", "DY"]):
+        if all(f"{score_name}_{st}_{subtype}" in stadi_data for subtype in ["EU", "DY"]):
             stadi_data.update(
                 {
-                    "{}_{}_Depression".format(score_name, st): stadi_data["{}_{}_EU".format(score_name, st)]
-                    + stadi_data["{}_{}_DY".format(score_name, st)]
+                    f"{score_name}_{st}_Depression": stadi_data[f"{score_name}_{st}_EU"]
+                    + stadi_data[f"{score_name}_{st}_DY"]
                 }
             )
 
-        if all("{}_{}_{}".format(score_name, st, subtype) in stadi_data for subtype in ["Anxiety", "Depression"]):
+        if all(f"{score_name}_{st}_{subtype}" in stadi_data for subtype in ["Anxiety", "Depression"]):
             stadi_data.update(
                 {
-                    "{}_{}_Total".format(score_name, st): stadi_data["{}_{}_Anxiety".format(score_name, st)]
-                    + stadi_data["{}_{}_Depression".format(score_name, st)]
+                    f"{score_name}_{st}_Total": stadi_data[f"{score_name}_{st}_Anxiety"]
+                    + stadi_data[f"{score_name}_{st}_Depression"]
                 }
             )
 
     df_stadi = pd.DataFrame(stadi_data, index=data.index)
     return df_stadi
 
 
 def _get_stadi_type(stadi_type: str) -> Sequence[str]:
-    if stadi_type is None:
-        stadi_type = ["State", "Trait"]
-    elif stadi_type == "state_trait":
+    if stadi_type is None or stadi_type == "state_trait":
         stadi_type = ["State", "Trait"]
     elif stadi_type == "state":
         stadi_type = ["State"]
     elif stadi_type == "trait":
         stadi_type = ["Trait"]
     else:
-        raise ValueError(
-            "Invalid 'stadi_type'! Must be one of 'state_trait', 'state', or 'trait', not {}.".format(stadi_type)
-        )
+        raise ValueError(f"Invalid 'stadi_type'! Must be one of 'state_trait', 'state', or 'trait', not {stadi_type}.")
     return stadi_type
 
 
 def svf_120(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
@@ -2492,34 +2486,34 @@
     The stress processing questionnaire enables the assessment of coping or processing measures in stressful
     situations.  The SVF is not a singular test instrument, but rather an inventory of methods that relate to various
     aspects of stress processing and coping and from which individual procedures can be selected depending on
     the study objective/question.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Trivialization/Minimalization (Bagatellisierung – ``Bag``): [10, 31, 50, 67, 88, 106]
-    * De-Emphasis by Comparison with Others (Herunterspielen – ``Her``): [17, 38, 52, 77, 97, 113]
-    * Rejection of Guilt (Schuldabwehr – ``Schab``): [5, 30, 43, 65, 104, 119]
-    * Distraction/Deflection from a Situation (Ablenkung – ``Abl``): [1, 20, 45, 86, 101, 111]
-    * Vicarious Satisfaction (Ersatzbefriedigung –``Ers``): [22, 36, 64, 74, 80, 103]
-    * Search for Self-Affirmation (Selbstbestätigung – ``Sebest``): [34, 47, 59, 78, 95, 115]
-    * Relaxation (Entspannung –``Entsp``): [12, 28, 58, 81, 99, 114]
-    * Attempt to Control Situation (Situationskontrolle – ``Sitkon``): [11, 18, 39, 66, 91, 116]
-    * Response Control (Reaktionskontrolle – ``Rekon``): [2, 26, 54, 68, 85, 109]
-    * Positive Self-Instruction (Positive Selbstinstruktion – ``Posi``): [15, 37, 56, 71, 83, 96]
-    * Need for Social Support (Soziales Unterstützungsbedürfnis – ``Sozube``): [3, 21, 42, 63, 84, 102]
-    * Avoidance Tendencies (Vermeidung – ``Verm``): [8, 29, 48, 69, 98, 118]
-    * Escapist Tendencies (Flucht – ``Flu``): [14, 24, 40, 62, 73, 120]
-    * Social Isolation (Soziale Abkapselung – ``Soza``): [6, 27, 49, 76, 92, 107]
-    * Mental Perseveration (Gedankliche Weiterbeschäftigung – ``Gedw``): [16, 23, 55, 72, 100, 110]
-    * Resignation (Resignation – ``Res``): [4, 32, 46, 60, 89, 105]
-    * Self-Pity (Selbstbemitleidung – ``Selmit``): [13, 41, 51, 79, 94, 117]
-    * Self-Incrimination (Selbstbeschuldigung – ``Sesch``): [9, 25, 35, 57, 75, 87]
-    * Aggression (Aggression – ``Agg``): [33, 44, 61, 82, 93, 112]
-    * Medicine-Taking (Pharmakaeinnahme – ``Pha``): [7, 19, 53, 70, 90, 108]
+    * Trivialization/Minimalization (Bagatellisierung - ``Bag``): [10, 31, 50, 67, 88, 106]
+    * De-Emphasis by Comparison with Others (Herunterspielen - ``Her``): [17, 38, 52, 77, 97, 113]
+    * Rejection of Guilt (Schuldabwehr - ``Schab``): [5, 30, 43, 65, 104, 119]
+    * Distraction/Deflection from a Situation (Ablenkung - ``Abl``): [1, 20, 45, 86, 101, 111]
+    * Vicarious Satisfaction (Ersatzbefriedigung -``Ers``): [22, 36, 64, 74, 80, 103]
+    * Search for Self-Affirmation (Selbstbestätigung - ``Sebest``): [34, 47, 59, 78, 95, 115]
+    * Relaxation (Entspannung -``Entsp``): [12, 28, 58, 81, 99, 114]
+    * Attempt to Control Situation (Situationskontrolle - ``Sitkon``): [11, 18, 39, 66, 91, 116]
+    * Response Control (Reaktionskontrolle - ``Rekon``): [2, 26, 54, 68, 85, 109]
+    * Positive Self-Instruction (Positive Selbstinstruktion - ``Posi``): [15, 37, 56, 71, 83, 96]
+    * Need for Social Support (Soziales Unterstützungsbedürfnis - ``Sozube``): [3, 21, 42, 63, 84, 102]
+    * Avoidance Tendencies (Vermeidung - ``Verm``): [8, 29, 48, 69, 98, 118]
+    * Escapist Tendencies (Flucht - ``Flu``): [14, 24, 40, 62, 73, 120]
+    * Social Isolation (Soziale Abkapselung - ``Soza``): [6, 27, 49, 76, 92, 107]
+    * Mental Perseveration (Gedankliche Weiterbeschäftigung - ``Gedw``): [16, 23, 55, 72, 100, 110]
+    * Resignation (Resignation - ``Res``): [4, 32, 46, 60, 89, 105]
+    * Self-Pity (Selbstbemitleidung - ``Selmit``): [13, 41, 51, 79, 94, 117]
+    * Self-Incrimination (Selbstbeschuldigung - ``Sesch``): [9, 25, 35, 57, 75, 87]
+    * Aggression (Aggression - ``Agg``): [33, 44, 61, 82, 93, 112]
+    * Medicine-Taking (Pharmakaeinnahme - ``Pha``): [7, 19, 53, 70, 90, 108]
 
     .. note::
         This implementation assumes a score range of [1, 5].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
     .. warning::
@@ -2615,17 +2609,15 @@
             "Posi",
         ),
         "NegGesamt": ("Flu", "Soza", "Gedw", "Res", "Selmit", "Sesch"),
     }
 
     for name, scale_items in meta_scales.items():
         if all(scale in subscales for scale in scale_items):
-            svf_data["{}_{}".format(score_name, name)] = svf_data[
-                ["{}_{}".format(score_name, s) for s in scale_items]
-            ].mean(axis=1)
+            svf_data[f"{score_name}_{name}"] = svf_data[[f"{score_name}_{s}" for s in scale_items]].mean(axis=1)
 
     return svf_data
 
 
 def svf_42(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
@@ -2636,34 +2628,34 @@
     The stress processing questionnaire enables the assessment of coping or processing measures in stressful
     situations.  The SVF is not a singular test instrument, but rather an inventory of methods that relate to various
     aspects of stress processing and coping and from which individual procedures can be selected depending on
     the study objective/question.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Trivialization/Minimalization (Bagatellisierung – ``Bag``): [7, 22]
-    * De-Emphasis by Comparison with Others (Herunterspielen – ``Her``): [11, 35]
-    * Rejection of Guilt (Schuldabwehr – ``Schab``): [2, 34]
-    * Distraction/Deflection from a Situation (Ablenkung – ``Abl``): [1, 32]
-    * Vicarious Satisfaction (Ersatzbefriedigung –``Ers``): [12, 42]
-    * Search for Self-Affirmation (Selbstbestätigung – ``Sebest``): [19, 37]
-    * Relaxation (Entspannung –``Entsp``): [13, 26]
-    * Attempt to Control Situation (Situationskontrolle – ``Sitkon``): [4, 23]
-    * Response Control (Reaktionskontrolle – ``Rekon``): [17, 33]
-    * Positive Self-Instruction (Positive Selbstinstruktion – ``Posi``): [9, 24]
-    * Need for Social Support (Soziales Unterstützungsbedürfnis – ``Sozube``): [14, 27]
-    * Avoidance Tendencies (Vermeidung – ``Verm``): [6, 30]
-    * Escapist Tendencies (Flucht – ``Flu``): [16, 40]
-    * Social Isolation (Soziale Abkapselung – ``Soza``): [20, 29]
-    * Mental Perseveration (Gedankliche Weiterbeschäftigung – ``Gedw``): [10, 25]
-    * Resignation (Resignation – ``Res``): [38, 15]
-    * Self-Pity (Selbstbemitleidung – ``Selmit``): [18, 28]
-    * Self-Incrimination (Selbstbeschuldigung – ``Sesch``): [8, 31]
-    * Aggression (Aggression – ``Agg``): [21, 36]
-    * Medicine-Taking (Pharmakaeinnahme – ``Pha``): [3, 39]
+    * Trivialization/Minimalization (Bagatellisierung - ``Bag``): [7, 22]
+    * De-Emphasis by Comparison with Others (Herunterspielen - ``Her``): [11, 35]
+    * Rejection of Guilt (Schuldabwehr - ``Schab``): [2, 34]
+    * Distraction/Deflection from a Situation (Ablenkung - ``Abl``): [1, 32]
+    * Vicarious Satisfaction (Ersatzbefriedigung -``Ers``): [12, 42]
+    * Search for Self-Affirmation (Selbstbestätigung - ``Sebest``): [19, 37]
+    * Relaxation (Entspannung -``Entsp``): [13, 26]
+    * Attempt to Control Situation (Situationskontrolle - ``Sitkon``): [4, 23]
+    * Response Control (Reaktionskontrolle - ``Rekon``): [17, 33]
+    * Positive Self-Instruction (Positive Selbstinstruktion - ``Posi``): [9, 24]
+    * Need for Social Support (Soziales Unterstützungsbedürfnis - ``Sozube``): [14, 27]
+    * Avoidance Tendencies (Vermeidung - ``Verm``): [6, 30]
+    * Escapist Tendencies (Flucht - ``Flu``): [16, 40]
+    * Social Isolation (Soziale Abkapselung - ``Soza``): [20, 29]
+    * Mental Perseveration (Gedankliche Weiterbeschäftigung - ``Gedw``): [10, 25]
+    * Resignation (Resignation - ``Res``): [38, 15]
+    * Self-Pity (Selbstbemitleidung - ``Selmit``): [18, 28]
+    * Self-Incrimination (Selbstbeschuldigung - ``Sesch``): [8, 31]
+    * Aggression (Aggression - ``Agg``): [21, 36]
+    * Medicine-Taking (Pharmakaeinnahme - ``Pha``): [3, 39]
 
 
     .. note::
         This implementation assumes a score range of [1, 5].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
@@ -2747,18 +2739,16 @@
     meta_scales = {
         "Denial": ["Verm", "Flu", "Soza"],
         "Distraction": ["Ers", "Entsp", "Sozube"],
         "Stressordevaluation": ["Bag", "Her", "Posi"],
     }
 
     for name, scale_items in meta_scales.items():
-        if all(scale in subscales.keys() for scale in scale_items):
-            svf_data["{}_{}".format(score_name, name)] = svf_data[
-                ["{}_{}".format(score_name, s) for s in scale_items]
-            ].mean(axis=1)
+        if all(scale in subscales for scale in scale_items):
+            svf_data[f"{score_name}_{name}"] = svf_data[[f"{score_name}_{s}" for s in scale_items]].mean(axis=1)
 
     return svf_data
 
 
 def brief_cope(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
@@ -2767,15 +2757,15 @@
     """Compute the **Brief-COPE (28 items) Questionnaire (Brief_COPE)**.
 
     The Brief-COPE is a 28 item self-report questionnaire designed to measure effective and ineffective ways to cope
     with a stressful life event. "Coping" is defined broadly as an effort used to minimize distress associated with
     negative life experiences. The scale is often used in health-care settings to ascertain how patients are
     responding to a serious diagnosis. It can be used to measure how someone is coping with a wide range of
     adversity, including cancer diagnosis, heart failure, injuries, assaults, natural disasters and financial stress.
-    The scale can determine someone’s primary coping styles as either Approach Coping, or Avoidant Coping.
+    The scale can determine someone`s primary coping styles as either Approach Coping, or Avoidant Coping.
     Higher scores indicate better coping capabilities.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
     * ``SelfDistraction``: [1, 19]
     * ``ActiveCoping``: [2, 7]
     * ``Denial``: [3, 8]
@@ -2829,15 +2819,15 @@
         if number of columns does not match
     :exc:`~biopsykit.utils.exceptions.ValueRangeError`
         if values are not within the required score range
 
 
     References
     ----------
-    Carver, C. S. (1997). You want to measure coping but your protocol’too long: Consider the brief cope.
+    Carver, C. S. (1997). You want to measure coping but your protocol`too long: Consider the brief cope.
     *International journal of behavioral medicine*, 4(1), 92-100.
 
     """
     score_name = "Brief_COPE"
     score_range = [1, 4]
 
     # create copy of data
@@ -3174,32 +3164,32 @@
     In addition to profile evaluations according to these four primary scales, evaluations according to secondary and
     tertiary scales are possible (generalized self-efficacy; generalized externality;
     internality versus externality in control beliefs).
 
     It consists of the primary subscales with the item indices (count-by-one, i.e.,
     the first question has the index 1!):
 
-    * Self-concept of Own Abilities (Selbstkonzept eigener Fähigkeiten – ``SK``): [4, 8, 12, 24, 16, 20, 28, 32]
-    * Internality (Internalität – ``I``): [1, 5, 6, 11, 23, 25, 27, 30]
-    * Socially Induced Externality (Sozial bedingte Externalität – ``P``) (P = powerful others control orientation):
+    * Self-concept of Own Abilities (Selbstkonzept eigener Fähigkeiten - ``SK``): [4, 8, 12, 24, 16, 20, 28, 32]
+    * Internality (Internalität - ``I``): [1, 5, 6, 11, 23, 25, 27, 30]
+    * Socially Induced Externality (Sozial bedingte Externalität - ``P``) (P = powerful others control orientation):
       [3, 10, 14, 17, 19, 22, 26, 29]
-    * Fatalistic Externality (Fatalistische Externalität – ``C``) (C = chance control orientation):
+    * Fatalistic Externality (Fatalistische Externalität - ``C``) (C = chance control orientation):
       [2, 7, 9, 13, 15, 18, 21, 31]
 
     Further, the following secondary subscales can be computed:
 
     * Self-Efficacy / Generalized self-efficacy Beliefs (Selbstwirksamkeit / generalisierte
-      Selbstwirksamkeitsüberzeugung – ``SKI``): ``SK`` + ``I``
-    * Generalized Externality in Control Beliefs (Generalisierte Externalität in Kontrollüberzeugungen – ``PC``):
+      Selbstwirksamkeitsüberzeugung - ``SKI``): ``SK`` + ``I``
+    * Generalized Externality in Control Beliefs (Generalisierte Externalität in Kontrollüberzeugungen - ``PC``):
       ``P`` + ``C``
 
     Further, the following tertiary subscale can be computed:
 
     * Generalized Internality (Generalisierte Internalität) vs. Externality in control beliefs
-      (Externalität in Kontrollüberzeugungen – ``SKI_PC``): ``SKI`` - ``PC``
+      (Externalität in Kontrollüberzeugungen - ``SKI_PC``): ``SKI`` - ``PC``
 
     .. note::
         This implementation assumes a score range of [1, 6].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
     .. warning::
@@ -3267,26 +3257,26 @@
     # by the subscale dict)
     data = _invert_subscales(data, subscales=subscales, idx_dict={"SK": [0, 1, 2, 5]}, score_range=score_range)
 
     fkk_data = _compute_questionnaire_subscales(data, score_name, subscales)
     fkk_data = pd.DataFrame(fkk_data, index=data.index)
 
     # Sekundärskalenwerte
-    if all("{}_{}".format(score_name, s) in fkk_data.columns for s in ["SK", "I"]):
+    if all(f"{score_name}_{s}" in fkk_data.columns for s in ["SK", "I"]):
         fkk_data["{}_{}".format(score_name, "SKI")] = (
             fkk_data["{}_{}".format(score_name, "SK")] + fkk_data["{}_{}".format(score_name, "I")]
         )
 
-    if all("{}_{}".format(score_name, s) in fkk_data.columns for s in ["P", "C"]):
+    if all(f"{score_name}_{s}" in fkk_data.columns for s in ["P", "C"]):
         fkk_data["{}_{}".format(score_name, "PC")] = (
             fkk_data["{}_{}".format(score_name, "P")] + fkk_data["{}_{}".format(score_name, "C")]
         )
 
     # Tertiärskalenwerte
-    if all("{}_{}".format(score_name, s) in fkk_data.columns for s in ["SKI", "PC"]):
+    if all(f"{score_name}_{s}" in fkk_data.columns for s in ["SKI", "PC"]):
         fkk_data["{}_{}".format(score_name, "SKI_PC")] = (
             fkk_data["{}_{}".format(score_name, "SKI")] - fkk_data["{}_{}".format(score_name, "PC")]
         )
 
     return fkk_data
 
 
@@ -3295,19 +3285,19 @@
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
     """Compute the **Balanced Inventory of Desirable Responding (BIDR)**.
 
     The BIDR is a 40-item instrument that is used to measure 2 constructs:
 
-    * Self-deceptive positivity – described as the tendency to give self-reports that are believed but have a
+    * Self-deceptive positivity - described as the tendency to give self-reports that are believed but have a
       positivety bias
-    * Impression management – deliberate self-presentation to an audience.
+    * Impression management - deliberate self-presentation to an audience.
 
-    The BIDR emphasizes exaggerated claims of positive cognitive attributes (overconfidence in one’s judgments and
+    The BIDR emphasizes exaggerated claims of positive cognitive attributes (overconfidence in one`s judgments and
     rationality). It is viewed as a measure of defense, i.e., people who score high on self-deceptive positivity
     tend to defend against negative self-evaluations and seek out inflated positive self-evaluations.
 
     .. note::
         This implementation assumes a score range of [1, 7].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
@@ -3548,15 +3538,15 @@
     score_range = [1, 4]
 
     if language is None:
         language = "english"
 
     supported_versions = ["english", "german"]
     if language not in supported_versions:
-        raise ValueError("questionnaire_version must be one of {}, not {}.".format(supported_versions, language))
+        raise ValueError(f"questionnaire_version must be one of {supported_versions}, not {language}.")
 
     if columns is not None:
         # if columns parameter is supplied: slice columns from dataframe
         _assert_has_columns(data, [columns])
         data = data.loc[:, columns]
 
     if language == "german":
@@ -3577,28 +3567,28 @@
             "ControlOverprotection": [4, 5, 10, 11, 13, 19, 21, 23],
         }
 
     _assert_value_range(data, score_range)
 
     # FEE is a mean score, not a sum score!
     fee_mother = _compute_questionnaire_subscales(df_mother, score_name, subscales, agg_type="mean")
-    fee_mother = {"{}_{}".format(key, mother): val for key, val in fee_mother.items()}
+    fee_mother = {f"{key}_{mother}": val for key, val in fee_mother.items()}
     fee_father = _compute_questionnaire_subscales(df_father, score_name, subscales, agg_type="mean")
-    fee_father = {"{}_{}".format(key, father): val for key, val in fee_father.items()}
+    fee_father = {f"{key}_{father}": val for key, val in fee_father.items()}
     fee_mother.update(fee_father)
 
     return pd.DataFrame(fee_mother, index=data.index)
 
 
 def mbi_gs(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
-    """Compute the **Maslach Burnout Inventory – General Survey (MBI-GS)**.
+    """Compute the **Maslach Burnout Inventory - General Survey (MBI-GS)**.
 
     The MBI measures burnout as defined by the World Health Organization (WHO) and in the ICD-11.
 
     The MBI-GS is a psychological assessment instrument comprising 16 symptom items pertaining to occupational burnout.
     It is designed for use with occupational groups other than human services and education, including those working
     in jobs such as customer service, maintenance, manufacturing, management, and most other professions.
 
@@ -3677,15 +3667,15 @@
 
 
 def mbi_gss(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
-    """Compute the **Maslach Burnout Inventory – General Survey for Students (MBI-GS (S))**.
+    """Compute the **Maslach Burnout Inventory - General Survey for Students (MBI-GS (S))**.
 
     The MBI measures burnout as defined by the World Health Organization (WHO) and in the ICD-11.
 
     The MBI-GS (S) is an adaptation of the MBI-GS designed to assess burnout in college and university students.
     It is available for use but its psychometric properties are not yet documented.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
@@ -3969,15 +3959,15 @@
         if number of columns does not match
     :exc:`~biopsykit.utils.exceptions.ValueRangeError`
         if values are not within the required score range
 
     References
     ----------
     Hinz, A., Stöbel-Richter, Y., & Brähler, E. (2001). Der Partnerschaftsfragebogen (PFB).
-    *Diagnostica*, 47(3), 132–141.
+    *Diagnostica*, 47(3), 132-141.
 
     """
     score_name = "PFB"
     score_range = [1, 4]
 
     if columns is not None:
         # if columns parameter is supplied: slice columns from dataframe
@@ -4019,15 +4009,15 @@
         if "Glueck" in subscales:
             raise ValueRangeError(
                 "This implementation of PFB expects all values in the range {}, except the column 'Glueck' ({}), "
                 "which is expected to be in the range {}! "
                 "Please consider converting to the correct range using "
                 "`biopsykit.questionnaire.utils.convert_scale()`.".format(score_range, subscales["Glueck"], [1, 6])
             ) from e
-        raise e
+        raise ValueRangeError from e
 
 
 def asq(data: pd.DataFrame, columns: Optional[Union[Sequence[str], pd.Index]] = None) -> pd.DataFrame:
     """Compute the **Anticipatory Stress Questionnaire (ASQ)**.
 
     The ASQ measures anticipation of stress on the upcoming day.
 
@@ -4102,17 +4092,17 @@
     :class:`~pandas.DataFrame`
         ASQ_MOD score
 
 
     References
     ----------
     Modified version:
-    Kramer, A. C., Neubauer, A. B., Stoffel, M., Voss, A., & Ditzen, B. (2019). Tomorrow’s gonna suck:
-    Today’s stress anticipation predicts tomorrow’s post-awakening cortisol increase. Psychoneuroendocrinology, 106,
-    38–46. https://doi.org/10.1016/j.psyneuen.2019.03.024
+    Kramer, A. C., Neubauer, A. B., Stoffel, M., Voss, A., & Ditzen, B. (2019). Tomorrow`s gonna suck:
+    Today`s stress anticipation predicts tomorrow`s post-awakening cortisol increase. Psychoneuroendocrinology, 106,
+    38-46. https://doi.org/10.1016/j.psyneuen.2019.03.024
 
     Original paper:
     Powell, D. J., & Schlotz, W. (2012). Daily Life Stress and the Cortisol Awakening Response:
     Testing the Anticipation Hypothesis. *PLoS ONE*, 7(12), e52067. https://doi.org/10.1371/journal.pone.0052067
 
     """
     score_name = "ASQ_MOD"
@@ -4324,17 +4314,17 @@
     data = invert(
         data,
         cols=to_idx([3, 8, 9, 11, 13, 15, 19]),
         score_range=score_range,
     )
 
     # recode items 11, 12, 19
-    data.iloc[:, to_idx(11)].replace({1: 0, 2: 2, 3: 4, 4: 6}, inplace=True)
-    data.iloc[:, to_idx(12)].replace({1: 0, 2: 2, 3: 3, 4: 5}, inplace=True)
-    data.iloc[:, to_idx(19)].replace({1: 0, 2: 2, 3: 4, 4: 6}, inplace=True)
+    data.iloc[:, to_idx(11)] = data.iloc[:, to_idx(11)].replace({1: 0, 2: 2, 3: 4, 4: 6})
+    data.iloc[:, to_idx(12)] = data.iloc[:, to_idx(12)].replace({1: 0, 2: 2, 3: 3, 4: 5})
+    data.iloc[:, to_idx(19)] = data.iloc[:, to_idx(19)].replace({1: 0, 2: 2, 3: 4, 4: 6})
 
     meq_data = pd.DataFrame(data.sum(axis=1), columns=[score_name])
 
     meq_data["Chronotype_Fine"] = bin_scale(meq_data[score_name], bins=[0, 30, 41, 58, 69, 86])
     meq_data["Chronotype_Coarse"] = bin_scale(meq_data[score_name], bins=[0, 41, 58, 86])
 
     return meq_data
@@ -4454,25 +4444,21 @@
         else:
             inverted = invert(data, score_range=[1, 4], cols=to_idx([3, 4, 7]))
 
         stai_data.update(stadi(data=inverted, columns=columns, subscales=subscales, stadi_type=st))
 
     stai = pd.DataFrame(stai_data, index=data.index)
 
-    if stai_type[0] == "state":
-        name = "SAI"
-    else:
-        name = "TAI"
+    name = "SAI" if stai_type[0] == "state" else "TAI"
 
-    stai.rename(
+    stai = stai.rename(
         columns={
             f"STADI_{stai_type[0].capitalize()}_GES": f"{name}_ges",
             f"STADI_{stai_type[0].capitalize()}_SKD": f"{name}_SKD",
         },
-        inplace=True,
     )
     stai[f"{name}_SKD"] /= 5
 
     return stai
 
 
 def idq_pre_scan(data: pd.DataFrame, columns: Optional[Union[Sequence[str], pd.Index]] = None) -> pd.DataFrame:
@@ -4904,16 +4890,16 @@
         }
 
     _assert_value_range(data, score_range)
 
     abims_data = _compute_questionnaire_subscales(data, score_name, subscales)
 
     if len(subscales.keys()) == 8:
-        kov_cols = ["{}_{}".format(score_name, ele) for ele in ["KOV1", "KOV2", "KOV3", "KOV4"]]
-        vig_cols = ["{}_{}".format(score_name, ele) for ele in ["VIG1", "VIG2", "VIG3", "VIG4"]]
+        kov_cols = [f"{score_name}_{ele}" for ele in ["KOV1", "KOV2", "KOV3", "KOV4"]]
+        vig_cols = [f"{score_name}_{ele}" for ele in ["VIG1", "VIG2", "VIG3", "VIG4"]]
         # compute total score if all columns are present
         abims_data[score_name + "_KOV"] = pd.DataFrame(abims_data)[kov_cols].sum(axis=1)
         abims_data[score_name + "_VIG"] = pd.DataFrame(abims_data)[vig_cols].sum(axis=1)
 
     return pd.DataFrame(abims_data, index=data.index)
 
 
@@ -4924,17 +4910,17 @@
 ) -> pd.DataFrame:
     """Compute the **Angstsensitivitätsindex-3 (ASI)** (Anxiety Sensitivity Index).
 
     The Angstsensitivitätsindex-3 is the German version of the Anxiety Sensitivity Index by
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Physical Concerns (Bedenken Somatisch – ``BSM``): [3, 4, 7, 8, 12],
-    * Social Concerns (Bedenken Sozial – ``BZS``): [1, 6, 9, 11]
-    * Cognitive Concerns (Bedenken Kognitiv – ``BKO``): [2, 5, 10]
+    * Physical Concerns (Bedenken Somatisch - ``BSM``): [3, 4, 7, 8, 12],
+    * Social Concerns (Bedenken Sozial - ``BZS``): [1, 6, 9, 11]
+    * Cognitive Concerns (Bedenken Kognitiv - ``BKO``): [2, 5, 10]
 
     .. note::
         This implementation assumes a score range of [1, 5].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
     .. warning::
@@ -4974,15 +4960,15 @@
 
     References
     ----------
     German Version: Kemper, C. J., Ziegler, M., & Taylor, S. (2009). Überprüfung der psychometrischen Qualität der
     deutschen Version des Angstsensitivitätsindex-3. *Diagnostica*, 55(4), 223-233.
 
     Original Version: Reiss, S., Peterson, R. A., Gursky, D. M., & McNally, R. J. (1986). Anxiety sensitivity, anxiety
-    frequency and the prediction of fearfulness. Behaviour Research and Therapy, 24(1), 1–8.
+    frequency and the prediction of fearfulness. Behaviour Research and Therapy, 24(1), 1-8.
     https://doi.org/10.1016/0005-7967(86)90143-9
 
     """
     score_name = "ASI"
     score_range = [0, 4]
 
     # create copy of data
@@ -5059,15 +5045,15 @@
         if number of columns does not match
     :exc:`~biopsykit.utils.exceptions.ValueRangeError`
         if values are not within the required score range
 
 
     References
     ----------
-    German version: Abler, B., & Kessler, H. (2009). Emotion regulation questionnaire – Eine deutschsprachige Fassung
+    German version: Abler, B., & Kessler, H. (2009). Emotion regulation questionnaire - Eine deutschsprachige Fassung
     des ERQ von Gross und John. *Diagnostica*, 55(3), 144-152.
 
     Original version: Gross, J. J., & John, O. P. (2003). Individual differences in two emotion regulation processes:
     implications for affect, relationships, and well-being. *Journal of personality and social psychology*, 85(2), 348.
 
     """
     score_name = "ERQ"
@@ -5089,15 +5075,15 @@
 
     erq_data = _compute_questionnaire_subscales(data, score_name, subscales)
 
     return pd.DataFrame(erq_data, index=data.index)
 
 
 def phq(data: pd.DataFrame, columns: Optional[Union[Sequence[str], pd.Index]] = None) -> pd.DataFrame:
-    """Compute the **Patient Health Questionnaire (Depression) – 9 items (PHQ-9)**.
+    """Compute the **Patient Health Questionnaire (Depression) - 9 items (PHQ-9)**.
 
     The PHQ-9 is a measure for depression.
 
     .. note::
         This implementation assumes a score range of [1, 4].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
@@ -5180,15 +5166,15 @@
     :exc:`~biopsykit.utils.exceptions.ValueRangeError`
         if values are not within the required score range
 
 
     References
     ----------
     Schumacher, J., Leppert, K., Gunzelmann, T., Strauß, B., & Brähler, E. (2005).
-    Die resilienzskala–ein fragebogen zur erfassung der psychischen widerstandsfähigkeit als personmerkmal.
+    Die resilienzskala-ein fragebogen zur erfassung der psychischen widerstandsfähigkeit als personmerkmal.
     *Klin Psychol Psychiatr Psychother*, 53(1), 16-39.
 
     """
     score_name = "RS"
     score_range = [1, 7]
 
     # create copy of data
@@ -5210,17 +5196,17 @@
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
     """Compute the **Stress und Coping Inventar** (SCI).
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Stress Scale 1 – Uncertainty (``Stress1``): [1, 2, 3, 4, 5, 6, 7],
-    * Stress Scale 2 – Load (``Stress2``): [8, 9, 10, 11, 12, 13, 14],
-    * Stress Scale 3 – Adverse (``Stress3``): [15, 16, 17, 18, 19, 20, 21],
+    * Stress Scale 1 - Uncertainty (``Stress1``): [1, 2, 3, 4, 5, 6, 7],
+    * Stress Scale 2 - Load (``Stress2``): [8, 9, 10, 11, 12, 13, 14],
+    * Stress Scale 3 - Adverse (``Stress3``): [15, 16, 17, 18, 19, 20, 21],
     * Physical and Psychological Symptoms (``PhysPsycSymp``): [22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34],
     * Positive Thinking (``PosThink``): [29, 33, 34, 44],
     * Active Coping (``ActiveCoping``): [31, 35, 47, 45],
     * Social Support (``SocSup``): [32, 41, 43, 47],
     * Faith (``Faith``): [36, 37, 38, 46],
     * Alcohol and Cigarette Consumption (``AlcCig``): [30, 39, 42, 48]
 
@@ -5316,27 +5302,25 @@
         data = invert(data, score_range=score_ranges["AlcCig"], cols=inv_idx)
 
     sci_data = _compute_questionnaire_subscales(data, score_name, subscales)
     sci_data = pd.DataFrame(sci_data, index=data.index)
 
     if {"Stress1", "Stress2", "Stress3"}.issubset(subscales.keys()):
         # compute total score if all columns are present
-        sci_data[score_name + "_StressTotal"] = sci_data[[score_name + "_Stress{}".format(i) for i in range(1, 4)]].sum(
-            axis=1
-        )
+        sci_data[score_name + "_StressTotal"] = sci_data[[score_name + f"_Stress{i}" for i in range(1, 4)]].sum(axis=1)
 
     return sci_data
 
 
 def bfi_10(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
-    """Compute the **Big Five Inventory – 10 items (BFI-10)**.
+    """Compute the **Big Five Inventory - 10 items (BFI-10)**.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
     * Extraversion (``E``): [1, 6],
     * Agreeableness (``A``): [2, 7],
     * Conscientiousness (``C``): [3, 8],
     * Neuroticism (``N``): [4, 9],
@@ -5479,16 +5463,16 @@
     subscales: Optional[Dict[str, Sequence[int]]] = None,
     invert_score: Optional[bool] = False,
 ) -> pd.DataFrame:
     """Compute the **Subjective Well-Being Scale (SWB)**.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Mood Level (Stimmungsniveau – ``SN``): [2, 5, 8, 10, 11, 13],
-    * General Life Satisfaction (Allgemeine Lebenszufriedenheit – ``ALZ``): [1, 3, 4, 6, 7, 9, 12]
+    * Mood Level (Stimmungsniveau - ``SN``): [2, 5, 8, 10, 11, 13],
+    * General Life Satisfaction (Allgemeine Lebenszufriedenheit - ``ALZ``): [1, 3, 4, 6, 7, 9, 12]
 
     .. note::
         This implementation assumes a score range of [1, 6].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
     .. warning::
@@ -5782,21 +5766,21 @@
 
 
 def tb(
     data: pd.DataFrame,
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
-    """Compute the **Technology Commitment Questionnaire (TB – Technologiebereitschaft)**.
+    """Compute the **Technology Commitment Questionnaire (TB - Technologiebereitschaft)**.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Technology Acceptance (Technikakzeptanz – ``TechAcc``): [1, 2, 3, 4]
-    * Technology Competence Beliefs (Technikkompetenzüberzeugungen – ``TechComp``): [5, 6, 7, 8]
-    * Technology Control Beliefs (Technikkontrollüberzeugungen – ``TechControl``): [9, 10, 11, 12]
+    * Technology Acceptance (Technikakzeptanz - ``TechAcc``): [1, 2, 3, 4]
+    * Technology Competence Beliefs (Technikkompetenzüberzeugungen - ``TechComp``): [5, 6, 7, 8]
+    * Technology Control Beliefs (Technikkontrollüberzeugungen - ``TechControl``): [9, 10, 11, 12]
 
     .. note::
         This implementation assumes a score range of [1, 5].
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
     .. warning::
@@ -5932,26 +5916,26 @@
     columns: Optional[Union[Sequence[str], pd.Index]] = None,
     subscales: Optional[Dict[str, Sequence[int]]] = None,
 ) -> pd.DataFrame:
     """Compute the **Wiener Patientenzufriedenheitsinventar (WPI)**.
 
     It consists of the subscales with the item indices (count-by-one, i.e., the first question has the index 1!):
 
-    * Access to Treatment (Zugang zur Behandlung – ``AccessTreatment``): [2, 3, 4, 5, 6]
-    * Staff Competence (Kompetenz des Personals – ``StaffCompetence``): [11, 12]
-    * Effectiveness of Treatment (Wirksamkeit der Behandlung – ``EffectTreatment``): [22, 23, 24]
-    * Station Equipment (Stationsaustattung – ``StationEquipment``): [8, 9, 10]
-    * Staff-Patient Relationship (Personal-Patientenbeziehung –``Relation``): [7, 15, 16, 17, 18, 19, 21]
-    * Information about and Influence on Disease (Information über und Einflussnahme auf Erkrankung – ``Information``):
+    * Access to Treatment (Zugang zur Behandlung - ``AccessTreatment``): [2, 3, 4, 5, 6]
+    * Staff Competence (Kompetenz des Personals - ``StaffCompetence``): [11, 12]
+    * Effectiveness of Treatment (Wirksamkeit der Behandlung - ``EffectTreatment``): [22, 23, 24]
+    * Station Equipment (Stationsaustattung - ``StationEquipment``): [8, 9, 10]
+    * Staff-Patient Relationship (Personal-Patientenbeziehung -``Relation``): [7, 15, 16, 17, 18, 19, 21]
+    * Information about and Influence on Disease (Information über und Einflussnahme auf Erkrankung - ``Information``):
       [13, 14, 20]
-    * Overall Satisfaction (Insgesamte Zufriedenheit – ``OverallSatisfaction``): [1],
-    * Special Treatment Interventions (Spezielle Behandlungsinterventionen –``TreatmentInterventions``):
+    * Overall Satisfaction (Insgesamte Zufriedenheit - ``OverallSatisfaction``): [1],
+    * Special Treatment Interventions (Spezielle Behandlungsinterventionen -``TreatmentInterventions``):
       [25, 28, 29, 30, 31],
-    * Education about Medications (Aufklärung über Medikamente – ``Education``): [26, 27],
-    * Psychosocial Support Offer (Psychosoziales Unterstützungsangebot – ``Support``): [32, 33, 34, 35]
+    * Education about Medications (Aufklärung über Medikamente - ``Education``): [26, 27],
+    * Psychosocial Support Offer (Psychosoziales Unterstützungsangebot - ``Support``): [32, 33, 34, 35]
 
     .. note::
         This implementation assumes a score range of [1, 4] (for items 1-24) and [1, 5] (for items 25-35).
         Use :func:`~biopsykit.questionnaires.utils.convert_scale()` to convert the items into the correct range
         beforehand.
 
     .. warning::
```

### Comparing `biopsykit-0.8.1/src/biopsykit/questionnaires/utils.py` & `biopsykit-0.9.0/src/biopsykit/questionnaires/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Module containing utility functions for manipulating and processing questionnaire data."""
 import re
 import warnings
 from inspect import getmembers, isfunction
-from typing import Any, Dict, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Literal, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from typing_extensions import Literal
-
 from biopsykit.utils._datatype_validation_helper import _assert_is_dtype, _assert_len_list, _assert_value_range
 from biopsykit.utils.dataframe_handling import wide_to_long as wide_to_long_utils
 
 __all__ = [
     "bin_scale",
     "compute_scores",
     "crop_scale",
@@ -407,19 +405,18 @@
 
 
 def _convert_scale_dataframe(
     data: pd.DataFrame, cols: Union[Sequence[int], Sequence[str]], offset: int
 ) -> pd.DataFrame:
     if cols is None:
         data.iloc[:, :] = data.iloc[:, :] + offset
-    else:
-        if isinstance(cols[0], int):
-            data.iloc[:, cols] = data.iloc[:, cols] + offset
-        elif isinstance(cols[0], str):
-            data.loc[:, cols] = data.loc[:, cols] + offset
+    elif isinstance(cols[0], int):
+        data.iloc[:, cols] = data.iloc[:, cols] + offset
+    elif isinstance(cols[0], str):
+        data.loc[:, cols] = data.loc[:, cols] + offset
 
     return data
 
 
 def crop_scale(
     data: Union[pd.DataFrame, pd.Series],
     score_range: Sequence[int],
@@ -448,18 +445,18 @@
     _assert_is_dtype(data, (pd.DataFrame, pd.Series))
     _assert_len_list(score_range, 2)
 
     if not inplace:
         data = data.copy()
 
     if set_nan:
-        data.mask((data < score_range[0]) | (data > score_range[1]), inplace=True)
+        data.mask((data < score_range[0]) | (data > score_range[1]), inplace=True)  # noqa: PD002
     else:
-        data.mask((data < score_range[0]), other=score_range[0], inplace=True)
-        data.mask((data > score_range[1]), other=score_range[1], inplace=True)
+        data.mask((data < score_range[0]), other=score_range[0], inplace=True)  # noqa: PD002
+        data.mask((data > score_range[1]), other=score_range[1], inplace=True)  # noqa: PD002
 
     if inplace:
         return None
     return data
 
 
 def bin_scale(
@@ -631,19 +628,19 @@
     df_scores = pd.DataFrame(index=data.index)
     quest_funcs = dict(getmembers(questionnaires, isfunction))
     if quest_kwargs is None:
         quest_kwargs = {}
 
     for score, columns in quest_dict.items():
         score_orig = score
-        score = score.lower()
+        score = score.lower()  # noqa: PLW2901
         suffix = None
         if "-" in score:
             score_split = score.split("-")
-            score = score_split[0]
+            score = score_split[0]  # noqa: PLW2901
             suffix = score_split[1]
 
         if score not in quest_funcs:
             raise ValueError(
                 "Unknown questionnaire '{}'! Call "
                 "'biopsykit.questionnaires.utils.get_supported_questionnaires()' "
                 "to get a list of all supported questionnaires.".format(score)
@@ -654,15 +651,15 @@
         except TypeError as e:
             raise TypeError(
                 "Error computing questionnaire '{}'. The computation failed with the following "
                 "error: \n\n{}.".format(score, str(e))
             ) from e
 
         if suffix is not None:
-            df.columns = ["{}_{}".format(col, suffix) for col in df.columns]
+            df.columns = [f"{col}_{suffix}" for col in df.columns]
         df_scores = df_scores.join(df)
 
     return df_scores
 
 
 def get_supported_questionnaires() -> Dict[str, str]:
     """List all supported (i.e., implemented) questionnaires.
@@ -727,15 +724,15 @@
             score = _compute_questionnaire_scores_str(data, items, agg_type)
         else:
             raise ValueError(
                 "Subscale columns are either expected as column names (list of strings) or "
                 "column indices (list of integers)!"
             )
 
-        out["{}_{}".format(score_name, key)] = score
+        out[f"{score_name}_{key}"] = score
 
     return out
 
 
 def _compute_questionnaire_scores_int(data: pd.DataFrame, items: Sequence[int], agg_type: str):
     if agg_type == "sum":
         return data.iloc[:, to_idx(items)].sum(axis=1)
@@ -773,20 +770,20 @@
 
     # ensure list
     bins = list(bins)
 
     if first_min:
         min_val = _bin_scale_get_min_val(data, col)
         if min_val < min(bins):
-            bins = [min_val - 0.01] + bins
+            bins = [min_val - 0.01, *bins]
 
     if last_max:
         max_val = _bin_scale_get_max_val(data, col)
         if max_val > max(bins):
-            bins = bins + [max_val + 0.01]
+            bins = [*bins, max_val + 0.01]
 
     return bins
 
 
 def _bin_scale_get_min_val(data: Union[pd.DataFrame, pd.Series], col: Union[int, str]) -> float:
     if isinstance(col, int):
         return data.iloc[:, col].min()
```

### Comparing `biopsykit-0.8.1/src/biopsykit/saliva/saliva.py` & `biopsykit-0.9.0/src/biopsykit/saliva/saliva.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Functions for processing saliva data and computing established features (AUC, slope, maximum increase, ...)."""
 import warnings
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.saliva.utils import (
     _check_sample_times,
     _get_group_cols,
     _get_saliva_idx_labels,
     _get_sample_times,
     _remove_s0,
 )
@@ -60,15 +59,15 @@
     is_saliva_raw_dataframe(data, saliva_type)
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             saliva_col = [saliva]
             if "time" in data:
-                saliva_col = saliva_col + ["time"]
+                saliva_col = [*saliva_col, "time"]
             dict_result[saliva] = max_value(
                 data[saliva_col],
                 saliva_type=saliva,
                 remove_s0=remove_s0,
             )
         return dict_result
 
@@ -80,15 +79,15 @@
 
     data = data[[saliva_type]].unstack(level="sample")
 
     max_val = data.max(axis=1)
 
     out = pd.DataFrame(
         max_val,
-        columns=["{}_max_val".format(saliva_type)],
+        columns=[f"{saliva_type}_max_val"],
         index=max_val.index,
     )
     out.columns.name = "saliva_feature"
 
     # check output
     is_saliva_feature_dataframe(out, saliva_type)
     return out
@@ -128,15 +127,15 @@
     is_saliva_raw_dataframe(data, saliva_type)
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             saliva_col = [saliva]
             if "time" in data:
-                saliva_col = saliva_col + ["time"]
+                saliva_col = [*saliva_col, "time"]
             dict_result[saliva] = initial_value(
                 data[saliva_col],
                 saliva_type=saliva,
                 remove_s0=remove_s0,
             )
         return dict_result
 
@@ -146,15 +145,15 @@
 
     data = data[[saliva_type]].unstack(level="sample")
 
     ini_val = data.iloc[:, 0]
 
     out = pd.DataFrame(
         ini_val.values,
-        columns=["{}_ini_val".format(saliva_type)],
+        columns=[f"{saliva_type}_ini_val"],
         index=ini_val.index,
     )
     out.columns.name = "saliva_feature"
 
     # check output
     is_saliva_feature_dataframe(out, saliva_type)
     return out
@@ -206,15 +205,15 @@
     is_saliva_raw_dataframe(data, saliva_type)
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             saliva_col = [saliva]
             if "time" in data:
-                saliva_col = saliva_col + ["time"]
+                saliva_col = [*saliva_col, "time"]
             dict_result[saliva] = max_increase(
                 data[saliva_col],
                 saliva_type=saliva,
                 remove_s0=remove_s0,
                 percent=percent,
             )
         return dict_result
@@ -227,15 +226,15 @@
 
     max_inc = data.iloc[:, 1:].max(axis=1) - data.iloc[:, 0]
     if percent:
         max_inc = 100.0 * max_inc / np.abs(data.iloc[:, 0])
 
     out = pd.DataFrame(
         max_inc,
-        columns=["{}_max_inc_percent".format(saliva_type) if percent else "{}_max_inc".format(saliva_type)],
+        columns=[f"{saliva_type}_max_inc_percent" if percent else f"{saliva_type}_max_inc"],
         index=max_inc.index,
     )
     out.columns.name = "saliva_feature"
 
     # check output
     is_saliva_feature_dataframe(out, saliva_type)
     return out
@@ -306,27 +305,27 @@
     :exc:`~biopsykit.utils.exceptions.ValidationError`
         if ``data`` is not a :obj:`~biopsykit.utils.datatype_helper.SalivaRawDataFrame`
 
     References
     ----------
     Pruessner, J. C., Kirschbaum, C., Meinlschmid, G., & Hellhammer, D. H. (2003).
     Two formulas for computation of the area under the curve represent measures of total hormone concentration
-    versus time-dependent change. Psychoneuroendocrinology, 28(7), 916–931.
+    versus time-dependent change. Psychoneuroendocrinology, 28(7), 916-931.
     https://doi.org/10.1016/S0306-4530(02)00108-7
 
     """
     # check input
     is_saliva_raw_dataframe(data, saliva_type)
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             saliva_col = [saliva]
             if "time" in data:
-                saliva_col = saliva_col + ["time"]
+                saliva_col = [*saliva_col, "time"]
             dict_result[saliva] = auc(
                 data[saliva_col],
                 saliva_type=saliva,
                 remove_s0=remove_s0,
                 sample_times=sample_times,
             )
         return dict_result
@@ -344,15 +343,15 @@
         "auc_g": np.trapz(data, sample_times),
         "auc_i": np.trapz(data.sub(data.iloc[:, 0], axis=0), sample_times),
     }
 
     if compute_auc_post:
         auc_data = _auc_compute_auc_post(data, auc_data, sample_times)
 
-    out = pd.DataFrame(auc_data, index=data.index).add_prefix("{}_".format(saliva_type))
+    out = pd.DataFrame(auc_data, index=data.index).add_prefix(f"{saliva_type}_")
     out.columns.name = "saliva_feature"
 
     # check output
     is_saliva_feature_dataframe(out, saliva_type)
 
     return _SalivaFeatureDataFrame(out)
 
@@ -435,15 +434,15 @@
         raise IndexError("Either `sample_labels` or `sample_idx` must be supplied as parameter, not both!")
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             saliva_col = [saliva]
             if "time" in data:
-                saliva_col = saliva_col + ["time"]
+                saliva_col = [*saliva_col, "time"]
             dict_result[saliva] = slope(
                 data[saliva_col],
                 sample_labels=sample_labels,
                 sample_idx=sample_idx,
                 saliva_type=saliva,
                 sample_times=sample_times,
             )
@@ -527,15 +526,15 @@
     is_saliva_raw_dataframe(data, saliva_type)
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             saliva_col = [saliva]
             if "time" in data:
-                saliva_col = saliva_col + ["time"]
+                saliva_col = [*saliva_col, "time"]
             dict_result[saliva] = standard_features(data[saliva_col], saliva_type=saliva)
         return dict_result
 
     group_cols = _get_group_cols(data, group_cols, "sample", "standard_features")
 
     out = (
         data[[saliva_type]]
@@ -560,15 +559,15 @@
                 "Consider setting 'keep_index' to 'False'. "
                 "The exact error was:\n\n{}".format(str(e))
             ) from e
 
     # drop 'saliva_type' multiindex column and add as prefix to columns to ensure consistent naming with
     # the other saliva functions
     out.columns = out.columns.droplevel(0)
-    out = out.add_prefix("{}_".format(saliva_type))
+    out = out.add_prefix(f"{saliva_type}_")
     out.columns.name = "saliva_feature"
 
     # check output
     is_saliva_feature_dataframe(out, saliva_type)
 
     return _SalivaFeatureDataFrame(out)
 
@@ -610,29 +609,29 @@
     is_saliva_raw_dataframe(data, saliva_type)
 
     if isinstance(saliva_type, list):
         dict_result = {}
         for biomarker in saliva_type:
             biomarker_cols = [biomarker]
             if "time" in data:
-                biomarker_cols = ["time"] + biomarker_cols
+                biomarker_cols = ["time", *biomarker_cols]
             dict_result[biomarker] = mean_se(data[biomarker_cols], saliva_type=biomarker, remove_s0=remove_s0)
         return dict_result
 
     if remove_s0:
         # We have a S0 sample => drop it
         data = _remove_s0(data)
 
     group_cols = _get_group_cols(data, group_cols, "subject", "mean_se")
     _mean_se_assert_group_cols(data, group_cols)
 
     if "time" in data.columns and "time" not in group_cols:
         # add 'time' column to grouper if it's in the data and wasn't added yet because otherwise
         # we would loose this column
-        group_cols = group_cols + ["time"]
+        group_cols = [*group_cols, "time"]
 
     data_mean_se = data.groupby(group_cols).agg([np.mean, se])[saliva_type]
     is_saliva_mean_se_dataframe(data_mean_se)
 
     return _SalivaMeanSeDataFrame(data_mean_se)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biopsykit-0.8.1/src/biopsykit/saliva/utils.py` & `biopsykit-0.9.0/src/biopsykit/saliva/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Utility functions for working with saliva dataframes."""
 import re
 from datetime import datetime, time
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_has_index_levels, _assert_is_dtype
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.datatype_helper import SalivaFeatureDataFrame, SalivaRawDataFrame, _SalivaRawDataFrame
 
 __all__ = [
     "saliva_feature_wide_to_long",
     "get_saliva_column_suggestions",
@@ -47,15 +46,15 @@
         i=index_cols,
         j=j,
         sep="_",
         suffix=r"\w+",
     )
 
     # reorder levels and sort
-    return data.reorder_levels(index_cols + [j]).sort_index()
+    return data.reorder_levels([*index_cols, j]).sort_index()
 
 
 def get_saliva_column_suggestions(data: pd.DataFrame, saliva_type: Union[str, Sequence[str]]) -> Sequence[str]:
     """Automatically extract possible saliva data columns from a pandas dataframe.
 
     This is for example useful when one large dataframe is used to store demographic information,
     questionnaire data and saliva data.
@@ -79,17 +78,15 @@
     if isinstance(saliva_type, list):
         dict_result = {}
         for saliva in saliva_type:
             dict_result[saliva] = get_saliva_column_suggestions(data=data, saliva_type=saliva)
         return dict_result
 
     if saliva_type not in _dict_saliva_type_suggs:
-        raise ValueError(
-            "Invalid saliva type '{}'! Must be one of {}.".format(saliva_type, list(_dict_saliva_type_suggs.keys()))
-        )
+        raise ValueError(f"Invalid saliva type '{saliva_type}'! Must be one of {list(_dict_saliva_type_suggs.keys())}.")
 
     sugg_filt = list(
         filter(
             lambda col: any(k in col for k in _dict_saliva_type_suggs[saliva_type]),
             data.columns,
         )
     )
@@ -112,15 +109,15 @@
                 )
             ),
             sugg_filt,
         )
     )
     # replace il{} with il6 since this was removed out by the previous filter operation
     sugg_filt = [re.sub(r"\d", "{}", s).replace("il{}", "il6").replace("IL{}", "IL6") for s in sugg_filt]
-    sugg_filt = sorted(list(filter(lambda s: "{}" in s, set(sugg_filt))))
+    sugg_filt = sorted(filter(lambda s: "{}" in s, set(sugg_filt)))
 
     # build regex for column extraction
     sugg_filt = ["^{}$".format(s.replace("{}", r"(\d)")) for s in sugg_filt]
     return sugg_filt
 
 
 def extract_saliva_columns(
@@ -165,15 +162,15 @@
         col_pattern = col_suggs[0]
     return data.filter(regex=col_pattern)
 
 
 def _sample_times_datetime_to_minute_apply(
     sample_times: Union[pd.DataFrame, pd.Series]
 ) -> Union[pd.DataFrame, pd.Series]:
-    if isinstance(sample_times.values.flatten()[0], (pd.Timedelta, np.timedelta64)):
+    if isinstance(sample_times.to_numpy().flatten()[0], (pd.Timedelta, np.timedelta64)):
         return sample_times.apply(pd.to_timedelta)
     return sample_times.astype(str).apply(pd.to_datetime)
 
 
 def sample_times_datetime_to_minute(sample_times: Union[pd.Series, pd.DataFrame]) -> Union[pd.Series, pd.DataFrame]:
     """Convert sample times from datetime or timedelta objects into minutes.
 
@@ -198,19 +195,21 @@
 
     Raises
     ------
     ValueError
         if sample times are not in a datetime- or timedelta-related format
 
     """
-    if isinstance(sample_times.values.flatten()[0], str):
+    if isinstance(sample_times.to_numpy().flatten()[0], str):
         sample_times = _get_sample_times_str(sample_times)
 
-    if not isinstance(sample_times.values.flatten()[0], (time, datetime, pd.Timedelta, np.timedelta64, np.datetime64)):
-        raise ValueError(
+    if not isinstance(
+        sample_times.to_numpy().flatten()[0], (time, datetime, pd.Timedelta, np.timedelta64, np.datetime64)
+    ):
+        raise TypeError(
             "Sample times must be instance of `datetime.datetime()`, `datetime.time()`,"
             " `np.datetime64`, `np.timedelta64`, or `pd.Timedelta`!"
         )
 
     is_series = isinstance(sample_times, pd.Series)
     if is_series:
         _assert_has_index_levels(sample_times, index_levels=["sample"], match_atleast=True)
@@ -218,15 +217,15 @@
         # Then stack it back together
         sample_times = sample_times.unstack(level="sample")
 
     sample_times = _sample_times_datetime_to_minute_apply(sample_times)
 
     sample_times = sample_times.diff(axis=1).apply(lambda s: (s.dt.total_seconds() / 60))
     sample_times = sample_times.cumsum(axis=1)
-    sample_times.iloc[:, 0].fillna(0, inplace=True)
+    sample_times.iloc[:, 0] = sample_times.iloc[:, 0].fillna(0)
     if is_series:
         sample_times = sample_times.stack()
     return sample_times
 
 
 def _get_sample_times_str(sample_times: Union[pd.Series, pd.DataFrame]) -> Union[pd.Series, pd.DataFrame]:
     if isinstance(sample_times, pd.DataFrame):
@@ -281,15 +280,15 @@
     if sample_times is None:
         # check if dataframe has 'time' index
         if "time" in data.index.names:
             data = data.reset_index("time")
         # check if dataframe has 'time' column
         if "time" in data.columns:
             sample_times = np.array(data.unstack(level="sample")["time"])
-            if np.all((sample_times == sample_times[0])):
+            if np.all(sample_times == sample_times[0]):
                 # all subjects have the same saliva times
                 sample_times = sample_times[0]
         else:
             raise ValueError("No sample times specified!")
 
     # ensure numpy
     sample_times = np.squeeze(sample_times)
@@ -331,15 +330,15 @@
         act_shape = sample_times.shape
         if act_shape != exp_shape:
             raise ValueError(
                 "Dimensions of 'sample_times' does not correspond to dimensions of 'data'! "
                 "Expected {}, got {}.".format(exp_shape, act_shape)
             )
     else:
-        raise ValueError("'sample_times' has invalid dimensions! Expected 1 or 2, got {}".format(sample_times.ndim))
+        raise ValueError(f"'sample_times' has invalid dimensions! Expected 1 or 2, got {sample_times.ndim}")
 
 
 def _get_saliva_idx_labels(
     columns: pd.Index,
     sample_labels: Optional[Union[Tuple, Sequence]] = None,
     sample_idx: Optional[Union[Tuple[int, int], Sequence[int]]] = None,
 ) -> Tuple[Sequence, Sequence]:
@@ -362,25 +361,25 @@
         list of sample indices
 
     """
     if sample_labels is not None:
         try:
             sample_idx = [columns.get_loc(label) for label in sample_labels]
         except KeyError as e:
-            raise IndexError("Invalid sample_labels `{}`".format(sample_labels)) from e
+            raise IndexError(f"Invalid sample_labels `{sample_labels}`") from e
     else:
         try:
             # ensure list
             sample_idx = list(sample_idx)
             sample_labels = columns[sample_idx]
         except IndexError as e:
             raise IndexError("`sample_idx[1]` is out of bounds!") from e
 
     if len(sample_idx) != 2:
-        raise IndexError("Exactly 2 indices needed for computing slope. Got {} indices.".format(len(sample_idx)))
+        raise IndexError(f"Exactly 2 indices needed for computing slope. Got {len(sample_idx)} indices.")
 
     sample_idx = _get_saliva_idx_labels_sanitize(sample_idx, columns)
     return sample_labels, sample_idx
 
 
 def _get_saliva_idx_labels_sanitize(sample_idx: List[int], columns: Sequence[str]):
     # replace idx values like '-1' with the actual index
@@ -388,15 +387,15 @@
         sample_idx[0] = len(columns) + sample_idx[0]
 
     if sample_idx[1] < 0:
         sample_idx[1] = len(columns) + sample_idx[1]
 
     # check that second index is bigger than first index
     if sample_idx[0] >= sample_idx[1]:
-        raise IndexError("`sample_idx[1]` must be bigger than `sample_idx[0]`. Got {}".format(sample_idx))
+        raise IndexError(f"`sample_idx[1]` must be bigger than `sample_idx[0]`. Got {sample_idx}")
     return sample_idx
 
 
 def _get_group_cols(
     data: SalivaRawDataFrame, group_cols: Union[str, Sequence[str]], group_type: str, function_name: str
 ) -> List[str]:
     """Get appropriate columns for grouping.
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/_base.py` & `biopsykit-0.9.0/src/biopsykit/signals/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Base class for implementing signal processing pipelines."""
 from typing import Dict, Optional, Sequence, Union
 
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_is_dtype
 from biopsykit.utils.data_processing import split_data
 
 
 class _BaseProcessor:
     """Base class for implementing signal processing pipelines in BioPsyKit."""
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/ecg/ecg.py` & `biopsykit-0.9.0/src/biopsykit/signals/ecg/ecg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Module for processing ECG data."""
 import warnings
 from typing import Callable, Dict, List, Literal, Optional, Sequence, Tuple, Union
 
 import neurokit2 as nk
 import numpy as np
 import pandas as pd
-from scipy.stats import iqr
-from tqdm.auto import tqdm
-
 from biopsykit.signals._base import _BaseProcessor
 from biopsykit.utils.array_handling import find_extrema_in_radius, remove_outlier_and_interpolate, sanitize_input_1d
 from biopsykit.utils.datatype_helper import (
     ECG_RESULT_DATAFRAME_COLUMNS,
     HEART_RATE_DATAFRAME_COLUMNS,
     R_PEAK_DATAFRAME_COLUMNS,
     EcgRawDataFrame,
@@ -20,14 +17,16 @@
     RPeakDataFrame,
     _EcgResultDataFrame,
     _RPeakDataFrame,
     is_ecg_raw_dataframe,
     is_ecg_result_dataframe,
     is_r_peak_dataframe,
 )
+from scipy.stats import iqr
+from tqdm.auto import tqdm
 
 __all__ = ["EcgProcessor"]
 
 from biopsykit.utils.exceptions import EcgProcessingError
 
 ERROR_HANDLING = Literal["raise", "warn", "ignore"]
 """Available behavior types when dealing with ECG processing errors."""
@@ -41,17 +40,15 @@
         hrv_types = list(_hrv_methods.keys())
     if isinstance(hrv_types, str):
         hrv_types = [hrv_types]
 
     # check whether all supplied hrv_types are valid
     for hrv_type in hrv_types:
         if hrv_type not in _hrv_methods:
-            raise ValueError(
-                "Invalid 'hrv_types'. Must be in {}, but got {}".format(list(_hrv_methods.keys()), hrv_type)
-            )
+            raise ValueError(f"Invalid 'hrv_types'. Must be in {list(_hrv_methods.keys())}, but got {hrv_type}")
     return hrv_types
 
 
 class EcgProcessor(_BaseProcessor):
     """Class for processing ECG data."""
 
     def __init__(
@@ -63,15 +60,15 @@
     ):
         """Initialize a new ``EcgProcessor`` instance.
 
         To use this class simply pass data in form of a :class:`~pandas.DataFrame` (or a dict of such).
         If the data was recorded during a study that consists of multiple phases, the ECG data can be split into single
         phases by passing time information via the ``time_intervals`` parameter.
 
-        Each instance of ``EcgProcessor`` the following attributes:
+        Each instance of ``EcgProcessor`` has the following attributes:
 
         * ``data``: dict with raw ECG data, split into the specified phases. If data was not split the
           dictionary only has one entry, accessible by the key ``Data``
         * ``ecg_result`` : dict with ECG processing results from ``data``. Each dataframe in the dict has the
           following columns:
 
           * ``ECG_Raw``: Raw ECG signal
@@ -304,15 +301,15 @@
                     x_values=np.squeeze(rpeaks["R_Peak_Idx"].values),
                     y_values=np.squeeze(heart_rate["Heart_Rate"].values),
                     x_new=np.arange(0, len(ecg_result["ECG_Clean"])),
                 )
                 ecg_result["Heart_Rate"] = heart_rate_interpolated
             except EcgProcessingError as e:
                 if errors == "raise":
-                    raise e
+                    raise EcgProcessingError from e
                 if errors == "warn":
                     warnings.warn(str(e))
                 ecg_result, rpeaks, heart_rate = (
                     pd.DataFrame(columns=ECG_RESULT_DATAFRAME_COLUMNS),
                     pd.DataFrame(columns=R_PEAK_DATAFRAME_COLUMNS),
                     pd.DataFrame(columns=HEART_RATE_DATAFRAME_COLUMNS),
                 )
@@ -341,15 +338,15 @@
         ecg_result : :class:`~biopsykit.utils.datatype_helper.EcgResultDataFrame`, optional
             Dataframe with processed ECG signal. Output from :meth:`~biopsykit.signals.ecg.EcgProcessor.ecg_process()`
         rpeaks : :class:`~biopsykit.utils.datatype_helper.RPeakDataFrame`, optional
             Dataframe with detected R peaks. Output from :meth:`~biopsykit.signals.ecg.EcgProcessor.ecg_process()`
 
         """
         # get numpy
-        ecg_signal = data["ecg"].values
+        ecg_signal = data["ecg"].to_numpy()
         # clean (i.e. filter) the ECG signal using the specified method
         ecg_cleaned = nk.ecg_clean(ecg_signal, sampling_rate=int(self.sampling_rate), method=method)
 
         # find peaks using the specified method
         # instant_peaks: array indicating where detected R peaks are in the raw ECG signal
         # rpeak_index array containing the indices of detected R peaks
         instant_peaks, rpeak_idx = nk.ecg_peaks(ecg_cleaned, sampling_rate=int(self.sampling_rate), method=method)
@@ -372,15 +369,15 @@
                 "R_Peak_Outlier": np.zeros(len(data)),
             },
             index=data.index,
         )
 
         # copy new dataframe consisting of R peaks indices (and their respective quality indicator)
         rpeaks = ecg_result.loc[ecg_result["ECG_R_Peaks"] == 1.0, ["ECG_Quality"]]
-        rpeaks.rename(columns={"ECG_Quality": "R_Peak_Quality"}, inplace=True)
+        rpeaks = rpeaks.rename(columns={"ECG_Quality": "R_Peak_Quality"})
         rpeaks.loc[:, "R_Peak_Idx"] = rpeak_idx
         # compute RR interval
         rpeaks["RR_Interval"] = np.ediff1d(rpeaks["R_Peak_Idx"], to_end=0) / self.sampling_rate
         # ensure equal length by filling the last value with the average RR interval
         rpeaks.loc[rpeaks.index[-1], "RR_Interval"] = rpeaks["RR_Interval"].mean()
 
         is_ecg_result_dataframe(ecg_result)
@@ -420,15 +417,15 @@
         -------
         list
             keys of all possible outlier correction methods
 
         References
         ----------
         Berntson, G. G., Quigley, K. S., Jang, J. F., & Boysen, S. T. (1990). An Approach to Artifact Identification:
-        Application to Heart Period Data. *Psychophysiology*, 27(5), 586–598.
+        Application to Heart Period Data. *Psychophysiology*, 27(5), 586-598.
         https://doi.org/10.1111/j.1469-8986.1990.tb01982.x
 
         """
         return list(_outlier_correction_methods.keys())
 
     @classmethod
     def outlier_params_default(cls) -> Dict[str, Union[float, Sequence[float]]]:
@@ -664,15 +661,15 @@
             dataframe containing corrected R peak indices
 
 
         References
         ----------
         Lipponen, J. A., & Tarvainen, M. P. (2019). A robust algorithm for heart rate variability time series artefact
         correction using novel beat classification. *Journal of Medical Engineering and Technology*,
-        43(3), 173–181. https://doi.org/10.1080/03091902.2019.1640306
+        43(3), 173-181. https://doi.org/10.1080/03091902.2019.1640306
 
 
         Examples
         --------
         >>> from biopsykit.signals.ecg import EcgProcessor
         >>> # initialize EcgProcessor instance
         >>> ep = EcgProcessor(...)
@@ -868,15 +865,15 @@
 
         is_ecg_result_dataframe(ecg_signal)
         is_r_peak_dataframe(rpeaks)
 
         if edr_type is None:
             edr_type = "peak_trough_mean"
         if edr_type not in _edr_methods:
-            raise ValueError("`edr_type` must be one of {}, not {}".format(list(_edr_methods.keys()), edr_type))
+            raise ValueError(f"`edr_type` must be one of {list(_edr_methods.keys())}, not {edr_type}")
         edr_func = _edr_methods[edr_type]
 
         # ensure numpy
         peaks = np.squeeze(rpeaks["R_Peak_Idx"].values)
 
         # find troughs (minimum 0.1s before R peak)
         troughs = find_extrema_in_radius(ecg_signal["ECG_Clean"], peaks, radius=(int(0.1 * sampling_rate), 0))
@@ -1105,17 +1102,15 @@
 
     """
     peak_vals = np.array(ecg.iloc[peaks])
     trough_vals = np.array(ecg.iloc[troughs])
     return peak_vals - trough_vals
 
 
-def _edr_peak_peak_interval(
-    ecg: pd.DataFrame, peaks: np.array, troughs: np.array  # pylint:disable=unused-argument
-) -> np.array:
+def _edr_peak_peak_interval(ecg: pd.DataFrame, peaks: np.array, troughs: np.array) -> np.array:  # noqa: ARG001
     """Estimate respiration signal from ECG based on `peak-peak-interval` method.
 
     The `peak-peak-interval` method is based on computing RR intervals.
 
     .. note::
         To ensure the same length for the resulting array after computing successive differences
         the first value will be replaced by the mean of all RR intervals in the array
@@ -1196,15 +1191,15 @@
     rpeaks["RR_Interval"] = np.ediff1d(rpeaks["R_Peak_Idx"], to_end=0) / sampling_rate
 
     # signal outlier: drop all beats that are below a correlation coefficient threshold
     return np.logical_or(bool_mask, rpeaks["R_Peak_Idx"].isin(corr_coeff[corr_coeff < corr_thres].index))
 
 
 def _correct_outlier_quality(
-    rpeaks: pd.DataFrame, bool_mask: np.array, quality_thres: float, **kwargs  # pylint:disable=unused-argument
+    rpeaks: pd.DataFrame, bool_mask: np.array, quality_thres: float, **kwargs  # noqa: ARG001
 ) -> np.array:
     """Apply outlier correction method 'quality'.
 
     This function uses the ``ECG_Quality`` indicator from ``neurokit`` to assess signal quality. It marks beats as
     outlier if the quality indicator is below a certain threshold.
 
 
@@ -1230,15 +1225,15 @@
     return np.logical_or(bool_mask, rpeaks["R_Peak_Quality"] < quality_thres)
 
 
 def _correct_outlier_statistical_rr(
     rpeaks: pd.DataFrame,
     bool_mask: np.array,
     stat_thres: float,
-    **kwargs,  # pylint:disable=unused-argument
+    **kwargs,  # noqa: ARG001
 ) -> np.array:
     """Apply outlier correction method 'statistical_rr'.
 
     This function marks beats as outlier if they are within the xx % highest or lowest RR intervals, i.e., if
     their z-score is above a threshold, e.g., ``1.96`` => 5% (2.5% highest, 2.5% lowest values);
     ``2.576`` => 1% (0.5% highest, 0.5% lowest values)
 
@@ -1266,15 +1261,15 @@
     rri = rpeaks["RR_Interval"]
     z_score = (rri - np.nanmean(rri)) / np.nanstd(rri, ddof=1)
 
     return np.logical_or(bool_mask, np.abs(z_score) > stat_thres)
 
 
 def _correct_outlier_statistical_rr_diff(
-    rpeaks: pd.DataFrame, bool_mask: np.array, stat_thres: float, **kwargs  # pylint:disable=unused-argument
+    rpeaks: pd.DataFrame, bool_mask: np.array, stat_thres: float, **kwargs  # noqa: ARG001
 ) -> np.array:
     """Apply outlier correction method 'statistical_rr_diff'.
 
     This function marks beats as outlier if their successive differences of RR intervals are within the xx % highest or
     lowest values, i.e. if their z-score is above a threshold, e.g. ``1.96`` => 5% (2.5% highest, 2.5% lowest values);
     ``2.576`` => 1% (0.5% highest, 0.5% lowest values).
 
@@ -1304,16 +1299,16 @@
 
     return np.logical_or(bool_mask, np.abs(z_score) > stat_thres)
 
 
 def _correct_outlier_artifact(
     rpeaks: pd.DataFrame,
     bool_mask: np.array,
-    art_thres: float,  # pylint:disable=unused-argument
-    **kwargs,  # pylint:disable=unused-argument
+    art_thres: float,  # noqa: ARG001
+    **kwargs,  # noqa: ARG001
 ) -> np.array:
     """Apply outlier correction method 'artifact'.
 
     This function uses the artifact detection algorithm from `Berntson et al. (1990)`.
     Marks beats as outlier if they detected as such by this algorithm.
 
 
@@ -1334,15 +1329,15 @@
         boolean array with beats marked as outlier. Logical 'or' combination of ``bool_mask`` and results from
         this algorithm
 
 
     References
     ----------
     Berntson, G. G., Quigley, K. S., Jang, J. F., & Boysen, S. T. (1990). An Approach to Artifact Identification:
-    Application to Heart Period Data. *Psychophysiology*, 27(5), 586–598.
+    Application to Heart Period Data. *Psychophysiology*, 27(5), 586-598.
     https://doi.org/10.1111/j.1469-8986.1990.tb01982.x
 
     """
     # QD = Quartile Deviation = IQR / 2
     qd = iqr(rpeaks["RR_Interval"], nan_policy="omit") / 2.0
     # MAD = Minimal Artifact Difference
     mad = (rpeaks["RR_Interval"].median() - 2.9 * qd) / 3.0
@@ -1353,15 +1348,15 @@
     return np.logical_or(
         bool_mask,
         np.abs(rpeaks["RR_Interval"] - rpeaks["RR_Interval"].median()) > criterion,
     )
 
 
 def _correct_outlier_physiological(
-    rpeaks: pd.DataFrame, bool_mask: np.array, hr_thres: Tuple[float, float], **kwargs  # pylint:disable=unused-argument
+    rpeaks: pd.DataFrame, bool_mask: np.array, hr_thres: Tuple[float, float], **kwargs  # noqa: ARG001
 ) -> np.array:
     """Apply outlier correction method 'physiological'.
 
     This function marks beats as outlier if their heart rate is above or below a threshold that is very unlikely to be
     achieved physiologically.
 
     Parameters
@@ -1517,15 +1512,15 @@
         raise ValueError("Both of 'ecg_signal' and 'rpeaks' must be passed as arguments!")
 
 
 def _get_imputation_type(imputation_type: str, imputation_types: Sequence[str]) -> str:
     if imputation_type is None:
         imputation_type = "moving_average"
     elif imputation_type not in imputation_types:
-        raise ValueError("'imputation_type' must be one of {}, not {}!".format(imputation_types, imputation_type))
+        raise ValueError(f"'imputation_type' must be one of {imputation_types}, not {imputation_type}!")
     return imputation_type
 
 
 def _check_dataframe_format(ecg_signal: EcgResultDataFrame, rpeaks: RPeakDataFrame):
     if ecg_signal is not None:
         is_ecg_result_dataframe(ecg_signal)
     is_r_peak_dataframe(rpeaks)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/ecg/plotting.py` & `biopsykit-0.9.0/src/biopsykit/signals/ecg/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 import matplotlib.gridspec as gs
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticks
 import neurokit2 as nk
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from fau_colors import cmaps, colors_all
-from neurokit2.hrv.hrv_frequency import _hrv_frequency_show
-from neurokit2.hrv.hrv_utils import _hrv_get_rri
-
 from biopsykit.signals.ecg.ecg import _assert_ecg_input
 from biopsykit.utils.array_handling import sanitize_input_1d
 from biopsykit.utils.datatype_helper import EcgResultDataFrame
+from fau_colors import cmaps, colors_all
+from neurokit2.hrv.hrv_frequency import _hrv_frequency_show
+from neurokit2.hrv.hrv_utils import _hrv_get_rri
 
 if TYPE_CHECKING:
     from biopsykit.signals.ecg import EcgProcessor
 
 __all__ = [
     "ecg_plot",
     "hr_plot",
@@ -159,15 +158,15 @@
     if isinstance(ecg_signal.index, pd.DatetimeIndex):
         plt.rcParams["timezone"] = ecg_signal.index.tz.zone
     plt.rcParams["mathtext.default"] = "regular"
 
 
 def _ecg_plot_set_title(fig: plt.Figure, title: str):
     if title:
-        fig.suptitle("Electrocardiogram (ECG) – {}".format(title), fontweight="bold")
+        fig.suptitle(f"Electrocardiogram (ECG) - {title}", fontweight="bold")
     else:
         fig.suptitle("Electrocardiogram (ECG)", fontweight="bold")
 
 
 def _get_ecg_plot_specs(  # pylint:disable=too-many-branches
     fig: plt.Figure, plot_ecg_signal: bool, plot_individual_beats: bool, plot_distribution: bool
 ) -> Dict[str, plt.Axes]:
@@ -183,19 +182,18 @@
         if plot_distribution and plot_individual_beats:
             axs["beats"] = fig.add_subplot(spec[0, -1])
             axs["dist"] = fig.add_subplot(spec[1, -1])
         elif plot_individual_beats:
             axs["beats"] = fig.add_subplot(spec[:, -1])
         elif plot_distribution:
             axs["dist"] = fig.add_subplot(spec[:, -1])
+    elif plot_ecg_signal:
+        axs = {"ecg": fig.add_subplot(2, 1, 1), "hr": fig.add_subplot(2, 1, 2)}
     else:
-        if plot_ecg_signal:
-            axs = {"ecg": fig.add_subplot(2, 1, 1), "hr": fig.add_subplot(2, 1, 2)}
-        else:
-            axs = {"hr": fig.add_subplot(1, 1, 1)}
+        axs = {"hr": fig.add_subplot(1, 1, 1)}
     return axs
 
 
 def _ecg_plot(
     axs: Dict[str, plt.Axes],
     ecg_signal: EcgResultDataFrame,
     peaks: np.array,
@@ -250,18 +248,15 @@
         )
     axs["ecg"].set_ylabel("ECG Signal (z-norm.)")
     axs["ecg"].set_ylim(ylim_ecg)
 
     # Optimize legend
     handles, labels = axs["ecg"].get_legend_handles_labels()
     # order = [2, 0, 1, 3]
-    if "R_Peak_Outlier" in ecg_signal:
-        order = [0, 1, 2, 3]
-    else:
-        order = [0, 1, 2]
+    order = [0, 1, 2, 3] if "R_Peak_Outlier" in ecg_signal else [0, 1, 2]
 
     axs["ecg"].legend(
         [handles[idx] for idx in order], [labels[idx] for idx in order], loc=legend_loc, fontsize=legend_fontsize
     )
 
     axs["ecg"].tick_params(axis="x", which="both", bottom=True, labelbottom=True)
     axs["ecg"].tick_params(axis="y", which="major", left=True)
@@ -333,15 +328,15 @@
         fig, ax = plt.subplots(figsize=kwargs.get("figsize"))
     else:
         fig = ax.get_figure()
 
     sns.set_palette(cmaps.faculties)
 
     if title:
-        ax.set_title("Heart Rate – {}".format(title))
+        ax.set_title(f"Heart Rate - {title}")
 
     ax.plot(heart_rate["Heart_Rate"], color=color, label="Heart Rate", linewidth=1.5, **kwargs)
 
     if plot_mean:
         _hr_plot_plot_mean(heart_rate, mean_color, ax)
 
     ax.set_ylim(auto=True)
@@ -359,15 +354,15 @@
     return fig, ax
 
 
 def _hr_plot_plot_mean(heart_rate: pd.DataFrame, mean_color: str, ax: plt.Axes):
     rate_mean = heart_rate["Heart_Rate"].mean()
     ax.axhline(
         y=rate_mean,
-        label="Mean: {:.1f} bpm".format(rate_mean),
+        label=f"Mean: {rate_mean:.1f} bpm",
         linestyle="--",
         color=mean_color,
         linewidth=2,
     )
     ax.margins(x=0)
 
 
@@ -496,15 +491,15 @@
     axs["poin"] = fig.add_subplot(spec_within[1:4, 0:3])
     axs["poin_x"] = fig.add_subplot(spec_within[0, 0:3])
     axs["poin_y"] = fig.add_subplot(spec_within[1:4, 3])
     axs["poin"].get_shared_x_axes().join(axs["poin"], axs["poin_x"])
     axs["poin"].get_shared_y_axes().join(axs["poin"], axs["poin_y"])
 
     if title:
-        fig.suptitle("Heart Rate Variability (HRV) – {}".format(title), fontweight="bold")
+        fig.suptitle(f"Heart Rate Variability (HRV) - {title}", fontweight="bold")
     else:
         fig.suptitle("Heart Rate Variability (HRV)", fontweight="bold")
 
     rr_distribution_plot(rpeaks, sampling_rate, ax=axs["dist"])
     hrv_poincare_plot(rpeaks, sampling_rate, axs=[axs["poin"], axs["poin_x"], axs["poin_y"]])
     if plot_psd:
         hrv_frequency_plot(rpeaks, sampling_rate, ax=axs["freq"])
@@ -625,22 +620,22 @@
     ax2.boxplot(
         rri,
         vert=False,
         positions=[ax2.get_ylim()[-1] / 10 + 0.05 * ax2.get_ylim()[-1]],
         widths=ax2.get_ylim()[-1] / 10,
         manage_ticks=False,
         patch_artist=True,
-        boxprops=dict(
-            linewidth=2.0,
-            color=tech_light,
-            facecolor=colors_all.tech,
-        ),
-        medianprops=dict(linewidth=2.0, color=tech_light),
-        whiskerprops=dict(linewidth=2.0, color=tech_light),
-        capprops=dict(linewidth=2.0, color=tech_light),
+        boxprops={
+            "linewidth": 2.0,
+            "color": tech_light,
+            "facecolor": colors_all.tech,
+        },
+        medianprops={"linewidth": 2.0, "color": tech_light},
+        whiskerprops={"linewidth": 2.0, "color": tech_light},
+        capprops={"linewidth": 2.0, "color": tech_light},
         zorder=4,
     )
 
     ax.set_xlim(0.95 * np.min(rri), 1.05 * np.max(rri))
 
     fig.tight_layout()
     return fig, ax
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/eeg/eeg.py` & `biopsykit-0.9.0/src/biopsykit/signals/eeg/eeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Module for processing EEG data."""
 
 from typing import Dict, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
-from tqdm.auto import tqdm
-
 from biopsykit.signals._base import _BaseProcessor
+from tqdm.auto import tqdm
 
 
 class EegProcessor(_BaseProcessor):
     """Class for processing EEG data."""
 
     def __init__(
         self,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/imu/activity_counts.py` & `biopsykit-0.9.0/src/biopsykit/signals/imu/activity_counts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Module for generating Activity Counts from raw acceleration signals."""
 import datetime
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import pytz
-from scipy import signal
-
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import add_datetime_index, downsample, sanitize_input_nd
 from biopsykit.utils.datatype_helper import is_acc1d_dataframe, is_acc3d_dataframe
 from biopsykit.utils.time import tz
+from scipy import signal
 
 
 class ActivityCounts:
     """Generate Activity Counts from raw acceleration signals.
 
     Actigraph Activity Counts are a unit used in many human activity studies.
     However, it can only be outputted by the official Actigraph Software.
     The following implementation uses a reverse engineered version of the Actigraph filter based on
     (Brønd et al., 2017).
 
 
     References
     ----------
     Brønd, J. C., Andersen, L. B., & Arvidsson, D. (2017). Generating ActiGraph Counts from Raw Acceleration Recorded
-    by an Alternative Monitor. *Medicine and Science in Sports and Exercise*, 49(11), 2351–2360.
+    by an Alternative Monitor. *Medicine and Science in Sports and Exercise*, 49(11), 2351-2360.
     https://doi.org/10.1249/MSS.0000000000001344
 
     """
 
     data: pd.DataFrame = None
     sampling_rate: float = None
     activity_counts_: np.ndarray = None
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/imu/feature_extraction/static_moments.py` & `biopsykit-0.9.0/src/biopsykit/signals/imu/feature_extraction/static_moments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Extract features from static moments of IMU data."""
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from scipy.stats import skew
-
 from biopsykit.utils.array_handling import sanitize_input_nd
 from biopsykit.utils.time import tz
+from scipy.stats import skew
 
 
 def compute_features(
     data: pd.DataFrame,
     static_moments: pd.DataFrame,
     start: Optional[Union[str, pd.Timestamp]] = None,
     end: Optional[Union[str, pd.Timestamp]] = None,
@@ -79,20 +78,20 @@
     # dominant_orientation = mean_orientations.iloc[mean_orientations.index.argmax()]
     # dict_ori = {'sm_dominant_orientation_{}'.format(x): dominant_orientation.loc['acc_{}'.format(x)] for x
     #             in
     #             ['x', 'y', 'z']}
     # feature_dict.update(dict_ori)
 
     for dur, suffix in zip([durations, durations_60], ["", "_60"]):
-        feature_dict["sm_number{}".format(suffix)] = len(dur)
-        feature_dict["sm_max{}".format(suffix)] = np.max(dur)
-        feature_dict["sm_median{}".format(suffix)] = np.median(dur)
-        feature_dict["sm_mean{}".format(suffix)] = np.mean(dur)
-        feature_dict["sm_std{}".format(suffix)] = np.std(dur, ddof=1)
-        feature_dict["sm_skewness{}".format(suffix)] = skew(dur)
+        feature_dict[f"sm_number{suffix}"] = len(dur)
+        feature_dict[f"sm_max{suffix}"] = np.max(dur)
+        feature_dict[f"sm_median{suffix}"] = np.median(dur)
+        feature_dict[f"sm_mean{suffix}"] = np.mean(dur)
+        feature_dict[f"sm_std{suffix}"] = np.std(dur, ddof=1)
+        feature_dict[f"sm_skewness{suffix}"] = skew(dur)
 
     if index is None:
         index = 0
     return pd.DataFrame(feature_dict, index=[index])
 
 
 def _get_start_end(
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/imu/imu.py` & `biopsykit-0.9.0/src/biopsykit/signals/imu/imu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Module with functions to process IMU data."""
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sliding_window
 from biopsykit.utils.datatype_helper import Acc3dDataFrame, Gyr3dDataFrame, ImuDataFrame
 from biopsykit.utils.time import utc
 
 
 def convert_acc_data_to_g(
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/imu/rest_periods.py` & `biopsykit-0.9.0/src/biopsykit/signals/imu/rest_periods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module for computing Rest Periods from raw acceleration signals."""
 import datetime
 from typing import Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_num_columns
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sliding_window
 
 
 class RestPeriods:
     """Compute Rest Periods from raw acceleration signals.
@@ -19,15 +18,15 @@
     of the day.
 
 
     References
     ----------
     van Hees, V. T., Sabia, S., Anderson, K. N., Denton, S. J., Oliver, J., Catt, M., Abell, J. G., Kivimäki, M.,
     Trenell, M. I., & Singh-Manoux, A. (2015). A Novel, Open Access Method to Assess Sleep Duration Using a
-    Wrist-Worn Accelerometer. *PLoS ONE*, 10(11), 1–13. https://doi.org/10.1371/journal.pone.0142533
+    Wrist-Worn Accelerometer. *PLoS ONE*, 10(11), 1-13. https://doi.org/10.1371/journal.pone.0142533
 
     """
 
     sampling_rate: float
 
     def __init__(self, sampling_rate: float):
         """Initialize a new ``RestPeriods`` instance.
@@ -50,18 +49,15 @@
 
         Returns
         -------
         :class:`~pandas.DataFrame`
             dataframe with start, end, and total duration of each rest period detected by the algorithm
 
         """
-        if isinstance(data, pd.DataFrame):
-            data = data.filter(like="acc")
-        else:
-            data = pd.DataFrame(data)
+        data = data.filter(like="acc") if isinstance(data, pd.DataFrame) else pd.DataFrame(data)
 
         _assert_num_columns(data, 3)
 
         # rolling median 5 second
         data = data.rolling(int(5 * self.sampling_rate), min_periods=0).median()
 
         # get angle
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/imu/static_moment_detection.py` & `biopsykit-0.9.0/src/biopsykit/signals/imu/static_moment_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """A set of util functions to detect static regions in a IMU signal given certain constrains."""
-from typing import Optional, Sequence, Tuple, Union
+from typing import Literal, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from numpy.linalg import norm
-from typing_extensions import Literal
-
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import (
     _bool_fill,
     bool_array_to_start_end_array,
     sanitize_input_nd,
     sanitize_sliding_window_input,
     sliding_window_view,
 )
+from numpy.linalg import norm
 
 # supported metric functions
 _METRIC_FUNCTIONS = {
     "maximum": np.nanmax,
     "variance": np.nanvar,
     "mean": np.nanmean,
     "median": np.nanmedian,
@@ -80,15 +78,15 @@
 
     """
     # test for correct input data shape
     if np.shape(data)[-1] != 3:
         raise ValueError("Invalid signal dimensions, signal must be of shape (n,3).")
 
     if metric not in _METRIC_FUNCTIONS:
-        raise ValueError("Invalid metric passed! {} as metric is not supported.".format(metric))
+        raise ValueError(f"Invalid metric passed! {metric} as metric is not supported.")
 
     # add default overlap value
     if overlap is None:
         overlap = window_length - 1
 
     # allocate output array
     inactive_signal_bool_array = np.zeros(len(data))
@@ -277,32 +275,31 @@
     --------
     >>> sensor_1_gyro = ...
     >>> sensor_2_gyro = ...
     >>> find_first_static_window_multi_sensor([sensor_1_gyro, sensor_2_gyro], window_length=128, inactive_signal_th=5)
 
     """
     if metric not in _METRIC_FUNCTIONS:
-        raise ValueError("`metric` must be one of {}".format(list(_METRIC_FUNCTIONS.keys())))
+        raise ValueError(f"`metric` must be one of {list(_METRIC_FUNCTIONS.keys())}")
 
     if not isinstance(signals, np.ndarray):
         # all signals should have the same shape
         if not all(signals[0].shape == signal.shape for signal in signals):
             raise ValueError("All provided signals need to have the same shape.")
         if signals[0].ndim != 2:
             raise ValueError(
                 "The array of each sensor must be 2D, where the first dimension is the time and the second dimension "
                 "the sensor axis."
             )
         signals = np.hstack(signals)
-    else:
-        if signals.ndim != 3:
-            raise ValueError(
-                "If a array is used as input, it must be 3D, where the first dimension is the time, "
-                "the second indicates the sensor and the third the axis of the sensor."
-            )
+    elif signals.ndim != 3:
+        raise ValueError(
+            "If a array is used as input, it must be 3D, where the first dimension is the time, "
+            "the second indicates the sensor and the third the axis of the sensor."
+        )
 
     n_signals = signals.shape[1]
 
     windows = sliding_window_view(
         signals.reshape((signals.shape[0], -1)),
         window_length=window_length,
         overlap=window_length - 1,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/imu/wear_detection.py` & `biopsykit-0.9.0/src/biopsykit/signals/imu/wear_detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 """Module for detection non-wear times from raw acceleration signals."""
 import datetime
 from typing import Tuple, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_has_columns
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sliding_window
 
 
 class WearDetection:
     """Detect non-wear times from raw acceleration signals.
 
     Non-wear times are estimated over 15 minute intervals over the day.
 
+    The non-wear detection was implemented according to [1] and modified according to [2].
+
+
+    References
+    ----------
+    [1] Van Hees, V. T., Renström, F., Wright, A., Gradmark, A., Catt, M., Chen, K. Y., Löf, M., Bluck, L.,
+    Pomeroy, J., Wareham, N. J., Ekelund, U., Brage, S., & Franks, P. W. (2011). Estimation of Daily Energy
+    Expenditure in Pregnant and Non-Pregnant Women Using a Wrist-Worn Tri-Axial Accelerometer. PLoS ONE, 6(7), e22922.
+    https://doi.org/10.1371/journal.pone.0022922
+
+    [2] van Hees, V. T., Gorzelniak, L., Taherian, S., & Ekelund, U. (2013). Separating Movement and Gravity Components
+    in an Acceleration Signal and Implications for the Assessment of Human Daily Physical Activity. PLOS ONE, 8(4), 10.
+    https://doi.org/doi.org/10.1371/journal.pone.0061691
+
     """
 
     sampling_rate: float
 
     def __init__(self, sampling_rate: float):
         """Initialize a new ``WearDetection`` instance.
 
@@ -45,18 +58,15 @@
 
         """
         index = None
         index_resample = None
         if isinstance(data, (pd.DataFrame, pd.Series)):
             index = data.index
 
-        if isinstance(data, pd.DataFrame):
-            data = data.filter(like="acc")
-        else:
-            data = pd.DataFrame(data)
+        data = data.filter(like="acc") if isinstance(data, pd.DataFrame) else pd.DataFrame(data)
 
         window = 60  # min
         overlap = 15  # min
         overlap_percent = 1.0 - (overlap / window)
 
         acc_sliding = {
             col: sliding_window(
@@ -110,41 +120,39 @@
         if np.isnan(start_end[-1, -1]):
             last_idx = index_resample[-1, np.where(~np.isnan(index_resample[-1, :]))[0][-1]]
             start_end[-1, -1] = last_idx
 
         start_end = start_end.astype(int)
 
         if isinstance(index, pd.DatetimeIndex):
-            index_resample = pd.DataFrame(index.values[start_end], columns=["start", "end"])
-            index_resample = index_resample.apply(
-                lambda df: pd.to_datetime(df).dt.tz_localize("UTC").dt.tz_convert(index.tzinfo)
-            )
+            index_resample = pd.DataFrame(index.to_numpy()[start_end], columns=["start", "end"])
         return index_resample
 
     @staticmethod
     def _rescore_wear_detection(data: pd.DataFrame) -> pd.DataFrame:
         # group classifications into wear and non-wear blocks
         data["block"] = data["wear"].diff().ne(0).cumsum()
         blocks = list(data.groupby("block"))
 
         # iterate through blocks
         for (_, prev), (idx_curr, curr), (_, post) in zip(blocks[0:-2], blocks[1:-1], blocks[2:]):
             if curr["wear"].unique():
                 # get hour lengths of the previous, current, and next blocks
                 dur_prev, dur_curr, dur_post = (len(dur) * 0.25 for dur in [prev, curr, post])
 
-                if dur_curr < 3 and dur_curr / (dur_prev + dur_post) < 0.8:
-                    # if the current block is less than 3 hours and the ratio to previous and post blocks is
+                if (dur_curr < 3 and dur_curr / (dur_prev + dur_post) < 0.8) or (
+                    dur_curr < 6 and dur_curr / (dur_prev + dur_post) < 0.3
+                ):
+                    # a) if the current block is less than 3 hours and the ratio to previous and post blocks is
                     # less than 80% rescore the wear period as non-wear
-                    data.loc[data["block"] == idx_curr, "wear"] = 0
-                elif dur_curr < 6 and dur_curr / (dur_prev + dur_post) < 0.3:
-                    # if the current block is less than 6 hours and the ratio to previous and post blocks is
+                    # b) if the current block is less than 6 hours and the ratio to previous and post blocks is
                     # less than 30% rescore the wear period as non-wear
                     data.loc[data["block"] == idx_curr, "wear"] = 0
-        data.drop(columns=["block"], inplace=True)
+
+        data = data.drop(columns=["block"])
         return data
 
     @staticmethod
     def get_major_wear_block(data: pd.DataFrame) -> Tuple[Union[datetime.datetime, int], Union[datetime.datetime, int]]:
         """Return major wear block.
 
         The major wear block is the longest continuous wear block in the data.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `biopsykit-0.8.1/src/biopsykit/signals/rsp/rsp.py` & `biopsykit-0.9.0/src/biopsykit/signals/rsp/rsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module for processing Respiration data."""
 from typing import Dict, Optional, Sequence, Union
 
 import neurokit2 as nk
 import numpy as np
 import pandas as pd
 import scipy.signal as ss
-
 from biopsykit.signals._base import _BaseProcessor
 from biopsykit.utils.array_handling import sanitize_input_1d
 
 __all__ = ["RspProcessor"]
 
 
 class RspProcessor(_BaseProcessor):
@@ -68,15 +67,15 @@
         float
             Respiration rate during the given interval in bpm (breaths per minute)
 
 
         References
         ----------
         Schäfer, A., & Kratky, K. W. (2008). Estimation of Breathing Rate from Respiratory Sinus Arrhythmia:
-        Comparison of Various Methods. *Annals of Biomedical Engineering*, 36(3), 476–485.
+        Comparison of Various Methods. *Annals of Biomedical Engineering*, 36(3), 476-485.
         https://doi.org/10.1007/s10439-007-9428-1
 
 
         Examples
         --------
         >>> from biopsykit.signals.ecg import EcgProcessor
         >>> # initialize EcgProcessor instance
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/plotting.py` & `biopsykit-0.9.0/src/biopsykit/sleep/plotting.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticks
 import pandas as pd
 import seaborn as sns
-from fau_colors import colors_all
-
 from biopsykit.utils.datatype_helper import Acc3dDataFrame, Gyr3dDataFrame, ImuDataFrame, SleepEndpointDict
+from fau_colors import colors_all
 
 _sleep_imu_plot_params = {
     "background_color": ["#e0e0e0", "#9e9e9e"],
     "background_alpha": [0.3, 0.3],
 }
 
-_bbox_default = dict(
-    fc=(1, 1, 1, plt.rcParams["legend.framealpha"]),
-    ec=plt.rcParams["legend.edgecolor"],
-    boxstyle="round",
-)
+_bbox_default = {
+    "fc": (1, 1, 1, plt.rcParams["legend.framealpha"]),
+    "ec": plt.rcParams["legend.edgecolor"],
+    "boxstyle": "round",
+}
 
 
 def sleep_imu_plot(
     data: Union[Acc3dDataFrame, Gyr3dDataFrame, ImuDataFrame],
     datastreams: Optional[Union[str, Sequence[str]]] = None,
     sleep_endpoints: Optional[SleepEndpointDict] = None,
     downsample_factor: Optional[int] = None,
@@ -82,15 +81,15 @@
         figure object
     axs : list of :class:`~matplotlib.axes.Axes`
         list of subplot axes objects
 
     """
     axs: List[plt.Axes] = kwargs.pop("ax", kwargs.pop("axs", None))
 
-    sns.set_palette(kwargs.get("palette", sns.light_palette(getattr(colors_all, "fau"), n_colors=4, reverse=True)[:-1]))
+    sns.set_palette(kwargs.get("palette", sns.light_palette(colors_all.fau, n_colors=4, reverse=True)[:-1]))
 
     if datastreams is None:
         datastreams = ["acc"]
     if isinstance(datastreams, str):
         # ensure list
         datastreams = [datastreams]
 
@@ -203,15 +202,15 @@
         ax.vlines(
             [date + pd.Timedelta("1d")],
             0,
             1,
             transform=ax.get_xaxis_transform(),
             linewidths=3,
             linestyles="dotted",
-            colors=getattr(colors_all, "tech"),
+            colors=colors_all.tech,
             zorder=0,
         )
 
     _sleep_imu_plot_add_annotations(sleep_onset, wake_onset, bed_start, bed_end, sleep_bouts, wake_bouts, ax, **kwargs)
 
     # wear_time['end'] = wear_time.index.shift(1, freq=pd.Timedelta("15M"))
     # wear_time = wear_time[wear_time['wear'] == 0.0]
@@ -219,15 +218,15 @@
     #
     # handle = None
     # for idx, row in wear_time.iterrows():
     #     handle = ax.axvspan(row['index'], row['end'], color=colors.fau_color('wiso'), alpha=0.5, lw=0)
     # if handle is not None:
     #     handles['non-wear'] = handle
 
-    ax.set_title("Sleep IMU Data: {} – {}".format(date.date(), (date + pd.Timedelta("1d")).date()))
+    ax.set_title("Sleep IMU Data: {} - {}".format(date.date(), (date + pd.Timedelta("1d")).date()))
 
 
 def _sleep_imu_plot_add_annotations(
     sleep_onset: datetime.datetime,
     wake_onset: datetime.datetime,
     bed_start: datetime.datetime,
     bed_end: datetime.datetime,
@@ -272,137 +271,137 @@
     ax.vlines(
         [sleep_onset],
         0,
         1,
         transform=ax.get_xaxis_transform(),
         linewidth=3,
         linestyles="--",
-        colors=getattr(colors_all, "nat"),
+        colors=colors_all.nat,
         zorder=3,
     )
 
     # Sleep Onset Text + Arrow
     ax.annotate(
         "Sleep Onset",
         xy=(mdates.date2num(sleep_onset), 0.90),
         xycoords=ax.get_xaxis_transform(),
         xytext=(mdates.date2num(sleep_onset + pd.Timedelta("20min")), 0.90),
         textcoords=ax.get_xaxis_transform(),
         ha="left",
         va="center",
         bbox=bbox,
-        arrowprops=dict(
-            arrowstyle="->",
-            lw=2,
-            color=getattr(colors_all, "nat"),
-            shrinkA=0.0,
-            shrinkB=0.0,
-        ),
+        arrowprops={
+            "arrowstyle": "->",
+            "lw": 2,
+            "color": colors_all.nat,
+            "shrinkA": 0.0,
+            "shrinkB": 0.0,
+        },
     )
 
 
 def _sleep_imu_plot_add_wake_onset(wake_onset, ax: plt.Axes, **kwargs):
     bbox = kwargs.get("bbox", _bbox_default)
     # Wake Onset vline
     ax.vlines(
         [wake_onset],
         0,
         1,
         transform=ax.get_xaxis_transform(),
         linewidth=3,
         linestyles="--",
-        colors=getattr(colors_all, "nat"),
+        colors=colors_all.nat,
         zorder=3,
     )
 
     # Wake Onset Text + Arrow
     ax.annotate(
         "Wake Onset",
         xy=(mdates.date2num(wake_onset), 0.90),
         xycoords=ax.get_xaxis_transform(),
         xytext=(mdates.date2num(wake_onset - pd.Timedelta("20min")), 0.90),
         textcoords=ax.get_xaxis_transform(),
         ha="right",
         va="center",
         bbox=bbox,
-        arrowprops=dict(
-            arrowstyle="->",
-            lw=2,
-            color=getattr(colors_all, "nat"),
-            shrinkA=0.0,
-            shrinkB=0.0,
-        ),
+        arrowprops={
+            "arrowstyle": "->",
+            "lw": 2,
+            "color": colors_all.nat,
+            "shrinkA": 0.0,
+            "shrinkB": 0.0,
+        },
     )
 
 
 def _sleep_imu_plot_add_bed_start(sleep_onset, bed_start, ax: plt.Axes, **kwargs):
     bbox = kwargs.get("bbox", _bbox_default)
 
     # Bed Start vline
     ax.vlines(
         [bed_start],
         0,
         1,
         transform=ax.get_xaxis_transform(),
         linewidth=3,
         linestyles="--",
-        colors=getattr(colors_all, "med"),
+        colors=colors_all.med,
         zorder=3,
     )
     # Bed Start Text + Arrow
     ax.annotate(
         "Bed Interval Start",
         xy=(mdates.date2num(bed_start), 0.80),
         xycoords=ax.get_xaxis_transform(),
         xytext=(mdates.date2num(sleep_onset + pd.Timedelta("20min")), 0.80),
         textcoords=ax.get_xaxis_transform(),
         ha="left",
         va="center",
         bbox=bbox,
-        arrowprops=dict(
-            arrowstyle="->",
-            lw=2,
-            color=getattr(colors_all, "med"),
-            shrinkA=0.0,
-            shrinkB=0.0,
-        ),
+        arrowprops={
+            "arrowstyle": "->",
+            "lw": 2,
+            "color": colors_all.med,
+            "shrinkA": 0.0,
+            "shrinkB": 0.0,
+        },
     )
 
 
 def _sleep_imu_plot_add_bed_end(wake_onset, bed_end, ax: plt.Axes, **kwargs):
     bbox = kwargs.get("bbox", _bbox_default)
 
     # Bed End vline
     ax.vlines(
         [bed_end],
         0,
         1,
         transform=ax.get_xaxis_transform(),
         linewidth=3,
         linestyles="--",
-        colors=getattr(colors_all, "med"),
+        colors=colors_all.med,
         zorder=3,
     )
     # Bed End Text + Arrow
     ax.annotate(
         "Bed Interval End",
         xy=(mdates.date2num(bed_end), 0.80),
         xycoords=ax.get_xaxis_transform(),
         xytext=(mdates.date2num(wake_onset - pd.Timedelta("20min")), 0.80),
         textcoords=ax.get_xaxis_transform(),
         ha="right",
         va="center",
         bbox=bbox,
-        arrowprops=dict(
-            arrowstyle="->",
-            lw=2,
-            color=getattr(colors_all, "med"),
-            shrinkA=0.0,
-            shrinkB=0.0,
-        ),
+        arrowprops={
+            "arrowstyle": "->",
+            "lw": 2,
+            "color": colors_all.med,
+            "shrinkA": 0.0,
+            "shrinkB": 0.0,
+        },
     )
 
 
 def _sleep_imu_plot_add_sleep_wake_bouts(
     sleep_bouts: pd.DataFrame, wake_bouts: pd.DataFrame, ax: plt.Axes, **kwargs
 ) -> Dict[str, plt.Artist]:
     handles = {}
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_endpoints/sleep_endpoints.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_endpoints/sleep_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Functions for computing sleep endpoints, i.e., parameters that characterize a recording during a sleep study."""
 from numbers import Number
 from typing import Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils.datatype_helper import SleepEndpointDataFrame, SleepEndpointDict, _SleepEndpointDataFrame
 
 
 def compute_sleep_endpoints(
     sleep_wake: pd.DataFrame, bed_interval: Sequence[Union[str, int, np.datetime64]]
 ) -> SleepEndpointDict:
     """Compute a set of sleep endpoints based on sleep/wake information and time spent in bed.
@@ -66,19 +65,19 @@
 
     # get percent of total time asleep
     sleep_efficiency = 100.0 * (len(net_sleep_time) / len(sleep_wake))
     # wake after sleep onset = duration of wake during first and last 'sleep' sample
     wake_after_sleep_onset = len(df_sw_sleep) - int(df_sw_sleep.sum()[0])
 
     df_sw_sleep["block"] = df_sw_sleep["sleep_wake"].diff().ne(0).cumsum()
-    df_sw_sleep.reset_index(inplace=True)
-    df_sw_sleep.rename(columns={"index": "time"}, inplace=True)
+    df_sw_sleep = df_sw_sleep.reset_index()
+    df_sw_sleep = df_sw_sleep.rename(columns={"index": "time"})
     bouts = df_sw_sleep.groupby(by="block")
     df_start_stop = bouts.first()
-    df_start_stop.rename(columns={"time": "start"}, inplace=True)
+    df_start_stop = df_start_stop.rename(columns={"time": "start"})
     df_start_stop["end"] = bouts.last()["time"]
 
     # add 1 min to end for continuous time coverage
     if df_start_stop["end"].dtype == np.int64:
         df_start_stop["end"] = df_start_stop["end"] + 1
     else:
         df_start_stop["end"] = df_start_stop["end"] + pd.Timedelta("1m")
@@ -143,23 +142,23 @@
         dataframe with computed Sleep Endpoints or ``None`` if ``sleep_endpoints`` is ``None``
 
     """
     if sleep_endpoints is None:
         return None
 
     sleep_endpoints = sleep_endpoints.copy()
-    sleep_bouts = sleep_endpoints.pop("sleep_bouts", None).values.tolist()
-    wake_bouts = sleep_endpoints.pop("wake_bouts", None).values.tolist()
+    sleep_bouts = sleep_endpoints.pop("sleep_bouts", None).to_numpy().tolist()
+    wake_bouts = sleep_endpoints.pop("wake_bouts", None).to_numpy().tolist()
 
     sleep_bouts = [tuple(v) for v in sleep_bouts]
     wake_bouts = [tuple(v) for v in wake_bouts]
 
     index = pd.to_datetime(pd.Index([sleep_endpoints["date"]], name="date"))
     sleep_endpoints.pop("date")
 
     df = pd.DataFrame(sleep_endpoints, index=index)
-    df.fillna(value=np.nan, inplace=True)
+    df = df.fillna(value=np.nan)
     df["sleep_bouts"] = None
     df["wake_bouts"] = None
-    df.at[df.index[0], "sleep_bouts"] = sleep_bouts
-    df.at[df.index[0], "wake_bouts"] = wake_bouts
+    df.at[df.index[0], "sleep_bouts"] = sleep_bouts  # noqa: PD008
+    df.at[df.index[0], "wake_bouts"] = wake_bouts  # noqa: PD008
     return _SleepEndpointDataFrame(df)
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_processing_pipeline/sleep_processing_pipeline.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_processing_pipeline/sleep_processing_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Functions to process sleep data from raw IMU data or Actigraph data."""
 from typing import Any, Dict, Optional, Sequence, Union
 
 import numpy as np
-
 from biopsykit.signals.imu import convert_acc_data_to_g
 from biopsykit.signals.imu.activity_counts import ActivityCounts
 from biopsykit.signals.imu.rest_periods import RestPeriods
 from biopsykit.signals.imu.wear_detection import WearDetection
 from biopsykit.sleep.sleep_endpoints import compute_sleep_endpoints
 from biopsykit.sleep.sleep_wake_detection.sleep_wake_detection import SleepWakeDetection
 from biopsykit.utils._types import arr_t
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/_base.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/_base.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Sleep/Wake detection using the *Cole/Kripke Algorithm*."""
 import numpy as np
 import pandas as pd
-
 from biopsykit.sleep.sleep_wake_detection.algorithms._base import _SleepWakeBase
 from biopsykit.sleep.sleep_wake_detection.utils import rescore
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sanitize_input_1d
 from biopsykit.utils.datatype_helper import SleepWakeDataFrame, _SleepWakeDataFrame
 
 
@@ -29,20 +28,20 @@
             The recommended range for the scale factor is between 0.1 and 0.25 depending on the sensitivity to activity
             desired, and possibly the population being observed. According to the paper by Cole and Kripke,
             the scale factor depends on the epoch length. See the paper for more details.
 
         References
         ----------
         Cole, R. J., Kripke, D. F., Gruen, W., Mullaney, D. J., & Gillin, J. C. (1992). Automatic Sleep/Wake
-        Identification From Wrist Activity. *Sleep*, 15(5), 461–469. https://doi.org/10.1093/sleep/15.5.461
+        Identification From Wrist Activity. *Sleep*, 15(5), 461-469. https://doi.org/10.1093/sleep/15.5.461
 
         """
         super().__init__(**kwargs)
 
-    def fit(self, data: arr_t, **kwargs):
+    def fit(self, data: arr_t, **kwargs):  # noqa: ARG002
         """Fit sleep/wake detection algorithm to input data.
 
         .. note::
             Algorithms that do not have to (re)fit a ML model before sleep/wake prediction, such as rule-based
             algorithms, will internally bypass this method as the ``fit`` step is not needed.
 
         Parameters
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke_old.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/cole_kripke_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Sleep/Wake detection using the *Cole/Kripke Algorithm*."""
 import numpy as np
 import pandas as pd
-
 from biopsykit.sleep.sleep_wake_detection.algorithms._base import _SleepWakeBase
 from biopsykit.sleep.sleep_wake_detection.utils import rescore
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sanitize_input_1d
 from biopsykit.utils.datatype_helper import SleepWakeDataFrame, _SleepWakeDataFrame
 
 
@@ -26,44 +25,44 @@
             the activity index, if other activity measures are desired the scale factor can be modified or optimized.)
             The recommended range for the scale factor is between 0.1 and 0.25 depending on the sensitivity to activity
             desired, and possibly the population being observed.
 
         References
         ----------
         Cole, R. J., Kripke, D. F., Gruen, W., Mullaney, D. J., & Gillin, J. C. (1992). Automatic Sleep/Wake
-        Identification From Wrist Activity. *Sleep*, 15(5), 461–469. https://doi.org/10.1093/sleep/15.5.461
+        Identification From Wrist Activity. *Sleep*, 15(5), 461-469. https://doi.org/10.1093/sleep/15.5.461
 
         """
         self.scale_factor: float = kwargs.pop("scale_factor", None)
         """Scale factor to use for the predictions (default corresponds to scale factor optimized for use with the
         activity index, if other activity measures are desired the scale factor can be modified or optimized).
         The recommended range for the scale factor is between 0.1 and 0.25 depending on the sensitivity to activity
         desired, and possibly the population being observed.
         """
 
         if self.scale_factor is None:
             self.scale_factor = 0.193125
         super().__init__(**kwargs)
 
-    def fit(self, data: arr_t, **kwargs) -> arr_t:
+    def fit(self, data: arr_t, **kwargs) -> arr_t:  # noqa: ARG002
         """Fit sleep/wake detection algorithm to input data.
 
         .. note::
             Algorithms that do not have to (re)fit a ML model before sleep/wake prediction, such as rule-based
             algorithms, will internally bypass this method as the ``fit`` step is not needed.
 
         Parameters
         ----------
         data : array_like
             input data
 
         """
         return
 
-    def predict(self, data: arr_t, **kwargs) -> SleepWakeDataFrame:
+    def predict(self, data: arr_t, **kwargs) -> SleepWakeDataFrame:  # noqa: ARG002
         """Apply sleep/wake prediction on activity index values.
 
         Parameters
         ----------
         data : array_like
             array with activity index values
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/sadeh.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/sadeh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Sleep/Wake detection using the *Sadeh Algorithm*."""
 import numpy as np
 import pandas as pd
-
 from biopsykit.sleep.sleep_wake_detection.algorithms._base import _SleepWakeBase
 from biopsykit.sleep.sleep_wake_detection.utils import rescore
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sanitize_input_1d, sliding_window
 from biopsykit.utils.datatype_helper import SleepWakeDataFrame, _SleepWakeDataFrame
 
 
@@ -22,15 +21,15 @@
         References
         ----------
         add reference
 
         """
         super().__init__(**kwargs)
 
-    def fit(self, data: arr_t, **kwargs):
+    def fit(self, data: arr_t, **kwargs):  # noqa: ARG002
         """Fit sleep/wake detection algorithm to input data.
 
         .. note::
             Algorithms that do not have to (re)fit a ML model before sleep/wake prediction, such as rule-based
             algorithms, will internally bypass this method as the ``fit`` step is not needed.
 
         Parameters
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/sazonov.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/sazonov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Sleep/Wake detection using the *Sazonov Algorithm*."""
 import numpy as np
 import pandas as pd
-from scipy.special import expit
-
 from biopsykit.sleep.sleep_wake_detection.algorithms._base import _SleepWakeBase
 from biopsykit.sleep.sleep_wake_detection.utils import rescore
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sanitize_input_1d, sliding_window
 from biopsykit.utils.datatype_helper import SleepWakeDataFrame, _SleepWakeDataFrame
+from scipy.special import expit
 
 
 class Sazonov(_SleepWakeBase):
     """Class representing the *Sazonov Algorithm* for sleep/wake detection based on activity counts."""
 
     def __init__(self, **kwargs):  # pylint:disable=useless-super-delegation
         """Class representing the *Sazonov Algorithm* for sleep/wake detection based on activity counts.
@@ -23,15 +22,15 @@
         References
         ----------
         add reference
 
         """
         super().__init__(**kwargs)
 
-    def fit(self, data: arr_t, **kwargs):
+    def fit(self, data: arr_t, **kwargs):  # noqa: ARG002
         """Fit sleep/wake detection algorithm to input data.
 
         .. note::
             Algorithms that do not have to (re)fit a ML model before sleep/wake prediction, such as rule-based
             algorithms, will internally bypass this method as the ``fit`` step is not needed.
 
         Parameters
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/scripps_clinic.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/scripps_clinic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Sleep/Wake detection using the *Scripps Clinic Algorithm*."""
 import numpy as np
 import pandas as pd
-
 from biopsykit.sleep.sleep_wake_detection.algorithms._base import _SleepWakeBase
 from biopsykit.sleep.sleep_wake_detection.utils import rescore
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sanitize_input_1d
 from biopsykit.utils.datatype_helper import SleepWakeDataFrame, _SleepWakeDataFrame
 
 
@@ -36,15 +35,15 @@
         self.scale_factor: float = scale_factor
         """scale factor to use for the predictions (default corresponds to scale factor optimized for use with the
         activity index, if other activity measures are desired the scale factor can be modified or optimized.).
         Default: 0.30
         """
         super().__init__(**kwargs)
 
-    def fit(self, data: arr_t, **kwargs):
+    def fit(self, data: arr_t, **kwargs):  # noqa: ARG002
         """Fit sleep/wake detection algorithm to input data.
 
         .. note::
             Algorithms that do not have to (re)fit a ML model before sleep/wake prediction, such as rule-based
             algorithms, will internally bypass this method as the ``fit`` step is not needed.
 
         Parameters
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/algorithms/webster.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/algorithms/webster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Sleep/Wake detection using the *Webster Algorithm*."""
 import numpy as np
 import pandas as pd
-
 from biopsykit.sleep.sleep_wake_detection.algorithms._base import _SleepWakeBase
 from biopsykit.sleep.sleep_wake_detection.utils import rescore
 from biopsykit.utils._types import arr_t
 from biopsykit.utils.array_handling import sanitize_input_1d
 from biopsykit.utils.datatype_helper import SleepWakeDataFrame, _SleepWakeDataFrame
 
 
@@ -36,15 +35,15 @@
         self.scale_factor: float = scale_factor
         """scale factor to use for the predictions (default corresponds to scale factor optimized for use with the
         activity index, if other activity measures are desired the scale factor can be modified or optimized.).
         Default: 0.025
         """
         super().__init__(**kwargs)
 
-    def fit(self, data: arr_t, **kwargs):
+    def fit(self, data: arr_t, **kwargs):  # noqa: ARG002
         """Fit sleep/wake detection algorithm to input data.
 
         .. note::
             Algorithms that do not have to (re)fit a ML model before sleep/wake prediction, such as rule-based
             algorithms, will internally bypass this method as the ``fit`` step is not needed.
 
         Parameters
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/sleep_wake_detection.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/sleep_wake_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 
         Returns
         -------
         :obj:`~biopsykit.utils.datatype_helper.SleepWakeDataFrame`
             dataframe with sleep/wake predictions
 
         """
-        return _SleepWakeDataFrame(getattr(self.sleep_wake_algo, "predict")(data, **kwargs))
+        return _SleepWakeDataFrame(self.sleep_wake_algo.predict(data, **kwargs))
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/sleep_wake_detection/utils.py` & `biopsykit-0.9.0/src/biopsykit/sleep/sleep_wake_detection/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utility functions for sleep/wake detection algorithms."""
 
-from typing import Optional
+from typing import Literal, Optional
 
 import numpy as np
-from typing_extensions import Literal
 
 EPOCH_LENGTH = Literal[30, 60]
 
 
 def rescore(predictions: np.ndarray, epoch_length: Optional[EPOCH_LENGTH] = 30) -> np.ndarray:
     """Apply Webster's rescoring rules to sleep/wake predictions.
 
@@ -39,37 +38,36 @@
 
 
 def _apply_recording_rules_a_c(rescored: np.ndarray, epoch_length: EPOCH_LENGTH):  # pylint:disable=too-many-branches
     wake_bin = 0
     for t in range(len(rescored)):  # pylint:disable=consider-using-enumerate
         if rescored[t] == 1:
             wake_bin += 1
+        elif epoch_length == 30:
+            if wake_bin >= 30:
+                # rule c: at least 15 minutes of wake, next 4 minutes of sleep get rescored
+                rescored[t : t + 8] = 0
+            elif 20 <= wake_bin < 30:
+                # rule b: at least 10 minutes of wake, next 3 minutes of sleep get rescored
+                rescored[t : t + 6] = 0
+            elif 8 <= wake_bin < 20:
+                # rule a: at least 4 minutes of wake, next 1 minute of sleep gets rescored
+                rescored[t : t + 2] = 0
+            wake_bin = 0
         else:
-            if epoch_length == 30:
-                if wake_bin >= 30:
-                    # rule c: at least 15 minutes of wake, next 4 minutes of sleep get rescored
-                    rescored[t : t + 8] = 0
-                elif 20 <= wake_bin < 30:
-                    # rule b: at least 10 minutes of wake, next 3 minutes of sleep get rescored
-                    rescored[t : t + 6] = 0
-                elif 8 <= wake_bin < 20:
-                    # rule a: at least 4 minutes of wake, next 1 minute of sleep gets rescored
-                    rescored[t : t + 2] = 0
-                wake_bin = 0
-            else:
-                if wake_bin >= 15:
-                    # rule c: at least 15 minutes of wake, next 4 minutes of sleep get rescored
-                    rescored[t : t + 4] = 0
-                elif 10 <= wake_bin < 15:
-                    # rule b: at least 10 minutes of wake, next 3 minutes of sleep get rescored
-                    rescored[t : t + 3] = 0
-                elif 4 <= wake_bin < 10:
-                    # rule a: at least 4 minutes of wake, next 1 minute of sleep gets rescored
-                    rescored[t : t + 1] = 0
-                wake_bin = 0
+            if wake_bin >= 15:
+                # rule c: at least 15 minutes of wake, next 4 minutes of sleep get rescored
+                rescored[t : t + 4] = 0
+            elif 10 <= wake_bin < 15:
+                # rule b: at least 10 minutes of wake, next 3 minutes of sleep get rescored
+                rescored[t : t + 3] = 0
+            elif 4 <= wake_bin < 10:
+                # rule a: at least 4 minutes of wake, next 1 minute of sleep gets rescored
+                rescored[t : t + 1] = 0
+            wake_bin = 0
 
     return rescored
 
 
 def _apply_recording_rules_d_e(rescored: np.ndarray, epoch_length: EPOCH_LENGTH):  # pylint:disable=too-many-branches
     # rule d/e: 6/10 minutes or less of sleep surrounded by at least 10/20 minutes of wake on each side get rescored
     if epoch_length == 30:
```

### Comparing `biopsykit-0.8.1/src/biopsykit/sleep/utils.py` & `biopsykit-0.9.0/src/biopsykit/sleep/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module with utility functions to handle sleep data."""
 import datetime
 from typing import Dict
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_is_dtype
 
 
 def split_nights(data: pd.DataFrame) -> Dict[str, pd.DataFrame]:
     """Split continuous data into individual nights.
 
     This function splits data into individual nights. The split is performed at 6pm because that's the time of day
```

### Comparing `biopsykit-0.8.1/src/biopsykit/stats/multicoll.py` & `biopsykit-0.9.0/src/biopsykit/stats/multicoll.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/stats/regression.py` & `biopsykit-0.9.0/src/biopsykit/stats/regression.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/stats/stats.py` & `biopsykit-0.9.0/src/biopsykit/stats/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Module for setting up a pipeline for statistical analysis."""
 import re
 import warnings
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union
 
 import pandas as pd
 import pingouin as pg
-from typing_extensions import Literal
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension, _assert_has_index_levels
 from biopsykit.utils._types import path_t, str_t
 
 MAP_STAT_TESTS = {
     "normality": pg.normality,
     "equal_var": pg.homoscedasticity,
     "anova": pg.anova,
@@ -230,15 +228,15 @@
 
             if step[0] == "prep":
                 grouper, specific_params = self._get_specific_params_prep(grouper, general_params, specific_params)
 
             test_func = MAP_STAT_TESTS[step[1]]
             if len(grouper) > 0:
                 result = data.groupby(grouper, sort=general_params.get("sort", True)).apply(
-                    lambda df: test_func(data=df, **specific_params, **params)  # pylint:disable=cell-var-from-loop
+                    lambda df, tf=test_func, sp=specific_params, p=params: tf(data=df, **sp, **p)
                 )
             else:
                 result = test_func(data=data, **specific_params, **params)
 
             if i == len(self.steps) - 1 and "multicomp" in general_params:
                 # apply multi-comparison correction (p-adjustment) for the last analysis step in the pipeline
                 # if it was enabled
@@ -367,18 +365,15 @@
         else:
             self._display_results(sig_only, **kwargs)
 
     def _get_sig_only(self, sig_only: Optional[Union[str, bool, Sequence[str], Dict[str, bool]]] = None):
         if sig_only is None:
             sig_only = {}
         if isinstance(sig_only, str):
-            if sig_only == "all":
-                sig_only = True
-            else:
-                sig_only = [sig_only]
+            sig_only = True if sig_only == "all" else [sig_only]
         if isinstance(sig_only, bool):
             sig_only = {cat: sig_only for cat in self.category_steps}
         if isinstance(sig_only, list):
             sig_only = {cat: cat in sig_only for cat in self.category_steps}
         return sig_only
 
     def _display_results(
@@ -888,18 +883,15 @@
         return data.groupby(group_cols, group_keys=False).apply(lambda df: self._multicomp_lambda(df, method=method))
 
     @classmethod
     def _multicomp_get_levels(cls, levels: Union[bool, str, Sequence[str]], data: pd.DataFrame) -> Sequence[str]:
         if levels is None:
             levels = []
         elif isinstance(levels, bool):
-            if levels:
-                levels = list(data.index.names)[:-1]
-            else:
-                levels = []
+            levels = list(data.index.names)[:-1] if levels else []
         elif isinstance(levels, str):
             levels = [levels]
         return levels
 
     @staticmethod
     def _multicomp_lambda(data: pd.DataFrame, method: str) -> pd.DataFrame:
         for col in list(reversed(_sig_cols[1:])):
@@ -914,15 +906,15 @@
     ):
         if isinstance(stats_category_or_data, (str, pd.DataFrame)):
             if isinstance(stats_category_or_data, str):
                 stats_data = self._filter_effect(stats_category_or_data, stats_effect_type)
             else:
                 stats_data = stats_category_or_data
         else:
-            raise ValueError(
+            raise TypeError(
                 "Either string with stats category (e.g., 'test' or 'posthoc') or dataframe with stats results must "
                 "be supplied as parameter! "
             )
         return self._filter_sig(stats_data)
 
     @staticmethod
     def _sanitize_features_input(features: Union[str, Sequence[str], Dict[str, Union[str, Sequence[str]]]]):
@@ -1055,46 +1047,40 @@
         return data
 
     def _extract_data_anova(self, data: pd.DataFrame, pcol: str, collapse_dof: bool) -> pd.DataFrame:
         rename_dict = {"ddof1": "df1", "ddof2": "df2", "DF": "df", "DF1": "df1", "DF2": "df2"}
         data = data.rename(columns=rename_dict)
         columns = []
         if collapse_dof:
-            if "df1" in data.columns:
-                dof_cols = ["df1", "df2"]
-            else:
-                dof_cols = ["df"]
-            dofs = tuple((data[col].unique() for col in dof_cols))
+            dof_cols = ["df1", "df2"] if "df1" in data.columns else ["df"]
+            dofs = tuple(data[col].unique() for col in dof_cols)
             if any(len(d) != 1 for d in dofs):
                 raise ValueError(f"Cannot collapse dof in table: dof are not unique! Got {dofs}.")
             dofs = [self._format_dof(dof[0]) for dof in dofs]
             f_col = MAP_LATEX_EXPORT["F_collapse"].format(*dofs)
             columns.append(f_col)
             data = data.rename(columns={"F": f_col})
             data = data.drop(columns=["df1", "df2", "df"], errors="ignore")
         else:
             if "df1" in data.columns:
                 data["df"] = "{" + data["df1"].astype(str) + ", " + data["df2"].astype(str) + "}"
                 data = data.drop(columns=["df1", "df2"])
             columns.append("df")
         eff_name = self._get_effsize_name(data)
-        columns = columns + [pcol, eff_name]
+        columns = [*columns, pcol, eff_name]
         data = data[columns]
         return data
 
     def _extract_data_friedman(self, data: pd.DataFrame, pcol: str, collapse_dof: bool) -> pd.DataFrame:
         rename_dict = {"ddof1": "df1", "ddof2": "df2"}
         data = data.rename(columns=rename_dict)
         columns = []
         if collapse_dof:
-            if "df2" in data.columns:
-                dof_cols = ["df1", "df2"]
-            else:
-                dof_cols = ["df1"]
-            dofs = tuple((data[col].unique() for col in dof_cols))
+            dof_cols = ["df1", "df2"] if "df2" in data.columns else ["df1"]
+            dofs = tuple(data[col].unique() for col in dof_cols)
             if any(len(d) != 1 for d in dofs):
                 raise ValueError(f"Cannot collapse dof in table: dof are not unique! Got {dofs}.")
             dofs = [self._format_dof(dof[0]) for dof in dofs]
             if "F" in data.columns:
                 f_col = MAP_LATEX_EXPORT["F_collapse"].format(*dofs)
                 columns.append(f_col)
                 data = data.rename(columns={"F": f_col})
@@ -1105,15 +1091,15 @@
                 data = data.rename(columns={"Q": q_col})
                 data = data.drop(columns=["df1", "df2", "df"], errors="ignore")
         else:
             if "df2" in data.columns:
                 data["df"] = "{" + data["df1"].astype(str) + ", " + data["df2"].astype(str) + "}"
                 data = data.drop(columns=["df1", "df2"])
             columns.append("df")
-        columns = columns + [pcol]
+        columns = [*columns, pcol]
         data = data[columns]
         return data
 
     @staticmethod
     def _extract_data_mwu(data: pd.DataFrame, pcol: str) -> pd.DataFrame:
         columns = ["U-val", pcol, StatsPipeline._get_effsize_name(data)]
         data = data[columns]
@@ -1202,43 +1188,41 @@
         data: pd.DataFrame, index_value_order: Union[Sequence[str], Dict[str, Sequence[str]]]
     ) -> pd.DataFrame:
         if isinstance(data.index, pd.MultiIndex):
             if isinstance(index_value_order, dict):
                 for key, val in index_value_order.items():
                     data = data.reindex(val, level=key)
             else:
-                raise ValueError(
+                raise TypeError(
                     "'index_value_order' must be a dictionary with index level names as keys and "
                     "index values as values."
                 )
+        elif isinstance(index_value_order, dict):
+            data = data.reindex(index_value_order[data.index.name])
         else:
-            if isinstance(index_value_order, dict):
-                data = data.reindex(index_value_order[data.index.name])
-            else:
-                data = data.reindex(index_value_order)
+            data = data.reindex(index_value_order)
         return data
 
     @staticmethod
     def _apply_column_value_order(
         data: pd.DataFrame, column_value_order: Union[Sequence[str], Dict[str, Sequence[str]]]
     ) -> pd.DataFrame:
         if isinstance(data.columns, pd.MultiIndex):
             if isinstance(column_value_order, dict):
                 for key, val in column_value_order.items():
                     data = data.reindex(val, level=key, axis=1)
             else:
-                raise ValueError(
+                raise TypeError(
                     "'column_value_order' must be a dictionary with column level names as keys and "
                     "column values as values."
                 )
+        elif isinstance(column_value_order, dict):
+            data = data.reindex(column_value_order[data.index.name], axis=1)
         else:
-            if isinstance(column_value_order, dict):
-                data = data.reindex(column_value_order[data.index.name], axis=1)
-            else:
-                data = data.reindex(column_value_order, axis=1)
+            data = data.reindex(column_value_order, axis=1)
         return data
 
     @staticmethod
     def _format_latex_column_format(data: pd.DataFrame):
         column_format = "l" * data.index.nlevels + "||"
         if isinstance(data.columns, pd.MultiIndex):
             ncols = len(data.columns)
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/_datatype_validation_helper.py` & `biopsykit-0.9.0/src/biopsykit/utils/_datatype_validation_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Internal helpers for dataset validation."""
 from pathlib import Path
 from typing import Any, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._types import _Hashable, path_t
 from biopsykit.utils.exceptions import FileExtensionError, ValidationError, ValueRangeError
 
 
 def _assert_is_dir(path: path_t, raise_exception: Optional[bool] = True) -> Optional[bool]:
     """Check if a path is a directory.
 
@@ -29,15 +28,15 @@
         if ``raise_exception`` is ``True`` and ``path`` is not a directory
 
     """
     # ensure pathlib
     file_name = Path(path)
     if not file_name.is_dir():
         if raise_exception:
-            raise ValueError("The path '{}' is expected to be a directory, but it's not!".format(path))
+            raise ValueError(f"The path '{path}' is expected to be a directory, but it's not!")
         return False
 
     return True
 
 
 def _assert_file_extension(
     file_name: path_t, expected_extension: Union[str, Sequence[str]], raise_exception: Optional[bool] = True
@@ -101,17 +100,15 @@
     ------
     :exc:`~biopsykit.exceptions.ValidationError`
         if ``raise_exception`` is ``True`` and ``obj`` is none of the expected data types
 
     """
     if not isinstance(obj, dtype):
         if raise_exception:
-            raise ValidationError(
-                "The data object is expected to be one of ({},). But it is a {}".format(dtype, type(obj))
-            )
+            raise ValidationError(f"The data object is expected to be one of ({dtype},). But it is a {type(obj)}")
         return False
     return True
 
 
 def _assert_has_multiindex(
     df: pd.DataFrame,
     expected: Optional[bool] = True,
@@ -234,17 +231,17 @@
     columns = df.columns
     result = False
     for col_set in columns_sets:
         result = result or all(v in columns for v in col_set)
 
     if result is False:
         if len(columns_sets) == 1:
-            helper_str = "the following columns: {}".format(columns_sets[0])
+            helper_str = f"the following columns: {columns_sets[0]}"
         else:
-            helper_str = "one of the following sets of columns: {}".format(columns_sets)
+            helper_str = f"one of the following sets of columns: {columns_sets}"
         if raise_exception:
             raise ValidationError(
                 "The dataframe is expected to have {}. Instead it has the following columns: {}".format(
                     helper_str, list(df.columns)
                 )
             )
     return result
@@ -332,17 +329,17 @@
     result = False
     for columns in column_levels:
         for col_set in columns_sets:
             result = result or all(v in columns for v in col_set)
 
     if result is False:
         if len(columns_sets) == 1:
-            helper_str = "the following columns: {}".format(columns_sets[0])
+            helper_str = f"the following columns: {columns_sets[0]}"
         else:
-            helper_str = "one of the following sets of columns: {}".format(columns_sets)
+            helper_str = f"one of the following sets of columns: {columns_sets}"
         if raise_exception:
             raise ValidationError(
                 "The dataframe is expected to have {} at any level of the MultiIndex. Instead it has the "
                 "following MultiIndex columns: {}".format(helper_str, column_levels)
             )
     return result
 
@@ -521,15 +518,15 @@
 
     Raises
     ------
     :exc:`~biopsykit.exceptions.ValidationError`
         if ``raise_exception`` is ``True`` and ``data`` does not have the required length
 
     """
-    if len(set(len(df) for df in df_list)) != 1:
+    if len({len(df) for df in df_list}) != 1:
         if raise_exception:
             raise ValidationError("Not all dataframes have the same length!")
         return False
     return True
 
 
 def _multiindex_level_names_helper_get_expected_levels(
@@ -540,19 +537,18 @@
 ) -> bool:
     if match_order:
         if match_atleast:
             ac_levels_slice = ac_levels[: len(ex_levels)]
             expected = ex_levels == ac_levels_slice
         else:
             expected = ex_levels == ac_levels
+    elif match_atleast:
+        expected = all(level in ac_levels for level in ex_levels)
     else:
-        if match_atleast:
-            expected = all(level in ac_levels for level in ex_levels)
-        else:
-            expected = sorted(ex_levels) == sorted(ac_levels)
+        expected = sorted(ex_levels) == sorted(ac_levels)
 
     return expected
 
 
 def _multiindex_level_names_helper(
     df: pd.DataFrame,
     level_names: Iterable[_Hashable],
@@ -562,18 +558,15 @@
     raise_exception: Optional[bool] = True,
 ) -> Optional[bool]:
 
     if isinstance(level_names, str):
         level_names = [level_names]
 
     ex_levels = list(level_names)
-    if idx_or_col == "index":
-        ac_levels = list(df.index.names)
-    else:
-        ac_levels = list(df.columns.names)
+    ac_levels = list(df.index.names) if idx_or_col == "index" else list(df.columns.names)
 
     expected = _multiindex_level_names_helper_get_expected_levels(ac_levels, ex_levels, match_atleast, match_order)
 
     if not expected:
         if raise_exception:
             raise ValidationError(
                 "The dataframe is expected to have exactly the following {} level names {}, "
@@ -594,18 +587,15 @@
 
     has_multiindex, nlevels_act = _multiindex_check_helper_get_levels(df, idx_or_col)
 
     if has_multiindex is not expected:
         return _multiindex_check_helper_not_expected(idx_or_col, nlevels, nlevels_act, expected, raise_exception)
 
     if has_multiindex is True:
-        if nlevels_atleast:
-            expected = nlevels_act >= nlevels
-        else:
-            expected = nlevels_act == nlevels
+        expected = nlevels_act >= nlevels if nlevels_atleast else nlevels_act == nlevels
         if not expected:
             if raise_exception:
                 raise ValidationError(
                     "The dataframe is expected to have a MultiIndex with {0} {1} levels. "
                     "But it has a MultiIndex with {2} {1} levels.".format(nlevels, idx_or_col, nlevels_act)
                 )
             return False
@@ -677,16 +667,14 @@
 
 
 def _check_has_column_prefix_single_col(
     columns: Sequence[str], col: Any, prefix: str, raise_exception: bool
 ) -> Optional[bool]:
     if not _assert_is_dtype(col, str, raise_exception=False):
         if raise_exception:
-            raise ValidationError("Column '{}' from {} is not a string!".format(col, columns))
+            raise ValidationError(f"Column '{col}' from {columns} is not a string!")
         return False
     if not col.startswith(prefix):
         if raise_exception:
-            raise ValidationError(
-                "Column '{}' from {} are starting with the required prefix '{}'!".format(col, columns, prefix)
-            )
+            raise ValidationError(f"Column '{col}' from {columns} are starting with the required prefix '{prefix}'!")
         return False
     return True
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/_types.py` & `biopsykit-0.9.0/src/biopsykit/utils/_types.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/array_handling.py` & `biopsykit-0.9.0/src/biopsykit/utils/array_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """Module providing various functions for low-level handling of array data."""
 from typing import List, Optional, Tuple, Union
 
 import neurokit2 as nk
 import numpy as np
 import pandas as pd
-from scipy import interpolate, signal
-
 from biopsykit.utils._types import arr_t, str_t
+from scipy import interpolate, signal
 
 
 def sanitize_input_1d(data: arr_t) -> np.ndarray:
-    """Convert 1-d array-like data (:class:`~numpy.ndarray`, :class:`~pandas.DataFrame`/:class:`~pandas.Series`) \
-    to a numpy array.
+    """Convert 1-d array-like data (:class:`~pandas.DataFrame`/:class:`~pandas.Series`) to a numpy array.
 
     Parameters
     ----------
     data : array_like
         input data. Needs to be 1-d
 
 
@@ -34,16 +32,15 @@
     return data
 
 
 def sanitize_input_nd(
     data: arr_t,
     ncols: Optional[Union[int, Tuple[int, ...]]] = None,
 ) -> np.ndarray:
-    """Convert n-d array-like data (:class:`~numpy.ndarray`, :class:`~pandas.DataFrame`/:class:`~pandas.Series`) \
-    to a numpy array.
+    """Convert n-d array-like data (:class:`~pandas.DataFrame`/:class:`~pandas.Series`) to a numpy array.
 
     Parameters
     ----------
     data : array_like
         input data
     ncols : int or tuple of ints
         number of columns (2nd dimension) the ``data`` is expected to have, a list of such if ``data``
@@ -57,23 +54,23 @@
 
     """
     # ensure list
     if isinstance(ncols, int):
         ncols = [ncols]
 
     if isinstance(data, (pd.Series, pd.DataFrame)):
-        data = data.values
+        data = data.to_numpy()
 
     if ncols is not None:
         if data.ndim == 1:
             if 1 in ncols:
                 return data
-            raise ValueError("Invalid number of columns! Expected one of {}, got 1.".format(ncols))
+            raise ValueError(f"Invalid number of columns! Expected one of {ncols}, got 1.")
         if data.shape[1] not in ncols:
-            raise ValueError("Invalid number of columns! Expected one of {}, got {}.".format(ncols, data.shape[1]))
+            raise ValueError(f"Invalid number of columns! Expected one of {ncols}, got {data.shape[1]}.")
     return data
 
 
 def find_extrema_in_radius(
     data: arr_t,
     indices: arr_t,
     radius: Union[int, Tuple[int, int]],
@@ -118,15 +115,15 @@
     >>> # search maxima in 'data' in a 5 samples before each entry of 'indices'
     >>> find_extrema_in_radius(data, indices, radius, extrema_type='max')
 
     """
     extrema_funcs = {"min": np.nanargmin, "max": np.nanargmax}
 
     if extrema_type not in extrema_funcs:
-        raise ValueError("`extrema_type` must be one of {}, not {}".format(list(extrema_funcs.keys()), extrema_type))
+        raise ValueError(f"`extrema_type` must be one of {list(extrema_funcs.keys())}, not {extrema_type}")
     extrema_func = extrema_funcs[extrema_type]
 
     # ensure numpy
     data = sanitize_input_1d(data)
     indices = sanitize_input_1d(indices)
     indices = indices.astype(int)
     # possible start offset if beginning of array needs to be padded to ensure radius
@@ -148,22 +145,16 @@
         windows[i] = data[index - lower_limit + start_padding : index + upper_limit + start_padding + 1]
 
     return extrema_func(windows, axis=1) + indices - lower_limit
 
 
 def _find_extrema_in_radius_get_limits(radius: Union[int, Tuple[int, int]]) -> Tuple[int, int]:
     # determine upper and lower limit
-    if isinstance(radius, tuple):
-        lower_limit = radius[0]
-    else:
-        lower_limit = radius
-    if isinstance(radius, tuple):
-        upper_limit = radius[-1]
-    else:
-        upper_limit = radius
+    lower_limit = radius[0] if isinstance(radius, tuple) else radius
+    upper_limit = radius[-1] if isinstance(radius, tuple) else radius
 
     # round up and make sure it's an integer
     lower_limit = np.ceil(lower_limit).astype(int)
     upper_limit = np.ceil(upper_limit).astype(int)
     return lower_limit, upper_limit
 
 
@@ -215,15 +206,15 @@
     if x_old is None and desired_length:
         raise ValueError("'x_old' must also be passed when 'desired_length' is passed!")
     x_old = np.array(x_old)
 
     # remove outlier
     data[outlier_mask] = np.nan
     # fill outlier by linear interpolation of neighbors
-    data = pd.Series(data).interpolate(limit_direction="both").values
+    data = pd.Series(data).interpolate(limit_direction="both").to_numpy()
     # interpolate signal
     x_new = np.linspace(x_old[0], x_old[-1], desired_length)
     return nk.signal_interpolate(x_old, data, x_new, method="linear")
 
 
 def sliding_window(
     data: arr_t,
@@ -612,18 +603,15 @@
     :class:`~pandas.DataFrame`
         dataframe with datetime index
 
     """
     if isinstance(column_name, str):
         # assert list
         column_name = [column_name]
-    if column_name is not None:
-        arr = pd.DataFrame(arr, columns=column_name)
-    else:
-        arr = pd.DataFrame(arr)
+    arr = pd.DataFrame(arr, columns=column_name) if column_name is not None else pd.DataFrame(arr)
 
     start_time_s = float(start_time.to_datetime64()) / 1e9
     arr.index = pd.to_datetime(
         (arr.index * 1 / sampling_rate + start_time_s).astype(int), utc=True, unit="s"
     ).tz_convert(start_time.tzinfo)
 
     arr.index.name = "time"
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/data_processing.py` & `biopsykit-0.9.0/src/biopsykit/utils/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Module providing various functions for processing more complex structured data (e.g., collected during a study)."""
 import warnings
 from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from scipy import interpolate
-
 from biopsykit.utils._datatype_validation_helper import (
     _assert_dataframes_same_length,
     _assert_has_index_levels,
     _assert_has_multiindex,
     _assert_is_dtype,
 )
 from biopsykit.utils.array_handling import sanitize_input_1d
@@ -25,14 +23,15 @@
     is_merged_study_data_dict,
     is_study_data_dict,
     is_subject_condition_dataframe,
     is_subject_condition_dict,
     is_subject_data_dict,
 )
 from biopsykit.utils.functions import se
+from scipy import interpolate
 
 
 def _split_data_series(data: pd.DataFrame, time_intervals: pd.Series, include_start: bool) -> Dict[str, pd.DataFrame]:
     if time_intervals.index.nlevels > 1:
         # multi-index series => second level contains start/end times of phases
         time_intervals = time_intervals.unstack().T
         time_intervals = {key: tuple(value.values()) for key, value in time_intervals.to_dict().items()}
@@ -103,20 +102,19 @@
     if isinstance(time_intervals, pd.DataFrame):
         if len(time_intervals) > 1:
             raise ValueError("Only dataframes with 1 row allowed!")
         time_intervals = time_intervals.iloc[0]
 
     if isinstance(time_intervals, pd.Series):
         time_intervals = _split_data_series(data, time_intervals, include_start)
-    else:
-        if include_start:
-            time_intervals["Start"] = (
-                data.index[0].to_pydatetime().time(),
-                list(time_intervals.values())[0][0],
-            )
+    elif include_start:
+        time_intervals["Start"] = (
+            data.index[0].to_pydatetime().time(),
+            list(time_intervals.values())[0][0],
+        )
 
     data_dict = {name: data.between_time(*start_end) for name, start_end in time_intervals.items()}
     data_dict = {name: data for name, data in data_dict.items() if not data.empty}
     return data_dict
 
 
 def exclude_subjects(
@@ -157,17 +155,17 @@
         if index_name in data.index.names:
             level_values = data.index.get_level_values(index_name)
             if (level_values.dtype == object and all(isinstance(s, str) for s in excluded_subjects)) or (
                 level_values.dtype == int and all(isinstance(s, int) for s in excluded_subjects)
             ):
                 cleaned_data[key] = _exclude_single_subject(data, excluded_subjects, index_name, key)
             else:
-                raise ValueError("{}: dtypes of index and subject ids to be excluded do not match!".format(key))
+                raise ValueError(f"{key}: dtypes of index and subject ids to be excluded do not match!")
         else:
-            raise ValueError("No '{}' level in index!".format(index_name))
+            raise ValueError(f"No '{index_name}' level in index!")
     if len(cleaned_data) == 1:
         cleaned_data = list(cleaned_data.values())[0]
     return cleaned_data
 
 
 def _exclude_single_subject(
     data: pd.DataFrame, excluded_subjects: Union[Sequence[str], Sequence[int]], index_name: str, dataset_name: str
@@ -176,15 +174,15 @@
     try:
         if isinstance(data.index, pd.MultiIndex):
             # MultiIndex => specify index level
             return data.drop(index=excluded_subjects, level=index_name)
         # Regular Index
         return data.drop(index=excluded_subjects)
     except KeyError:
-        warnings.warn("Not all subjects of {} exist in '{}'!".format(excluded_subjects, dataset_name))
+        warnings.warn(f"Not all subjects of {excluded_subjects} exist in '{dataset_name}'!")
         return data
 
 
 def normalize_to_phase(subject_data_dict: SubjectDataDict, phase: Union[str, pd.DataFrame]) -> SubjectDataDict:
     """Normalize time series data per subject to the phase specified by ``normalize_to``.
 
     The result is the relative change (of, for example, heart rate) compared to the mean value in ``phase``.
@@ -204,18 +202,15 @@
     dict
         dictionary with normalized data per subject
 
     """
     _assert_is_dtype(phase, (str, pd.DataFrame))
     dict_subjects_norm = {}
     for subject_id, data in subject_data_dict.items():
-        if isinstance(phase, str):
-            bl_mean = data[phase].mean()
-        else:
-            bl_mean = phase.mean()
+        bl_mean = data[phase].mean() if isinstance(phase, str) else phase.mean()
         dict_subjects_norm[subject_id] = {p: (df - bl_mean) / bl_mean * 100 for p, df in data.items()}
 
     return dict_subjects_norm
 
 
 def resample_sec(data: Union[pd.DataFrame, pd.Series]) -> pd.DataFrame:
     """Resample input data to a frequency of 1 Hz.
@@ -241,18 +236,15 @@
     ------
     ValueError
         If ``data`` is not a DataFrame or Series
 
     """
     _assert_is_dtype(data, (pd.DataFrame, pd.Series))
 
-    if isinstance(data, pd.DataFrame):
-        column_name = data.columns
-    else:
-        column_name = [data.name]
+    column_name = data.columns if isinstance(data, pd.DataFrame) else [data.name]
 
     if isinstance(data.index, pd.DatetimeIndex):
         x_old = np.array((data.index - data.index[0]).total_seconds())
     else:
         x_old = np.array(data.index - data.index[0])
     x_new = np.arange(1, np.ceil(x_old[-1]) + 1)
     data = sanitize_input_1d(data)
@@ -291,15 +283,15 @@
     result_dict = {}
     for key, value in data_dict.items():
         if isinstance(value, (pd.DataFrame, pd.Series)):
             result_dict[key] = resample_sec(value)
         elif isinstance(value, dict):
             result_dict[key] = resample_dict_sec(value)
         else:
-            raise ValueError("Invalid input format!")
+            raise TypeError("Invalid input format!")
     return result_dict
 
 
 def select_dict_phases(subject_data_dict: SubjectDataDict, phases: Union[str, Sequence[str]]) -> SubjectDataDict:
     """Select specific phases from :obj:`~biopsykit.utils.datatype_helper.SubjectDataDict`.
 
     Parameters
@@ -322,18 +314,18 @@
         subject: {phase: dict_subject[phase] for phase in phases} for subject, dict_subject in subject_data_dict.items()
     }
 
 
 def rearrange_subject_data_dict(
     subject_data_dict: SubjectDataDict,
 ) -> StudyDataDict:
-    """Rearrange :obj:`~biopsykit.utils.datatype_helper.SubjectDataDict` to \
-    :obj:`~biopsykit.utils.datatype_helper.StudyDataDict`.
+    """Rearrange ``SubjectDataDict`` to ``StudyDataDict``.
 
-    A ``StudyDataDict`` is constructed from a ``SubjectDataDict`` by swapping outer (subject IDs) and inner
+    A :obj:`~biopsykit.utils.datatype_helper.StudyDataDict` is constructed from a
+    :obj:`~biopsykit.utils.datatype_helper.SubjectDataDict` by swapping outer (subject IDs) and inner
     (phase names) dictionary keys.
 
     The **input** needs to be a :obj:`~biopsykit.utils.datatype_helper.SubjectDataDict`,
     a nested dictionary in the following format:
 
     | {
     |   "subject1" : { "phase_1" : dataframe, "phase_2" : dataframe, ... },
@@ -496,16 +488,16 @@
             result_dict[key] = split_dict_into_subphases(value, subphases)
         else:
             subphase_times = get_subphase_durations(value, subphases)
             subphase_dict = {}
             for subphase, times in zip(subphases.keys(), subphase_times):
                 if isinstance(value.index, pd.DatetimeIndex):
                     # slice the current subphase by dropping the preceding subphases
-                    value_cpy = value.drop(value.first("{}s".format(times[0])).index)
-                    value_cpy = value_cpy.first("{}s".format(times[1] - times[0]))
+                    value_cpy = value.drop(value.first(f"{times[0]}s").index)
+                    value_cpy = value_cpy.first(f"{times[1] - times[0]}s")
                     subphase_dict[subphase] = value_cpy
                 else:
                     subphase_dict[subphase] = value.iloc[times[0] : times[1]]
             result_dict[key] = subphase_dict
     return result_dict
 
 
@@ -556,15 +548,15 @@
     if subphase_durations.ndim == 1:
         # 1d array => subphase values are integer => they are consecutive and each entry is the duration
         # of the subphase, so the start and end times of each subphase must be computed
         times_cum = np.cumsum(subphase_durations)
         if subphase_durations[-1] == 0:
             # last subphase has duration 0 => end of last subphase is length of dataframe
             times_cum[-1] = len(data)
-        subphase_times = list(zip([0] + list(times_cum), times_cum))
+        subphase_times = list(zip([0, *list(times_cum)], times_cum))
     else:
         # 2d array => subphase values are tuples => start end end time of each subphase are already provided and do
         # not need to be computed
         subphase_times = subphase_durations
     return subphase_times
 
 
@@ -670,27 +662,24 @@
     one_col_df = False
     for key, value in data.items():
         _assert_is_dtype(value, (dict, pd.DataFrame))
         if isinstance(value, dict):
             if len(dict_levels) <= 1:
                 raise ValueError("Invalid number of 'dict_levels' specified!")
             # nested dictionary
-            if isinstance(key, (str, int)):
-                key_len = 1
-            else:
-                key_len = len(key)
+            key_len = 1 if isinstance(key, (str, int)) else len(key)
             result_data[key] = mean_per_subject_dict(value, dict_levels[key_len:], param_name)
         else:
             value.columns.name = "subject"
             if len(value.columns) == 1:
                 one_col_df = True
             df = pd.DataFrame(value.mean(axis=0), columns=[param_name])
             result_data[key] = df
 
-    key_lengths = list(set(1 if isinstance(k, (str, int)) else len(k) for k in result_data))
+    key_lengths = list({1 if isinstance(k, (str, int)) else len(k) for k in result_data})
     if len(key_lengths) != 1:
         raise ValueError("Inconsistent dictionary key lengths!")
     key_lengths = key_lengths[0]
     names = dict_levels[0:key_lengths]
     if isinstance(names, str):
         names = [names]
     ret = pd.concat(result_data, names=names)
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/dataframe_handling.py` & `biopsykit-0.9.0/src/biopsykit/utils/dataframe_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module providing various functions for advanced handling of pandas dataframes."""
 import re
 from typing import Callable, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import _assert_has_columns, _assert_has_index_levels, _assert_is_dtype
 from biopsykit.utils.datatype_helper import CodebookDataFrame, is_codebook_dataframe
 
 __all__ = [
     "apply_codebook",
     "add_space_to_camel",
     "camel_to_snake",
@@ -213,17 +212,17 @@
         dataframe with replaced missing values or ``None`` if ``inplace`` is ``True``
 
     """
     _assert_is_dtype(data, pd.DataFrame)
     if not inplace:
         data = data.copy()
 
-    data[target_col].fillna(data[source_col], inplace=True)
+    data[target_col].fillna(data[source_col], inplace=True)  # noqa: PD002
     if dropna:
-        data.dropna(subset=[target_col], inplace=True)
+        data = data.dropna(subset=[target_col])
 
     if inplace:
         return None
     return data
 
 
 def convert_nan(
@@ -250,15 +249,15 @@
         dataframe with converted missing values or ``None`` if ``inplace`` is ``True``
 
     """
     _assert_is_dtype(data, (pd.DataFrame, pd.Series))
 
     if not inplace:
         data = data.copy()
-    data.replace([-99.0, -77.0, -66.0, "-99", "-77", "-66"], np.nan, inplace=True)
+    data = data.replace([-99.0, -77.0, -66.0, "-99", "-77", "-66"], np.nan)
     if inplace:
         return None
     return data
 
 
 def multi_xs(
     data: Union[pd.DataFrame, pd.Series],
@@ -384,19 +383,19 @@
     >>> apply_codebook(codebook, data)
 
     """
     is_codebook_dataframe(codebook)
 
     for col in data.index.names:
         if col in codebook.index:
-            data.rename(index=codebook.loc[col], level=col, inplace=True)
+            data = data.rename(index=codebook.loc[col], level=col)
 
     for col in data.columns:
         if col in codebook.index:
-            data.loc[:, col].replace(codebook.loc[col], inplace=True)
+            data.loc[:, col].replace(codebook.loc[col], inplace=True)  # noqa: PD002
 
     return data
 
 
 def wide_to_long(
     data: pd.DataFrame,
     stubname: str,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/datatype_helper.py` & `biopsykit-0.9.0/src/biopsykit/utils/datatype_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """A couple of helper functions that ease the use of the typical biopsykit data formats."""
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
-
 from biopsykit.utils._datatype_validation_helper import (
     _assert_has_column_multiindex,
     _assert_has_column_prefix,
     _assert_has_columns,
     _assert_has_columns_any_level,
     _assert_has_index_levels,
     _assert_has_multiindex,
@@ -992,15 +991,15 @@
         if saliva_type is None:
             raise ValidationError("`saliva_type` is None!")
         if isinstance(saliva_type, str):
             saliva_type = [saliva_type]
         _assert_is_dtype(data, pd.DataFrame)
         _assert_has_multiindex(data, nlevels=2, nlevels_atleast=True)
         _assert_has_index_levels(data, index_levels=["subject", "sample"], match_atleast=True, match_order=False)
-        _assert_has_columns(data, [saliva_type, saliva_type + ["time"]])
+        _assert_has_columns(data, [saliva_type, [*saliva_type, "time"]])
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be a SalivaRawDataFrame. "
                 "The validation failed with the following error:\n\n{}".format(str(e))
             ) from e
         return False
@@ -1161,15 +1160,15 @@
         dictionary format
 
     """
     try:
         _assert_is_dtype(data, dict)
         expected_keys = ["date", "sleep_onset", "wake_onset", "total_sleep_duration"]
         if any(col not in list(data.keys()) for col in expected_keys):
-            raise ValidationError("Not all of {} are in the dictionary!".format(expected_keys))
+            raise ValidationError(f"Not all of {expected_keys} are in the dictionary!")
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be a SleepEndpointDict. "
                 "The validation failed with the following error:\n\n{}".format(str(e))
             ) from e
         return False
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/exceptions.py` & `biopsykit-0.9.0/src/biopsykit/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/file_handling.py` & `biopsykit-0.9.0/src/biopsykit/utils/file_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Helper functions for file handling."""
 import re
 from pathlib import Path
 from typing import Optional, Sequence, Union
 
 import matplotlib.pyplot as plt
-
 from biopsykit.utils._datatype_validation_helper import _assert_file_extension
 from biopsykit.utils._types import path_t
 
 
 def mkdirs(dir_list: Union[path_t, Sequence[path_t]]) -> None:
     """Batch-create a list of directories.
 
@@ -29,16 +28,16 @@
     >>> mkdirs(path_list)
 
     """
     if isinstance(dir_list, (str, Path)):
         dir_list = [dir_list]
     for directory in dir_list:
         # ensure pathlib
-        directory = Path(directory)
-        directory.mkdir(exist_ok=True, parents=True)
+        directory_path = Path(directory)
+        directory_path.mkdir(exist_ok=True, parents=True)
 
 
 def get_subject_dirs(base_path: path_t, pattern: str) -> Optional[Sequence[Path]]:
     """Filter for subject directories using a name pattern.
 
     Parameters
     ----------
@@ -65,15 +64,15 @@
 
     """
     # ensure pathlib
     base_path = Path(base_path)
     subject_dirs = [p for p in sorted(base_path.glob("*")) if p.is_dir()]
     subject_dirs = list(filter(lambda s: len(re.findall(pattern, s.name)) > 0, subject_dirs))
     if len(subject_dirs) == 0:
-        raise FileNotFoundError("No subfolders matching the pattern '{}' found in {}.".format(pattern, base_path))
+        raise FileNotFoundError(f"No subfolders matching the pattern '{pattern}' found in {base_path}.")
     return subject_dirs
 
 
 def export_figure(
     fig: plt.Figure,
     filename: path_t,
     base_dir: path_t,
```

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/functions.py` & `biopsykit-0.9.0/src/biopsykit/utils/functions.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/legacy_helper.py` & `biopsykit-0.9.0/src/biopsykit/utils/legacy_helper.py`

 * *Files identical despite different names*

### Comparing `biopsykit-0.8.1/src/biopsykit/utils/time.py` & `biopsykit-0.9.0/src/biopsykit/utils/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import re
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 import pytz
-
 from biopsykit.utils._datatype_validation_helper import _assert_is_dtype
 from biopsykit.utils._types import path_t
 
 tz = pytz.timezone("Europe/Berlin")
 utc = pytz.timezone("UTC")
 
 __all__ = [
```

### Comparing `biopsykit-0.8.1/PKG-INFO` & `biopsykit-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biopsykit
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Python package for the analysis of biopsychological data.
 Home-page: https://github.com/mad-lab-fau/biopsykit
 License: MIT
 Author: Robert Richer
 Author-email: robert.richer@fau.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

