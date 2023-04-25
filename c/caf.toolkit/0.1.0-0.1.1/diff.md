# Comparing `tmp/caf.toolkit-0.1.0.tar.gz` & `tmp/caf.toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caf.toolkit-0.1.0.tar", last modified: Mon Apr  3 14:00:53 2023, max compression
+gzip compressed data, was "caf.toolkit-0.1.1.tar", last modified: Tue Apr 25 07:11:53 2023, max compression
```

## Comparing `caf.toolkit-0.1.0.tar` & `caf.toolkit-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.592439 caf.toolkit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-03 14:00:53.592439 caf.toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-03 14:00:53.592439 caf.toolkit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.584438 caf.toolkit-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.588438 caf.toolkit-0.1.0/src/caf/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.592439 caf.toolkit-0.1.0/src/caf/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-03 14:00:53.592439 caf.toolkit-0.1.0/src/caf/toolkit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/array_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.588438 caf.toolkit-0.1.0/src/caf/toolkit/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/config_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.588438 caf.toolkit-0.1.0/src/caf/toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/iterative_proportional_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.588438 caf.toolkit-0.1.0/src/caf/toolkit/pandas_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/pandas_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/pandas_utils/df_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/pandas_utils/numpy_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/tqdm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/src/caf/toolkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.588438 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-03 14:00:53.000000 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-03 14:00:53.000000 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 14:00:53.000000 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-03 14:00:53.000000 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-03 14:00:53.000000 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-03 14:00:53.000000 caf.toolkit-0.1.0/src/caf.toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 14:00:53.592439 caf.toolkit-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/tests/test_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/tests/test_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/tests/test_iterative_proportional_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/tests/test_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    41797 2023-04-03 14:00:42.000000 caf.toolkit-0.1.0/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.857313 caf.toolkit-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.857313 caf.toolkit-0.1.1/src/caf/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/array_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/config_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/iterative_proportional_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/df_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/numpy_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/tqdm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29933 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/src/caf/toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.857313 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 07:11:53.000000 caf.toolkit-0.1.1/src/caf.toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:11:53.861313 caf.toolkit-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_iterative_proportional_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41797 2023-04-25 07:11:39.000000 caf.toolkit-0.1.1/tests/test_translation.py
```

### Comparing `caf.toolkit-0.1.0/LICENSE` & `caf.toolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/PKG-INFO` & `caf.toolkit-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolkit of transport planning and appraisal functionalities
 Home-page: https://github.com/Transport-for-the-North/caf.toolkit
 Author: Transport for the North
 Maintainer: Ben Taylor
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.toolkit/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.toolkit
@@ -33,7 +33,13 @@
 
 
 The Common Analytical Framework (CAF) Toolkit is a toolkit of transport
 planning and appraisal functionalities. It's the beginning of a project to make
 a lot of the useful stuff from
 [NorMITs Demand](https://github.com/Transport-for-the-North/NorMITs-Demand)
 more widely available and easily accessible.
+
+
+## Contributing
+CAF.Toolkit happily accepts contributions.
+
+The best way to contribute to this project is to go to the issues tab and report bugs or submit a feature request. This helps CAF.Toolkit become more stable and full-featured. Please check the closed bugs before submitting a bug report to see if your question has already been answered.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.0 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.1 Summary: A toolkit of
 transport planning and appraisal functionalities Home-page: https://github.com/
 Transport-for-the-North/caf.toolkit Author: Transport for the North Maintainer:
 Ben Taylor License: GPL-3.0 Project-URL: Bug Tracker, https://github.com/
 Transport-for-the-North/caf.toolkit/issues Project-URL: Source, https://
 github.com/Transport-for-the-North/caf.toolkit Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
@@ -11,8 +11,13 @@
 TFN_Landscape_Colour_CMYK.png)
                            ****** CAF.Toolkit ******
    [PyPI_Latest_Release] [Coverage] [Testing_Badge] [License:_GNU_GPL_v3.0]
     [linting:_pylint] [code_format:_Google_Style_Guide] [code_style:_black]
 The Common Analytical Framework (CAF) Toolkit is a toolkit of transport
 planning and appraisal functionalities. It's the beginning of a project to make
 a lot of the useful stuff from [NorMITs Demand](https://github.com/Transport-
-for-the-North/NorMITs-Demand) more widely available and easily accessible.
+for-the-North/NorMITs-Demand) more widely available and easily accessible. ##
+Contributing CAF.Toolkit happily accepts contributions. The best way to
+contribute to this project is to go to the issues tab and report bugs or submit
+a feature request. This helps CAF.Toolkit become more stable and full-featured.
+Please check the closed bugs before submitting a bug report to see if your
+question has already been answered.
```

### Comparing `caf.toolkit-0.1.0/pyproject.toml` & `caf.toolkit-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/setup.cfg` & `caf.toolkit-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/array_utils.py` & `caf.toolkit-0.1.1/src/caf/toolkit/array_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/concurrency/multiprocessing_wrapper.py` & `caf.toolkit-0.1.1/src/caf/toolkit/concurrency/multiprocessing_wrapper.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/config_base.py` & `caf.toolkit-0.1.1/src/caf/toolkit/config_base.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/iterative_proportional_fitting.py` & `caf.toolkit-0.1.1/src/caf/toolkit/iterative_proportional_fitting.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/math_utils.py` & `caf.toolkit-0.1.1/src/caf/toolkit/math_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 """A toolbox of useful math related functionality.
 
 Most will be used elsewhere in the codebase too
 """
 # Built-Ins
 import math
+import warnings
+
+from typing import Any
 from typing import Union
 from typing import Collection
 
 # Third Party
 import sparse
 import numpy as np
 import pandas as pd
@@ -171,14 +174,69 @@
             squared_diffs += diffs.todense().flatten().tolist()
         else:
             raise TypeError(f"Cannot handle arrays of type '{type(diffs)}'.")
 
     return float(np.mean(squared_diffs) ** 0.5)
 
 
+def curve_convergence(
+    target: np.ndarray,
+    achieved: np.ndarray,
+) -> float:
+    """Calculate the convergence between two curves.
+
+    Similar to r-squared, but weighted by the target values.
+
+    Parameters
+    ----------
+    target:
+        A np.array listing y values on the curve we are aiming for
+
+    achieved:
+        A np.array listing y values on the curve we have achieved
+
+    Returns
+    -------
+    convergence:
+        A float value between 0 and 1. Values closer to 1 indicate a better
+        convergence.
+
+    Raises
+    ------
+    ValueError:
+        If target and achieved are not the same shape
+    """
+    if target.shape != achieved.shape:
+        raise ValueError(
+            f"Shape of target and achieved do not match.\n"
+            f"\tTarget: {target.shape}\n"
+            f"\tAchieved: {achieved.shape}"
+        )
+
+    # Always return 0 if we achieved NaN
+    if np.isnan(achieved).sum() > 0:
+        return 0
+
+    # If NaN in our target, raise a warning too
+    if np.isnan(target).sum() > 0:
+        warnings.warn(
+            "Found NaN in the target while calculating curve_convergence. "
+            "A NaN value in target will mean 0 is always returned."
+        )
+        return 0
+
+    # Calculate convergence
+    convergence = np.sum((achieved - target) ** 2) / np.sum(
+        (target - np.sum(target) / len(target)) ** 2
+    )
+
+    # Limit between 0 and 1
+    return max(1 - convergence, 0)
+
+
 def nan_report_with_input(
     array: np.ndarray, input_dict: dict[str, np.ndarray]
 ) -> pd.DataFrame:
     """Create a report of NaN values in relative matrix locations.
 
     Uses an input `array` (usually the result of a calculation) to find the
     locations of all np.NaN values. Once found, the index of these values are
@@ -210,7 +268,53 @@
     in_cols = {k: v[mat_idxs] for k, v in input_dict.items()}
 
     # Combine and convert to DataFrame
     final_dict = dict()
     for ddict in [idx_cols, output_col, in_cols]:
         final_dict.update(ddict)
     return pd.DataFrame(final_dict)
+
+
+def check_numeric(check_dict: dict[str, Any]) -> None:
+    """Check if check_dict values are numeric.
+
+    Numeric values are counted as anything that is float or int.
+
+    Parameters
+    ----------
+    check_dict:
+        A dictionary of argument names and argument values to check.
+        The names are used for the error if the value isn't a numeric.
+
+    Raises
+    ------
+    ValueError
+        If any of the parameters aren't floats or ints,
+        includes the parameter name in the message.
+    """
+    for name, val in check_dict.items():
+        if not (np.issubdtype(type(val), np.floating) or np.issubdtype(type(val), np.integer)):
+            raise ValueError(
+                f"{name} should be a scalar number (float or int) " f"not {type(val)}"
+            )
+
+
+def clip_small_non_zero(array: np.ndarray, min_val: float) -> np.ndarray:
+    """Clip all small, non-zero values in an array up to a minimal value.
+
+    Any 0 values will be left as is, and only the values less than `min_val`,
+    and greater than 0 will be changed to `min_val`.
+
+    Parameters
+    ----------
+    array:
+        The array to clip
+
+    min_val:
+        The minimum non-zero value to allow in `array`.
+
+    Returns
+    -------
+    clipped_array:
+        `array`, with all non-zero values clipped to min_val.
+    """
+    return np.where((array < min_val) & (array > 0), min_val, array)
```

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/pandas_utils/df_handling.py` & `caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/df_handling.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/pandas_utils/numpy_conversions.py` & `caf.toolkit-0.1.1/src/caf/toolkit/pandas_utils/numpy_conversions.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/tqdm_utils.py` & `caf.toolkit-0.1.1/src/caf/toolkit/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/translation.py` & `caf.toolkit-0.1.1/src/caf/toolkit/translation.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf/toolkit/validators.py` & `caf.toolkit-0.1.1/src/caf/toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/src/caf.toolkit.egg-info/PKG-INFO` & `caf.toolkit-0.1.1/src/caf.toolkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolkit of transport planning and appraisal functionalities
 Home-page: https://github.com/Transport-for-the-North/caf.toolkit
 Author: Transport for the North
 Maintainer: Ben Taylor
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.toolkit/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.toolkit
@@ -33,7 +33,13 @@
 
 
 The Common Analytical Framework (CAF) Toolkit is a toolkit of transport
 planning and appraisal functionalities. It's the beginning of a project to make
 a lot of the useful stuff from
 [NorMITs Demand](https://github.com/Transport-for-the-North/NorMITs-Demand)
 more widely available and easily accessible.
+
+
+## Contributing
+CAF.Toolkit happily accepts contributions.
+
+The best way to contribute to this project is to go to the issues tab and report bugs or submit a feature request. This helps CAF.Toolkit become more stable and full-featured. Please check the closed bugs before submitting a bug report to see if your question has already been answered.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.0 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.1 Summary: A toolkit of
 transport planning and appraisal functionalities Home-page: https://github.com/
 Transport-for-the-North/caf.toolkit Author: Transport for the North Maintainer:
 Ben Taylor License: GPL-3.0 Project-URL: Bug Tracker, https://github.com/
 Transport-for-the-North/caf.toolkit/issues Project-URL: Source, https://
 github.com/Transport-for-the-North/caf.toolkit Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
@@ -11,8 +11,13 @@
 TFN_Landscape_Colour_CMYK.png)
                            ****** CAF.Toolkit ******
    [PyPI_Latest_Release] [Coverage] [Testing_Badge] [License:_GNU_GPL_v3.0]
     [linting:_pylint] [code_format:_Google_Style_Guide] [code_style:_black]
 The Common Analytical Framework (CAF) Toolkit is a toolkit of transport
 planning and appraisal functionalities. It's the beginning of a project to make
 a lot of the useful stuff from [NorMITs Demand](https://github.com/Transport-
-for-the-North/NorMITs-Demand) more widely available and easily accessible.
+for-the-North/NorMITs-Demand) more widely available and easily accessible. ##
+Contributing CAF.Toolkit happily accepts contributions. The best way to
+contribute to this project is to go to the issues tab and report bugs or submit
+a feature request. This helps CAF.Toolkit become more stable and full-featured.
+Please check the closed bugs before submitting a bug report to see if your
+question has already been answered.
```

### Comparing `caf.toolkit-0.1.0/src/caf.toolkit.egg-info/SOURCES.txt` & `caf.toolkit-0.1.1/src/caf.toolkit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,33 @@
 src/caf.toolkit.egg-info/namespace_packages.txt
 src/caf.toolkit.egg-info/requires.txt
 src/caf.toolkit.egg-info/top_level.txt
 src/caf/toolkit/__init__.py
 src/caf/toolkit/_version.py
 src/caf/toolkit/array_utils.py
 src/caf/toolkit/config_base.py
+src/caf/toolkit/cost_utils.py
+src/caf/toolkit/io.py
 src/caf/toolkit/iterative_proportional_fitting.py
 src/caf/toolkit/math_utils.py
 src/caf/toolkit/py.typed
+src/caf/toolkit/timing.py
 src/caf/toolkit/toolbox.py
 src/caf/toolkit/tqdm_utils.py
 src/caf/toolkit/translation.py
 src/caf/toolkit/validators.py
 src/caf/toolkit/concurrency/__init__.py
 src/caf/toolkit/concurrency/multiprocessing_wrapper.py
 src/caf/toolkit/core/__init__.py
 src/caf/toolkit/core/types.py
 src/caf/toolkit/pandas_utils/__init__.py
 src/caf/toolkit/pandas_utils/df_handling.py
 src/caf/toolkit/pandas_utils/numpy_conversions.py
 tests/test_array_utils.py
 tests/test_config_base.py
+tests/test_cost_utils.py
+tests/test_io.py
 tests/test_iterative_proportional_fitting.py
 tests/test_math_utils.py
+tests/test_timing.py
 tests/test_toolbox.py
 tests/test_translation.py
```

### Comparing `caf.toolkit-0.1.0/tests/test_array_utils.py` & `caf.toolkit-0.1.1/tests/test_array_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,19 @@
     @pytest.mark.parametrize("sum_axis", axis_permutations(3))
     def test_sum_axis_subset(
         self, random_3d_sparse_matrix: sparse.COO, sum_axis: tuple[int, ...]
     ):
         """Test that all axis can be summed together"""
         target = random_3d_sparse_matrix.sum(axis=sum_axis)
         achieved = array_utils.sparse_sum(random_3d_sparse_matrix, axis=sum_axis)
-        np.testing.assert_almost_equal(achieved.todense(), target.todense())
+        # One of these sometimes returns a float instead of sparse. Leave separate
+        # until error comes back
+        one = achieved.todense()
+        two = target.todense()
+        np.testing.assert_almost_equal(one, two)
 
     def test_sum_axis_int(self, random_3d_sparse_matrix: sparse.COO):
         """Test that all axis can be summed together"""
         target = random_3d_sparse_matrix.sum(axis=1)
         achieved = array_utils.sparse_sum(random_3d_sparse_matrix, axis=1)
         np.testing.assert_almost_equal(achieved.todense(), target.todense())
```

### Comparing `caf.toolkit-0.1.0/tests/test_config_base.py` & `caf.toolkit-0.1.1/tests/test_config_base.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/tests/test_iterative_proportional_fitting.py` & `caf.toolkit-0.1.1/tests/test_iterative_proportional_fitting.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.0/tests/test_translation.py` & `caf.toolkit-0.1.1/tests/test_translation.py`

 * *Files identical despite different names*

