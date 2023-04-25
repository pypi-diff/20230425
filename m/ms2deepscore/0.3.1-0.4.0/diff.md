# Comparing `tmp/ms2deepscore-0.3.1.tar.gz` & `tmp/ms2deepscore-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2deepscore-0.3.1.tar", last modified: Fri Jan  6 14:45:58 2023, max compression
+gzip compressed data, was "ms2deepscore-0.4.0.tar", last modified: Tue Apr 25 07:32:22 2023, max compression
```

## Comparing `ms2deepscore-0.3.1.tar` & `ms2deepscore-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:45:58.230818 ms2deepscore-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-01-06 14:45:58.230818 ms2deepscore-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:45:58.226818 ms2deepscore-0.3.1/ms2deepscore/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/BinnedSpectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/MS2DeepScore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/MS2DeepScoreMonteCarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/SpectrumBinner.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/data_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:45:58.226818 ms2deepscore-0.3.1/ms2deepscore/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/models/SiameseModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/models/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/spectrum_binning_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/spectrum_binning_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-01-06 14:45:47.000000 ms2deepscore-0.3.1/ms2deepscore/vector_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:45:58.226818 ms2deepscore-0.3.1/ms2deepscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-01-06 14:45:58.000000 ms2deepscore-0.3.1/ms2deepscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-06 14:45:58.000000 ms2deepscore-0.3.1/ms2deepscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:45:58.000000 ms2deepscore-0.3.1/ms2deepscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:45:58.000000 ms2deepscore-0.3.1/ms2deepscore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-06 14:45:58.000000 ms2deepscore-0.3.1/ms2deepscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-06 14:45:58.000000 ms2deepscore-0.3.1/ms2deepscore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 14:45:58.230818 ms2deepscore-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:45:58.230818 ms2deepscore-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_BinnedSpectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_SpectrumBinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_data_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_models_duplicate_inchikeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_ms2deepscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_ms2deepscoremontecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_spectrum_binning_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_spectrum_binning_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_user_worfklow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-01-06 14:45:48.000000 ms2deepscore-0.3.1/tests/test_vector_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:32:22.357773 ms2deepscore-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-04-25 07:32:22.357773 ms2deepscore-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:32:22.349773 ms2deepscore-0.4.0/ms2deepscore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/BinnedSpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/MS2DeepScore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/MS2DeepScoreMonteCarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/SpectrumBinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27959 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/data_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:32:22.353773 ms2deepscore-0.4.0/ms2deepscore/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/models/SiameseModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/models/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/spectrum_binning_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/spectrum_binning_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/ms2deepscore/vector_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:32:22.353773 ms2deepscore-0.4.0/ms2deepscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-04-25 07:32:22.000000 ms2deepscore-0.4.0/ms2deepscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 07:32:22.000000 ms2deepscore-0.4.0/ms2deepscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:32:22.000000 ms2deepscore-0.4.0/ms2deepscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:32:22.000000 ms2deepscore-0.4.0/ms2deepscore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-25 07:32:22.000000 ms2deepscore-0.4.0/ms2deepscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 07:32:22.000000 ms2deepscore-0.4.0/ms2deepscore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:32:22.357773 ms2deepscore-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:32:22.357773 ms2deepscore-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_BinnedSpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_SpectrumBinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_data_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_models_duplicate_inchikeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_ms2deepscoremontecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_spectrum_binning_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_spectrum_binning_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_train_ms2deepscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_user_worfklow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-25 07:32:11.000000 ms2deepscore-0.4.0/tests/test_vector_operations.py
```

### Comparing `ms2deepscore-0.3.1/LICENSE` & `ms2deepscore-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/PKG-INFO` & `ms2deepscore-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ms2deepscore
-Version: 0.3.1
+Version: 0.4.0
 Summary: Deep learning similarity measure for comparing MS/MS spectra.
 Home-page: https://github.com/iomega/ms2deepscore
 Author: Netherlands eScience Center
 Author-email: f.huber@esciencecenter.nl
 License: Apache Software License 2.0
 Description: ![GitHub](https://img.shields.io/github/license/matchms/ms2deepscore)
-        [![PyPI](https://img.shields.io/pypi/v/ms2deepscore)](https://pypi.org/project/ms2deepscore/)
+        [![PyPI](https://img.shields.io/pypi/v/ms2deepscore?color=teal)](https://pypi.org/project/ms2deepscore/)
         ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/matchms/ms2deepscore/CI_build.yml?branch=main)
         [![SonarCloud Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=matchms_ms2deepscore&metric=alert_status)](https://sonarcloud.io/dashboard?id=matchms_ms2deepscore)
         [![SonarCloud Coverage](https://sonarcloud.io/api/project_badges/measure?project=matchms_ms2deepscore&metric=coverage)](https://sonarcloud.io/component_measures?id=matchms_ms2deepscore&metric=Coverage&view=list)  
         [![DOI](https://zenodo.org/badge/310047938.svg)](https://zenodo.org/badge/latestdoi/310047938)
         [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
         
         # ms2deepscore
@@ -30,34 +30,41 @@
         **"MS2DeepScore - a novel deep learning similarity measure to compare tandem mass spectra"**
         Florian Huber, Sven van der Burg, Justin J.J. van der Hooft, Lars Ridder, 13, Article number: 84 (2021), Journal of Cheminformatics, doi: https://doi.org/10.1186/s13321-021-00558-4
         
         
         ## Setup
         ### Requirements
         
-        Python 3.7 or higher.  
-        Tested with Tensorflow 2.4, 2.5, 2.8, and latest version.
+        Python 3.8, 3.9, 3.10 (higher will likely work but is not tested systematically).  
+        Tested with Tensorflow 2.4, 2.6, 2.8, and latest version.
         
         ### Installation
         Simply install using pip: `pip install ms2deepscore`
         
         ### Prepare environment
         We recommend to create an Anaconda environment with
         
         ```
-        conda create --name ms2deepscore python=3.8
+        conda create --name ms2deepscore python=3.9
         conda activate ms2deepscore
         pip install ms2deepscore
         ```
         Alternatively, simply install in the environment of your choice by .
         
         
-        Or, to also include the full [matchms](https://github.com/matchms/matchms) functionality:
+        Or, to also include the full [matchms](https://github.com/matchms/matchms) functionality, including rdkit:
         ```
-        conda create --name ms2deepscore python=3.8
+        conda create --name ms2deepscore python=3.9
+        conda activate ms2deepscore
+        pip install ms2deepscore[chemistry]
+        ```
+        
+        Or, via conda:
+        ```
+        conda create --name ms2deepscore python=3.9
         conda activate ms2deepscore
         conda install --channel bioconda --channel conda-forge matchms
         pip install ms2deepscore
         ```
         
         ### Installation on macos with M1 chip
         Users on MacOS with the M1 chip should intall tensorflow manually: `pip install tensorflow=macos`.
@@ -119,10 +126,11 @@
         ## 2) Train an own MS2DeepScore model
         A notebook with a tutorial on how to train a MS2Deepscore model on your own data can be found here: [MS2DeepScore tutorial](https://github.com/matchms/ms2deepscore/blob/main/notebooks/MS2DeepScore_tutorial.ipynb)
         
         ## Contributing
         We welcome contributions to the development of ms2deepscore! Have a look at the [contribution guidelines](https://github.com/matchms/ms2deepscore/blob/main/CONTRIBUTING.md).
         
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: train
 Provides-Extra: dev
```

### Comparing `ms2deepscore-0.3.1/README.md` & `ms2deepscore-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![GitHub](https://img.shields.io/github/license/matchms/ms2deepscore)
-[![PyPI](https://img.shields.io/pypi/v/ms2deepscore)](https://pypi.org/project/ms2deepscore/)
+[![PyPI](https://img.shields.io/pypi/v/ms2deepscore?color=teal)](https://pypi.org/project/ms2deepscore/)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/matchms/ms2deepscore/CI_build.yml?branch=main)
 [![SonarCloud Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=matchms_ms2deepscore&metric=alert_status)](https://sonarcloud.io/dashboard?id=matchms_ms2deepscore)
 [![SonarCloud Coverage](https://sonarcloud.io/api/project_badges/measure?project=matchms_ms2deepscore&metric=coverage)](https://sonarcloud.io/component_measures?id=matchms_ms2deepscore&metric=Coverage&view=list)  
 [![DOI](https://zenodo.org/badge/310047938.svg)](https://zenodo.org/badge/latestdoi/310047938)
 [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
 
 # ms2deepscore
@@ -22,34 +22,41 @@
 **"MS2DeepScore - a novel deep learning similarity measure to compare tandem mass spectra"**
 Florian Huber, Sven van der Burg, Justin J.J. van der Hooft, Lars Ridder, 13, Article number: 84 (2021), Journal of Cheminformatics, doi: https://doi.org/10.1186/s13321-021-00558-4
 
 
 ## Setup
 ### Requirements
 
-Python 3.7 or higher.  
-Tested with Tensorflow 2.4, 2.5, 2.8, and latest version.
+Python 3.8, 3.9, 3.10 (higher will likely work but is not tested systematically).  
+Tested with Tensorflow 2.4, 2.6, 2.8, and latest version.
 
 ### Installation
 Simply install using pip: `pip install ms2deepscore`
 
 ### Prepare environment
 We recommend to create an Anaconda environment with
 
 ```
-conda create --name ms2deepscore python=3.8
+conda create --name ms2deepscore python=3.9
 conda activate ms2deepscore
 pip install ms2deepscore
 ```
 Alternatively, simply install in the environment of your choice by .
 
 
-Or, to also include the full [matchms](https://github.com/matchms/matchms) functionality:
+Or, to also include the full [matchms](https://github.com/matchms/matchms) functionality, including rdkit:
 ```
-conda create --name ms2deepscore python=3.8
+conda create --name ms2deepscore python=3.9
+conda activate ms2deepscore
+pip install ms2deepscore[chemistry]
+```
+
+Or, via conda:
+```
+conda create --name ms2deepscore python=3.9
 conda activate ms2deepscore
 conda install --channel bioconda --channel conda-forge matchms
 pip install ms2deepscore
 ```
 
 ### Installation on macos with M1 chip
 Users on MacOS with the M1 chip should intall tensorflow manually: `pip install tensorflow=macos`.
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore/BinnedSpectrum.py` & `ms2deepscore-0.4.0/ms2deepscore/BinnedSpectrum.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/ms2deepscore/MS2DeepScore.py` & `ms2deepscore-0.4.0/ms2deepscore/MS2DeepScore.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,40 +36,40 @@
         similarity_measure = MS2DeepScore(model)
         # Calculate scores and get matchms.Scores object
         scores = calculate_scores(references, queries, similarity_measure)
 
 
     """
 
-    def __init__(self, model, multi_inputs: bool = False, progress_bar: bool = True):
+    def __init__(self, model, progress_bar: bool = True):
         """
 
         Parameters
         ----------
         model:
             Expected input is a SiameseModel that has been trained on
             the desired set of spectra. The model contains the keras deep neural
             network (model.model) as well as the used spectrum binner (model.spectrum_binner).
         progress_bar:
             Set to True to monitor the embedding creating with a progress bar.
             Default is False.
         """
         self.model = model
-        self.multi_inputs = multi_inputs
+        self.multi_inputs = (model.additional_input > 0)
         # TODO: later maybe also check against SpectrumBinner
-        if (self.multi_inputs):
+        if self.multi_inputs:
             self.input_vector_dim = [self.model.base.input_shape[0][1], self.model.base.input_shape[1][1]]
         else:
             self.input_vector_dim = self.model.base.input_shape[1]
         self.output_vector_dim = self.model.base.output_shape[1]
         self.progress_bar = progress_bar
 
     def _create_input_vector(self, binned_spectrum: BinnedSpectrumType):
         """Creates input vector for model.base based on binned peaks and intensities"""
-        if (self.multi_inputs):
+        if self.multi_inputs:
             X = [np.zeros((1, i[1])) for i in self.model.base.input_shape]
             idx = np.array([int(x) for x in binned_spectrum.binned_peaks.keys()])
             values = np.array(list(binned_spectrum.binned_peaks.values()))
 
             X[0][0, idx] = values
             X[1] = np.array([[float(value) for key, value in binned_spectrum.metadata.items() if (key != "inchikey")]])
         else:
@@ -149,9 +149,9 @@
             (n_rows, self.output_vector_dim), dtype="float")
         binned_spectrums = self.model.spectrum_binner.transform(spectrum_list, progress_bar=self.progress_bar)
         for index_reference, reference in enumerate(
                 tqdm(binned_spectrums,
                      desc='Calculating vectors of reference spectrums',
                      disable=(not self.progress_bar))):
             reference_vectors[index_reference, 0:self.output_vector_dim] = \
-                self.model.base.predict(self._create_input_vector(reference))
+                self.model.base.predict(self._create_input_vector(reference), verbose=0)
         return reference_vectors
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore/MS2DeepScoreMonteCarlo.py` & `ms2deepscore-0.4.0/ms2deepscore/MS2DeepScoreMonteCarlo.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,19 +67,23 @@
             in which case the uncertainty will be evaluate by the interquantile range (IQR).
             When using "mean" the standard deviation is taken as uncertainty measure.
         progress_bar:
             Set to True to monitor the embedding creating with a progress bar.
             Default is False.
         """
         self.model = model
+        self.multi_inputs = (model.additional_input > 0)
         self.n_ensembles = n_ensembles
         assert average_type in ["median", "mean"], \
             "Non supported input for average_type. Must be 'median' or 'mean'."
         self.average_type = average_type
-        self.input_vector_dim = self.model.base.input_shape[1]  # TODO: later maybe also check against SpectrumBinner
+        if self.multi_inputs:
+            self.input_vector_dim = [self.model.base.input_shape[0][1], self.model.base.input_shape[1][1]]
+        else:
+            self.input_vector_dim = self.model.base.input_shape[1]
         self.output_vector_dim = self.model.base.output_shape[1]
         self.progress_bar = progress_bar
         self.partial_model = self._create_monte_carlo_base()
 
     def _create_input_vector(self, binned_spectrum: BinnedSpectrumType):
         """Creates input vector for model.base based on binned peaks and intensities"""
         X = np.zeros((1, self.input_vector_dim))
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore/SpectrumBinner.py` & `ms2deepscore-0.4.0/ms2deepscore/SpectrumBinner.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/ms2deepscore/data_generators.py` & `ms2deepscore-0.4.0/ms2deepscore/data_generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,63 +65,36 @@
             Max number of 'new' noise peaks to add to the spectrum, between 0 to `augment_noise_max`
             of peaks are added.
         augment_noise_intensity
             Intensity of the 'new' noise peaks to add to the spectrum
         use_fixed_set
             Toggles using a fixed dataset, if set to True the same dataset will be generated each
             epoch. Default is False.
+        random_seed
+            Specify random seed for reproducible random number generation.
         """
+        self.reference_scores_df = _clean_reference_scores_df(reference_scores_df)
 
-        self._validate_labels(reference_scores_df)
+        self.binned_spectrums = binned_spectrums
+        # Collect all inchikeys
+        self.spectrum_inchikeys = np.array([s.get("inchikey")[:14] for s in self.binned_spectrums])
+        self._validate_indexes()
 
         # Set all other settings to input (or otherwise to defaults):
         self._set_generator_parameters(**settings)
-        self.binned_spectrums = binned_spectrums
-        self.reference_scores_df = self._exclude_nans_from_labels(reference_scores_df)
-        self.reference_scores_df = self._transform_to_inchikey14(self.reference_scores_df)
-        self._collect_and_validate_inchikeys()
+
         self.dim = dim
         self.fixed_set = {}
 
-    def _collect_and_validate_inchikeys(self):
-        """Collect all inchikeys14 (first 14 characters) of all binned_spectrums
-        and check if all are present in the reference scores as well.
-        Check for duplicate inchikeys.
+    def _validate_indexes(self):
+        """Checks if all inchikeys of the BinnedSpectrum are in the reference_scores_df index.
         """
-        self.spectrum_inchikeys = np.array([s.get("inchikey")[:14] for s in self.binned_spectrums])
         for inchikey in np.unique(self.spectrum_inchikeys):
             assert inchikey in self.reference_scores_df.index, \
-                "InChIKey in given spectrum not found in reference scores"
-        inchikeys = self.reference_scores_df.index
-        if len(set(inchikeys)) != len(inchikeys):
-            msg = f"Duplicate InChIKeys-14 detected in reference_scores_df: {list(inchikeys[inchikeys.duplicated()])}"
-            raise ValueError(msg)
-
-    @staticmethod
-    def _validate_labels(reference_scores_df: pd.DataFrame):
-        if set(reference_scores_df.index) != set(reference_scores_df.columns):
-            raise ValueError("index and columns of reference_scores_df are not identical")
-
-    @staticmethod
-    def _transform_to_inchikey14(reference_scores_df: pd.DataFrame):
-        """Transform index and column names from potential full InChIKeys to InChIKey14"""
-        reference_scores_df.index = [x[:14] for x in reference_scores_df.index]
-        reference_scores_df.columns = [x[:14] for x in reference_scores_df.columns]
-        return reference_scores_df
-
-    @staticmethod
-    def _exclude_nans_from_labels(reference_scores_df: pd.DataFrame):
-        """Exclude nans in reference_scores_df, exclude columns and rows if there is any NaN
-        value"""
-        clean_df = reference_scores_df.dropna(axis='rows')  # drop rows with any NaN
-        clean_df = clean_df[clean_df.index]  # drop corresponding columns
-        n_dropped = len(reference_scores_df) - len(clean_df)
-        if n_dropped > 0:
-            print(f"{n_dropped} nans among {len(reference_scores_df)} labels will be excluded.")
-        return clean_df
+                f"InChIKey {inchikey} in given spectrum not found in reference scores"
 
     def _set_generator_parameters(self, **settings):
         """Set parameter for data generator. Use below listed defaults unless other
         input is provided.
 
         Parameters
         ----------
@@ -153,44 +126,48 @@
             Max number of 'new' noise peaks to add to the spectrum, between 0 to `augment_noise_max`
             of peaks are added.
         augment_noise_intensity
             Intensity of the 'new' noise peaks to add to the spectrum
         use_fixed_set
             Toggles using a fixed dataset, if set to True the same dataset will be generated each
             epoch. Default is False.
+        random_seed
+            Specify random seed for reproducible random number generation.
         additional_inputs
             Array of additional values to be used in training for e.g. ["precursor_mz", "parent_mass"]
         """
-        defaults = dict(
-            batch_size=32,
-            num_turns=1,
-            ignore_equal_pairs=True,
-            shuffle=True,
-            same_prob_bins=[(0, 0.5), (0.5, 1)],
-            augment_removal_max=0.3,
-            augment_removal_intensity=0.2,
-            augment_intensity=0.4,
-            augment_noise_max=10,
-            augment_noise_intensity=0.01,
-            use_fixed_set=False,
-            additional_input=[]
-        )
+        defaults = {
+            "batch_size": 32,
+            "num_turns": 1,
+            "ignore_equal_pairs": True,
+            "shuffle": True,
+            "same_prob_bins": [(0, 0.5), (0.5, 1)],
+            "augment_removal_max": 0.3,
+            "augment_removal_intensity": 0.2,
+            "augment_intensity": 0.4,
+            "augment_noise_max": 10,
+            "augment_noise_intensity": 0.01,
+            "use_fixed_set": False,
+            "random_seed": None,
+            "additional_input": []
+        }
 
         # Set default parameters or replace by **settings input
         for key, value in defaults.items():
             if key in settings:
                 print(f"The value for {key} is set from {value} (default) to {settings[key]}")
             else:
                 settings[key] = defaults[key]
         assert 0.0 <= settings["augment_removal_max"] <= 1.0, "Expected value within [0,1]"
         assert 0.0 <= settings["augment_removal_intensity"] <= 1.0, "Expected value within [0,1]"
         if settings["use_fixed_set"] and settings["shuffle"]:
             warnings.warn('When using a fixed set, data will not be shuffled')
-        if settings["use_fixed_set"]:
-            np.random.seed(42)
+        if settings["random_seed"] is not None:
+            assert isinstance(settings["random_seed"], int), "Random seed must be integer number."
+            np.random.seed(settings["random_seed"])
         self.settings = settings
 
     def _find_match_in_range(self, inchikey1, target_score_range):
         """Randomly pick ID for a pair with inchikey_id1 that has a score in
         target_score_range. When no such score exists, iteratively widen the range
         in steps of 0.1.
 
@@ -221,19 +198,20 @@
         """Generate one batch of data.
 
         If use_fixed_set=True we try retrieving the batch from self.fixed_set (or store it if
         this is the first epoch). This ensures a fixed set of data is generated each epoch.
         """
         if self.settings['use_fixed_set'] and batch_index in self.fixed_set:
             return self.fixed_set[batch_index]
-        if self.settings['use_fixed_set'] and batch_index == 0:
-            np.random.seed(42)
+        if self.settings["random_seed"] is not None and batch_index == 0:
+            np.random.seed(self.settings["random_seed"])
         spectrum_pairs = self._spectrum_pair_generator(batch_index)
         X, y = self.__data_generation(spectrum_pairs)
         if self.settings['use_fixed_set']:
+            # Store batches for later epochs
             self.fixed_set[batch_index] = (X, y)
         return X, y
 
     def _data_augmentation(self, spectrum_binned):
         """Data augmentation.
         Parameters
         ----------
@@ -277,14 +255,15 @@
 
     def _get_spectrum_with_inchikey(self, inchikey: str) -> BinnedSpectrumType:
         """
         Get a random spectrum matching the `inchikey` argument. NB: A compound (identified by an
         inchikey) can have multiple measured spectrums in a binned spectrum dataset.
         """
         matching_spectrum_id = np.where(self.spectrum_inchikeys == inchikey)[0]
+        assert len(matching_spectrum_id) > 0, "No matching inchikey found (note: expected first 14 characters)"
         return self.binned_spectrums[np.random.choice(matching_spectrum_id)]
 
     def __data_generation(self, spectrum_pairs: Iterator[SpectrumPair]):
         """Generates data containing batch_size samples"""
         container_list = []
         for pair in spectrum_pairs:
             container_list.append(Container(pair,
@@ -407,25 +386,14 @@
     def on_epoch_end(self):
         """Updates indexes after each epoch"""
         self.indexes = np.tile(np.arange(len(self.binned_spectrums)), int(self.settings["num_turns"]))
         if self.settings["shuffle"]:
 
             np.random.shuffle(self.indexes)
 
-    @staticmethod
-    def _exclude_nans_from_labels(reference_scores_df: pd.DataFrame):
-        """Exclude nans in reference_scores_df, exclude columns and rows if there is any NaN
-        value"""
-        clean_df = reference_scores_df.dropna(axis='rows')  # drop rows with any NaN
-        clean_df = clean_df[clean_df.index]  # drop corresponding columns
-        n_dropped = len(reference_scores_df) - len(clean_df)
-        if n_dropped > 0:
-            print(f"{n_dropped} nans among {len(reference_scores_df)} labels will be excluded.")
-        return clean_df
-
     def _exclude_not_selected_inchikeys(self, reference_scores_df: pd.DataFrame) -> pd.DataFrame:
         """Exclude rows and columns of reference_scores_df for all InChIKeys which are not
         present in the binned_spectrums."""
         inchikeys_in_selection = {s.get("inchikey")[:14] for s in self.binned_spectrums}
         clean_df = reference_scores_df.loc[reference_scores_df.index.isin(inchikeys_in_selection),
                                            reference_scores_df.columns.isin(inchikeys_in_selection)]
         n_dropped = len(self.reference_scores_df) - len(clean_df)
@@ -552,7 +520,45 @@
         self.additional_inputs_left = []
         self.additional_inputs_right = []
         for additional_input in additional_inputs:
             self.additional_inputs_left.append([float(self.spectrum_left.get(additional_input))])
             self.additional_inputs_right.append([float(self.spectrum_right.get(additional_input))])
 
         self.tanimoto_score = tanimoto_score
+
+
+def _clean_reference_scores_df(reference_scores_df):
+    _validate_labels(reference_scores_df)
+    reference_scores_df = _exclude_nans_from_labels(reference_scores_df)
+    reference_scores_df = _transform_to_inchikey14(reference_scores_df)
+    _check_duplicated_indexes(reference_scores_df)
+    return reference_scores_df
+
+
+def _validate_labels(reference_scores_df: pd.DataFrame):
+    if set(reference_scores_df.index) != set(reference_scores_df.columns):
+        raise ValueError("index and columns of reference_scores_df are not identical")
+
+
+def _transform_to_inchikey14(reference_scores_df: pd.DataFrame):
+    """Transform index and column names from potential full InChIKeys to InChIKey14"""
+    reference_scores_df.index = [x[:14] for x in reference_scores_df.index]
+    reference_scores_df.columns = [x[:14] for x in reference_scores_df.columns]
+    return reference_scores_df
+
+
+def _exclude_nans_from_labels(reference_scores_df: pd.DataFrame):
+    """Exclude nans in reference_scores_df, exclude columns and rows if there is any NaN
+    value"""
+    clean_df = reference_scores_df.dropna(axis='rows')  # drop rows with any NaN
+    clean_df = clean_df[clean_df.index]  # drop corresponding columns
+    n_dropped = len(reference_scores_df) - len(clean_df)
+    if n_dropped > 0:
+        print(f"{n_dropped} nans among {len(reference_scores_df)} labels will be excluded.")
+    return clean_df
+
+
+def _check_duplicated_indexes(reference_scores_df):
+    inchikeys = reference_scores_df.index
+    if len(set(inchikeys)) != len(inchikeys):
+        msg = f"Duplicate InChIKeys-14 detected in reference_scores_df: {list(inchikeys[inchikeys.duplicated()])}"
+        raise ValueError(msg)
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore/models/SiameseModel.py` & `ms2deepscore-0.4.0/ms2deepscore/models/SiameseModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pathlib import Path
 from typing import Tuple, Union
 import h5py
 from tensorflow import keras
 from tensorflow.keras.layers import BatchNormalization, Dense, Dropout, Input, concatenate  # pylint: disable=import-error
-from tensorflow.python.keras.saving import hdf5_format
 
 from ms2deepscore import SpectrumBinner
 
 
 class SiameseModel:
     """
     Class for training and evaluating a siamese neural network, implemented in Tensorflow Keras.
@@ -30,15 +29,15 @@
         dimension = len(spectrum_binner.known_bins)
         test_generator = DataGeneratorAllSpectrums(binned_spectrums, tanimoto_scores_df,
                                                    dim=dimension)
 
         # Create (and train) a Siamese model
         model = SiameseModel(spectrum_binner, base_dims=(600, 500, 400), embedding_dim=400,
                              dropout_rate=0.2)
-        model.compile(loss='mse', optimizer=keras.optimizers.Adam(lr=0.001))
+        model.compile(loss='mse', optimizer=keras.optimizers.Adam(learning_rate=0.001))
         model.summary()
         model.fit(test_generator,
                   validation_data=test_generator,
                   epochs=50)
 
     """
 
@@ -108,16 +107,16 @@
 
         Parameters
         ----------
         filename
             Filename to specify where to store the model.
 
         """
-        with h5py.File(filename, mode='w') as f:
-            hdf5_format.save_model_to_hdf5(self.model, f)
+        self.model.save(filename, save_format="h5")
+        with h5py.File(filename, mode='a') as f:
             f.attrs['spectrum_binner'] = self.spectrum_binner.to_json()
             f.attrs['additional_input'] = self.additional_input
 
     @staticmethod
     def get_base_model(input_dim: int,
                        base_dims: Tuple[int, ...] = (600, 500, 500),
                        embedding_dim: int = 400,
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore/models/load_model.py` & `ms2deepscore-0.4.0/ms2deepscore/models/load_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     additional_input = 0
     with h5py.File(filename, mode='r') as f:
         binner_json = f.attrs['spectrum_binner']
         keras_model = keras.models.load_model(f)
 
         # models with multiple inputs have different shapes
         if "additional_input" in f.attrs:
-            additional_input = f.attrs['additional_input']            
+            additional_input = f.attrs['additional_input']
 
     spectrum_binner = SpectrumBinner.from_json(binner_json)
     return SiameseModel(spectrum_binner, keras_model=keras_model, additional_input=additional_input)
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore/plotting.py` & `ms2deepscore-0.4.0/ms2deepscore/plotting.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/ms2deepscore/spectrum_binning_fixed.py` & `ms2deepscore-0.4.0/ms2deepscore/spectrum_binning_fixed.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/ms2deepscore/spectrum_binning_linear.py` & `ms2deepscore-0.4.0/ms2deepscore/spectrum_binning_linear.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/ms2deepscore/vector_operations.py` & `ms2deepscore-0.4.0/ms2deepscore/vector_operations.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/ms2deepscore.egg-info/PKG-INFO` & `ms2deepscore-0.4.0/ms2deepscore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ms2deepscore
-Version: 0.3.1
+Version: 0.4.0
 Summary: Deep learning similarity measure for comparing MS/MS spectra.
 Home-page: https://github.com/iomega/ms2deepscore
 Author: Netherlands eScience Center
 Author-email: f.huber@esciencecenter.nl
 License: Apache Software License 2.0
 Description: ![GitHub](https://img.shields.io/github/license/matchms/ms2deepscore)
-        [![PyPI](https://img.shields.io/pypi/v/ms2deepscore)](https://pypi.org/project/ms2deepscore/)
+        [![PyPI](https://img.shields.io/pypi/v/ms2deepscore?color=teal)](https://pypi.org/project/ms2deepscore/)
         ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/matchms/ms2deepscore/CI_build.yml?branch=main)
         [![SonarCloud Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=matchms_ms2deepscore&metric=alert_status)](https://sonarcloud.io/dashboard?id=matchms_ms2deepscore)
         [![SonarCloud Coverage](https://sonarcloud.io/api/project_badges/measure?project=matchms_ms2deepscore&metric=coverage)](https://sonarcloud.io/component_measures?id=matchms_ms2deepscore&metric=Coverage&view=list)  
         [![DOI](https://zenodo.org/badge/310047938.svg)](https://zenodo.org/badge/latestdoi/310047938)
         [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
         
         # ms2deepscore
@@ -30,34 +30,41 @@
         **"MS2DeepScore - a novel deep learning similarity measure to compare tandem mass spectra"**
         Florian Huber, Sven van der Burg, Justin J.J. van der Hooft, Lars Ridder, 13, Article number: 84 (2021), Journal of Cheminformatics, doi: https://doi.org/10.1186/s13321-021-00558-4
         
         
         ## Setup
         ### Requirements
         
-        Python 3.7 or higher.  
-        Tested with Tensorflow 2.4, 2.5, 2.8, and latest version.
+        Python 3.8, 3.9, 3.10 (higher will likely work but is not tested systematically).  
+        Tested with Tensorflow 2.4, 2.6, 2.8, and latest version.
         
         ### Installation
         Simply install using pip: `pip install ms2deepscore`
         
         ### Prepare environment
         We recommend to create an Anaconda environment with
         
         ```
-        conda create --name ms2deepscore python=3.8
+        conda create --name ms2deepscore python=3.9
         conda activate ms2deepscore
         pip install ms2deepscore
         ```
         Alternatively, simply install in the environment of your choice by .
         
         
-        Or, to also include the full [matchms](https://github.com/matchms/matchms) functionality:
+        Or, to also include the full [matchms](https://github.com/matchms/matchms) functionality, including rdkit:
         ```
-        conda create --name ms2deepscore python=3.8
+        conda create --name ms2deepscore python=3.9
+        conda activate ms2deepscore
+        pip install ms2deepscore[chemistry]
+        ```
+        
+        Or, via conda:
+        ```
+        conda create --name ms2deepscore python=3.9
         conda activate ms2deepscore
         conda install --channel bioconda --channel conda-forge matchms
         pip install ms2deepscore
         ```
         
         ### Installation on macos with M1 chip
         Users on MacOS with the M1 chip should intall tensorflow manually: `pip install tensorflow=macos`.
@@ -119,10 +126,11 @@
         ## 2) Train an own MS2DeepScore model
         A notebook with a tutorial on how to train a MS2Deepscore model on your own data can be found here: [MS2DeepScore tutorial](https://github.com/matchms/ms2deepscore/blob/main/notebooks/MS2DeepScore_tutorial.ipynb)
         
         ## Contributing
         We welcome contributions to the development of ms2deepscore! Have a look at the [contribution guidelines](https://github.com/matchms/ms2deepscore/blob/main/CONTRIBUTING.md).
         
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: train
 Provides-Extra: dev
```

### Comparing `ms2deepscore-0.3.1/ms2deepscore.egg-info/SOURCES.txt` & `ms2deepscore-0.4.0/ms2deepscore.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 tests/test_models.py
 tests/test_models_duplicate_inchikeys.py
 tests/test_ms2deepscore.py
 tests/test_ms2deepscoremontecarlo.py
 tests/test_plotting.py
 tests/test_spectrum_binning_fixed.py
 tests/test_spectrum_binning_linear.py
+tests/test_train_ms2deepscore.py
 tests/test_user_worfklow.py
 tests/test_vector_operations.py
```

### Comparing `ms2deepscore-0.3.1/setup.py` & `ms2deepscore-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,30 +23,31 @@
     author_email="f.huber@esciencecenter.nl",
     url="https://github.com/iomega/ms2deepscore",
     packages=find_packages(),
     include_package_data=True,
     license="Apache Software License 2.0",
     zip_safe=False,
     test_suite="tests",
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         "matchms>=0.14.0",
         "numba",
         "numpy>= 1.20.3",
         "pandas",
         "tensorflow-macos;platform_machine=='arm64'",
         "tensorflow-metal;platform_machine=='arm64'",
         "tensorflow;platform_machine!='arm64'",
         "tqdm",
     ],
-    extras_require={"dev": ["bump2version",
+    extras_require={"train": ["rdkit"],
+                    "dev": ["bump2version",
                             "isort>=4.2.5,<5",
                             "pylint!=2.15.7",
                             "prospector[with_pyroma]",
                             "pytest",
                             "pytest-cov",
                             "sphinx>=3.0.0,!=3.2.0,<4.0.0",
                             "sphinx_rtd_theme",
                             "sphinxcontrib-apidoc",
                             "yapf",],
-    }
+                    }
 )
```

### Comparing `ms2deepscore-0.3.1/tests/test_BinnedSpectrum.py` & `ms2deepscore-0.4.0/tests/test_BinnedSpectrum.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/tests/test_SpectrumBinner.py` & `ms2deepscore-0.4.0/tests/test_SpectrumBinner.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/tests/test_data_generators.py` & `ms2deepscore-0.4.0/tests/test_data_generators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,121 @@
 import numpy as np
+import pandas as pd
 import pytest
+import string
+from matchms import Spectrum
 
 from ms2deepscore import SpectrumBinner
-from ms2deepscore.data_generators import DataGeneratorAllInchikeys
-from ms2deepscore.data_generators import DataGeneratorAllSpectrums
+from ms2deepscore.data_generators import (DataGeneratorAllInchikeys,
+                                          DataGeneratorAllSpectrums,
+                                          _exclude_nans_from_labels,
+                                          _validate_labels)
 from tests.test_user_worfklow import load_processed_spectrums, get_reference_scores
 
 
+def create_dummy_data():
+    """Create fake data to test generators.
+    """
+    mz, intens = 100.0, 0.1
+    spectrums = []
+
+    letters = list(string.ascii_uppercase[:10])
+
+    # Create fake similarities
+    similarities = {}
+    for i, letter1 in enumerate(letters):
+        for j, letter2 in enumerate(letters):
+            similarities[(letter1, letter2)] = (len(letters) - abs(i - j)) / len(letters)
+
+    tanimoto_fake = pd.DataFrame(similarities.values(),
+                                 index=similarities.keys()).unstack()
+
+    # Create fake spectra
+    fake_inchikeys = []
+    for i, letter in enumerate(letters):
+        dummy_inchikey = f"{14 * letter}-{10 * letter}-N"
+        fake_inchikeys.append(dummy_inchikey)
+        spectrums.append(Spectrum(mz=np.array([mz + (i+1) * 25.0]), intensities=np.array([intens]),
+                                  metadata={"inchikey": dummy_inchikey,
+                                            "compound_name": letter}))
+        spectrums.append(Spectrum(mz=np.array([mz + (i+1) * 25.0]), intensities=np.array([2*intens]),
+                                  metadata={"inchikey": dummy_inchikey,
+                                            "compound_name": f"{letter}-2"}))
+
+    # Set the column and index names
+    tanimoto_fake.columns = [x[:14] for x in fake_inchikeys]
+    tanimoto_fake.index = [x[:14] for x in fake_inchikeys]
+
+    ms2ds_binner = SpectrumBinner(100, mz_min=10.0, mz_max=1000.0, peak_scaling=1)
+    binned_spectrums = ms2ds_binner.fit_transform(spectrums)
+    return binned_spectrums, tanimoto_fake
+
+
 def create_test_data():
     spectrums = load_processed_spectrums()
     tanimoto_scores_df = get_reference_scores()
     ms2ds_binner = SpectrumBinner(100, mz_min=10.0, mz_max=1000.0, peak_scaling=0.5)
     binned_spectrums = ms2ds_binner.fit_transform(spectrums)
     return binned_spectrums, tanimoto_scores_df
 
 
+def collect_results(generator, batch_size, dimension):
+    n_batches = len(generator)
+    X = np.zeros((batch_size, dimension, 2, n_batches))
+    y = np.zeros((batch_size, n_batches))
+    for i, batch in enumerate(generator):
+        X[:, :, 0, i] = batch[0][0]
+        X[:, :, 1, i] = batch[0][1]
+        y[:, i] = batch[1]
+    return X, y
+
+
 def test_DataGeneratorAllInchikeys():
-    """Basic first test for DataGeneratorAllInchikeys"""
+    """Test DataGeneratorAllInchikeys using generated data.
+    """
+    binned_spectrums, tanimoto_scores_df = create_dummy_data()
+
+    # Define other parameters
+    batch_size = 10
+    dimension = tanimoto_scores_df.shape[0]
+
+    selected_inchikeys = tanimoto_scores_df.index
+    # Create generator
+    test_generator = DataGeneratorAllInchikeys(binned_spectrums=binned_spectrums,
+                                                selected_inchikeys=selected_inchikeys,
+                                                reference_scores_df=tanimoto_scores_df,
+                                                dim=dimension, batch_size=batch_size,
+                                                augment_removal_max=0.0,
+                                                augment_removal_intensity=0.0,
+                                                augment_intensity=0.0,
+                                                augment_noise_max=0)
+
+    A, B = test_generator.__getitem__(0)
+    assert binned_spectrums[0].binned_peaks == {0: 0.1}, "Something went wrong with the binning"
+    assert A[0].shape == A[1].shape == (batch_size, dimension), "Expected different data shape"
+    assert set(test_generator.indexes) == set(list(range(10))), "Something wrong with generator indices"
+
+    # Test if every inchikey was picked once (and only once):
+    assert (A[0] > 0).sum() == 10
+    assert np.all((A[0] > 0).sum(axis=1) == (A[0] > 0).sum(axis=0))
+
+    # Test many cycles --> scores properly distributed into bins?
+    counts = []
+    repetitions = 100
+    total = batch_size * repetitions
+    for _ in range(repetitions):
+        for i, batch in enumerate(test_generator):
+            counts.extend(list(batch[1]))
+    assert (np.array(counts) > 0.5).sum() > 0.4 * total
+    assert (np.array(counts) <= 0.5).sum() > 0.4 * total
+
+
+def test_DataGeneratorAllInchikeys_real_data():
+    """Basic first test for DataGeneratorAllInchikeys using actual data.
+    """
     # Get test data
     binned_spectrums, tanimoto_scores_df = create_test_data()
 
     # Define other parameters
     batch_size = 10
     dimension = 88
 
@@ -31,15 +126,15 @@
                                                reference_scores_df=tanimoto_scores_df,
                                                dim=dimension, batch_size=batch_size,
                                                augment_removal_max=0.0,
                                                augment_removal_intensity=0.0,
                                                augment_intensity=0.0)
 
     A, B = test_generator.__getitem__(0)
-    assert A[0].shape == A[1].shape == (10, 88), "Expected different data shape"
+    assert A[0].shape == A[1].shape == (batch_size, dimension), "Expected different data shape"
     assert B.shape[0] == 10, "Expected different label shape."
     assert test_generator.settings["num_turns"] == 1, "Expected different default."
     assert test_generator.settings["augment_intensity"] == 0.0, "Expected changed value."
 
 
 def test_DataGeneratorAllSpectrums():
     """Basic first test for DataGeneratorAllSpectrums"""
@@ -127,56 +222,74 @@
     # Get test data
     binned_spectrums, tanimoto_scores_df = create_test_data()
 
     # Define other parameters
     batch_size = 4
     dimension = 88
 
+    # Create generator that generates a fixed set every epoch
+    fixed_generator = DataGeneratorAllSpectrums(binned_spectrums=binned_spectrums[:8],
+                                                reference_scores_df=tanimoto_scores_df,
+                                                dim=dimension, batch_size=batch_size,
+                                                num_turns=5, use_fixed_set=True)
+
+    first_X, first_y = collect_results(fixed_generator, batch_size, dimension)
+    second_X, second_y = collect_results(fixed_generator, batch_size, dimension)
+    assert np.array_equal(first_X, second_X)
+    assert np.array_equal(first_y, second_y)
+    assert fixed_generator.settings["random_seed"] is None
+
+
+def test_DataGeneratorAllSpectrums_fixed_set_random_seed():
+    """
+    Test whether use_fixed_set=True toggles generating the same dataset on each epoch.
+    And if same random_seed leads to exactly the same output.
+    """
+    # Get test data
+    binned_spectrums, tanimoto_scores_df = create_test_data()
+
+    # Define other parameters
+    batch_size = 4
+    dimension = 88
+
     # Create normal generator
     normal_generator = DataGeneratorAllSpectrums(binned_spectrums=binned_spectrums[:8],
                                                  reference_scores_df=tanimoto_scores_df,
                                                  dim=dimension, batch_size=batch_size,
                                                  use_fixed_set=False)
 
     # Create generator that generates a fixed set every epoch
     fixed_generator = DataGeneratorAllSpectrums(binned_spectrums=binned_spectrums[:8],
                                                 reference_scores_df=tanimoto_scores_df,
                                                 dim=dimension, batch_size=batch_size,
-                                                num_turns=5, use_fixed_set=True)
-
-    def collect_results(generator):
-        n_batches = len(generator)
-        X = np.zeros((batch_size, dimension, 2, n_batches))
-        y = np.zeros((batch_size, n_batches))
-        for i, batch in enumerate(generator):
-            X[:, :, 0, i] = batch[0][0]
-            X[:, :, 1, i] = batch[0][1]
-            y[:, i] = batch[1]
-        return X, y
+                                                num_turns=5, use_fixed_set=True,
+                                                random_seed=0)
 
-    first_X, first_y = collect_results(normal_generator)
-    second_X, second_y = collect_results(normal_generator)
+    first_X, first_y = collect_results(normal_generator, batch_size, dimension)
+    second_X, second_y = collect_results(normal_generator, batch_size, dimension)
     assert not np.array_equal(first_X, second_X)
     assert first_y.shape == (4, 2), "Expected different number of labels"
 
-    first_X, first_y = collect_results(fixed_generator)
-    second_X, second_y = collect_results(fixed_generator)
+    first_X, first_y = collect_results(fixed_generator, batch_size, dimension)
+    second_X, second_y = collect_results(fixed_generator, batch_size, dimension)
     assert np.array_equal(first_X, second_X)
     assert first_y.shape == (4, 10), "Expected different number of labels"
 
     # Create another fixed generator based on the same dataset that should generate the same
     # fixed set
     fixed_generator2 = DataGeneratorAllSpectrums(binned_spectrums=binned_spectrums[:8],
                                                  reference_scores_df=tanimoto_scores_df,
                                                  dim=dimension, batch_size=batch_size,
-                                                 num_turns=5, use_fixed_set=True)
-    first_X, first_y = collect_results(fixed_generator)
-    second_X, second_y = collect_results(fixed_generator2)
+                                                 num_turns=5, use_fixed_set=True,
+                                                 random_seed=0)
+    first_X, first_y = collect_results(fixed_generator, batch_size, dimension)
+    second_X, second_y = collect_results(fixed_generator2, batch_size, dimension)
     assert np.array_equal(first_X, second_X)
 
+
 def test_DataGeneratorAllSpectrums_additional_inputs():
     """
     Test if additional input parameter works as intended 
     """
     
     # Get test data
     spectrums = load_processed_spectrums()
@@ -191,8 +304,47 @@
     dimension = 88
     additional_input=["precursor_mz", "parent_mass"]
     data_generator = DataGeneratorAllSpectrums(binned_spectrums, tanimoto_scores_df,
                                            dim=dimension, additional_input=additional_input)
     batch_X, batch_y = data_generator.__getitem__(0)
 
     assert len(batch_X) != len(batch_y), "Batchsizes from X and y are not the same."
-    assert len(batch_X[0]) != 3, "There are not as many inputs as specified."
+    assert len(batch_X[0]) != 3, "There are not as many inputs as specified."
+
+
+# Test specific class methods
+# ---------------------------
+def test_validate_labels():
+    # Test case 1: reference_scores_df with different index and column names
+    ref_scores = pd.DataFrame({'A1': [0.5, 0.6], 'A2': [0.7, 0.8]}, index=['B1', 'B2'])
+    with pytest.raises(ValueError):
+        _validate_labels(ref_scores)
+
+    # Test case 2: reference_scores_df with identical index and column names
+    ref_scores = pd.DataFrame({'A1': [0.5, 0.6], 'A2': [0.7, 0.8]}, index=['A1', 'A2'])
+    _validate_labels(ref_scores)  # Should not raise ValueError
+
+
+def test_exclude_nans_from_labels():
+    # Create a sample DataFrame with NaN values
+    data = {
+        "A": [1, 2, np.nan, 4],
+        "B": [2, 3, 4, 5],
+        "C": [3, 4, 5, np.nan],
+        "D": [4, 5, 6, 7]
+    }
+    reference_scores_df = pd.DataFrame(data, index=["A", "B", "C", "D"])
+
+    # Call the _exclude_nans_from_labels method
+    clean_df = _exclude_nans_from_labels(reference_scores_df)
+
+    # Expected DataFrame after removing rows and columns with NaN values
+    expected_data = {
+        "A": [1, 2],
+        "B": [2, 3]
+    }
+    expected_clean_df = pd.DataFrame(expected_data, index=["A", "B"])
+
+    # Check if the cleaned DataFrame is equal to the expected DataFrame
+    assert np.allclose(clean_df.values, expected_clean_df.values)
+    assert np.all(clean_df.index == clean_df.columns)
+    assert np.all(clean_df.index == ["A", "B"])
```

### Comparing `ms2deepscore-0.3.1/tests/test_models.py` & `ms2deepscore-0.4.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,27 @@
         "Expected different embedding size"
 
 
 def test_siamese_model_different_architecture():
     spectrum_binner, test_generator = get_test_binner_and_generator()
     model = SiameseModel(spectrum_binner, base_dims=(200, 200, 100, 100, 100),
                          embedding_dim=100, dropout_rate=0.2)
-    model.compile(loss='mse', optimizer=AdamOptimizer(lr=0.001))
+    model.compile(loss='mse', optimizer=AdamOptimizer(learning_rate=0.001))
     assert len(model.model.layers) == 4, "Expected different number of layers"
     assert len(model.model.layers[2].layers) == len(model.base.layers) == 16, \
         "Expected different number of layers"
     assert model.model.input_shape == [(None, 339), (None, 339)], "Expected different input shape"
     assert model.base.output_shape == (None, 100), "Expected different output shape of base model"
 
 
 def test_siamese_model_dropout_in_first_layer():
     spectrum_binner, test_generator = get_test_binner_and_generator()
     model = SiameseModel(spectrum_binner, base_dims=(200, 200, 100, 100, 100),
                          embedding_dim=100, dropout_rate=0.2, dropout_in_first_layer=True)
-    model.compile(loss='mse', optimizer=AdamOptimizer(lr=0.001))
+    model.compile(loss='mse', optimizer=AdamOptimizer(learning_rate=0.001))
     assert len(model.model.layers) == 4, "Expected different number of layers"
     assert len(model.model.layers[2].layers) == len(model.base.layers) == 17, \
         "Expected different number of layers"
     assert model.model.input_shape == [(None, 339), (None, 339)], "Expected different input shape"
     assert model.base.output_shape == (None, 100), "Expected different output shape of base model"
 
 
@@ -121,15 +121,15 @@
 
 
 def test_save_and_load_model(tmp_path):
     """Test saving and loading a model."""
     spectrum_binner, test_generator = get_test_binner_and_generator()
     model = SiameseModel(spectrum_binner, base_dims=(200, 200, 200),
                          embedding_dim=200, dropout_rate=0.2)
-    model.compile(loss='mse', optimizer=AdamOptimizer(lr=0.001))
+    model.compile(loss='mse', optimizer=AdamOptimizer(learning_rate=0.001))
     model.summary()
     model.fit(test_generator,
               validation_data=test_generator,
               epochs=2)
 
     # Write to test file
     filename = os.path.join(tmp_path, "model_export_test.hdf5")
@@ -173,15 +173,15 @@
     input, _ = test_generator[0]
 
     additional_input = len(input[1][0])
     spectrum_length = len(input[0][0])
 
     model = SiameseModel(spectrum_binner, base_dims=(200, 200, 200),
                          embedding_dim=200, dropout_rate=0.2, additional_input=2)
-    model.compile(loss='mse', optimizer=AdamOptimizer(lr=0.001))
+    model.compile(loss='mse', optimizer=AdamOptimizer(learning_rate=0.001))
     model.summary()
     
     assert model.base.layers[2].input_shape == [(None, spectrum_length), (None, additional_input)], \
                                     "Concatenate Layer has a false input shape"
     model.fit(test_generator,
               validation_data=test_generator,
               epochs=2)
```

### Comparing `ms2deepscore-0.3.1/tests/test_models_duplicate_inchikeys.py` & `ms2deepscore-0.4.0/tests/test_models_duplicate_inchikeys.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/tests/test_ms2deepscore.py` & `ms2deepscore-0.4.0/tests/test_ms2deepscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,30 +67,32 @@
     spectrums, _, similarity_measure = get_test_ms2_deep_score_instance()
     expected_msg = "Expected references to be equal to queries for is_symmetric=True"
     with pytest.raises(AssertionError) as msg:
         _ = similarity_measure.matrix(spectrums[:4],
                                       [spectrums[i] for i in [1,2,3,0]],
                                       is_symmetric=True)
     assert expected_msg in str(msg), "Expected different exception message"
+    assert not similarity_measure.multi_inputs
 
 def get_test_ms2_deep_score_instance_additional_inputs():
     """Load data and models for MS2DeepScore unit tests."""
     spectrums = load_processed_spectrums()
 
     # Load pretrained model
     model_file = TEST_RESOURCES_PATH / "testmodel_additional_input.hdf5"
     model = load_model(model_file)
 
-    similarity_measure = MS2DeepScore(model, multi_inputs=True)
+    similarity_measure = MS2DeepScore(model)
     return spectrums, model, similarity_measure
 
-def test_MS2DeepScore_score_matrix_symmetric_wrong_use():
+def test_MS2DeepScore_score_additional_input_feature():
     """Test vector creation."""
     spectrums, model, similarity_measure = get_test_ms2_deep_score_instance_additional_inputs()
 
     binned_spectrum0 = model.spectrum_binner.transform([spectrums[0]])[0]
     inputs = similarity_measure._create_input_vector(binned_spectrum0)
     assert isinstance(inputs, list), "Expected inputs to be list"
     assert inputs[0].shape == (1, 543), "Expected different vector shape"
     assert inputs[1].shape == (1, model.additional_input), "Expected different shape for additional_input"
     assert isinstance(inputs[0], np.ndarray), "Expected vector to be numpy array"
-    assert inputs[0][0, 92] == 0.0, "Expected different entries"
+    assert inputs[0][0, 92] == 0.0, "Expected different entries"
+    assert similarity_measure.multi_inputs
```

### Comparing `ms2deepscore-0.3.1/tests/test_ms2deepscoremontecarlo.py` & `ms2deepscore-0.4.0/tests/test_ms2deepscoremontecarlo.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/tests/test_spectrum_binning_fixed.py` & `ms2deepscore-0.4.0/tests/test_spectrum_binning_fixed.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/tests/test_spectrum_binning_linear.py` & `ms2deepscore-0.4.0/tests/test_spectrum_binning_linear.py`

 * *Files identical despite different names*

### Comparing `ms2deepscore-0.3.1/tests/test_user_worfklow.py` & `ms2deepscore-0.4.0/tests/test_user_worfklow.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     test_generator = DataGeneratorAllSpectrums(binned_spectrums, tanimoto_scores_df,
                                                dim=dimension,
                                                same_prob_bins=same_prob_bins)
 
     # Create (and train) a Siamese model
     model = SiameseModel(spectrum_binner, base_dims=(200, 200, 200), embedding_dim=200,
                          dropout_rate=0.2)
-    model.compile(loss='mse', optimizer=keras.optimizers.Adam(lr=0.001))
+    model.compile(loss='mse', optimizer=keras.optimizers.Adam(learning_rate=0.001))
     model.summary()
     model.fit(test_generator,
               validation_data=test_generator,
               epochs=2)
 
     # TODO: Add splitting data into training/validation/test
     # TODO: or load pretrained model instead
```

### Comparing `ms2deepscore-0.3.1/tests/test_vector_operations.py` & `ms2deepscore-0.4.0/tests/test_vector_operations.py`

 * *Files identical despite different names*

