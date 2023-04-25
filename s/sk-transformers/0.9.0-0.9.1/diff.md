# Comparing `tmp/sk_transformers-0.9.0.tar.gz` & `tmp/sk_transformers-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_transformers-0.9.0.tar", max compression
+gzip compressed data, was "sk_transformers-0.9.1.tar", max compression
```

## Comparing `sk_transformers-0.9.0.tar` & `sk_transformers-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6517 2023-01-20 20:18:44.401112 sk_transformers-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-01-20 20:18:44.401112 sk_transformers-0.9.0/LICENSE
--rw-r--r--   0        0        0    16045 2023-01-20 20:18:44.401112 sk_transformers-0.9.0/docs/README.md
--rw-r--r--   0        0        0     2957 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      902 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/__init__.py
--rw-r--r--   0        0        0      772 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/base_transformer.py
--rw-r--r--   0        0        0     3848 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/datetime_transformer.py
--rw-r--r--   0        0        0     6890 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/deep_transformer.py
--rw-r--r--   0        0        0     1970 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/encoder_transformer.py
--rw-r--r--   0        0        0    25404 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/generic_transformer.py
--rw-r--r--   0        0        0     4977 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/number_transformer.py
--rw-r--r--   0        0        0    14539 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/string_transformer.py
--rw-r--r--   0        0        0     6484 2023-01-20 20:18:44.405112 sk_transformers-0.9.0/src/sk_transformers/utils.py
--rw-r--r--   0        0        0    17211 1970-01-01 00:00:00.000000 sk_transformers-0.9.0/setup.py
--rw-r--r--   0        0        0    18004 1970-01-01 00:00:00.000000 sk_transformers-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7028 2023-01-23 09:46:14.764688 sk_transformers-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-01-23 09:46:14.764688 sk_transformers-0.9.1/LICENSE
+-rw-r--r--   0        0        0    16322 2023-01-23 09:46:14.772688 sk_transformers-0.9.1/docs/README.md
+-rw-r--r--   0        0        0     2957 2023-01-23 09:46:14.780688 sk_transformers-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      902 2023-01-23 09:46:14.784688 sk_transformers-0.9.1/src/sk_transformers/__init__.py
+-rw-r--r--   0        0        0      772 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/base_transformer.py
+-rw-r--r--   0        0        0     3848 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/datetime_transformer.py
+-rw-r--r--   0        0        0     6890 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/deep_transformer.py
+-rw-r--r--   0        0        0     1970 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/encoder_transformer.py
+-rw-r--r--   0        0        0    25404 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/generic_transformer.py
+-rw-r--r--   0        0        0     4977 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/number_transformer.py
+-rw-r--r--   0        0        0    14539 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/string_transformer.py
+-rw-r--r--   0        0        0     6483 2023-01-23 09:46:14.788688 sk_transformers-0.9.1/src/sk_transformers/utils.py
+-rw-r--r--   0        0        0    17489 1970-01-01 00:00:00.000000 sk_transformers-0.9.1/setup.py
+-rw-r--r--   0        0        0    18281 1970-01-01 00:00:00.000000 sk_transformers-0.9.1/PKG-INFO
```

### Comparing `sk_transformers-0.9.0/CHANGELOG.md` & `sk_transformers-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [0.9.1](https://github.com/chrislemke/sk-transformers/compare/v0.9.0...v0.9.1) (2023-01-23)
+
+
+### CI/CD
+
+* add auto comment github action ([#58](https://github.com/chrislemke/sk-transformers/issues/58)) ([bed2782](https://github.com/chrislemke/sk-transformers/commit/bed2782594ac6881d4ac1f2e7643de4f293cf80b))
+* improve github actions ([#64](https://github.com/chrislemke/sk-transformers/issues/64)) ([e1f07e1](https://github.com/chrislemke/sk-transformers/commit/e1f07e1b41e1ae81c72b7306c6323a54ff9d0319))
+
 ## [0.9.0](https://github.com/chrislemke/sk-transformers/compare/v0.8.0...v0.9.0) (2023-01-20)
 
 
 ### Features
 
 * add ColumnEvalTransformer ([#52](https://github.com/chrislemke/sk-transformers/issues/52)) ([a03b079](https://github.com/chrislemke/sk-transformers/commit/a03b079d1818674c7115b4f3122656f0f1af1b1d))
 * add string_splitter_transformer ([#53](https://github.com/chrislemke/sk-transformers/issues/53)) ([fdf89e1](https://github.com/chrislemke/sk-transformers/commit/fdf89e1dd9cb9de1348a9be11796a24023ec1817))
```

### Comparing `sk_transformers-0.9.0/LICENSE` & `sk_transformers-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/docs/README.md` & `sk_transformers-0.9.1/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ![The Transformer](https://raw.githubusercontent.com/chrislemke/sk-transformers/master/docs/assets/images/icon.png)
 
 # sk-transformers
 ***A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering steps*** 🛠
 
 [![testing](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/44093b8f6b28454fb8e0336ccb83cdc5)](https://www.codacy.com/gh/chrislemke/sk-transformers/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=chrislemke/sk-transformers&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/github/chrislemke/sk-transformers/branch/main/graph/badge.svg?token=LJLXQXX6M8)](https://codecov.io/github/chrislemke/sk-transformers)
 [![deploy package](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml/badge.svg)](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml)
 [![pypi](https://img.shields.io/pypi/v/sk-transformers)](https://pypi.org/project/sk-transformers/)
 [![python version](https://img.shields.io/pypi/pyversions/sk-transformers?logo=python&logoColor=yellow)](https://www.python.org/)
 [![downloads](https://img.shields.io/pypi/dm/sk-transformers)](https://pypistats.org/packages/sk-transformers)
 [![docs](https://img.shields.io/badge/docs-mkdoks%20material-blue)](https://chrislemke.github.io/sk-transformers/)
 [![license](https://img.shields.io/github/license/chrislemke/sk-transformers)](https://github.com/chrislemke/sk-transformers/blob/main/LICENSE)
```

### Comparing `sk_transformers-0.9.0/pyproject.toml` & `sk_transformers-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sk-transformers"
-version = "0.9.0"
+version = "0.9.1"
 description = "A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering"
 authors = ["Christopher Lemke <1@lemke.ai>"]
 license = "MIT"
 readme = "docs/README.md"
 packages = [{ include = "sk_transformers", from = "src" }]
 include = ["CHANGELOG.md"]
 classifiers = [
```

### Comparing `sk_transformers-0.9.0/src/sk_transformers/__init__.py` & `sk_transformers-0.9.1/src/sk_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/base_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/base_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/datetime_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/deep_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/deep_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/encoder_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/generic_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/generic_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/number_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/number_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/string_transformer.py` & `sk_transformers-0.9.1/src/sk_transformers/string_transformer.py`

 * *Files identical despite different names*

### Comparing `sk_transformers-0.9.0/src/sk_transformers/utils.py` & `sk_transformers-0.9.1/src/sk_transformers/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     Raises:
         TypeError: If the input `transformer` is not a subclass of `BaseEstimator`.
         ValueError: If the input `X` is not a Pandas dataframe.
         ValueError: If the input is an empty Pandas dataframe.
         ValueError: If the input `X` does not contain the feature.
         ValueError: if the input `X` does not contain all features.
 
-
     Returns:
         pandas.DataFrame: A checked copy of original dataframe.
     """
 
     if isinstance(features, str):
         features = [features]
```

### Comparing `sk_transformers-0.9.0/setup.py` & `sk_transformers-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'phonenumbers>=8.13.4,<9.0.0',
  'pytorch-widedeep==1.2.1',
  'scikit-learn>=1.2.0,<2.0.0',
  'swifter>=1.3.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'sk-transformers',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering',
-    'long_description': '![The Transformer](https://raw.githubusercontent.com/chrislemke/sk-transformers/master/docs/assets/images/icon.png)\n\n# sk-transformers\n***A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering steps*** 🛠\n\n[![testing](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml)\n[![codecov](https://codecov.io/github/chrislemke/sk-transformers/branch/main/graph/badge.svg?token=LJLXQXX6M8)](https://codecov.io/github/chrislemke/sk-transformers)\n[![deploy package](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml/badge.svg)](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml)\n[![pypi](https://img.shields.io/pypi/v/sk-transformers)](https://pypi.org/project/sk-transformers/)\n[![python version](https://img.shields.io/pypi/pyversions/sk-transformers?logo=python&logoColor=yellow)](https://www.python.org/)\n[![downloads](https://img.shields.io/pypi/dm/sk-transformers)](https://pypistats.org/packages/sk-transformers)\n[![docs](https://img.shields.io/badge/docs-mkdoks%20material-blue)](https://chrislemke.github.io/sk-transformers/)\n[![license](https://img.shields.io/github/license/chrislemke/sk-transformers)](https://github.com/chrislemke/sk-transformers/blob/main/LICENSE)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://github.com/python/mypy)\n[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)\n## Introduction\nEvery tabular data is different. Every column needs to be treated differently. Pandas is already great! And [scikit-learn](https://scikit-learn.org/stable/index.html) has a nice [collection of dataset transformers](https://scikit-learn.org/stable/data_transforms.html). But the possibilities of data transformation are infinite. This project tries to provide a brought collection of data transformers that can be easily used together with [scikit-learn](https://scikit-learn.org/stable/index.html) - either in a [pipeline](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html) or just on its own. See the [usage chapter](#usage) for some examples.\n\nThe idea is simple. It is like a well-equipped toolbox 🧰: You always find the tool you need and sometimes you get inspired by seeing a tool you did not know before. Please feel free to [contribute](https://chrislemke.github.io/sk-transformers/CONTRIBUTING/) your tools and ideas.\n\nCheck out some examples in the [Jupyter notebook](https://github.com/chrislemke/sk-transformers/blob/main/examples/playground.ipynb).<br>\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/chrislemke/sk-transformers/blob/main/examples/playground.ipynb)\n\n## Installation\nIf you are using [pip](https://pip.pypa.io/en/stable/), you can install the package with the following command:\n```bash\npip install sk-transformers\n```\n\nIf you are using [Poetry](https://python-poetry.org/), you can install the package with the following command:\n```bash\npoetry add sk-transformers\n```\n\n## installing dependencies\nWith [pip](https://pip.pypa.io/en/stable/):\n```bash\npip install -r requirements.txt\n```\n\nWith [Poetry](https://python-poetry.org/):\n```bash\npoetry install\n```\n\n## Available transformers\n| Module | Transformer | Description |\n| ------ | ----------- | ----------- |\n|[`Datetime transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/datetime_transformer/)|[`DurationCalculatorTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/datetime_transformer/#sk_transformers.datetime_transformer.DurationCalculatorTransformer)|Calculates the duration between to given dates.|\n|[`Deep transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/deep_transformer/)|[`ToVecTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/deep_transformer/#sk_transformers.deep_transformer.ToVecTransformer)|This transformer trains an [FT-Transformer](https://paperswithcode.com/method/ft-transformer) using the [pytorch-widedeep package](https://github.com/jrzaurin/pytorch-widedeep) and extracts the embeddings from its embedding layer.|\n|[`Encoder transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/encoder_transformer/)|[`MeanEncoderTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/encoder_transformer/#sk_transformers.encoder_transformer.MeanEncoderTransformer)|Scikit-learn API for the [feature-engine MeanEncoder](https://feature-engine.readthedocs.io/en/latest/api_doc/encoding/MeanEncoder.html).|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`AggregateTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.AggregateTransformer)|This transformer uses Pandas groupby method and aggregate to apply function on a column grouped by another column.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`AllowedValuesTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.AllowedValuesTransformer)|This transformer replaces values that are *not* in a list with another value.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ColumnDropperTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ColumnDropperTransformer)|Drops columns from a dataframe using Pandas drop method.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ColumnEvalTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ColumnEvalTransformer)|Provides the possibility to use Pandas methods on columns.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`DtypeTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.DtypeTransformer)|Transformer that converts a column to a different dtype.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`FunctionsTransformer`]( https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.FunctionsTransformer)|This transformer is a plain wrapper around the [sklearn.preprocessing.FunctionTransformer](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.FunctionTransformer.html).|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`LeftJoinTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.LeftJoinTransformer)|Uses Pandas merge function to perform a left-join based on the column of a dataframe and the index of another dataframe. The right dataframe is essentially a lookup table.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`MapTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.MapTransformer)|This transformer iterates over all columns in the `features` list and applies the given callback to the column. For this it uses the `pandas.Series.map` method.\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`NaNTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.NaNTransformer)|Replace NaN values with a specified value. Internally Pandas fillna method is used.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`QueryTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.QueryTransformer)|Applies a list of queries to a dataframe. If it operates on a dataset used for supervised learning this transformer should be applied on the dataframe containing `X` and `y`.\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ValueIndicatorTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ValueIndicatorTransformer)|Adds a column to a dataframe indicating if a value is equal to a specified value.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ValueReplacerTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ValueReplacerTransformer)|Uses Pandas replace method to replace values in a column.|\n[`Number transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/number_transformer/)|[`MathExpressionTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/number_transformer/#sk_transformers.number_transformer.MathExpressionTransformer)|Applies an operation to a column and a given value or column. The operation can be any operation from the `numpy` or `operator` package.\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`EmailTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.EmailTransformer)|Transforms an email address into multiple features.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`IPAddressEncoderTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.IPAddressEncoderTransformer)|Encodes IPv4 and IPv6 strings addresses to a float representation.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`PhoneTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.PhoneTransformer)|Transforms a phone number into multiple features.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`StringSimilarityTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.StringSimilarityTransformer)|Calculates the similarity between two strings using the `gestalt pattern matching` algorithm from the `SequenceMatcher` class.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`StringSlicerTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.StringSlicerTransformer)|Slices all entries of specified string features using the slice() function.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`StringSplitterTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.StringSplitterTransformer)|Splits a string column into multiple columns based on the occurrence of a character.|\n\n## Usage\nLet\'s assume you want to use some method from [NumPy\'s mathematical functions, to sum up the values of column `foo` and column `bar`. You could\nuse the [`MathExpressionTransformer`](https://chrislemke.github.io/sk-transformers/number_transformer-reference/#sk-transformers.transformer.number_transformer.MathExpressionTransformer).\n```python\nimport pandas as pd\nfrom sk_transformers import MathExpressionTransformer\n\nX = pd.DataFrame({"foo": [1, 2, 3], "bar": [4, 5, 6]})\ntransformer = MathExpressionTransformer([("foo", "np.sum", "bar", {"axis": 0})])\ntransformer.fit_transform(X).to_numpy()\n```\n```\narray([[1, 4, 5],\n       [2, 5, 7],\n       [3, 6, 9]])\n```\nEven if we only pass one tuple to the transformer - in this example. Like with most other transformers the idea is to simplify preprocessing by giving the possibility to operate on multiple columns at the same time. In this case, the [`MathExpressionTransformer`](https://chrislemke.github.io/sk-transformers/number_transformer-reference/#sk-transformers.transformer.number_transformer.MathExpressionTransformer) has created an extra column with the name `foo_sum_bar`.\n\nIn the next example, we additionally add the [`MapTransformer`](https://chrislemke.github.io/sk-transformers/generic_transformer-reference/#sk_transformers.transformer.generic_transformer.MapTransformer).\nTogether with [scikit-learn\'s pipelines](https://scikit-learn.org/stable/modules/compose.html#combining-estimators) it would look like this:\n```python\nimport pandas as pd\nfrom sk_transformers import MathExpressionTransformer\nfrom sk_transformers import MapTransformer\nfrom sklearn.pipeline import Pipeline\n\nX = pd.DataFrame({"foo": [1, 2, 3], "bar": [4, 5, 6]})\nmap_step = MapTransformer([("foo", lambda x: x + 100)])\nsum_step = MathExpressionTransformer([("foo", "np.sum", "bar", {"axis": 0})])\npipeline = Pipeline([("map_step", map_step), ("sum_step", sum_step)])\npipeline.fit_transform(X)\n```\n\n```\n   foo  bar  foo_sum_bar\n0  101    4          105\n1  102    5          107\n2  103    6          109\n```\n\n## Contributing\nWe\'re all kind of in the same boat. Preprocessing/feature engineering in data science is somehow very individual - every feature is different and must be handled and processed differently. But somehow we all have the same problems: sometimes date columns have to be changed. Sometimes strings have to be formatted, sometimes durations have to be calculated, etc. There is a huge number of preprocessing possibilities but we all use the same tools.\n\n[scikit-learns pipelines](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html) help to use formalized functions. So why not also share these so-called transformers with others? This open-source project has the goal to collect useful preprocessing pipeline steps. Let us all collect what we used for preprocessing and share it with others. This way we can all benefit from each other\'s work and save a lot of time. So if you have a preprocessing step that you use regularly, please feel free to contribute it to this project. The idea is that this is not only a toolbox but also an inspiration for what is possible. Maybe you have not thought about this preprocessing step before.\n\nPlease check out the [guide](https://chrislemke.github.io/sk-transformers/CONTRIBUTING/) on how to contribute to this project.\n',
+    'long_description': '![The Transformer](https://raw.githubusercontent.com/chrislemke/sk-transformers/master/docs/assets/images/icon.png)\n\n# sk-transformers\n***A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering steps*** 🛠\n\n[![testing](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/44093b8f6b28454fb8e0336ccb83cdc5)](https://www.codacy.com/gh/chrislemke/sk-transformers/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=chrislemke/sk-transformers&amp;utm_campaign=Badge_Grade)\n[![codecov](https://codecov.io/github/chrislemke/sk-transformers/branch/main/graph/badge.svg?token=LJLXQXX6M8)](https://codecov.io/github/chrislemke/sk-transformers)\n[![deploy package](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml/badge.svg)](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml)\n[![pypi](https://img.shields.io/pypi/v/sk-transformers)](https://pypi.org/project/sk-transformers/)\n[![python version](https://img.shields.io/pypi/pyversions/sk-transformers?logo=python&logoColor=yellow)](https://www.python.org/)\n[![downloads](https://img.shields.io/pypi/dm/sk-transformers)](https://pypistats.org/packages/sk-transformers)\n[![docs](https://img.shields.io/badge/docs-mkdoks%20material-blue)](https://chrislemke.github.io/sk-transformers/)\n[![license](https://img.shields.io/github/license/chrislemke/sk-transformers)](https://github.com/chrislemke/sk-transformers/blob/main/LICENSE)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://github.com/PyCQA/isort)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](https://github.com/python/mypy)\n[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)\n## Introduction\nEvery tabular data is different. Every column needs to be treated differently. Pandas is already great! And [scikit-learn](https://scikit-learn.org/stable/index.html) has a nice [collection of dataset transformers](https://scikit-learn.org/stable/data_transforms.html). But the possibilities of data transformation are infinite. This project tries to provide a brought collection of data transformers that can be easily used together with [scikit-learn](https://scikit-learn.org/stable/index.html) - either in a [pipeline](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html) or just on its own. See the [usage chapter](#usage) for some examples.\n\nThe idea is simple. It is like a well-equipped toolbox 🧰: You always find the tool you need and sometimes you get inspired by seeing a tool you did not know before. Please feel free to [contribute](https://chrislemke.github.io/sk-transformers/CONTRIBUTING/) your tools and ideas.\n\nCheck out some examples in the [Jupyter notebook](https://github.com/chrislemke/sk-transformers/blob/main/examples/playground.ipynb).<br>\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/chrislemke/sk-transformers/blob/main/examples/playground.ipynb)\n\n## Installation\nIf you are using [pip](https://pip.pypa.io/en/stable/), you can install the package with the following command:\n```bash\npip install sk-transformers\n```\n\nIf you are using [Poetry](https://python-poetry.org/), you can install the package with the following command:\n```bash\npoetry add sk-transformers\n```\n\n## installing dependencies\nWith [pip](https://pip.pypa.io/en/stable/):\n```bash\npip install -r requirements.txt\n```\n\nWith [Poetry](https://python-poetry.org/):\n```bash\npoetry install\n```\n\n## Available transformers\n| Module | Transformer | Description |\n| ------ | ----------- | ----------- |\n|[`Datetime transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/datetime_transformer/)|[`DurationCalculatorTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/datetime_transformer/#sk_transformers.datetime_transformer.DurationCalculatorTransformer)|Calculates the duration between to given dates.|\n|[`Deep transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/deep_transformer/)|[`ToVecTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/deep_transformer/#sk_transformers.deep_transformer.ToVecTransformer)|This transformer trains an [FT-Transformer](https://paperswithcode.com/method/ft-transformer) using the [pytorch-widedeep package](https://github.com/jrzaurin/pytorch-widedeep) and extracts the embeddings from its embedding layer.|\n|[`Encoder transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/encoder_transformer/)|[`MeanEncoderTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/encoder_transformer/#sk_transformers.encoder_transformer.MeanEncoderTransformer)|Scikit-learn API for the [feature-engine MeanEncoder](https://feature-engine.readthedocs.io/en/latest/api_doc/encoding/MeanEncoder.html).|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`AggregateTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.AggregateTransformer)|This transformer uses Pandas groupby method and aggregate to apply function on a column grouped by another column.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`AllowedValuesTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.AllowedValuesTransformer)|This transformer replaces values that are *not* in a list with another value.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ColumnDropperTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ColumnDropperTransformer)|Drops columns from a dataframe using Pandas drop method.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ColumnEvalTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ColumnEvalTransformer)|Provides the possibility to use Pandas methods on columns.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`DtypeTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.DtypeTransformer)|Transformer that converts a column to a different dtype.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`FunctionsTransformer`]( https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.FunctionsTransformer)|This transformer is a plain wrapper around the [sklearn.preprocessing.FunctionTransformer](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.FunctionTransformer.html).|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`LeftJoinTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.LeftJoinTransformer)|Uses Pandas merge function to perform a left-join based on the column of a dataframe and the index of another dataframe. The right dataframe is essentially a lookup table.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`MapTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.MapTransformer)|This transformer iterates over all columns in the `features` list and applies the given callback to the column. For this it uses the `pandas.Series.map` method.\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`NaNTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.NaNTransformer)|Replace NaN values with a specified value. Internally Pandas fillna method is used.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`QueryTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.QueryTransformer)|Applies a list of queries to a dataframe. If it operates on a dataset used for supervised learning this transformer should be applied on the dataframe containing `X` and `y`.\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ValueIndicatorTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ValueIndicatorTransformer)|Adds a column to a dataframe indicating if a value is equal to a specified value.|\n|[`Generic transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/)|[`ValueReplacerTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/generic_transformer/#sk_transformers.generic_transformer.ValueReplacerTransformer)|Uses Pandas replace method to replace values in a column.|\n[`Number transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/number_transformer/)|[`MathExpressionTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/number_transformer/#sk_transformers.number_transformer.MathExpressionTransformer)|Applies an operation to a column and a given value or column. The operation can be any operation from the `numpy` or `operator` package.\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`EmailTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.EmailTransformer)|Transforms an email address into multiple features.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`IPAddressEncoderTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.IPAddressEncoderTransformer)|Encodes IPv4 and IPv6 strings addresses to a float representation.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`PhoneTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.PhoneTransformer)|Transforms a phone number into multiple features.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`StringSimilarityTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.StringSimilarityTransformer)|Calculates the similarity between two strings using the `gestalt pattern matching` algorithm from the `SequenceMatcher` class.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`StringSlicerTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.StringSlicerTransformer)|Slices all entries of specified string features using the slice() function.|\n[`String transformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/)|[`StringSplitterTransformer`](https://chrislemke.github.io/sk-transformers/API-reference/transformer/string_transformer/#sk_transformers.string_transformer.StringSplitterTransformer)|Splits a string column into multiple columns based on the occurrence of a character.|\n\n## Usage\nLet\'s assume you want to use some method from [NumPy\'s mathematical functions, to sum up the values of column `foo` and column `bar`. You could\nuse the [`MathExpressionTransformer`](https://chrislemke.github.io/sk-transformers/number_transformer-reference/#sk-transformers.transformer.number_transformer.MathExpressionTransformer).\n```python\nimport pandas as pd\nfrom sk_transformers import MathExpressionTransformer\n\nX = pd.DataFrame({"foo": [1, 2, 3], "bar": [4, 5, 6]})\ntransformer = MathExpressionTransformer([("foo", "np.sum", "bar", {"axis": 0})])\ntransformer.fit_transform(X).to_numpy()\n```\n```\narray([[1, 4, 5],\n       [2, 5, 7],\n       [3, 6, 9]])\n```\nEven if we only pass one tuple to the transformer - in this example. Like with most other transformers the idea is to simplify preprocessing by giving the possibility to operate on multiple columns at the same time. In this case, the [`MathExpressionTransformer`](https://chrislemke.github.io/sk-transformers/number_transformer-reference/#sk-transformers.transformer.number_transformer.MathExpressionTransformer) has created an extra column with the name `foo_sum_bar`.\n\nIn the next example, we additionally add the [`MapTransformer`](https://chrislemke.github.io/sk-transformers/generic_transformer-reference/#sk_transformers.transformer.generic_transformer.MapTransformer).\nTogether with [scikit-learn\'s pipelines](https://scikit-learn.org/stable/modules/compose.html#combining-estimators) it would look like this:\n```python\nimport pandas as pd\nfrom sk_transformers import MathExpressionTransformer\nfrom sk_transformers import MapTransformer\nfrom sklearn.pipeline import Pipeline\n\nX = pd.DataFrame({"foo": [1, 2, 3], "bar": [4, 5, 6]})\nmap_step = MapTransformer([("foo", lambda x: x + 100)])\nsum_step = MathExpressionTransformer([("foo", "np.sum", "bar", {"axis": 0})])\npipeline = Pipeline([("map_step", map_step), ("sum_step", sum_step)])\npipeline.fit_transform(X)\n```\n\n```\n   foo  bar  foo_sum_bar\n0  101    4          105\n1  102    5          107\n2  103    6          109\n```\n\n## Contributing\nWe\'re all kind of in the same boat. Preprocessing/feature engineering in data science is somehow very individual - every feature is different and must be handled and processed differently. But somehow we all have the same problems: sometimes date columns have to be changed. Sometimes strings have to be formatted, sometimes durations have to be calculated, etc. There is a huge number of preprocessing possibilities but we all use the same tools.\n\n[scikit-learns pipelines](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html) help to use formalized functions. So why not also share these so-called transformers with others? This open-source project has the goal to collect useful preprocessing pipeline steps. Let us all collect what we used for preprocessing and share it with others. This way we can all benefit from each other\'s work and save a lot of time. So if you have a preprocessing step that you use regularly, please feel free to contribute it to this project. The idea is that this is not only a toolbox but also an inspiration for what is possible. Maybe you have not thought about this preprocessing step before.\n\nPlease check out the [guide](https://chrislemke.github.io/sk-transformers/CONTRIBUTING/) on how to contribute to this project.\n',
     'author': 'Christopher Lemke',
     'author_email': '1@lemke.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://chrislemke.github.io/sk-transformers/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `sk_transformers-0.9.0/PKG-INFO` & `sk_transformers-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-transformers
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering
 Home-page: https://chrislemke.github.io/sk-transformers/
 License: MIT
 Keywords: feature engineering,preprocessing,pandas,scikit-learn,transformer,pipelines,machine learning,data science,artificial intelligence
 Author: Christopher Lemke
 Author-email: 1@lemke.ai
 Requires-Python: >=3.8,<3.11
@@ -38,14 +38,15 @@
 
 ![The Transformer](https://raw.githubusercontent.com/chrislemke/sk-transformers/master/docs/assets/images/icon.png)
 
 # sk-transformers
 ***A collection of various pandas & scikit-learn compatible transformers for all kinds of preprocessing and feature engineering steps*** 🛠
 
 [![testing](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/chrislemke/sk-transformers/actions/workflows/testing.yml)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/44093b8f6b28454fb8e0336ccb83cdc5)](https://www.codacy.com/gh/chrislemke/sk-transformers/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=chrislemke/sk-transformers&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/github/chrislemke/sk-transformers/branch/main/graph/badge.svg?token=LJLXQXX6M8)](https://codecov.io/github/chrislemke/sk-transformers)
 [![deploy package](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml/badge.svg)](https://github.com/chrislemke/sk-transformers/actions/workflows/deploy-package.yml)
 [![pypi](https://img.shields.io/pypi/v/sk-transformers)](https://pypi.org/project/sk-transformers/)
 [![python version](https://img.shields.io/pypi/pyversions/sk-transformers?logo=python&logoColor=yellow)](https://www.python.org/)
 [![downloads](https://img.shields.io/pypi/dm/sk-transformers)](https://pypistats.org/packages/sk-transformers)
 [![docs](https://img.shields.io/badge/docs-mkdoks%20material-blue)](https://chrislemke.github.io/sk-transformers/)
 [![license](https://img.shields.io/github/license/chrislemke/sk-transformers)](https://github.com/chrislemke/sk-transformers/blob/main/LICENSE)
```

