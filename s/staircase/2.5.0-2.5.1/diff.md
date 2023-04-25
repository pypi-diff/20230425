# Comparing `tmp/staircase-2.5.0.tar.gz` & `tmp/staircase-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staircase-2.5.0.tar", max compression
+gzip compressed data, was "staircase-2.5.1.tar", max compression
```

## Comparing `staircase-2.5.0.tar` & `staircase-2.5.1.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     1074 2022-10-19 09:16:36.878805 staircase-2.5.0/LICENSE
--rw-r--r--   0        0        0     8425 2022-10-19 09:16:36.878805 staircase-2.5.0/README.md
--rw-r--r--   0        0        0     2332 2022-10-19 09:16:36.890805 staircase-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1044 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/__init__.py
--rw-r--r--   0        0        0      255 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/_typing.py
--rw-r--r--   0        0        0      706 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/constants.py
--rw-r--r--   0        0        0        0 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/__init__.py
--rw-r--r--   0        0        0      756 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/accessor.py
--rw-r--r--   0        0        0     2439 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/arrays/__init__.py
--rw-r--r--   0        0        0     2151 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/arrays/accessor.py
--rw-r--r--   0        0        0    21413 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/arrays/docstrings.py
--rw-r--r--   0        0        0     9372 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/arrays/extension.py
--rw-r--r--   0        0        0      409 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/exceptions/__init__.py
--rw-r--r--   0        0        0     6408 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/layering.py
--rw-r--r--   0        0        0     1890 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/__init__.py
--rw-r--r--   0        0        0     5454 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/arithmetic.py
--rw-r--r--   0        0        0     4217 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/common.py
--rw-r--r--   0        0        0    13779 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/docstrings.py
--rw-r--r--   0        0        0     3615 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/logical.py
--rw-r--r--   0        0        0     6875 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/masking.py
--rw-r--r--   0        0        0     4785 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/relational.py
--rw-r--r--   0        0        0     1097 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/ops/rops.py
--rw-r--r--   0        0        0     3259 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/sampling.py
--rw-r--r--   0        0        0     6310 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/slicing.py
--rw-r--r--   0        0        0    24270 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/stairs.py
--rw-r--r--   0        0        0      721 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/stats/__init__.py
--rw-r--r--   0        0        0     4001 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/stats/distribution.py
--rw-r--r--   0        0        0    11489 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/stats/docstrings.py
--rw-r--r--   0        0        0     9555 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/core/stats/statistic.py
--rw-r--r--   0        0        0     2377 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/docstrings/__init__.py
--rw-r--r--   0        0        0     7256 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/docstrings/examples.py
--rw-r--r--   0        0        0     9798 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/docstrings/slicing.py
--rw-r--r--   0        0        0        0 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/io/__init__.py
--rw-r--r--   0        0        0        0 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/io/json.py
--rw-r--r--   0        0        0        0 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/io/pickle.py
--rw-r--r--   0        0        0        0 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/plotting/__init__.py
--rw-r--r--   0        0        0      959 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/plotting/accessor.py
--rw-r--r--   0        0        0      826 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/plotting/docstrings.py
--rw-r--r--   0        0        0     3081 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/plotting/matplotlib.py
--rw-r--r--   0        0        0     3950 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/test_data.py
--rw-r--r--   0        0        0     1498 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/util/__init__.py
--rw-r--r--   0        0        0     1630 2022-10-19 09:16:36.890805 staircase-2.5.0/staircase/util/_decorators.py
--rw-r--r--   0        0        0     9923 1970-01-01 00:00:00.000000 staircase-2.5.0/setup.py
--rw-r--r--   0        0        0    10280 1970-01-01 00:00:00.000000 staircase-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-25 05:39:05.351480 staircase-2.5.1/LICENSE
+-rw-r--r--   0        0        0     8425 2023-04-25 05:39:05.351480 staircase-2.5.1/README.md
+-rw-r--r--   0        0        0     2713 2023-04-25 05:39:05.363480 staircase-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1044 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/__init__.py
+-rw-r--r--   0        0        0      255 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/_typing.py
+-rw-r--r--   0        0        0      806 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/constants.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/accessor.py
+-rw-r--r--   0        0        0     2439 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/__init__.py
+-rw-r--r--   0        0        0     2183 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/accessor.py
+-rw-r--r--   0        0        0    21413 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/docstrings.py
+-rw-r--r--   0        0        0     9629 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/arrays/extension.py
+-rw-r--r--   0        0        0      409 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     6496 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/layering.py
+-rw-r--r--   0        0        0     1890 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/__init__.py
+-rw-r--r--   0        0        0     5454 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/arithmetic.py
+-rw-r--r--   0        0        0     4217 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/common.py
+-rw-r--r--   0        0        0    13779 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/docstrings.py
+-rw-r--r--   0        0        0     3615 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/logical.py
+-rw-r--r--   0        0        0     6875 2023-04-25 05:39:05.363480 staircase-2.5.1/staircase/core/ops/masking.py
+-rw-r--r--   0        0        0     4785 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/ops/relational.py
+-rw-r--r--   0        0        0     1097 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/ops/rops.py
+-rw-r--r--   0        0        0     3420 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/sampling.py
+-rw-r--r--   0        0        0     6651 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/slicing.py
+-rw-r--r--   0        0        0    25237 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stairs.py
+-rw-r--r--   0        0        0      721 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/__init__.py
+-rw-r--r--   0        0        0     4001 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/distribution.py
+-rw-r--r--   0        0        0    11489 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/docstrings.py
+-rw-r--r--   0        0        0     9555 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/core/stats/statistic.py
+-rw-r--r--   0        0        0     2377 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/docstrings/__init__.py
+-rw-r--r--   0        0        0     7256 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/docstrings/examples.py
+-rw-r--r--   0        0        0     9798 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/docstrings/slicing.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/io/json.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/io/pickle.py
+-rw-r--r--   0        0        0        0 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/accessor.py
+-rw-r--r--   0        0        0      826 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/docstrings.py
+-rw-r--r--   0        0        0     3081 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/plotting/matplotlib.py
+-rw-r--r--   0        0        0     4185 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/test_data.py
+-rw-r--r--   0        0        0     1498 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/util/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-25 05:39:05.367480 staircase-2.5.1/staircase/util/_decorators.py
+-rw-r--r--   0        0        0    10381 1970-01-01 00:00:00.000000 staircase-2.5.1/PKG-INFO
```

### Comparing `staircase-2.5.0/LICENSE` & `staircase-2.5.1/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2021 Riley Clement
+Copyright (c) 2020-2023 Riley Clement
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `staircase-2.5.0/README.md` & `staircase-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/pyproject.toml` & `staircase-2.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "staircase"
-version = "2.5.0"
+version = "2.5.1"
 description = "A data analysis package based on modelling and manipulation of mathematical step functions. Strongly aligned with pandas."
 readme = "README.md"
 authors = ["Riley Clement <venaturum@gmail.com>"]
 maintainers = ["Riley Clement <venaturum@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/staircase-dev/staircase"
 homepage = "https://staircase.dev"
@@ -30,62 +30,85 @@
 classifiers=[
 	'Operating System :: OS Independent',
 	'Intended Audience :: Science/Research',
 	'Programming Language :: Python :: 3.7',
 	'Programming Language :: Python :: 3.8',
 	'Programming Language :: Python :: 3.9',
 	'Programming Language :: Python :: 3.10',
+	'Programming Language :: Python :: 3.11',
 	'Topic :: Scientific/Engineering',
 ]
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/staircase-dev/staircase/issues"
+
+
 [tool.poetry.dependencies]
 python = "^3.7"
 matplotlib = ">=2"
 pytz = "*"
+typing-extensions = "^4.4.0"
 
 [[tool.poetry.dependencies.pandas]]
 python = ">=3.7,<3.10"
 version = "^1"
 
 [[tool.poetry.dependencies.pandas]]
 python = "^3.10"
-version = "^1.3.4"
+version = ">=1.3.4,<3"
 
 [[tool.poetry.dependencies.numpy]]
 python = ">=3.7,<3.10"
 version = "^1.15"
 
 [[tool.poetry.dependencies.numpy]]
 python = "^3.10"
 version = "^1.21.2"
 
 
-
-
 [tool.poetry.dev-dependencies]
 ipykernel = "^6"
 pytest = "^6"
 pytest-cov = "*"
 sphinx = "*"
 nbsphinx = ">=0.8.5"
 sphinx-autobuild = "*"
 seaborn = ">=0.8.0"
 notebook = ">= 6.0"
-isort = ">=5.8"
-black = {version = "*", python = "^3.6.2"}
-flake8 = ">=3.9"
-pre-commit = {version = ">=2.13", python = "^3.6.1"}
+isort = ">=5.8,<5.12"
+black = ">=22.10"
+flake8 = ">=5"
+pre-commit = ">=2.20"
 tox=">=3.15"
-
+mypy = "^0.982"
 
 [tool.poetry.extras]
 codecov = ["codecov"]
 
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/staircase-dev/staircase/issues"
+[tool.black]
+line-length=88
+
+[tool.mypy]
+# disallow_untyped_defs='true'
+# disallow_incomplete_defs='true'
+# no_implicit_optional='true'
+exclude = [
+    '^docs/.',
+	'^core/ops.',
+	'docstrings\\.pyi$',
+	'^tests/.',
+	'^staircase/plotting.',
+]
+
+[[tool.mypy.overrides]]
+module=[
+    'matplotlib.*',
+    'pandas.*',
+]
+ignore_missing_imports='true'
 
 [tool.isort]
 # make it compatible with black
 profile = "black"
 multi_line_output = 3
 src_paths = ["staircase", "tests"]
```

### Comparing `staircase-2.5.0/staircase/__init__.py` & `staircase-2.5.1/staircase/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/constants.py` & `staircase-2.5.1/staircase/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,43 @@
+from __future__ import annotations
+
+
 class NegInf:
     def __init__(self):
         pass
 
-    def __lt__(self, other):
+    def __lt__(self, other) -> bool:
         assert not isinstance(other, NegInf)
         return True
 
-    def __gt__(self, other):
+    def __gt__(self, other) -> bool:
         assert not isinstance(other, (Inf, NegInf))
         return False
 
-    def __neg__(self):
+    def __neg__(self) -> Inf:
         return inf
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "-inf"
 
 
 class Inf:
     def __init__(self):
         pass
 
-    def __gt__(self, other):
+    def __gt__(self, other) -> bool:
         assert not isinstance(other, Inf)
         return True
 
-    def __lt__(self, other):
+    def __lt__(self, other) -> bool:
         assert not isinstance(other, (Inf, NegInf))
         return False
 
-    def __neg__(self):
+    def __neg__(self) -> NegInf:
         return neginf
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "inf"
 
 
 neginf = NegInf()
 inf = Inf()
```

### Comparing `staircase-2.5.0/staircase/core/accessor.py` & `staircase-2.5.1/staircase/core/accessor.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/arrays/__init__.py` & `staircase-2.5.1/staircase/core/arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/arrays/accessor.py` & `staircase-2.5.1/staircase/core/arrays/accessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         if not isinstance(pandas_obj.dtype, StairsDtype):
             raise AttributeError(
                 'sc accessor only valid for Series with Stairs dtype.  Convert using .astype("Stairs").'
             )
         self._obj = pandas_obj
 
     @Appender(docstrings.make_docstring("accessor", "corr"), join="\n", indents=1)
-    def corr(self, where=(-inf, inf)):
+    def corr(self, where=(-inf, inf)) -> pd.DataFrame:
         return pd.DataFrame(
             self._obj.values.corr(where),
             index=self._obj.index,
             columns=self._obj.index,
         )
 
     @Appender(docstrings.make_docstring("accessor", "cov"), join="\n", indents=1)
-    def cov(self, where=(-inf, inf)):
+    def cov(self, where=(-inf, inf)) -> pd.DataFrame:
         return pd.DataFrame(
             self._obj.values.cov(where),
             index=self._obj.index,
             columns=self._obj.index,
         )
 
     @Appender(docstrings.make_docstring("accessor", "logical_or"), join="\n", indents=1)
```

### Comparing `staircase-2.5.0/staircase/core/arrays/docstrings.py` & `staircase-2.5.1/staircase/core/arrays/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/arrays/extension.py` & `staircase-2.5.1/staircase/core/arrays/extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 import numbers
 from collections.abc import Iterable
+from typing import Any, Callable, Type
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from pandas.api.extensions import (
     ExtensionArray,
     ExtensionDtype,
@@ -23,30 +26,30 @@
 class StairsDtype(ExtensionDtype):
 
     type = Stairs
     name = "Stairs"
     na_value = pd.NA
 
     @classmethod
-    def construct_from_string(cls, string):
+    def construct_from_string(cls, string: str) -> StairsDtype:
         if string == cls.name:
             return cls()
         else:
             raise TypeError("Cannot construct a '{}' from '{}'".format(cls, string))
 
     @classmethod
-    def construct_array_type(cls):
+    def construct_array_type(cls) -> Type[StairsArray]:
         return StairsArray
 
 
-def _isna(value):
+def _isna(value: pd.Series) -> pd.Series:
     return pd.isna(value)
 
 
-def _make_logical(func):
+def _make_logical(func: Callable) -> Callable:
     def logical_func(x, axis=0):
         return np.where(
             np.logical_or.reduce(np.isnan(x), axis=axis),
             np.nan,
             func.reduce(x, axis=axis),
         )
 
@@ -71,21 +74,21 @@
             self.data = np.array([data[k] for k in data.keys()])
         elif isinstance(data, Stairs) or is_list_like(data):
             self.data = np.array(data, ndmin=1)
         else:
             raise TypeError("'data' should be array of Stairs objects.")
 
     @property
-    def dtype(self):
+    def dtype(self) -> type:
         return self._dtype
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.data)
 
-    def __getitem__(self, idx):
+    def __getitem__(self, idx: int) -> Any:
         if isinstance(idx, numbers.Integral):
             return self.data[idx]
         elif isinstance(idx, (Iterable, slice)):
             return StairsArray(self.data[idx])
         else:
             raise TypeError("Index type not supported", idx)
 
@@ -181,15 +184,15 @@
                 index=index,
                 name="value",
             ).to_frame(),
             closed=self.data[0].closed,
         )._remove_redundant_step_points()
 
     @Appender(docstrings.make_docstring("array", "sample"), join="\n", indents=1)
-    def sample(self, x):
+    def sample(self, x) -> pd.Series:
         array = pd.Series(self.data)
         return array.apply(Stairs.sample, x=x, include_index=True)
 
     @Appender(docstrings.make_docstring("array", "limit"), join="\n", indents=1)
     def limit(self, x, side="right"):
         array = pd.Series(self.data)
         return array.apply(Stairs.limit, x=x, side=side, include_index=True)
@@ -230,15 +233,15 @@
     @Appender(docstrings.negate_docstring, join="\n", indents=1)
     def negate(self):
         return StairsArray(-self.data)
 
     __neg__ = negate
 
 
-def _make_binary_func(func_str):
+def _make_binary_func(func_str: str) -> Callable:
 
     stairs_func = getattr(Stairs, func_str)
     docstring = docstrings.make_binop_docstring(funcstr)
 
     @Appender(docstring, join="\n", indents=1)
     def func(self, other):
         if isinstance(other, (int, float, Stairs)):
@@ -281,15 +284,17 @@
         "rsubtract": "rsub",
         "rmultiply": "rmul",
         "rdivide": "rtruediv",
     }.get(funcstr, funcstr)
     setattr(StairsArray, f"__{magic}__", func)
 
 
-def _make_corr_cov_func(docstring, stairs_method, assume_ones_diagonal):
+def _make_corr_cov_func(
+    docstring: str, stairs_method: Callable, assume_ones_diagonal: int
+) -> Callable:
     @Appender(docstring, join="\n", indents=1)
     def func(self, where=(-inf, inf)):
         size = len(self.data)
         vals = np.ones(shape=(size, size))
         for i in range(size):
             for j in range(i + assume_ones_diagonal, size):
                 vals[i, j] = stairs_method(self.data[i], self.data[j], where=where)
```

### Comparing `staircase-2.5.0/staircase/core/layering.py` & `staircase-2.5.1/staircase/core/layering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
+
 import datetime
 import warnings
+from typing import Any
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import (
     is_datetime64_any_dtype,
     is_list_like,
     is_number,
@@ -19,15 +22,15 @@
 def _check_args_dtypes(*vectors):
     approved_dtypes_checks = [
         is_datetime64_any_dtype,
         is_timedelta64_dtype,
         is_numeric_dtype,
     ]
 
-    def _check_approved_dtype(vec):
+    def _check_approved_dtype(vec: pd.Series):
         approved = any(map(lambda func: func(vec), approved_dtypes_checks))
         if not approved:
             warnings.warn(
                 f"An argument supplied has dtype {vec.dtype}.  Only numerical, datetime-like, or timedelta dtypes have been tested.  Using other dtypes is considered experimental."
             )
 
     for vec in vectors:
@@ -55,15 +58,15 @@
                 f"An argument supplied for 'start' or 'end' has type '{type(arg)}'.  Only numerical, datetime-like, or timedelta types have been tested.  Using other types is considered experimental."
             )
 
     _check_approved_type(start, tuple(base_approved_types + [Inf]))
     _check_approved_type(end, tuple(base_approved_types + [NegInf]))
 
 
-def _convert_to_series(vec):
+def _convert_to_series(vec: Any) -> pd.Series:
     if not isinstance(vec, pd.Series):
         if vec is None or (isinstance(vec, (tuple, list)) and not len(vec)):
             vec = pd.Series(vec, dtype="float64")
         else:
             vec = pd.Series(vec)
     else:
         vec = vec.reset_index(drop=True)
```

### Comparing `staircase-2.5.0/staircase/core/ops/__init__.py` & `staircase-2.5.1/staircase/core/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/arithmetic.py` & `staircase-2.5.1/staircase/core/ops/arithmetic.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/common.py` & `staircase-2.5.1/staircase/core/ops/common.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/docstrings.py` & `staircase-2.5.1/staircase/core/ops/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/logical.py` & `staircase-2.5.1/staircase/core/ops/logical.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/masking.py` & `staircase-2.5.1/staircase/core/ops/masking.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/relational.py` & `staircase-2.5.1/staircase/core/ops/relational.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/ops/rops.py` & `staircase-2.5.1/staircase/core/ops/rops.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/sampling.py` & `staircase-2.5.1/staircase/core/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+from __future__ import annotations
+
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_list_like
 
+from staircase.core.stairs import Stairs
 from staircase.docstrings import examples
 from staircase.util import _is_datetime_like
 from staircase.util._decorators import Appender
 
 
 # capable of single or vector
 @Appender(examples.sample_example, join="\n", indents=1)
-def sample(self, x, include_index=False):
+def sample(
+    self: Stairs, x: int | float | np.array | pd.Series, include_index=False
+) -> pd.Series:
     """
     Evaluates the value of the step function at one, or more, points.
 
     The function can be called using parentheses.  See example below.
 
     Parameters
     ----------
@@ -38,15 +43,15 @@
         if not is_list_like(x):
             x = [x]
         values = pd.Series(values, index=x)
     return values
 
 
 @Appender(examples.limit_example, join="\n", indents=1)
-def limit(self, x, side, include_index=False):
+def limit(self: Stairs, x, side, include_index=False) -> pd.Series:
     """
     Evaluates the limit of the step function as it approaches one, or more, points.
 
     The results of this function should be considered as :math:`\\lim_{x \\to z^{-}} f(x)`
     or :math:`\\lim_{x \\to z^{+}} f(x)`, when side = 'left' or side = 'right' respectively. See
     :ref:`A note on interval endpoints<getting_started.interval_endpoints>` for an explanation.
```

### Comparing `staircase-2.5.0/staircase/core/slicing.py` & `staircase-2.5.1/staircase/core/slicing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,70 @@
+from __future__ import annotations
+
+from typing import Callable
+
 import numpy as np
 import pandas as pd
 from pandas.api.types import is_list_like
+from typing_extensions import Literal
 
 import staircase as sc
 from staircase.core.ops.masking import clip
 from staircase.core.stats.statistic import _get_stairs_method
 from staircase.docstrings import slicing as docstrings
 from staircase.util._decorators import Appender
 
 
 class StairsSlicer:
-    def __init__(self, stairs, interval_index):
+    def __init__(self, stairs: sc.Stairs, interval_index):
         self._stairs = stairs
         self._interval_index = interval_index
-        self._slices = None
+        self._slices: pd.Series | None = None
 
-    def _create_slices(self):
+    def _create_slices(self) -> None:
         slices = self._interval_index.map(lambda i: clip(self._stairs, i.left, i.right))
         self._slices = pd.Series(slices, index=self._interval_index)
 
-    def _ensure_slices(self):
+    def _ensure_slices(self) -> StairsSlicer:
         if self._slices is None:
             self._create_slices()
         return self
 
     @Appender(docstrings.agg_docstring, join="\n", indents=1)
-    def agg(self, funcs):
+    def agg(self, funcs) -> pd.DataFrame:
         if isinstance(funcs, str):
             funcs = [funcs]
         self._ensure_slices()
         df = pd.DataFrame(index=self._slices.index)
         for func in funcs:
             df[func] = getattr(self, func)()
         return df
 
     @Appender(docstrings.apply_docstring, join="\n", indents=1)
-    def apply(self, func, *args, **kwargs):
+    def apply(self, func: Callable, *args, **kwargs) -> pd.Series:
         self._ensure_slices()
         return self._slices.apply(func, args=args, **kwargs)
 
     @Appender(docstrings._docstrings["max"], join="\n", indents=1)
-    def max(self):
+    def max(self) -> float:
         result = self._max()
         if self._stairs._closed == "left" and self._interval_index.closed in (
             "right",
             "both",
         ):
             result = np.maximum(result, self._stairs(self._interval_index.right))
         elif self._stairs._closed == "right" and self._interval_index.closed in (
             "left",
             "both",
         ):
             result = np.maximum(result, self._stairs(self._interval_index.left))
         return result
 
     @Appender(docstrings._docstrings["min"], join="\n", indents=1)
-    def min(self):
+    def min(self) -> float:
         result = self._min()
         if self._stairs._closed == "left" and self._interval_index.closed in (
             "right",
             "both",
         ):
             result = np.minimum(result, self._stairs(self._interval_index.right))
         elif self._stairs._closed == "right" and self._interval_index.closed in (
@@ -68,21 +73,21 @@
         ):
             result = np.minimum(result, self._stairs(self._interval_index.left))
         return result
 
     @Appender(docstrings.hist_docstring, join="\n", indents=1)
     def hist(self, *args, **kwargs):
         self._ensure_slices()
-        zero = (  # hack to get 0 or pd.Timedelta(0)
+        zero = (
             self._stairs._data.index[0] - self._stairs._data.index[0]
-        )
+        )  # hack to get 0 or pd.Timedelta(0)
         return self._slices.apply(sc.Stairs.hist, *args, **kwargs).fillna(zero)
 
     @Appender(docstrings.resample_docstring, join="\n", indents=1)
-    def resample(self, func):
+    def resample(self, func: str):
         if not self._interval_index.is_non_overlapping_monotonic:
             raise ValueError(
                 "Slices must be monotonic increasing (ascending order) and not overlapping"
             )
         self._ensure_slices()
         new_values = getattr(self, func)()
         left_bound = self._slices.index.left.min()
@@ -92,15 +97,15 @@
             self._stairs.mask((left_bound, right_bound))
             .fillna(0)
             .mask(stairs_na)
             .layer(new_values.index.left, new_values.index.right, new_values.values)
         )
 
 
-def make_slice_method(method_name):
+def make_slice_method(method_name: str) -> Callable:
 
     func = _get_stairs_method(method_name)
     docstring = docstrings._docstrings.get(method_name, "")
 
     @Appender(docstring, join="\n", indents=1)
     def method(self):
         self._ensure_slices()
@@ -110,23 +115,26 @@
 
 
 for method_name in ["_max", "_min", "mean", "median", "integral", "mode"]:
     method = make_slice_method(method_name)
     setattr(StairsSlicer, method_name, method)
 
 
-def slice(self, cuts, closed="left"):
+def slice(
+    self: sc.Stairs, cuts, closed: Literal["left", "right", "both", "neither"] = "left"
+) -> StairsSlicer:
     """
     Slice the step function into pieces.
 
     A slice corresponding to an interval *(a,b)* will be equal to *self* everywhere
     in *(a,b)* and undefined elsewhere.
 
     Parameters
     ----------
+    self : Stairs : class
     cuts : sequence, :class:`pandas.IntervalIndex`, :class:`pandas.PeriodIndex`.
         Used to slice the step function.  If *cuts* is a sequence then it should comprised
         of monotonically increasing values from the step function domain.
     closed : {'left', 'right', 'both', 'neither'}
         Only relevant if *cuts* is not a :class:`pandas.IntervalIndex`, and indicates
         if the intervals derived from *cuts* should closed on the left-side, right-side, both or neither.
```

### Comparing `staircase-2.5.0/staircase/core/stairs.py` & `staircase-2.5.1/staircase/core/stairs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,68 +2,71 @@
 
 staircase
 ==============
 
 staircase is a MIT licensed library, written in pure-Python, for
 modelling step functions. See :ref:`Getting Started <getting_started>` for more information.
 """
+from __future__ import annotations
 
 import warnings
+from typing import Any, Callable
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import (
     is_datetime64_dtype,
     is_number,
     is_numeric_dtype,
     is_timedelta64_dtype,
 )
+from typing_extensions import Literal
 
 from staircase import docstrings
 from staircase.constants import inf
 from staircase.core import stats
 from staircase.core.accessor import CachedAccessor
 from staircase.core.layering import _check_args_dtypes
 from staircase.plotting.accessor import PlotAccessor
 from staircase.util import _replace_none_with_infs
 from staircase.util._decorators import Appender
 
 
-def _make_deltas_from_vals(init_val, vals):
+def _make_deltas_from_vals(init_val, vals: pd.DataFrame) -> pd.Series:
     if not np.isnan(vals).any():
         result = pd.Series(np.diff((np.append([init_val], vals.values))))
     else:
         temp = pd.Series(np.append([init_val], vals.values))
         result = pd.Series.add(
             temp[pd.notnull(temp)].diff(), temp[pd.isnull(temp)], fill_value=0
         )[1:]
     if np.isnan(init_val):
         result.iloc[0] = vals.iloc[0]
     result.index = vals.index
     return result
 
 
-def _make_vals_from_deltas(init_val, deltas):
+def _make_vals_from_deltas(init_val: float, deltas: pd.DataFrame):
     base = 0 if np.isnan(init_val) else init_val
     return deltas.cumsum() + base
 
 
 class Stairs:
 
     class_name = "Stairs"
 
     @Appender(docstrings.Stairs_docstring, join="\n", indents=2)
     def __init__(
         self,
-        frame=None,
-        start=None,
+        frame: pd.DataFrame | None = None,
+        start: int | None = None,
         end=None,
         value=None,
         initial_value=0,
-        closed="left",
+        closed: Literal["left", "right"] = "left",
     ):
         assert frame is None or isinstance(frame, pd.DataFrame)
         self._data = None
         self._valid_deltas = False
         self._valid_values = False
         self._masked = False
         self._closed = closed
@@ -74,24 +77,34 @@
             self.layer(start, end, value, frame)
 
     def _clear_cache(self):
         self.dist._reset()
         self._integral_and_mean = None
 
     @classmethod
-    def _new(cls, initial_value, data, closed="left"):
+    def _new(
+        cls,
+        initial_value: float,
+        data: pd.DataFrame,
+        closed: Literal["left", "right"] = "left",
+    ) -> Stairs:
         new_instance = cls(closed=closed)
         new_instance.initial_value = initial_value
         new_instance._data = data
         new_instance._valid_deltas = False if data is None else "delta" in data.columns
         new_instance._valid_values = False if data is None else "value" in data.columns
         return new_instance
 
     @classmethod
-    def from_values(cls, initial_value, values=None, closed="left"):
+    def from_values(
+        cls,
+        initial_value: float = 0,
+        values: pd.Series | None = None,
+        closed: Literal["left", "right"] = "left",
+    ) -> Stairs:
         """
         Construct :class:`Stairs` from :class:`pandas.Series`.
 
         Parameters
         ----------
         initial_value : float, default 0
             The value of the step function at negative infinity.
@@ -128,41 +141,41 @@
         new_instance = cls(closed=closed)
         new_instance.initial_value = initial_value
         new_instance._data = values.to_frame("value")
         new_instance._valid_deltas = False
         new_instance._valid_values = True
         return new_instance
 
-    def _has_na(self):
+    def _has_na(self) -> bool | np.array:
         return np.isnan(self._data.values).any() or np.isnan(self.initial_value)
 
-    def _create_values(self):
+    def _create_values(self) -> Stairs:
         assert self._valid_deltas
         self._data["value"] = _make_vals_from_deltas(
             self.initial_value, self._data["delta"]
         )
         self._valid_values = True
         return self
 
-    def _create_deltas(self):
+    def _create_deltas(self) -> Stairs:
         assert self._valid_values
         self._data["delta"] = _make_deltas_from_vals(
             self.initial_value, self._data["value"]
         )
         self._valid_deltas = True
         return self
 
-    def _get_deltas(self):
+    def _get_deltas(self) -> pd.Series:
         if self._data is None:
             return pd.Series(dtype="float64")
         if not self._valid_deltas:
             self._create_deltas()
         return self._data["delta"]
 
-    def _get_values(self):
+    def _get_values(self) -> pd.Series:
         if self._data is None:
             return pd.Series(dtype="float64")
         if not self._valid_values:
             self._create_values()
         return self._data["value"]
 
     @property
@@ -304,15 +317,15 @@
 
         Returns
         -------
         :class:`pandas.DataFrame`
         """
         return self.dist.hist(bins=bins, closed=closed, stat=stat)
 
-    def quantiles(self, q):
+    def quantiles(self, q: int):
         """
         Returns an array of q-quantiles.
 
         Quantiles are cut points which divide a distribution into continuous intervals with equal probabilities.
         The 2-quantile is more commonly known as the median.
         The 4-quantiles are more commonly known as quartiles.
         The 100-quantiles are more commonly known as percentiles.
@@ -344,15 +357,15 @@
 
         >>> sf.quantiles(4)
         array([2., 3., 4.])
         """
         return self.dist.quantiles(q)
 
     @Appender(stats.docstrings.simple_max_example, join="\n", indents=2)
-    def max(self):
+    def max(self) -> float:
         """
         The maximum of the step function.
 
         Returns
         -------
         float
             The maximum of the step function
@@ -360,15 +373,15 @@
         See Also
         --------
         Stairs.min, Stairs.values_in_range
         """
         return stats.max(self)
 
     @Appender(stats.docstrings.simple_min_example, join="\n", indents=2)
-    def min(self):
+    def min(self) -> float:
         """
         The minimum of the step function.
 
         Returns
         -------
         float
             The minimum of the step function
@@ -378,15 +391,15 @@
         Stairs.max, Stairs.values_in_range
         """
         return stats.min(self)
 
     plot = CachedAccessor("plot", PlotAccessor)
 
     @property
-    def step_changes(self):
+    def step_changes(self) -> pd.Series:
         """
         A pandas Series of key, value pairs of indicating where step changes occur in the step function, and the change in value
 
         Returns
         -------
         :class:`pandas.Series`
 
@@ -443,15 +456,15 @@
             4   -1
             5    0
             dtype: int64
         """
         return self._get_values().copy()
 
     @property
-    def step_points(self):
+    def step_points(self) -> np.array:
         """
         A numpy arrauy of domain values indicating where step changes occur in the step function.
 
         Returns
         -------
         :class:`numpy.ndarray`
 
@@ -473,15 +486,15 @@
         """
         if self._data is None:
             return np.array([])
         return self._data.index.values
 
     @Appender(docstrings.examples.number_of_steps_example, join="\n", indents=2)
     @property
-    def number_of_steps(self):
+    def number_of_steps(self) -> int:
         """
         Calculates the number of step changes
 
         Returns
         -------
         int
 
@@ -489,25 +502,25 @@
         --------
         Stairs.step_changes
         Stairs.step_values
         Stairs.step_points
         """
         return len(self.step_points)
 
-    def _remove_redundant_step_points(self):
+    def _remove_redundant_step_points(self) -> Stairs:
 
         # preferred over values method
-        def remove_via_deltas():
+        def remove_via_deltas() -> None:
             remove_index = (
                 self._data["delta"].isna() & self._data["delta"].isna().shift()
             ) | (self._data["delta"] == 0)
             self._data = self._data.loc[~remove_index]
 
         # do we just make deltas and then run above method?
-        def remove_via_values():
+        def remove_via_values() -> None:
             remove_index = (
                 self._data["value"].isna() & self._data["value"].isna().shift()
             ) | (self._data["value"] == self._data["value"].shift())
             if (self._data["value"].iloc[0] == self.initial_value) or (
                 pd.isnull(self._data.loc[:, "value"].iloc[0])
                 and pd.isnull(self.initial_value)
             ):
@@ -522,43 +535,48 @@
             else:
                 assert False, "no deltas or values valid!"
             if len(self._data) == 0:
                 self._data = None
 
         return self
 
-    def copy(self):
+    def copy(self) -> Stairs:
         """
         Returns a deep copy of this Stairs instance
 
         Returns
         -------
         :class:`Stairs`
         """
         new_instance = Stairs._new(
             initial_value=self.initial_value,
             data=self._data.copy() if self._data is not None else None,
             closed=self.closed,
         )
         return new_instance
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         """
         Return True if and only if step function has a value of 1 everywhere.
 
         Returns
         -------
         boolean
         """
         if self.initial_value == 1 and self.number_of_steps == 0:
             return True
         return False
 
     @Appender(docstrings.examples.describe_example, join="\n", indents=2)
-    def describe(self, where=(-inf, inf), percentiles=(25, 50, 75)):
+    def describe(
+        self,
+        where: tuple[float | int, float | int]
+        | list[float | int, float | int] = (-inf, inf),
+        percentiles: list[float | int] | tuple[float | int] = (25, 50, 75),
+    ) -> pd.Series:
         """
         Generate descriptive statistics for the step function values over a specified domain.
 
         Parameters
         ----------
         where : tuple or list of length two, optional
             Indicates the domain interval over which to evaluate the step function.
@@ -587,15 +605,15 @@
                 },
                 **{f"{perc}%": stairs.percentile(perc) for perc in percentiles},
                 **{"max": stairs.max},
             }
         )
 
     @Appender(docstrings.examples.shift_example, join="\n", indents=2)
-    def shift(self, delta):
+    def shift(self, delta: pd.Series | int | float) -> Stairs:
         """
         Returns a stairs instance corresponding to a horizontal translation by delta
 
         If delta is positive the corresponding step function is moved right.
         If delta is negative the corresponding step function is moved left.
 
         Parameters
@@ -617,15 +635,15 @@
         return Stairs._new(
             initial_value=self.initial_value,
             data=self._data.set_index(self._data.index + delta),
             closed=self.closed,
         )
 
     @Appender(docstrings.examples.diff_example, join="\n", indents=2)
-    def diff(self, delta):
+    def diff(self, delta: int | float | pd.Timedelta) -> Stairs:
         """
         Returns a stairs instance corresponding to the difference between the step function corresponding to *self*
         and the same step-function translated by delta.
 
         Parameters
         ----------
         delta : int, float or pandas.Timedelta
@@ -639,15 +657,19 @@
         See Also
         --------
         Stairs.shift
         """
         return self - self.shift(delta)
 
     @Appender(docstrings.examples.rolling_mean_example, join="\n", indents=2)
-    def rolling_mean(self, window=(0, 0), where=(-inf, inf)):
+    def rolling_mean(
+        self,
+        window: tuple[int | int] = (0, 0),
+        where: tuple[float | float] = (-inf, inf),
+    ) -> pd.Series:
         """
         Returns coordinates defining rolling mean
 
         The rolling mean of a step function is a continous piece-wise linear function, hence it can
         be described by a sequence of x,y coordinates which mark where function changes gradient.  These
         x,y coordinates are returned as a :class:`pandas.Series` which could then be used with
         :meth:`matplotlib.axes.Axes.plot`, or equivalent, to visualise.
@@ -695,15 +717,15 @@
         )
         if lower != -inf:
             s = s.loc[s.index >= lower - left_delta]
         if upper != inf:
             s = s.loc[s.index <= upper - right_delta]
         return s
 
-    def to_frame(self):
+    def to_frame(self) -> pd.DataFrame:
         """
         Returns a pandas.DataFrame with columns 'start', 'end' and 'value'
 
         The rows of the dataframe can be interpreted as the interval definitions
         which make up the step function.
 
         Returns
@@ -735,15 +757,15 @@
                 self._create_values()
             step_points = self._data.index
             starts = [-inf] + step_points.to_list()
             ends = step_points.to_list() + [inf]
             values = np.append(self.initial_value, self._data["value"].values)
         return pd.DataFrame({"start": starts, "end": ends, "value": values})
 
-    def pipe(self, func, *args, **kwargs):
+    def pipe(self, func: Callable, *args, **kwargs) -> Any:
         """
         Applies func and returns the result.
 
         Primarily intended to facilitate method chaining.
 
         Parameters
         ----------
@@ -757,31 +779,31 @@
         Returns
         -------
         object
             return type of *func*
         """
         return func(self, *args, **kwargs)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """
         Return str(self)
         """
         return f"<staircase.{self.class_name}, id={id(self)}>"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """
         Return string representation of Stairs
         """
         return str(self)
 
     def __call__(self, *args, **kwargs):
         return self.sample(*args, **kwargs)
 
 
-def _add_operations():
+def _add_operations() -> None:
     from staircase.core import layering, ops, sampling, slicing
 
     ops.add_operations(Stairs)
     stats.add_methods(Stairs)
     sampling.add_methods(Stairs)
     layering.add_methods(Stairs)
     slicing.add_methods(Stairs)
```

### Comparing `staircase-2.5.0/staircase/core/stats/__init__.py` & `staircase-2.5.1/staircase/core/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/stats/distribution.py` & `staircase-2.5.1/staircase/core/stats/distribution.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/stats/docstrings.py` & `staircase-2.5.1/staircase/core/stats/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/core/stats/statistic.py` & `staircase-2.5.1/staircase/core/stats/statistic.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/docstrings/__init__.py` & `staircase-2.5.1/staircase/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/docstrings/examples.py` & `staircase-2.5.1/staircase/docstrings/examples.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/docstrings/slicing.py` & `staircase-2.5.1/staircase/docstrings/slicing.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/plotting/accessor.py` & `staircase-2.5.1/staircase/plotting/accessor.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/plotting/docstrings.py` & `staircase-2.5.1/staircase/plotting/docstrings.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/plotting/matplotlib.py` & `staircase-2.5.1/staircase/plotting/matplotlib.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/test_data.py` & `staircase-2.5.1/staircase/test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+from __future__ import annotations
+
+from typing import Optional
+
 import numpy as np
 import pandas as pd
 
 
-def make_test_data(dates=True, positive_only=True, groups=(), seed=None):
+def make_test_data(
+    dates: bool = True,
+    positive_only: bool = True,
+    groups: tuple[Optional[str]] | list[Optional[str]] = (),
+    seed: int | None = None,
+) -> pd.DataFrame:
     """
     Creates interval data for use with staircase.
 
     The result will be a :class:`pandas.DataFrame` with columns "start", "end", "value", and optionally "group".
 
     Parameters
     ----------
@@ -73,15 +82,17 @@
         rs = np.random.RandomState(seed)
         return rs.randint, rs.uniform
 
     rng = np.random.default_rng(seed)
     return rng.integers, rng.random
 
 
-def _make_test_data(dates=True, positive_only=True, seed=None):
+def _make_test_data(
+    dates: bool = True, positive_only: bool = True, seed: str | bool | None = None
+) -> pd.DataFrame:
 
     random_integers, random_floats = _get_random_functions(seed)
 
     n_intervals = random_integers(100, 1000)
     smallest_interval = random_integers(1, 6)
     largest_interval = random_integers(15, 20)
     interval_lengths = (
```

### Comparing `staircase-2.5.0/staircase/util/__init__.py` & `staircase-2.5.1/staircase/util/__init__.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/staircase/util/_decorators.py` & `staircase-2.5.1/staircase/util/_decorators.py`

 * *Files identical despite different names*

### Comparing `staircase-2.5.0/setup.py` & `staircase-2.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,188 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: staircase
+Version: 2.5.1
+Summary: A data analysis package based on modelling and manipulation of mathematical step functions. Strongly aligned with pandas.
+Home-page: https://staircase.dev
+License: MIT
+Keywords: Staircase,Step Functions,Mathematics,Data Analysis,Analysis,Data Structures,Time Signal,Simulation Output
+Author: Riley Clement
+Author-email: venaturum@gmail.com
+Maintainer: Riley Clement
+Maintainer-email: venaturum@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Provides-Extra: codecov
+Requires-Dist: matplotlib (>=2)
+Requires-Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: numpy (>=1.21.2,<2.0.0) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: pandas (>=1,<2) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: pandas (>=1.3.4,<3) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: pytz
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Bug Tracker, https://github.com/staircase-dev/staircase/issues
+Project-URL: Documentation, https://staircase.dev
+Project-URL: Repository, https://github.com/staircase-dev/staircase
+Description-Content-Type: text/markdown
+
+<p align="center"><a href="https://github.com/staircase-dev/staircase"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/staircase2.png?raw=true" title="staircase logo" alt="staircase logo"></a></p>
+
+
+<p align="center">
+	<a href="https://pepy.tech/project/staircase/" alt="PyPI downloads">
+        <img src="https://pepy.tech/badge/staircase" /></a>
+    <a href="https://www.python.org/" alt="Python version">
+        <img src="https://img.shields.io/pypi/pyversions/staircase" /></a>
+    <a href="https://pypi.org/project/staircase/" alt="PyPI version">
+        <img src="https://img.shields.io/pypi/v/staircase" /></a>
+    <a href="https://anaconda.org/conda-forge/staircase" alt="Conda Forge version">
+        <img src="https://anaconda.org/conda-forge/staircase/badges/version.svg?branch=master&kill_cache=1" /></a>
+    <a href="https://github.com/staircase-dev/staircase/blob/master/LICENSE" alt="License">
+        <img src="http://img.shields.io/:license-mit-blue.svg?style=flat-square"></a>
+</p>
+<p align="center">
+	<a href="https://github.com/staircase-dev/staircase/actions/workflows/ci.yml" alt"Github CI">
+		<img src="https://github.com/staircase-dev/staircase/actions/workflows/ci.yml/badge.svg"/></a>
+    <a href="https://www.staircase.dev/en/latest/" alt="Documentation">
+        <img src="https://readthedocs.org/projects/railing/badge/?version=latest" /></a>
+	<a href="https://app.codacy.com/gh/staircase-dev/staircase/dashboard" alt="Codacy Grade">
+        <img src="https://app.codacy.com/project/badge/Grade/845ecfb2fd6748cc87a66f9a97cd9492" /></a>	
+	<a href="https://app.codecov.io/gh/staircase-dev/staircase"  alt="Codecov coverage">
+		<img src="https://codecov.io/gh/staircase-dev/staircase/branch/master/graph/badge.svg"/></a>
+</p>
+
+The staircase package enables data analysis through mathematical step functions. Step functions can be used to represent continuous time series - think changes in state over time, queue size over time, utilisation over time, success rates over time etc.
+
+The package is built upon `numpy` and `pandas`, with a deliberate, stylistic alignment to the latter in order to integrate seamlessly into the [pandas ecosystem](https://pandas.pydata.org/docs/ecosystem.html).
+
+The staircase package makes converting raw, temporal data into time series easy and readable. Furthermore there is a rich variety of [arithmetic operations](https://www.staircase.dev/en/latest/reference/Stairs.html#arithmetic-operators), [relational operations](https://www.staircase.dev/en/latest/reference/Stairs.html#relational-operators), [logical operations](https://www.staircase.dev/en/latest/reference/Stairs.html#logical-operators), [statistical operations](https://www.staircase.dev/en/latest/reference/Stairs.html#statistical-operators), to enable analysis, in addition to functions for [univariate analysis](https://www.staircase.dev/en/latest/reference/Stairs.html#summary-statistics), [aggregations](https://www.staircase.dev/en/latest/reference/arrays.html#aggregation) and compatibility with datetimes.
+
+**New in 2022:** staircase now provides support for [pandas extension arrays](https://pandas.pydata.org/docs/ecosystem.html#extension-data-types) and a [Series accessor](https://www.staircase.dev/en/latest/user_guide/arraymethods.html).
+
+
+## An example
+
+In this example, we consider data corresponding to site views for a website in October 2021.  The start and end times have been logged for each session, in addition to one of three countries codes (AU, UK, US).  These times are recorded with `pandas.Timestamp` and any time which falls outside of October is logged as `NAT`.
+
+
+```python
+>>> data
+                       start                   end   country
+0                        NaT   2021-10-01 00:00:50        AU
+1                        NaT   2021-10-01 00:07:45        AU
+2                        NaT   2021-10-01 00:05:58        AU
+3                        NaT   2021-10-01 00:08:48        AU
+4                        NaT   2021-10-01 00:05:26        AU
+...                      ...                   ...       ...
+425728   2021-10-31 23:57:16                   NaT        US
+425729   2021-10-31 23:57:25                   NaT        US
+425730   2021-10-31 23:58:59                   NaT        US
+425731   2021-10-31 23:59:45                   NaT        US
+425732   2021-10-31 23:59:59                   NaT        US
+```
+
+Note that the number of users viewing the site over time can be modelled as a step function.  The value of the function increases by 1 every time a user arrives at the site, and decreases by 1 every time a user leaves the site.  This step function can be thought of as the sum of three step functions: AU users + UK users + US users.  Creating a step function for AU users, for example, is simple.  To achieve it we use the *[Stairs](https://www.staircase.dev/en/latest/reference/Stairs.html)* class, which represents a step function:
+
+
+```python
+>>> import staircase as sc
+
+>>> views_AU = sc.Stairs(data.query("country == 'AU'"), "start", "end")
+>>> views_AU
+<staircase.Stairs, id=1609972469384>
+```
+
+We can visualise the function with the plot function:
+```python
+>>> views_AU.plot()
+```
+
+<p align="left"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/AU_views.png?raw=true" title="AU views example" alt="AU views example"></p>
+
+Rather than creating a separate variable for each country, we can create a `pandas.Series` to hold a step function for each country.  We can even give this Series a "Stairs" type.
+
+```python
+>>> october = (pd.Timestamp("2021-10"), pd.Timestamp("2021-11"))
+>>> series_stepfunctions = (
+...     data.groupby("country")
+...     .apply(sc.Stairs, "start", "end")
+...     .apply(sc.Stairs.clip, october)  # set step functions to be undefined outside of October
+...     .astype("Stairs")
+... )
+>>> series_stepfunctions
+country
+AU    <staircase.Stairs, id=2516367680328>
+UK    <staircase.Stairs, id=2516362550664>
+US    <staircase.Stairs, id=2516363585928>
+dtype: Stairs
+```
+
+The plotting backend to `staircase` is provided by `matplotlib`.
+
+```python
+>>> import matplotlib.pyplot as plt
+>>> _, ax = plt.subplots(figsize=(15,4))
+>>> series_stepfunctions.sc.plot(ax, alpha=0.7)
+>>> ax.legend()
+```
+<p align="left"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/all_views.png?raw=true" title="all views example" alt="all views example"></p>
+
+Now plotting step functions is useful, but the real fun starts when we go beyond this:
+
+<p align="left"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/staircase_analysis.gif?raw=true" title="staircase analysis examples" alt="staircase analysis examples"></p>
+
+
+## Installation
+
+staircase can be installed from PyPI:
+
+```bash
+python -m pip install staircase
+```
+
+or also with conda:
+
+```bash
+conda install -c conda-forge staircase
+```
+
+## Documentation
+The complete guide to using staircase can be found at [staircase.dev](https://www.staircase.dev)
+
+## Contributing
+There are many ways in which contributions can be made - the first and foremost being *using staircase and giving feedback*.
+
+Bug reports, feature requests and ideas can be submitted via the [Github issue tracker](https://github.com/staircase-dev/staircase/issues).
+
+Additionally, bug fixes. enhancements, and improvements to the code and documentation are also appreciated and can be done via pull requests.
+Take a look at the current issues and if there is one you would like to work on please leave a comment to that effect.
+
+See this [beginner's guide to contributing](https://github.com/firstcontributions/first-contributions), or [Pandas' guide to contributing](https://pandas.pydata.org/pandas-docs/stable/development/contributing.html), to learn more about the process.
+
+
+## Versioning
+
+We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/staircase-dev/staircase/tags).  It is highly recommended to use staircase 2.*, for both performance and additional features.
 
-packages = \
-['staircase',
- 'staircase.core',
- 'staircase.core.arrays',
- 'staircase.core.exceptions',
- 'staircase.core.ops',
- 'staircase.core.stats',
- 'staircase.docstrings',
- 'staircase.io',
- 'staircase.plotting',
- 'staircase.util']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['matplotlib>=2', 'pytz']
-
-extras_require = \
-{':python_version >= "3.10" and python_version < "4.0"': ['pandas>=1.3.4,<2.0.0',
-                                                          'numpy>=1.21.2,<2.0.0'],
- ':python_version >= "3.7" and python_version < "3.10"': ['pandas>=1,<2',
-                                                          'numpy>=1.15,<2.0']}
-
-setup_kwargs = {
-    'name': 'staircase',
-    'version': '2.5.0',
-    'description': 'A data analysis package based on modelling and manipulation of mathematical step functions. Strongly aligned with pandas.',
-    'long_description': '<p align="center"><a href="https://github.com/staircase-dev/staircase"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/staircase2.png?raw=true" title="staircase logo" alt="staircase logo"></a></p>\n\n\n<p align="center">\n\t<a href="https://pepy.tech/project/staircase/" alt="PyPI downloads">\n        <img src="https://pepy.tech/badge/staircase" /></a>\n    <a href="https://www.python.org/" alt="Python version">\n        <img src="https://img.shields.io/pypi/pyversions/staircase" /></a>\n    <a href="https://pypi.org/project/staircase/" alt="PyPI version">\n        <img src="https://img.shields.io/pypi/v/staircase" /></a>\n    <a href="https://anaconda.org/conda-forge/staircase" alt="Conda Forge version">\n        <img src="https://anaconda.org/conda-forge/staircase/badges/version.svg?branch=master&kill_cache=1" /></a>\n    <a href="https://github.com/staircase-dev/staircase/blob/master/LICENSE" alt="License">\n        <img src="http://img.shields.io/:license-mit-blue.svg?style=flat-square"></a>\n</p>\n<p align="center">\n\t<a href="https://github.com/staircase-dev/staircase/actions/workflows/ci.yml" alt"Github CI">\n\t\t<img src="https://github.com/staircase-dev/staircase/actions/workflows/ci.yml/badge.svg"/></a>\n    <a href="https://www.staircase.dev/en/latest/" alt="Documentation">\n        <img src="https://readthedocs.org/projects/railing/badge/?version=latest" /></a>\n\t<a href="https://app.codacy.com/gh/staircase-dev/staircase/dashboard" alt="Codacy Grade">\n        <img src="https://app.codacy.com/project/badge/Grade/845ecfb2fd6748cc87a66f9a97cd9492" /></a>\t\n\t<a href="https://app.codecov.io/gh/staircase-dev/staircase"  alt="Codecov coverage">\n\t\t<img src="https://codecov.io/gh/staircase-dev/staircase/branch/master/graph/badge.svg"/></a>\n</p>\n\nThe staircase package enables data analysis through mathematical step functions. Step functions can be used to represent continuous time series - think changes in state over time, queue size over time, utilisation over time, success rates over time etc.\n\nThe package is built upon `numpy` and `pandas`, with a deliberate, stylistic alignment to the latter in order to integrate seamlessly into the [pandas ecosystem](https://pandas.pydata.org/docs/ecosystem.html).\n\nThe staircase package makes converting raw, temporal data into time series easy and readable. Furthermore there is a rich variety of [arithmetic operations](https://www.staircase.dev/en/latest/reference/Stairs.html#arithmetic-operators), [relational operations](https://www.staircase.dev/en/latest/reference/Stairs.html#relational-operators), [logical operations](https://www.staircase.dev/en/latest/reference/Stairs.html#logical-operators), [statistical operations](https://www.staircase.dev/en/latest/reference/Stairs.html#statistical-operators), to enable analysis, in addition to functions for [univariate analysis](https://www.staircase.dev/en/latest/reference/Stairs.html#summary-statistics), [aggregations](https://www.staircase.dev/en/latest/reference/arrays.html#aggregation) and compatibility with datetimes.\n\n**New in 2022:** staircase now provides support for [pandas extension arrays](https://pandas.pydata.org/docs/ecosystem.html#extension-data-types) and a [Series accessor](https://www.staircase.dev/en/latest/user_guide/arraymethods.html).\n\n\n## An example\n\nIn this example, we consider data corresponding to site views for a website in October 2021.  The start and end times have been logged for each session, in addition to one of three countries codes (AU, UK, US).  These times are recorded with `pandas.Timestamp` and any time which falls outside of October is logged as `NAT`.\n\n\n```python\n>>> data\n                       start                   end   country\n0                        NaT   2021-10-01 00:00:50        AU\n1                        NaT   2021-10-01 00:07:45        AU\n2                        NaT   2021-10-01 00:05:58        AU\n3                        NaT   2021-10-01 00:08:48        AU\n4                        NaT   2021-10-01 00:05:26        AU\n...                      ...                   ...       ...\n425728   2021-10-31 23:57:16                   NaT        US\n425729   2021-10-31 23:57:25                   NaT        US\n425730   2021-10-31 23:58:59                   NaT        US\n425731   2021-10-31 23:59:45                   NaT        US\n425732   2021-10-31 23:59:59                   NaT        US\n```\n\nNote that the number of users viewing the site over time can be modelled as a step function.  The value of the function increases by 1 every time a user arrives at the site, and decreases by 1 every time a user leaves the site.  This step function can be thought of as the sum of three step functions: AU users + UK users + US users.  Creating a step function for AU users, for example, is simple.  To achieve it we use the *[Stairs](https://www.staircase.dev/en/latest/reference/Stairs.html)* class, which represents a step function:\n\n\n```python\n>>> import staircase as sc\n\n>>> views_AU = sc.Stairs(data.query("country == \'AU\'"), "start", "end")\n>>> views_AU\n<staircase.Stairs, id=1609972469384>\n```\n\nWe can visualise the function with the plot function:\n```python\n>>> views_AU.plot()\n```\n\n<p align="left"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/AU_views.png?raw=true" title="AU views example" alt="AU views example"></p>\n\nRather than creating a separate variable for each country, we can create a `pandas.Series` to hold a step function for each country.  We can even give this Series a "Stairs" type.\n\n```python\n>>> october = (pd.Timestamp("2021-10"), pd.Timestamp("2021-11"))\n>>> series_stepfunctions = (\n...     data.groupby("country")\n...     .apply(sc.Stairs, "start", "end")\n...     .apply(sc.Stairs.clip, october)  # set step functions to be undefined outside of October\n...     .astype("Stairs")\n... )\n>>> series_stepfunctions\ncountry\nAU    <staircase.Stairs, id=2516367680328>\nUK    <staircase.Stairs, id=2516362550664>\nUS    <staircase.Stairs, id=2516363585928>\ndtype: Stairs\n```\n\nThe plotting backend to `staircase` is provided by `matplotlib`.\n\n```python\n>>> import matplotlib.pyplot as plt\n>>> _, ax = plt.subplots(figsize=(15,4))\n>>> series_stepfunctions.sc.plot(ax, alpha=0.7)\n>>> ax.legend()\n```\n<p align="left"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/all_views.png?raw=true" title="all views example" alt="all views example"></p>\n\nNow plotting step functions is useful, but the real fun starts when we go beyond this:\n\n<p align="left"><img src="https://github.com/staircase-dev/staircase/blob/master/docs/img/staircase_analysis.gif?raw=true" title="staircase analysis examples" alt="staircase analysis examples"></p>\n\n\n## Installation\n\nstaircase can be installed from PyPI:\n\n```bash\npython -m pip install staircase\n```\n\nor also with conda:\n\n```bash\nconda install -c conda-forge staircase\n```\n\n## Documentation\nThe complete guide to using staircase can be found at [staircase.dev](https://www.staircase.dev)\n\n## Contributing\nThere are many ways in which contributions can be made - the first and foremost being *using staircase and giving feedback*.\n\nBug reports, feature requests and ideas can be submitted via the [Github issue tracker](https://github.com/staircase-dev/staircase/issues).\n\nAdditionally, bug fixes. enhancements, and improvements to the code and documentation are also appreciated and can be done via pull requests.\nTake a look at the current issues and if there is one you would like to work on please leave a comment to that effect.\n\nSee this [beginner\'s guide to contributing](https://github.com/firstcontributions/first-contributions), or [Pandas\' guide to contributing](https://pandas.pydata.org/pandas-docs/stable/development/contributing.html), to learn more about the process.\n\n\n## Versioning\n\nWe use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/staircase-dev/staircase/tags).  It is highly recommended to use staircase 2.*, for both performance and additional features.\n\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](https://github.com/staircase-dev/staircase/blob/master/LICENSE) file for details\n\n## Acknowledgments\n\nThe seeds of *staircase* began developing at the Hunter Valley Coal Chain Coordinator, where it finds strong application in analysing simulated data.  Thanks for the support!\n',
-    'author': 'Riley Clement',
-    'author_email': 'venaturum@gmail.com',
-    'maintainer': 'Riley Clement',
-    'maintainer_email': 'venaturum@gmail.com',
-    'url': 'https://staircase.dev',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
 
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/staircase-dev/staircase/blob/master/LICENSE) file for details
+
+## Acknowledgments
+
+The seeds of *staircase* began developing at the Hunter Valley Coal Chain Coordinator, where it finds strong application in analysing simulated data.  Thanks for the support!
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,114 +1,117 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['staircase',
-'staircase.core', 'staircase.core.arrays', 'staircase.core.exceptions',
-'staircase.core.ops', 'staircase.core.stats', 'staircase.docstrings',
-'staircase.io', 'staircase.plotting', 'staircase.util'] package_data = \ {'':
-['*']} install_requires = \ ['matplotlib>=2', 'pytz'] extras_require = \ {':
-python_version >= "3.10" and python_version < "4.0"': ['pandas>=1.3.4,<2.0.0',
-'numpy>=1.21.2,<2.0.0'], ':python_version >= "3.7" and python_version <
-"3.10"': ['pandas>=1,<2', 'numpy>=1.15,<2.0']} setup_kwargs = { 'name':
-'staircase', 'version': '2.5.0', 'description': 'A data analysis package based
-on modelling and manipulation of mathematical step functions. Strongly aligned
-with pandas.', 'long_description': '
+Metadata-Version: 2.1 Name: staircase Version: 2.5.1 Summary: A data analysis
+package based on modelling and manipulation of mathematical step functions.
+Strongly aligned with pandas. Home-page: https://staircase.dev License: MIT
+Keywords: Staircase,Step Functions,Mathematics,Data Analysis,Analysis,Data
+Structures,Time Signal,Simulation Output Author: Riley Clement Author-email:
+venaturum@gmail.com Maintainer: Riley Clement Maintainer-email:
+venaturum@gmail.com Requires-Python: >=3.7,<4.0 Classifier: Intended Audience
+:: Science/Research Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Topic :: Scientific/Engineering Provides-Extra: codecov Requires-Dist:
+matplotlib (>=2) Requires-Dist: numpy (>=1.15,<2.0) ; python_version >= "3.7"
+and python_version < "3.10" Requires-Dist: numpy (>=1.21.2,<2.0.0) ;
+python_version >= "3.10" and python_version < "4.0" Requires-Dist: pandas
+(>=1,<2) ; python_version >= "3.7" and python_version < "3.10" Requires-Dist:
+pandas (>=1.3.4,<3) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: pytz Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) Project-
+URL: Bug Tracker, https://github.com/staircase-dev/staircase/issues Project-
+URL: Documentation, https://staircase.dev Project-URL: Repository, https://
+github.com/staircase-dev/staircase Description-Content-Type: text/markdown
                                [staircase_logo]
-\n\n\n
- \n\t\n_[https://pepy.tech/badge/staircase]\n \n_[https://img.shields.io/pypi/
-  pyversions/staircase]\n \n_[https://img.shields.io/pypi/v/staircase]\n \n_
-              [https://anaconda.org/conda-forge/staircase/badges/
- version.svg?branch=master&kill_cache=1]\n \n_[http://img.shields.io/:license-
-                       mit-blue.svg?style=flat-square]\n
-\n
-   \n\tGithub CI">\n\t\t[https://github.com/staircase-dev/staircase/actions/
-                          workflows/ci.yml/badge.svg]
-\n \n_[https://readthedocs.org/projects/railing/badge/?version=latest]\n\t\n_
-[https://app.codacy.com/project/badge/Grade/
-845ecfb2fd6748cc87a66f9a97cd9492]\t\n\t\n\t\t[https://codecov.io/gh/staircase-
-dev/staircase/branch/master/graph/badge.svg]\n
-\n\nThe staircase package enables data analysis through mathematical step
+ [https://pepy.tech/badge/staircase] [https://img.shields.io/pypi/pyversions/
+  staircase] [https://img.shields.io/pypi/v/staircase] [https://anaconda.org/
+ conda-forge/staircase/badges/version.svg?branch=master&kill_cache=1] [http://
+            img.shields.io/:license-mit-blue.svg?style=flat-square]
+  Github CI"> [https://github.com/staircase-dev/staircase/actions/workflows/
+                               ci.yml/badge.svg]
+ [https://readthedocs.org/projects/railing/badge/?version=latest] [https://
+app.codacy.com/project/badge/Grade/845ecfb2fd6748cc87a66f9a97cd9492]
+ [https://codecov.io/gh/staircase-dev/staircase/branch/master/graph/badge.svg]
+The staircase package enables data analysis through mathematical step
 functions. Step functions can be used to represent continuous time series -
 think changes in state over time, queue size over time, utilisation over time,
-success rates over time etc.\n\nThe package is built upon `numpy` and `pandas`,
+success rates over time etc. The package is built upon `numpy` and `pandas`,
 with a deliberate, stylistic alignment to the latter in order to integrate
 seamlessly into the [pandas ecosystem](https://pandas.pydata.org/docs/
-ecosystem.html).\n\nThe staircase package makes converting raw, temporal data
-into time series easy and readable. Furthermore there is a rich variety of
+ecosystem.html). The staircase package makes converting raw, temporal data into
+time series easy and readable. Furthermore there is a rich variety of
 [arithmetic operations](https://www.staircase.dev/en/latest/reference/
 Stairs.html#arithmetic-operators), [relational operations](https://
 www.staircase.dev/en/latest/reference/Stairs.html#relational-operators),
 [logical operations](https://www.staircase.dev/en/latest/reference/
 Stairs.html#logical-operators), [statistical operations](https://
 www.staircase.dev/en/latest/reference/Stairs.html#statistical-operators), to
 enable analysis, in addition to functions for [univariate analysis](https://
 www.staircase.dev/en/latest/reference/Stairs.html#summary-statistics),
 [aggregations](https://www.staircase.dev/en/latest/reference/
-arrays.html#aggregation) and compatibility with datetimes.\n\n**New in 2022:**
+arrays.html#aggregation) and compatibility with datetimes. **New in 2022:**
 staircase now provides support for [pandas extension arrays](https://
 pandas.pydata.org/docs/ecosystem.html#extension-data-types) and a [Series
-accessor](https://www.staircase.dev/en/latest/user_guide/
-arraymethods.html).\n\n\n## An example\n\nIn this example, we consider data
-corresponding to site views for a website in October 2021. The start and end
-times have been logged for each session, in addition to one of three countries
-codes (AU, UK, US). These times are recorded with `pandas.Timestamp` and any
-time which falls outside of October is logged as `NAT`.\n\n\n```python\n>>>
-data\n start end country\n0 NaT 2021-10-01 00:00:50 AU\n1 NaT 2021-10-01 00:07:
-45 AU\n2 NaT 2021-10-01 00:05:58 AU\n3 NaT 2021-10-01 00:08:48 AU\n4 NaT 2021-
-10-01 00:05:26 AU\n... ... ... ...\n425728 2021-10-31 23:57:16 NaT US\n425729
-2021-10-31 23:57:25 NaT US\n425730 2021-10-31 23:58:59 NaT US\n425731 2021-10-
-31 23:59:45 NaT US\n425732 2021-10-31 23:59:59 NaT US\n```\n\nNote that the
-number of users viewing the site over time can be modelled as a step function.
-The value of the function increases by 1 every time a user arrives at the site,
-and decreases by 1 every time a user leaves the site. This step function can be
-thought of as the sum of three step functions: AU users + UK users + US users.
-Creating a step function for AU users, for example, is simple. To achieve it we
-use the *[Stairs](https://www.staircase.dev/en/latest/reference/Stairs.html)*
-class, which represents a step function:\n\n\n```python\n>>> import staircase
-as sc\n\n>>> views_AU = sc.Stairs(data.query("country == \'AU\'"), "start",
-"end")\n>>> views_AU\n
-Stairs, id=1609972469384>\n```\n\nWe can visualise the function with the plot
-function:\n```python\n>>> views_AU.plot()\n```\n\n
+accessor](https://www.staircase.dev/en/latest/user_guide/arraymethods.html). ##
+An example In this example, we consider data corresponding to site views for a
+website in October 2021. The start and end times have been logged for each
+session, in addition to one of three countries codes (AU, UK, US). These times
+are recorded with `pandas.Timestamp` and any time which falls outside of
+October is logged as `NAT`. ```python >>> data start end country 0 NaT 2021-10-
+01 00:00:50 AU 1 NaT 2021-10-01 00:07:45 AU 2 NaT 2021-10-01 00:05:58 AU 3 NaT
+2021-10-01 00:08:48 AU 4 NaT 2021-10-01 00:05:26 AU ... ... ... ... 425728
+2021-10-31 23:57:16 NaT US 425729 2021-10-31 23:57:25 NaT US 425730 2021-10-31
+23:58:59 NaT US 425731 2021-10-31 23:59:45 NaT US 425732 2021-10-31 23:59:59
+NaT US ``` Note that the number of users viewing the site over time can be
+modelled as a step function. The value of the function increases by 1 every
+time a user arrives at the site, and decreases by 1 every time a user leaves
+the site. This step function can be thought of as the sum of three step
+functions: AU users + UK users + US users. Creating a step function for AU
+users, for example, is simple. To achieve it we use the *[Stairs](https://
+www.staircase.dev/en/latest/reference/Stairs.html)* class, which represents a
+step function: ```python >>> import staircase as sc >>> views_AU = sc.Stairs
+(data.query("country == 'AU'"), "start", "end") >>> views_AU
+Stairs, id=1609972469384> ``` We can visualise the function with the plot
+function: ```python >>> views_AU.plot() ```
 [AU views example]
-\n\nRather than creating a separate variable for each country, we can create a
+Rather than creating a separate variable for each country, we can create a
 `pandas.Series` to hold a step function for each country. We can even give this
-Series a "Stairs" type.\n\n```python\n>>> october = (pd.Timestamp("2021-10"),
-pd.Timestamp("2021-11"))\n>>> series_stepfunctions = (\n... data.groupby
-("country")\n... .apply(sc.Stairs, "start", "end")\n... .apply(sc.Stairs.clip,
-october) # set step functions to be undefined outside of October\n... .astype
-("Stairs")\n... )\n>>> series_stepfunctions\ncountry\nAU
-Stairs, id=2516367680328>\nUK
-Stairs, id=2516362550664>\nUS
-Stairs, id=2516363585928>\ndtype: Stairs\n```\n\nThe plotting backend to
-`staircase` is provided by `matplotlib`.\n\n```python\n>>> import
-matplotlib.pyplot as plt\n>>> _, ax = plt.subplots(figsize=(15,4))\n>>>
-series_stepfunctions.sc.plot(ax, alpha=0.7)\n>>> ax.legend()\n```\n
+Series a "Stairs" type. ```python >>> october = (pd.Timestamp("2021-10"),
+pd.Timestamp("2021-11")) >>> series_stepfunctions = ( ... data.groupby
+("country") ... .apply(sc.Stairs, "start", "end") ... .apply(sc.Stairs.clip,
+october) # set step functions to be undefined outside of October ... .astype
+("Stairs") ... ) >>> series_stepfunctions country AU
+Stairs, id=2516367680328> UK
+Stairs, id=2516362550664> US
+Stairs, id=2516363585928> dtype: Stairs ``` The plotting backend to `staircase`
+is provided by `matplotlib`. ```python >>> import matplotlib.pyplot as plt >>>
+_, ax = plt.subplots(figsize=(15,4)) >>> series_stepfunctions.sc.plot(ax,
+alpha=0.7) >>> ax.legend() ```
 [all views example]
-\n\nNow plotting step functions is useful, but the real fun starts when we go
-beyond this:\n\n
+Now plotting step functions is useful, but the real fun starts when we go
+beyond this:
 [staircase analysis examples]
-\n\n\n## Installation\n\nstaircase can be installed from PyPI:
-\n\n```bash\npython -m pip install staircase\n```\n\nor also with conda:
-\n\n```bash\nconda install -c conda-forge staircase\n```\n\n##
-Documentation\nThe complete guide to using staircase can be found at
-[staircase.dev](https://www.staircase.dev)\n\n## Contributing\nThere are many
-ways in which contributions can be made - the first and foremost being *using
-staircase and giving feedback*.\n\nBug reports, feature requests and ideas can
-be submitted via the [Github issue tracker](https://github.com/staircase-dev/
-staircase/issues).\n\nAdditionally, bug fixes. enhancements, and improvements
+## Installation staircase can be installed from PyPI: ```bash python -m pip
+install staircase ``` or also with conda: ```bash conda install -c conda-forge
+staircase ``` ## Documentation The complete guide to using staircase can be
+found at [staircase.dev](https://www.staircase.dev) ## Contributing There are
+many ways in which contributions can be made - the first and foremost being
+*using staircase and giving feedback*. Bug reports, feature requests and ideas
+can be submitted via the [Github issue tracker](https://github.com/staircase-
+dev/staircase/issues). Additionally, bug fixes. enhancements, and improvements
 to the code and documentation are also appreciated and can be done via pull
-requests.\nTake a look at the current issues and if there is one you would like
-to work on please leave a comment to that effect.\n\nSee this [beginner\'s
-guide to contributing](https://github.com/firstcontributions/first-
-contributions), or [Pandas\' guide to contributing](https://pandas.pydata.org/
-pandas-docs/stable/development/contributing.html), to learn more about the
-process.\n\n\n## Versioning\n\nWe use [SemVer](http://semver.org/) for
-versioning. For the versions available, see the [tags on this repository]
-(https://github.com/staircase-dev/staircase/tags). It is highly recommended to
-use staircase 2.*, for both performance and additional features.\n\n\n##
-License\n\nThis project is licensed under the MIT License - see the [LICENSE]
-(https://github.com/staircase-dev/staircase/blob/master/LICENSE) file for
-details\n\n## Acknowledgments\n\nThe seeds of *staircase* began developing at
-the Hunter Valley Coal Chain Coordinator, where it finds strong application in
-analysing simulated data. Thanks for the support!\n', 'author': 'Riley
-Clement', 'author_email': 'venaturum@gmail.com', 'maintainer': 'Riley Clement',
-'maintainer_email': 'venaturum@gmail.com', 'url': 'https://staircase.dev',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'extras_require': extras_require, 'python_requires':
-'>=3.7,<4.0', } setup(**setup_kwargs)
+requests. Take a look at the current issues and if there is one you would like
+to work on please leave a comment to that effect. See this [beginner's guide to
+contributing](https://github.com/firstcontributions/first-contributions), or
+[Pandas' guide to contributing](https://pandas.pydata.org/pandas-docs/stable/
+development/contributing.html), to learn more about the process. ## Versioning
+We use [SemVer](http://semver.org/) for versioning. For the versions available,
+see the [tags on this repository](https://github.com/staircase-dev/staircase/
+tags). It is highly recommended to use staircase 2.*, for both performance and
+additional features. ## License This project is licensed under the MIT License
+- see the [LICENSE](https://github.com/staircase-dev/staircase/blob/master/
+LICENSE) file for details ## Acknowledgments The seeds of *staircase* began
+developing at the Hunter Valley Coal Chain Coordinator, where it finds strong
+application in analysing simulated data. Thanks for the support!
```

