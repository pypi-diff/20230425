# Comparing `tmp/bs_python_utils-0.0.1.tar.gz` & `tmp/bs_python_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.0.1.tar", max compression
+gzip compressed data, was "bs_python_utils-0.0.2.tar", max compression
```

## Comparing `bs_python_utils-0.0.1.tar` & `bs_python_utils-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.1/LICENSE
--rw-r--r--   0        0        0     2062 2023-04-21 14:06:07.426483 bs_python_utils-0.0.1/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.1/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.1/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28450 2023-04-24 21:46:50.367154 bs_python_utils-0.0.1/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.1/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.1/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.1/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    14997 2023-04-24 20:25:24.254572 bs_python_utils-0.0.1/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.1/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.1/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1337 2023-04-24 20:25:24.506789 bs_python_utils-0.0.1/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.1/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    29170 2023-04-24 20:25:24.806746 bs_python_utils-0.0.1/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.1/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.1/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.1/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.1/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1351 2023-04-24 21:46:31.381627 bs_python_utils-0.0.1/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     4316 2023-04-24 20:34:32.213666 bs_python_utils-0.0.1/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 21:45:53.138176 bs_python_utils-0.0.1/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      551 2023-04-24 21:45:53.146175 bs_python_utils-0.0.1/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.1/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      787 2023-04-24 21:17:50.679542 bs_python_utils-0.0.1/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.1/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.1/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1871 2023-04-23 22:27:40.997198 bs_python_utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 bs_python_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1073 2023-04-24 22:34:42.827734 bs_python_utils-0.0.2/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.2/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.2/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28450 2023-04-24 21:46:50.367154 bs_python_utils-0.0.2/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.2/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.2/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.2/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    14997 2023-04-24 20:25:24.254572 bs_python_utils-0.0.2/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.2/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.2/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1337 2023-04-24 20:25:24.506789 bs_python_utils-0.0.2/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.2/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    29170 2023-04-24 20:25:24.806746 bs_python_utils-0.0.2/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.2/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.2/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.2/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.2/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1351 2023-04-24 21:46:31.381627 bs_python_utils-0.0.2/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     4316 2023-04-24 20:34:32.213666 bs_python_utils-0.0.2/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 21:45:53.138176 bs_python_utils-0.0.2/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      551 2023-04-24 21:45:53.146175 bs_python_utils-0.0.2/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.2/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      787 2023-04-24 21:17:50.679542 bs_python_utils-0.0.2/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.2/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.2/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1871 2023-04-24 22:33:47.638981 bs_python_utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 bs_python_utils-0.0.2/PKG-INFO
```

### Comparing `bs_python_utils-0.0.1/LICENSE` & `bs_python_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/Timer.py` & `bs_python_utils-0.0.2/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_altair.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_logging.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_mem.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_opt.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.0.2/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.0.2/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bsnputils.py` & `bs_python_utils-0.0.2/bs_python_utils/bsnputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bssputils.py` & `bs_python_utils-0.0.2/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bsstats.py` & `bs_python_utils-0.0.2/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/bsutils.py` & `bs_python_utils-0.0.2/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.0.2/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/example_opt.py` & `bs_python_utils-0.0.2/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/examples_altair.py` & `bs_python_utils-0.0.2/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.0.2/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/examples_mem.py` & `bs_python_utils-0.0.2/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.0.2/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.0.2/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.0.2/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.0.2/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.1/pyproject.toml` & `bs_python_utils-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.0.1"
+version = "0.0.2"
 description = "my Python utilities"
 authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.0.1/PKG-INFO` & `bs_python_utils-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: fbsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,52 +20,24 @@
 Requires-Dist: vega-datasets (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://bsalanie.github.io/bs-python-utils/
 Project-URL: Repository, https://github.com/bsalanie/bs-python-utils
 Description-Content-Type: text/markdown
 
 # bs-python-utils
 
-[![Release](https://img.shields.io/github/v/release/bsalanie/bs-python-utils)](https://img.shields.io/github/v/release/bsalanie/bs-python-utils)
+<!-- [![Release](https://img.shields.io/github/v/release/bsalanie/bs-python-utils)](https://img.shields.io/github/v/release/bsalanie/bs-python-utils) -->
 [![Build status](https://img.shields.io/github/actions/workflow/status/bsalanie/bs-python-utils/main.yml?branch=main)](https://github.com/bsalanie/bs-python-utils/actions/workflows/main.yml?query=branch%3Amain)
-[![codecov](https://codecov.io/gh/bsalanie/bs-python-utils/branch/main/graph/badge.svg)](https://codecov.io/gh/bsalanie/bs-python-utils)
+<!-- [![codecov](https://codecov.io/gh/bsalanie/bs-python-utils/branch/main/graph/badge.svg)](https://codecov.io/gh/bsalanie/bs-python-utils) -->
 [![Commit activity](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)](https://img.shields.io/github/commit-activity/m/bsalanie/bs-python-utils)
 [![License](https://img.shields.io/github/license/bsalanie/bs-python-utils)](https://img.shields.io/github/license/bsalanie/bs-python-utils)
 
-my Python utilities
+My Python utilities.
 
 - **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 - **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
-## Getting started with your project
 
-First, create a repository on GitHub with the same name as this project, and then run the following commands:
+### Release notes
 
-``` bash
-git init -b main
-git add .
-git commit -m "init commit"
-git remote add origin git@github.com:bsalanie/bs-python-utils.git
-git push -u origin main
-```
+#### 0.0.2  (April 24, 2023)
+Fixed main PyPI page.
 
-Finally, install the environment and the pre-commit hooks with 
-
-```bash
-make install
-```
-
-You are now ready to start development on your project! The CI/CD
-pipeline will be triggered when you open a pull request, merge to main,
-or when you create a new release.
-
-
-## Releasing a new version
-
-<!-- - Create an API Token on [Pypi](https://pypi.org/).
-- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting 
-[this page](https://github.com/bsalanie/bs-python-utils/settings/secrets/actions/new). -->
-- Create a [new release](https://github.com/bsalanie/bs-python-utils/releases/new) on Github. 
-Create a new tag in the form ``*.*.*``.
-
----
-
-Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
```

