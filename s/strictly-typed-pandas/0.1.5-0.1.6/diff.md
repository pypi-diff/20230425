# Comparing `tmp/strictly_typed_pandas-0.1.5.tar.gz` & `tmp/strictly_typed_pandas-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictly_typed_pandas-0.1.5.tar", last modified: Sun Mar 19 13:28:16 2023, max compression
+gzip compressed data, was "strictly_typed_pandas-0.1.6.tar", last modified: Sun Apr  9 07:53:39 2023, max compression
```

## Comparing `strictly_typed_pandas-0.1.5.tar` & `strictly_typed_pandas-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:28:16.748431 strictly_typed_pandas-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-19 13:28:16.748431 strictly_typed_pandas-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 13:28:16.748431 strictly_typed_pandas-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:28:16.748431 strictly_typed_pandas-0.1.5/strictly_typed_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/create_empty_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/pandas_types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/typeguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-03-19 13:28:05.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 13:28:16.748431 strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-19 13:28:16.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-19 13:28:16.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 13:28:16.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-19 13:28:16.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-19 13:28:16.000000 strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/strictly_typed_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/create_empty_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/pandas_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/typeguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/top_level.txt
```

### Comparing `strictly_typed_pandas-0.1.5/LICENSE` & `strictly_typed_pandas-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.5/PKG-INFO` & `strictly_typed_pandas-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: strictly_typed_pandas
-Version: 0.1.5
+Version: 0.1.6
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
-Requires-Python: >3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================================================================
 Strictly Typed Pandas: static type checking of pandas DataFrames
 ================================================================
```

### Comparing `strictly_typed_pandas-0.1.5/README.rst` & `strictly_typed_pandas-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.5/setup.py` & `strictly_typed_pandas-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,13 +19,13 @@
     author_email="nanne.aben@gmail.com",
     description="Static type checking of pandas DataFrames",
     keywords="typing type checking pandas mypy linting",
     long_description=get_long_description(),
     long_description_content_type="text/x-rst",
     packages=find_packages(include=["strictly_typed_pandas", "strictly_typed_pandas.*"]),
     install_requires=get_requirements(),
-    python_requires=">3.7.0",
+    python_requires=">=3.8.0",
     classifiers=["Typing :: Typed"],
     version_config=True,
     setup_requires=['setuptools-git-versioning'],
     package_data={"strictly_typed_pandas": ["py.typed"]},
 )
```

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas/create_empty_dataframe.py` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas/create_empty_dataframe.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas/dataset.py` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from abc import ABC, abstractmethod
 from typing import Any, Generic, TypeVar, get_type_hints
 
 from strictly_typed_pandas.immutable import (
     _ImmutableiLocIndexer, _ImmutableLocIndexer, immutable_error_msg, inplace_argument_interceptor
 )
 from strictly_typed_pandas.validate_schema import (
-    check_for_duplicate_columns, check_index_for_unsupported_datatypes, validate_schema
+    check_for_duplicate_columns, validate_schema
 )
 from strictly_typed_pandas.create_empty_dataframe import create_empty_dataframe, create_empty_indexed_dataframe
 
 
 dataframe_functions = dict(inspect.getmembers(pd.DataFrame, predicate=inspect.isfunction))
 dataframe_member_names = dict(inspect.getmembers(pd.DataFrame)).keys()
 
@@ -160,16 +160,14 @@
             set(schema_data_expected.keys())
         )
 
         if self.shape == (0, 0) and self.index.shape == (0,):
             df = create_empty_indexed_dataframe(schema_index_expected, schema_data_expected)
             super().__init__(df)
         else:
-            check_index_for_unsupported_datatypes(schema_index_expected)
-
             schema_data_observed = dict(zip(self.columns, self.dtypes))
             schema_index_observed = {
                 name: self.index.get_level_values(i).dtype
                 for i, name in enumerate(self.index.names)
             }
 
             validate_schema(schema_index_expected, schema_index_observed)
```

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas/immutable.py` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas/immutable.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas/pandas_types.py` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas/pandas_types.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas/typeguard.py` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas/typeguard.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas/validate_schema.py` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas/validate_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 import numpy as np  # type: ignore
-import warnings
 
 from typing import Dict, Any, Set
 from pandas.core.dtypes.common import is_dtype_equal
 from pandas.api.extensions import ExtensionDtype
 
-from strictly_typed_pandas.pandas_types import SparseDtype, StringDtype
+from strictly_typed_pandas.pandas_types import StringDtype
 
 
 def check_for_duplicate_columns(names_index: Set[str], names_data: Set[str]) -> None:
     intersection = names_index & names_data
     if len(intersection) > 0:
         msg = "The following column is present in both the index schema and the data schema: {}"
         raise TypeError(msg.format(intersection))
 
 
-def check_index_for_unsupported_datatypes(schema: Dict[str, Any]) -> None:
-    dtypes = [dtype for _, dtype in schema.items() if isinstance(dtype, SparseDtype)]
-    if len(dtypes) > 0:
-        msg = (
-            "As of Pandas 1.5.3, there is no support for the following data types in the index: {}. While this " +
-            "may change in future versions, we suggest you proceed with caution."
-        )
-        warnings.warn(msg.format(dtypes), SyntaxWarning)
-
-
 def validate_schema(schema_expected: Dict[str, Any], schema_observed: Dict[str, Any]):
     _check_names(set(schema_expected.keys()), set(schema_observed.keys()))
     _check_dtypes(schema_expected, schema_observed)
 
 
 def _check_names(names_expected: Set[str], names_observed: Set[str]) -> None:
     diff = names_observed - names_expected
```

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/PKG-INFO` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: strictly-typed-pandas
-Version: 0.1.5
+Version: 0.1.6
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
-Requires-Python: >3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ================================================================
 Strictly Typed Pandas: static type checking of pandas DataFrames
 ================================================================
```

### Comparing `strictly_typed_pandas-0.1.5/strictly_typed_pandas.egg-info/SOURCES.txt` & `strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

