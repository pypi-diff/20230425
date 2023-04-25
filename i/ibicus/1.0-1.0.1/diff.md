# Comparing `tmp/ibicus-1.0.tar.gz` & `tmp/ibicus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibicus-1.0.tar", last modified: Tue Apr 25 09:21:48 2023, max compression
+gzip compressed data, was "ibicus-1.0.1.tar", last modified: Tue Apr 25 09:35:18 2023, max compression
```

## Comparing `ibicus-1.0.tar` & `ibicus-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.262123 ibicus-1.0/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    11357 2023-04-25 09:21:19.000000 ibicus-1.0/LICENSE
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     5512 2023-04-25 09:21:48.262123 ibicus-1.0/PKG-INFO
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4087 2023-04-25 09:21:19.000000 ibicus-1.0/README.rst
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.258123 ibicus-1.0/ibicus/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      411 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/__init__.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      786 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/__meta__.py
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.258123 ibicus-1.0/ibicus/debias/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    13038 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/__init__.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    19026 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_cdft.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    25250 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_debiaser.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     5383 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_delta_change.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     9274 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_ecdfm.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    64791 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_isimip.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4847 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_isimip_options.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4209 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_linear_scaling.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    23812 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_quantile_delta_mapping.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    10603 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_quantile_mapping.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    18051 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/debias/_scaled_distribution_mapping.py
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.262123 ibicus-1.0/ibicus/evaluate/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8615 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/__init__.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8252 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/assumptions.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4471 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/correlation.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    25882 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/marginal.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    40184 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/metrics.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    15125 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/multivariate.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    24928 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/evaluate/trend.py
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.262123 ibicus-1.0/ibicus/utils/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      600 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/utils/__init__.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    24236 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/utils/_math_utils.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    22066 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/utils/_running_window_mode.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    15060 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/utils/_utils.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     7118 2023-04-25 09:21:19.000000 ibicus-1.0/ibicus/variables.py
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.258123 ibicus-1.0/ibicus.egg-info/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     5512 2023-04-25 09:21:48.000000 ibicus-1.0/ibicus.egg-info/PKG-INFO
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     1226 2023-04-25 09:21:48.000000 ibicus-1.0/ibicus.egg-info/SOURCES.txt
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)        1 2023-04-25 09:21:48.000000 ibicus-1.0/ibicus.egg-info/dependency_links.txt
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)       88 2023-04-25 09:21:48.000000 ibicus-1.0/ibicus.egg-info/requires.txt
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)       13 2023-04-25 09:21:48.000000 ibicus-1.0/ibicus.egg-info/top_level.txt
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     1730 2023-04-25 09:21:48.262123 ibicus-1.0/setup.cfg
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      448 2023-04-25 09:21:19.000000 ibicus-1.0/setup.py
-drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:48.262123 ibicus-1.0/tests/
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:19.000000 ibicus-1.0/tests/__init__.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8662 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_cdft.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     1836 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_delta_change.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8389 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_ecdfm.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     9011 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_isimip.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4785 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_linear_scaling.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    13367 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_math_utils.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     9842 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_quantile_delta_mapping.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     2652 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_quantile_mapping.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8860 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_running_window_mode.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     2450 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_scaled_distribution_mapping.py
--rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      862 2023-04-25 09:21:19.000000 ibicus-1.0/tests/test_utils.py
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.276266 ibicus-1.0.1/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    11357 2023-04-25 09:21:19.000000 ibicus-1.0.1/LICENSE
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     5474 2023-04-25 09:35:18.276266 ibicus-1.0.1/PKG-INFO
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4087 2023-04-25 09:21:19.000000 ibicus-1.0.1/README.rst
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.268266 ibicus-1.0.1/ibicus/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      411 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/__init__.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      788 2023-04-25 09:34:50.000000 ibicus-1.0.1/ibicus/__meta__.py
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.272266 ibicus-1.0.1/ibicus/debias/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    13038 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/__init__.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    19026 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_cdft.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    25250 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_debiaser.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     5383 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_delta_change.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     9274 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_ecdfm.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    64791 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_isimip.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4847 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_isimip_options.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4209 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_linear_scaling.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    23812 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_quantile_delta_mapping.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    10603 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_quantile_mapping.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    18051 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/debias/_scaled_distribution_mapping.py
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.272266 ibicus-1.0.1/ibicus/evaluate/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8615 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/__init__.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8252 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/assumptions.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4471 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/correlation.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    25882 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/marginal.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    40184 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/metrics.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    15125 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/multivariate.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    24928 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/evaluate/trend.py
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.272266 ibicus-1.0.1/ibicus/utils/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      600 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/utils/__init__.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    24236 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/utils/_math_utils.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    22066 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/utils/_running_window_mode.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    15060 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/utils/_utils.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     7118 2023-04-25 09:21:19.000000 ibicus-1.0.1/ibicus/variables.py
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.272266 ibicus-1.0.1/ibicus.egg-info/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     5474 2023-04-25 09:35:18.000000 ibicus-1.0.1/ibicus.egg-info/PKG-INFO
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     1226 2023-04-25 09:35:18.000000 ibicus-1.0.1/ibicus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)        1 2023-04-25 09:35:18.000000 ibicus-1.0.1/ibicus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)       88 2023-04-25 09:35:18.000000 ibicus-1.0.1/ibicus.egg-info/requires.txt
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)       13 2023-04-25 09:35:18.000000 ibicus-1.0.1/ibicus.egg-info/top_level.txt
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     1684 2023-04-25 09:35:18.276266 ibicus-1.0.1/setup.cfg
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      448 2023-04-25 09:21:19.000000 ibicus-1.0.1/setup.py
+drwxrwxr-x   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:35:18.276266 ibicus-1.0.1/tests/
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)        0 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/__init__.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8662 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_cdft.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     1836 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_delta_change.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8389 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_ecdfm.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     9011 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_isimip.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     4785 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_linear_scaling.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)    13367 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_math_utils.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     9842 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_quantile_delta_mapping.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     2652 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_quantile_mapping.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     8860 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_running_window_mode.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)     2450 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_scaled_distribution_mapping.py
+-rw-rw-r--   0 jakobwes  (1000) jakobwes  (1000)      862 2023-04-25 09:21:19.000000 ibicus-1.0.1/tests/test_utils.py
```

### Comparing `ibicus-1.0/LICENSE` & `ibicus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/PKG-INFO` & `ibicus-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibicus
-Version: 1.0
+Version: 1.0.1
 Summary: ibicus provides a flexible and user-friendly toolkit for the bias correction of climate models and associated evaluation.
 Home-page: https://github.com/ecmwf-projects/ibicus
 Author: Fiona Spuler, Jakob Wessel & European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: ibicus.py@gmail.com
 License: Apache License Version 2.0
 Project-URL: Documentation, https://ibicus.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ecmwf-projects/ibicus
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ******
 ibicus
 ******
```

### Comparing `ibicus-1.0/README.rst` & `ibicus-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/__meta__.py` & `ibicus-1.0.1/ibicus/__meta__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 
 """Container for ibicus metadata."""
 
 __name__ = "ibicus"
-__version__ = "1.0"
+__version__ = "1.0.1"
 __author__ = "Fiona Spuler, Jakob Wessel & European Centre for Medium-Range Weather Forecasts (ECMWF)"
 __author_email__ = "ibicus.py@gmail.com"
 __license__ = "Apache License Version 2.0"
 __description__ = "ibicus provides a flexible and user-friendly toolkit for the bias correction of climate models and associated evaluation."
```

### Comparing `ibicus-1.0/ibicus/debias/__init__.py` & `ibicus-1.0.1/ibicus/debias/__init__.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_cdft.py` & `ibicus-1.0.1/ibicus/debias/_cdft.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_debiaser.py` & `ibicus-1.0.1/ibicus/debias/_debiaser.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_delta_change.py` & `ibicus-1.0.1/ibicus/debias/_delta_change.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_ecdfm.py` & `ibicus-1.0.1/ibicus/debias/_ecdfm.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_isimip.py` & `ibicus-1.0.1/ibicus/debias/_isimip.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_isimip_options.py` & `ibicus-1.0.1/ibicus/debias/_isimip_options.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_linear_scaling.py` & `ibicus-1.0.1/ibicus/debias/_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_quantile_delta_mapping.py` & `ibicus-1.0.1/ibicus/debias/_quantile_delta_mapping.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_quantile_mapping.py` & `ibicus-1.0.1/ibicus/debias/_quantile_mapping.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/debias/_scaled_distribution_mapping.py` & `ibicus-1.0.1/ibicus/debias/_scaled_distribution_mapping.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/__init__.py` & `ibicus-1.0.1/ibicus/evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/assumptions.py` & `ibicus-1.0.1/ibicus/evaluate/assumptions.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/correlation.py` & `ibicus-1.0.1/ibicus/evaluate/correlation.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/marginal.py` & `ibicus-1.0.1/ibicus/evaluate/marginal.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/metrics.py` & `ibicus-1.0.1/ibicus/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/multivariate.py` & `ibicus-1.0.1/ibicus/evaluate/multivariate.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/evaluate/trend.py` & `ibicus-1.0.1/ibicus/evaluate/trend.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/utils/__init__.py` & `ibicus-1.0.1/ibicus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/utils/_math_utils.py` & `ibicus-1.0.1/ibicus/utils/_math_utils.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/utils/_running_window_mode.py` & `ibicus-1.0.1/ibicus/utils/_running_window_mode.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/utils/_utils.py` & `ibicus-1.0.1/ibicus/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus/variables.py` & `ibicus-1.0.1/ibicus/variables.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/ibicus.egg-info/PKG-INFO` & `ibicus-1.0.1/ibicus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibicus
-Version: 1.0
+Version: 1.0.1
 Summary: ibicus provides a flexible and user-friendly toolkit for the bias correction of climate models and associated evaluation.
 Home-page: https://github.com/ecmwf-projects/ibicus
 Author: Fiona Spuler, Jakob Wessel & European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: ibicus.py@gmail.com
 License: Apache License Version 2.0
 Project-URL: Documentation, https://ibicus.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ecmwf-projects/ibicus
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ******
 ibicus
 ******
```

### Comparing `ibicus-1.0/ibicus.egg-info/SOURCES.txt` & `ibicus-1.0.1/ibicus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/setup.cfg` & `ibicus-1.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [metadata]
 name = ibicus
 version = attr: ibicus.__meta__.__version__
 author = Fiona Spuler, Jakob Wessel & European Centre for Medium-Range Weather Forecasts (ECMWF)
 author_email = ibicus.py@gmail.com
 license = Apache License Version 2.0
 description = ibicus provides a flexible and user-friendly toolkit for the bias correction of climate models and associated evaluation.
-long_description_content_type = text/markdown
 long_description = file: README.rst
 url = https://github.com/ecmwf-projects/ibicus
 project_urls = 
 	Documentation = https://ibicus.readthedocs.io/en/latest/
 	Source = https://github.com/ecmwf-projects/ibicus
 	Tracker = https://github.com/ecmwf-projects/ibicus/issues
 classifiers =
```

### Comparing `ibicus-1.0/tests/test_cdft.py` & `ibicus-1.0.1/tests/test_cdft.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_delta_change.py` & `ibicus-1.0.1/tests/test_delta_change.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_ecdfm.py` & `ibicus-1.0.1/tests/test_ecdfm.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_isimip.py` & `ibicus-1.0.1/tests/test_isimip.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_linear_scaling.py` & `ibicus-1.0.1/tests/test_linear_scaling.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_math_utils.py` & `ibicus-1.0.1/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_quantile_delta_mapping.py` & `ibicus-1.0.1/tests/test_quantile_delta_mapping.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_quantile_mapping.py` & `ibicus-1.0.1/tests/test_quantile_mapping.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_running_window_mode.py` & `ibicus-1.0.1/tests/test_running_window_mode.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_scaled_distribution_mapping.py` & `ibicus-1.0.1/tests/test_scaled_distribution_mapping.py`

 * *Files identical despite different names*

### Comparing `ibicus-1.0/tests/test_utils.py` & `ibicus-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

