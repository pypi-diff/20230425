# Comparing `tmp/owid_repack-0.1.1.tar.gz` & `tmp/owid_repack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owid_repack-0.1.1.tar", max compression
+gzip compressed data, was "owid_repack-0.1.2.tar", max compression
```

## Comparing `owid_repack-0.1.1.tar` & `owid_repack-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2022-12-22 01:55:57.375131 owid_repack-0.1.1/LICENSE
--rw-r--r--   0        0        0     1714 2022-12-22 02:36:57.490891 owid_repack-0.1.1/README.md
--rw-r--r--   0        0        0     4295 2022-12-22 01:48:54.012253 owid_repack-0.1.1/owid/repack/__init__.py
--rw-r--r--   0        0        0      694 2022-12-22 02:37:01.989665 owid_repack-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2521 1970-01-01 00:00:00.000000 owid_repack-0.1.1/setup.py
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 owid_repack-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-25 06:54:05.693844 owid_repack-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1879 2023-04-25 07:26:36.531810 owid_repack-0.1.2/README.md
+-rw-r--r--   0        0        0     4388 2023-04-25 07:24:50.748828 owid_repack-0.1.2/owid/repack/__init__.py
+-rw-r--r--   0        0        0      694 2023-04-25 07:26:42.067485 owid_repack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 owid_repack-0.1.2/setup.py
+-rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 owid_repack-0.1.2/PKG-INFO
```

### Comparing `owid_repack-0.1.1/LICENSE` & `owid_repack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `owid_repack-0.1.1/README.md` & `owid_repack-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # owid-repack-py
 
-![version](https://img.shields.io/badge/version-0.1.1-blue) ![version](https://img.shields.io/badge/python-3.8—3.11-blue.svg?&logo=python&logoColor=yellow)
+![build status](https://github.com/owid/owid-repack-py/actions/workflows/python-package.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/owid-repack.svg)](https://badge.fury.io/py/owid-repack)
+![](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11-blue.svg)
 
 _Pack Pandas DataFrames into smaller, more memory efficient types._
 
 ## Overview
 
 When you load data into Pandas, it will use standard types by default:
 
@@ -58,11 +60,13 @@
 dtype: Int8
 ```
 
 The `repack_frame()` method simply does this across every column in your DataFrame, returning a new DataFrame.
 
 ## Releases
 
+- `0.1.2`:
+    - Shrink columns with all NaNs to Int8
 - `0.1.1`:
     - Fix Python support in package metadata to support 3.8.1 onwards
 - `0.1.0`:
   - Migrate first version from `owid-catalog-py` repo
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `owid_repack-0.1.1/owid/repack/__init__.py` & `owid_repack-0.1.2/owid/repack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,18 @@
 
 def shrink_integer(s: pd.Series) -> pd.Series:
     """
     Take an Int64 series and make it as small as possible.
     """
     assert s.dtype.name in ("Int64", "int64", "UInt64", "uint64")
 
-    if s.isnull().any():
+    if s.isnull().all():
+        # shrink all NaNs to Int8
+        return s.astype("Int8")
+    elif s.isnull().any():
         if s.min() < 0:
             series = ["Int32", "Int16", "Int8"]
         else:
             series = ["UInt32", "UInt16", "UInt8"]
     else:
         if s.min() < 0:
             series = ["int32", "int16", "int8"]
```

### Comparing `owid_repack-0.1.1/pyproject.toml` & `owid_repack-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "owid-repack"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pack Pandas data frames into smaller, more memory-efficient data types."
 authors = ["Our World In Data <tech@ourworldindata.org>"]
 license = "MIT"
 packages = [{ include = "owid" }]
 readme = "README.md"
 repository = "https://github.com/owid/owid-catalog-py"
 homepage = "https://github.com/owid/owid-catalog-py"
```

### Comparing `owid_repack-0.1.1/setup.py` & `owid_repack-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.0,<2.0.0', 'pandas>=1.5.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'owid-repack',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Pack Pandas data frames into smaller, more memory-efficient data types.',
-    'long_description': '# owid-repack-py\n\n![version](https://img.shields.io/badge/version-0.1.1-blue) ![version](https://img.shields.io/badge/python-3.8—3.11-blue.svg?&logo=python&logoColor=yellow)\n\n_Pack Pandas DataFrames into smaller, more memory efficient types._\n\n## Overview\n\nWhen you load data into Pandas, it will use standard types by default:\n\n- `object` for strings\n- `int64` for integers\n- `float64` for floating point numbers\n\nHowever, for many datasets there is a much more compact representation that Pandas could be using for that data. Using a more compact representation leads to lower memory usage, and smaller binary files on disk when using formats such as Feather and Parquet.\n\nThis library does just one thing: it shrinks your data frames to use smaller types.\n\n## Installing\n\n`pip install owid-repack`\n\n## Usage\n\nThe `owid.repack` module exposes two methods, `repack_series()` and `repack_frame()`.\n\n`repack_series()` will detect the smallest type that can accurately fit the existing data in the series.\n\n```ipython\nIn [1]: from owid import repack\n\nIn [2]: pd.Series([1, 2, 3])\nOut[2]:\n0    1\n1    2\n2    3\ndtype: int64\n\nIn [3]: repack.repack_series(pd.Series([1.5, 2, 3]))\nOut[3]:\n0    1.5\n1    2.0\n2    3.0\ndtype: float32\n\nIn [4]: repack.repack_series(pd.Series([1, None, 3]))\nOut[4]:\n0       1\n1    <NA>\n2       3\ndtype: UInt8\n\nIn [5]: repack.repack_series(pd.Series([-1, None, 3]))\nOut[5]:\n0      -1\n1    <NA>\n2       3\ndtype: Int8\n```\n\nThe `repack_frame()` method simply does this across every column in your DataFrame, returning a new DataFrame.\n\n## Releases\n\n- `0.1.1`:\n    - Fix Python support in package metadata to support 3.8.1 onwards\n- `0.1.0`:\n  - Migrate first version from `owid-catalog-py` repo\n',
+    'long_description': '# owid-repack-py\n\n![build status](https://github.com/owid/owid-repack-py/actions/workflows/python-package.yml/badge.svg)\n[![PyPI version](https://badge.fury.io/py/owid-repack.svg)](https://badge.fury.io/py/owid-repack)\n![](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11-blue.svg)\n\n_Pack Pandas DataFrames into smaller, more memory efficient types._\n\n## Overview\n\nWhen you load data into Pandas, it will use standard types by default:\n\n- `object` for strings\n- `int64` for integers\n- `float64` for floating point numbers\n\nHowever, for many datasets there is a much more compact representation that Pandas could be using for that data. Using a more compact representation leads to lower memory usage, and smaller binary files on disk when using formats such as Feather and Parquet.\n\nThis library does just one thing: it shrinks your data frames to use smaller types.\n\n## Installing\n\n`pip install owid-repack`\n\n## Usage\n\nThe `owid.repack` module exposes two methods, `repack_series()` and `repack_frame()`.\n\n`repack_series()` will detect the smallest type that can accurately fit the existing data in the series.\n\n```ipython\nIn [1]: from owid import repack\n\nIn [2]: pd.Series([1, 2, 3])\nOut[2]:\n0    1\n1    2\n2    3\ndtype: int64\n\nIn [3]: repack.repack_series(pd.Series([1.5, 2, 3]))\nOut[3]:\n0    1.5\n1    2.0\n2    3.0\ndtype: float32\n\nIn [4]: repack.repack_series(pd.Series([1, None, 3]))\nOut[4]:\n0       1\n1    <NA>\n2       3\ndtype: UInt8\n\nIn [5]: repack.repack_series(pd.Series([-1, None, 3]))\nOut[5]:\n0      -1\n1    <NA>\n2       3\ndtype: Int8\n```\n\nThe `repack_frame()` method simply does this across every column in your DataFrame, returning a new DataFrame.\n\n## Releases\n\n- `0.1.2`:\n    - Shrink columns with all NaNs to Int8\n- `0.1.1`:\n    - Fix Python support in package metadata to support 3.8.1 onwards\n- `0.1.0`:\n  - Migrate first version from `owid-catalog-py` repo\n',
     'author': 'Our World In Data',
     'author_email': 'tech@ourworldindata.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/owid/owid-catalog-py',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `owid_repack-0.1.1/PKG-INFO` & `owid_repack-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owid-repack
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pack Pandas data frames into smaller, more memory-efficient data types.
 Home-page: https://github.com/owid/owid-catalog-py
 License: MIT
 Author: Our World In Data
 Author-email: tech@ourworldindata.org
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,17 @@
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Project-URL: Repository, https://github.com/owid/owid-catalog-py
 Description-Content-Type: text/markdown
 
 # owid-repack-py
 
-![version](https://img.shields.io/badge/version-0.1.1-blue) ![version](https://img.shields.io/badge/python-3.8—3.11-blue.svg?&logo=python&logoColor=yellow)
+![build status](https://github.com/owid/owid-repack-py/actions/workflows/python-package.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/owid-repack.svg)](https://badge.fury.io/py/owid-repack)
+![](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11-blue.svg)
 
 _Pack Pandas DataFrames into smaller, more memory efficient types._
 
 ## Overview
 
 When you load data into Pandas, it will use standard types by default:
 
@@ -77,12 +79,14 @@
 dtype: Int8
 ```
 
 The `repack_frame()` method simply does this across every column in your DataFrame, returning a new DataFrame.
 
 ## Releases
 
+- `0.1.2`:
+    - Shrink columns with all NaNs to Int8
 - `0.1.1`:
     - Fix Python support in package metadata to support 3.8.1 onwards
 - `0.1.0`:
   - Migrate first version from `owid-catalog-py` repo
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

