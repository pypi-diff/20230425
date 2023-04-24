# Comparing `tmp/bs_python_utils-0.0.2.tar.gz` & `tmp/bs_python_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.0.2.tar", max compression
+gzip compressed data, was "bs_python_utils-0.0.3.tar", max compression
```

## Comparing `bs_python_utils-0.0.2.tar` & `bs_python_utils-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.2/LICENSE
--rw-r--r--   0        0        0     1073 2023-04-24 22:34:42.827734 bs_python_utils-0.0.2/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.2/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.2/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28450 2023-04-24 21:46:50.367154 bs_python_utils-0.0.2/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.2/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.2/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.2/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    14997 2023-04-24 20:25:24.254572 bs_python_utils-0.0.2/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.2/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.2/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1337 2023-04-24 20:25:24.506789 bs_python_utils-0.0.2/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.2/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    29170 2023-04-24 20:25:24.806746 bs_python_utils-0.0.2/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.2/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.2/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.2/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.2/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1351 2023-04-24 21:46:31.381627 bs_python_utils-0.0.2/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     4316 2023-04-24 20:34:32.213666 bs_python_utils-0.0.2/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 21:45:53.138176 bs_python_utils-0.0.2/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      551 2023-04-24 21:45:53.146175 bs_python_utils-0.0.2/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.2/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      787 2023-04-24 21:17:50.679542 bs_python_utils-0.0.2/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.2/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.2/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1871 2023-04-24 22:33:47.638981 bs_python_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 bs_python_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1119 2023-04-24 22:47:51.485025 bs_python_utils-0.0.3/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.3/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.3/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.3/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.3/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.3/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.3/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.3/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.3/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.3/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.3/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.3/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    29170 2023-04-24 20:25:24.806746 bs_python_utils-0.0.3/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.3/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.3/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.3/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.3/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.3/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.3/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.3/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.3/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.3/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.3/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.3/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.3/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1871 2023-04-24 22:47:22.264599 bs_python_utils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 bs_python_utils-0.0.3/PKG-INFO
```

### Comparing `bs_python_utils-0.0.2/LICENSE` & `bs_python_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/README.md` & `bs_python_utils-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,9 +10,12 @@
 
 - **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 - **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 
 ### Release notes
 
+#### 0.0.3  (April 24, 2023)
+Satisfied mypy.
+
 #### 0.0.2  (April 24, 2023)
 Fixed main PyPI page.
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/Timer.py` & `bs_python_utils-0.0.3/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_altair.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_altair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ a personal library of Altair plots
 """
 
-from typing import Callable
+from typing import Callable, cast
 
 import altair as alt
 import numpy as np
 import pandas as pd
 from altair_saver import save as alt_save
 
 from bs_python_utils.bsnputils import check_matrix, check_vector
@@ -591,15 +591,15 @@
                 f"_stack_estimates: we have {n_estimates} names of estimators and"
                 f" {shape_est[1]} estimators"
             )
         for i_est, est_name in enumerate(estimate_names):
             df1[est_name] = estimates[:, i_est]
         ordered_estimates = [*estimate_names, "True value"]
 
-    return df1, ordered_estimates
+    return df1, cast(list[str], ordered_estimates)
 
 
 def plot_parameterized_estimates(
     parameter_name: str,
     parameter_values: np.ndarray,
     coeff_names: str | list[str],
     true_values: np.ndarray,
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_logging.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_mem.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_opt.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_opt.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Any, Callable, Iterable, Optional, Union, cast
 
 import numpy as np
 import scipy.linalg as spla
 import scipy.optimize as spopt
 
 from bs_python_utils.bsnputils import TwoArrays, check_vector, npmaxabs
-from bs_python_utils.bssputils import describe_array
 from bs_python_utils.bsutils import bs_error_abort, print_stars
 from bs_python_utils.Timer import timeit
 
 ScalarFunctionAndGradient = Callable[
     [np.ndarray, Iterable, Optional[bool]], Union[float, tuple[float, np.ndarray]]
 ]
 """Type of f(v, args, gr) that returns a scalar value and also a gradient if gr is True"""
@@ -457,62 +456,7 @@
     xdt = x_diff.T
     xpg = xdt @ gradient_diff
     hdg = hess_inv @ gradient_diff
     dgp_hdg = gradient_diff.T @ hdg
     u = x_diff / xpg - hdg / dgp_hdg
     hess_inv_new = dfp_update(hess_inv, gradient_diff, x_diff) + dgp_hdg * (u @ u.T)
     return cast(np.ndarray, hess_inv_new)
-
-
-if __name__ == "__main__":
-    print_stars("Testing acc_grad_descent")
-
-    def grad_f(x, p):
-        xp = x - p[0]
-        return 4.0 * xp * xp * xp
-
-    x_init = np.random.normal(size=10000)
-
-    p = 1.0
-    x_conv, ret_code = acc_grad_descent(
-        grad_f, x_init, other_params=np.array([p]), tol=1e-12, verbose=False
-    )
-
-    describe_array(x_conv - p, "x-p should be close to zero")
-
-    def obj(x, args):
-        res = x - args
-        return np.sum(res * res)
-
-    def grad_obj(x, args):
-        res = x - args
-        return 2.0 * res
-
-    n = 5
-    x_init = np.full(n, 0.5)
-    args = np.arange(n)
-    bounds = [(-10.0, 10.0) for _ in range(n)]
-
-    fixed_vars = [1, 3]
-    fixed_vals = -np.ones(2)
-
-    resopt = minimize_some_fixed(
-        obj,
-        grad_obj,
-        x_init,
-        args,
-        fixed_vars=fixed_vars,
-        fixed_vals=fixed_vals,
-        bounds=bounds,
-    )
-
-    print(resopt)
-
-    # test the step routines
-    g = grad_obj(x_init, args)
-    alpha_a = armijo_alpha(obj, x_init, -g, args)
-    print(f"\nArmijo alpha={alpha_a}")
-
-    alpha_b, g_b = barzilai_borwein_alpha(grad_obj, x_init, args)
-    print(f"\nBarzilai-Borwein alpha={alpha_a}")
-    print("g and g_b:")
-    print(np.column_stack((g, g_b)))
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.0.3/bs_python_utils/bs_sparse_gaussian.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Args:
         ndims: number of dimensions (1 to 5)
         iprec: precision (must be 9, 13, or 17)
 
     Returns:
         a pair of  arrays `nodes` and `weights`;
-        `nodes` has `ndims`-1 columns and weights is a vector
+        `nodes` has `ndims`-1 columns and `weights` is a vector
     """
     GHdir = (
         Path.home() / "Dropbox" / "GHsparseGrids"
         if GHsparsedir is None
         else Path(GHsparsedir)
     )
     if iprec not in [9, 13, 17]:
@@ -40,7 +40,8 @@
         weights = grid[:, 0]
         nodes = grid[:, 1:]
         return nodes, weights
     else:
         bs_error_abort(
             f"We only do sparse integration in one to five dimensions, not {ndims}"
         )
+        return np.zeros(1), np.zeros(1)  # for mypy
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.0.3/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bsnputils.py` & `bs_python_utils-0.0.3/bs_python_utils/bsnputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bssputils.py` & `bs_python_utils-0.0.3/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bsstats.py` & `bs_python_utils-0.0.3/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/bsutils.py` & `bs_python_utils-0.0.3/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.0.3/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/example_opt.py` & `bs_python_utils-0.0.3/bs_python_utils/example_opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """examples of optimization"""
 
 import numpy as np
 
-from bs_python_utils.bsutils import print_stars
-from bs_python_utils.bssputils import describe_array
 from bs_python_utils.bs_opt import (
     acc_grad_descent,
-    minimize_some_fixed,
     armijo_alpha,
     barzilai_borwein_alpha,
+    minimize_some_fixed,
 )
-
+from bs_python_utils.bssputils import describe_array
+from bs_python_utils.bsutils import print_stars
 
 print_stars("Testing acc_grad_descent")
 
 
 def grad_f(x, p):
     xp = x - p[0]
     return 4.0 * xp * xp * xp
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.0.3/bs_python_utils/examples_distance_covariances.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """examples using distance_covariances"""
 
 import numpy as np
 
-from bs_python_utils.distance_covariances import pvalue_pdcov, dcov_dcor, pdcov_pdcor
+from bs_python_utils.distance_covariances import dcov_dcor, pdcov_pdcor, pvalue_pdcov
 
 # example page 2396 of Szekely and Rizzo 2014
 n = 2000
 do_bootstrap = False
 Z1 = np.random.normal(size=n)
 Z2 = np.random.normal(size=n)
 Z3 = np.random.normal(size=n)
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/examples_mem.py` & `bs_python_utils-0.0.3/bs_python_utils/examples_mem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ example of using bs_mem"""
-import numpy as np
 import tracemalloc
 
+import numpy as np
+
 from bs_python_utils.bs_mem import (
     memory_display_top,
     memory_display_top_diffs,
     memory_usage,
 )
 
 tracemalloc.start()
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.0.3/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.0.3/bs_python_utils/examples_sklearn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """examples using my sklearn code"""
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
 from sklearn.preprocessing import PolynomialFeatures, StandardScaler
 
 from bs_python_utils.sklearn_utils import skl_npreg_lasso
 
-
 n_obs = 10000
 X1 = -2.0 + 3.0 * np.random.uniform(size=n_obs)
 X2 = np.random.normal(loc=1.0, scale=2.0, size=n_obs)
 y = X1 * X2 * X2 / 100.0 - (X1 / 5.0 - X2 / 3.0) ** 3 + np.random.normal(size=n_obs)
 
 X = np.column_stack((X1, X2))
```

### Comparing `bs_python_utils-0.0.2/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.0.3/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.0.3/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.2/pyproject.toml` & `bs_python_utils-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.0.2"
+version = "0.0.3"
 description = "my Python utilities"
 authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.0.2/PKG-INFO` & `bs_python_utils-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: fbsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -34,10 +34,13 @@
 
 - **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 - **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 
 ### Release notes
 
+#### 0.0.3  (April 24, 2023)
+Satisfied mypy.
+
 #### 0.0.2  (April 24, 2023)
 Fixed main PyPI page.
```

