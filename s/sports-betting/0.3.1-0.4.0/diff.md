# Comparing `tmp/sports-betting-0.3.1.tar.gz` & `tmp/sports-betting-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports-betting-0.3.1.tar", last modified: Wed Apr 12 13:14:57 2023, max compression
+gzip compressed data, was "sports-betting-0.4.0.tar", last modified: Tue Apr 25 11:31:34 2023, max compression
```

## Comparing `sports-betting-0.3.1.tar` & `sports-betting-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,38 @@
--rw-r--r--   0        0        0     1072 2023-04-12 10:43:30.277668 sports-betting-0.3.1/LICENSE
--rw-r--r--   0        0        0     4879 2023-04-12 10:43:30.473663 sports-betting-0.3.1/README.md
--rw-r--r--   0        0        0     5343 2023-04-12 10:43:30.475057 sports-betting-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1029 2023-04-12 10:43:30.475247 sports-betting-0.3.1/src/sportsbet/__init__.py
--rw-r--r--   0        0        0      131 2023-03-29 08:50:29.899413 sports-betting-0.3.1/src/sportsbet/__main__.py
--rw-r--r--   0        0        0     9737 2023-04-11 16:49:24.909001 sports-betting-0.3.1/src/sportsbet/cli.py
--rw-r--r--   0        0        0      298 2023-04-11 16:49:24.909882 sports-betting-0.3.1/src/sportsbet/datasets/__init__.py
--rw-r--r--   0        0        0    18249 2023-04-11 16:49:24.910843 sports-betting-0.3.1/src/sportsbet/datasets/_base.py
--rw-r--r--   0        0        0    15554 2023-04-03 15:00:25.774832 sports-betting-0.3.1/src/sportsbet/datasets/_dummy.py
--rw-r--r--   0        0        0        0 2023-04-11 16:17:21.696007 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/__init__.py
--rw-r--r--   0        0        0    21586 2023-04-03 15:00:25.775440 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_data.py
--rw-r--r--   0        0        0    28790 2023-04-03 15:00:25.775835 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fd.py
--rw-r--r--   0        0        0     5122 2023-04-03 15:00:25.776337 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fte.py
--rw-r--r--   0        0        0     2595 2023-03-27 20:39:08.417256 sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_utils.py
--rw-r--r--   0        0        0      200 2023-04-03 10:27:16.832023 sports-betting-0.3.1/src/sportsbet/evaluation/__init__.py
--rw-r--r--   0        0        0    10944 2023-04-11 16:49:24.911729 sports-betting-0.3.1/src/sportsbet/evaluation/_base.py
--rw-r--r--   0        0        0     5529 2023-04-03 09:48:05.265783 sports-betting-0.3.1/src/sportsbet/evaluation/_classifier.py
--rw-r--r--   0        0        0        0 2023-04-12 10:43:30.443650 sports-betting-0.3.1/src/sportsbet/py.typed
--rw-r--r--   0        0        0      162 2023-04-12 10:43:30.222813 sports-betting-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      310 2023-04-12 10:43:30.475416 sports-betting-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0       28 2023-03-24 22:39:56.568853 sports-betting-0.3.1/tests/datasets/__init__.py
--rw-r--r--   0        0        0    18705 2023-03-28 15:26:00.605472 sports-betting-0.3.1/tests/datasets/test_dummy.py
--rw-r--r--   0        0        0       30 2023-03-24 22:40:31.109809 sports-betting-0.3.1/tests/evaluation/__init__.py
--rw-r--r--   0        0        0     7350 2023-04-02 15:06:18.413287 sports-betting-0.3.1/tests/evaluation/test_classifier.py
--rw-r--r--   0        0        0     7311 2023-04-02 21:31:27.333484 sports-betting-0.3.1/tests/test_cli.py
--rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 sports-betting-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-12 10:43:30.277668 sports-betting-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9397 2023-04-24 09:43:10.763453 sports-betting-0.4.0/README.md
+-rw-r--r--   0        0        0     5438 2023-04-24 21:31:06.056541 sports-betting-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1026 2023-04-24 09:43:10.783945 sports-betting-0.4.0/src/sportsbet/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-19 07:06:57.452684 sports-betting-0.4.0/src/sportsbet/__main__.py
+-rw-r--r--   0        0        0      124 2023-04-24 09:43:10.712522 sports-betting-0.4.0/src/sportsbet/cli/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-24 09:43:10.713830 sports-betting-0.4.0/src/sportsbet/cli/_cli.py
+-rw-r--r--   0        0        0     3905 2023-04-24 09:43:10.715546 sports-betting-0.4.0/src/sportsbet/cli/_datasets.py
+-rw-r--r--   0        0        0     3328 2023-04-24 09:43:10.716418 sports-betting-0.4.0/src/sportsbet/cli/_evaluation.py
+-rw-r--r--   0        0        0      874 2023-04-24 09:43:10.717061 sports-betting-0.4.0/src/sportsbet/cli/_options.py
+-rw-r--r--   0        0        0     4912 2023-04-24 09:43:10.717626 sports-betting-0.4.0/src/sportsbet/cli/_utils.py
+-rw-r--r--   0        0        0      320 2023-04-24 09:43:10.784738 sports-betting-0.4.0/src/sportsbet/datasets/__init__.py
+-rw-r--r--   0        0        0    18296 2023-04-24 09:43:10.786065 sports-betting-0.4.0/src/sportsbet/datasets/_base.py
+-rw-r--r--   0        0        0    15883 2023-04-24 09:43:10.787051 sports-betting-0.4.0/src/sportsbet/datasets/_dummy.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:17:21.696007 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/__init__.py
+-rw-r--r--   0        0        0    21957 2023-04-24 09:43:10.788101 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_data.py
+-rw-r--r--   0        0        0    28799 2023-04-24 09:43:10.735625 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fd.py
+-rw-r--r--   0        0        0     5122 2023-04-03 15:00:25.776337 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fte.py
+-rw-r--r--   0        0        0     2595 2023-03-27 20:39:08.417256 sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_utils.py
+-rw-r--r--   0        0        0      326 2023-04-24 09:43:10.695223 sports-betting-0.4.0/src/sportsbet/evaluation/__init__.py
+-rw-r--r--   0        0        0    11881 2023-04-24 09:43:10.696860 sports-betting-0.4.0/src/sportsbet/evaluation/_base.py
+-rw-r--r--   0        0        0     6783 2023-04-24 09:43:10.697929 sports-betting-0.4.0/src/sportsbet/evaluation/_classifier.py
+-rw-r--r--   0        0        0     7919 2023-04-24 09:43:10.699163 sports-betting-0.4.0/src/sportsbet/evaluation/_rules.py
+-rw-r--r--   0        0        0        0 2023-04-12 10:43:30.443650 sports-betting-0.4.0/src/sportsbet/py.typed
+-rw-r--r--   0        0        0      162 2023-04-12 10:43:30.222813 sports-betting-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-24 09:43:10.718388 sports-betting-0.4.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-24 09:43:10.719615 sports-betting-0.4.0/tests/cli/configs/bettor.py
+-rw-r--r--   0        0        0      316 2023-04-24 09:43:10.720456 sports-betting-0.4.0/tests/cli/configs/dataloader.py
+-rw-r--r--   0        0        0     2919 2023-04-24 09:43:10.721300 sports-betting-0.4.0/tests/cli/test_datasets.py
+-rw-r--r--   0        0        0     2050 2023-04-24 09:43:10.721779 sports-betting-0.4.0/tests/cli/test_evaluation.py
+-rw-r--r--   0        0        0      482 2023-04-24 09:43:10.722335 sports-betting-0.4.0/tests/cli/test_main.py
+-rw-r--r--   0        0        0      310 2023-04-12 10:43:30.475416 sports-betting-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0       28 2023-03-24 22:39:56.568853 sports-betting-0.4.0/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    18705 2023-03-28 15:26:00.605472 sports-betting-0.4.0/tests/datasets/test_dummy.py
+-rw-r--r--   0        0        0       30 2023-03-24 22:40:31.109809 sports-betting-0.4.0/tests/evaluation/__init__.py
+-rw-r--r--   0        0        0     7350 2023-04-02 15:06:18.413287 sports-betting-0.4.0/tests/evaluation/test_classifier.py
+-rw-r--r--   0        0        0     2897 2023-04-24 09:22:43.246577 sports-betting-0.4.0/tests/evaluation/test_rules.py
+-rw-r--r--   0        0        0    10739 1970-01-01 00:00:00.000000 sports-betting-0.4.0/PKG-INFO
```

### Comparing `sports-betting-0.3.1/LICENSE` & `sports-betting-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sports-betting-0.3.1/pyproject.toml` & `sports-betting-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 description = "Python sports betting toolbox."
 authors = [
     { name = "Georgios Douzas", email = "gdouzas@icloud.com" },
 ]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9, <3.11"
-keywords = []
+keywords = [
+    "sports betting",
+    "sports analytics",
+    "machine learning",
+]
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -36,25 +40,25 @@
     "beautifulsoup4>=4.0.0",
     "vectorbt>=0.24.5",
     "QuantStats>=0.0.47",
     "typing-extensions>=4.5.0",
     "click>=8.1.3",
     "rich>=13.3.3",
 ]
-version = "0.3.1"
+version = "0.4.0"
 
 [project.urls]
 Homepage = "https://georgedouzas.github.io/sports-betting"
 Documentation = "https://georgedouzas.github.io/sports-betting"
 Changelog = "https://georgedouzas.github.io/sports-betting/changelog"
-Repository = "https://github/georgedouzas/sports-betting"
+Repository = "https://github.com/georgedouzas/sports-betting"
 Issues = "https://github/georgedouzas/sports-betting/issues"
-Discussions = "https://github/georgedouzas/sports-betting/discussions"
+Discussions = "https://github.com/georgedouzas/sports-betting/discussions"
 Gitter = "https://gitter.im/sports-betting/community"
-Funding = "https://github/sponsors/georgedouzas"
+Funding = "https://github.com/sponsors/georgedouzas"
 
 [project.scripts]
 sportsbet = "sportsbet.cli:main"
 
 [tool.pdm.version]
 source = "scm"
 
@@ -79,15 +83,15 @@
 ]
 docs = [
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
-    "mkdocs-gallery>=0.7.6",
+    "mkdocs-gallery<=0.7.6",
     "mkdocs-section-index>=0.3",
     "mkdocstrings[python]>=0.20",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
     "pandas>=1.5.0",
 ]
 formatting = [
@@ -173,14 +177,15 @@
     "S101",
     "INP001",
     "Q000",
     "TRY002",
     "PLR0913",
     "EXE001",
     "EXE002",
+    "E741",
 ]
 fix = true
 fixable = [
     "C",
     "E",
     "F",
     "W",
```

### Comparing `sports-betting-0.3.1/src/sportsbet/__init__.py` & `sports-betting-0.4.0/src/sportsbet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
 import numpy as np
 import pandas as pd
 from nptyping import Bool, Float, NDArray, Shape
 
 Param = dict[str, Any]
 ParamGrid = Union[dict[str, list[Any]], list[dict[str, list[Any]]]]
-TrainingData = tuple[pd.DataFrame, pd.DataFrame, Union[pd.DataFrame, None]]
+TrainData = tuple[pd.DataFrame, pd.DataFrame, Union[pd.DataFrame, None]]
 FixturesData = tuple[pd.DataFrame, None, Union[pd.DataFrame, None]]
 Data = NDArray[Shape['*, *'], Float]
 BoolData = NDArray[Shape['*, *'], Bool]
 Schema = list[tuple[str, Union[type[int], type[float], type[object], type[np.datetime64]]]]
 Outputs = list[tuple[str, Callable[..., pd.DataFrame]]]
```

### Comparing `sports-betting-0.3.1/src/sportsbet/datasets/_base.py` & `sports-betting-0.4.0/src/sportsbet/datasets/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import cloudpickle
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import ParameterGrid
 from sklearn.utils import check_scalar
 from typing_extensions import Self
 
-from .. import FixturesData, Outputs, Param, ParamGrid, Schema, TrainingData
+from .. import FixturesData, Outputs, Param, ParamGrid, Schema, TrainData
 
 
 def _create_names_mapping_table(data_source1: pd.DataFrame, data_source2: pd.DataFrame, keys: list) -> pd.DataFrame:
     def _cols(x: str) -> list[str]:
         return [f'{col}_team{x}' for col in ('home', 'away')]
 
     # Generate teams names combinations
@@ -126,15 +126,15 @@
                 {
                     col
                     for col, selected_data_type in self.SCHEMA
                     if selected_data_type is data_type and col in data.columns
                 },
             )
             if converted_cols:
-                data_converted_cols = data[converted_cols].fillna(-1 if data_type is int else np.nan)
+                data_converted_cols = data[converted_cols].fillna(-1 if data_type is np.int64 else np.nan)
                 data[converted_cols] = (
                     data_converted_cols.to_numpy().astype(data_type)
                     if data_type is not np.datetime64
                     else pd.to_datetime(data_converted_cols.iloc[:, 0])
                 )
         return data
 
@@ -182,15 +182,15 @@
             error_msg = 'The raw data and available parameters are incompatible.'
             raise ValueError(error_msg) from e
 
         return data
 
     def _extract_train_data(self: Self, data: pd.DataFrame) -> pd.DataFrame:
         data = data[~data['fixtures']].drop(columns=['fixtures'])
-        data = data.reset_index().merge(pd.DataFrame(self.param_grid_)).set_index('date')
+        data = data.reset_index().merge(pd.DataFrame(self.param_grid_)).set_index('date').sort_index()
         return data
 
     def _check_dropped_na_cols(self: Self, data: pd.DataFrame, drop_na_thres: float) -> Self:
         thres = int(data.shape[0] * drop_na_thres)
         dropped_all_na_cols = data.columns.difference(data.dropna(axis=1, how='all').columns)
         dropped_thres_na_cols = data.columns.difference(data.dropna(axis=1, thresh=thres).columns)
         dropped_na_cols = dropped_all_na_cols.union(dropped_thres_na_cols)
@@ -203,15 +203,15 @@
             raise ValueError(error_msg)
         return self
 
     def extract_train_data(
         self: Self,
         drop_na_thres: float = 0.0,
         odds_type: str | None = None,
-    ) -> TrainingData:
+    ) -> TrainData:
         """Extract the training data.
 
         Read more in the [user guide][dataloader].
 
         It returns historical data that can be used to create a betting
         strategy based on heuristics or machine learning models.
 
@@ -311,15 +311,19 @@
             func = outputs_mapping[col]
             Y_train.append(pd.Series(func(data[self.target_cols_]), name=col))
         Y_train = pd.concat(Y_train, axis=1).reset_index(drop=True)
 
         # Extract odds
         O_train = data[self.odds_cols_].reset_index(drop=True) if self.odds_type_ is not None else None
 
-        return data[self.input_cols_], Y_train, O_train
+        self.train_data_ = data[self.input_cols_], Y_train, O_train
+        if hasattr(self, 'fixtures_data_'):
+            delattr(self, 'fixtures_data_')
+
+        return self.train_data_
 
     def extract_fixtures_data(self: Self) -> FixturesData:
         """Extract the fixtures data.
 
         Read more in the [user guide][dataloader].
 
         It returns fixtures data that can be used to make predictions for
@@ -340,20 +344,15 @@
         Returns:
             (X, None, O):
                 Each of the components represent the fixtures input data `X`, the
                 multi-output targets `Y` equal to `None` and the
                 corresponding odds `O`, respectively.
         """
         # Extract fixtures data
-        if not (
-            hasattr(self, 'input_cols_')
-            and hasattr(self, 'output_cols_')
-            and hasattr(self, 'odds_cols_')
-            and hasattr(self, 'target_cols_')
-        ):
+        if not hasattr(self, 'train_data_'):
             error_msg = 'Extract the training data before extracting the fixtures data.'
             raise AttributeError(error_msg)
 
         data = self._validate_data()
 
         # Extract fixtures data
         data = data[data['fixtures']].drop(columns=['fixtures'])
@@ -363,15 +362,17 @@
 
         # Remove past data
         data = data.loc[data.index >= pd.to_datetime('today')]
 
         # Extract odds
         O_fix = data[self.odds_cols_].reset_index(drop=True) if self.odds_type_ is not None else None
 
-        return data[self.input_cols_], None, O_fix
+        self.fixtures_data_ = data[self.input_cols_], None, O_fix
+
+        return self.fixtures_data_
 
     def save(self: Self, path: str) -> Self:
         """Save the dataloader object.
 
         Args:
             path:
                 The path to save the object.
@@ -426,15 +427,15 @@
 
         # Drop columns with only missing values
         dropped_all_na_cols = data.columns.difference(data.dropna(axis=1, how='all').columns)
 
         return sorted({col.split('__')[1] for col in self._cols(data, 'odds') if col not in dropped_all_na_cols})
 
 
-def load(path: str) -> _BaseDataLoader:
+def load_dataloader(path: str) -> _BaseDataLoader:
     """Load the dataloader object.
 
     Args:
         path:
             The path of the dataloader pickled file.
 
     Returns:
```

### Comparing `sports-betting-0.3.1/src/sportsbet/datasets/_dummy.py` & `sports-betting-0.4.0/src/sportsbet/datasets/_dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import pandas as pd
 import pytz
 from sklearn.model_selection import ParameterGrid
 from typing_extensions import Self
 
-from .. import FixturesData, ParamGrid, TrainingData
+from .. import FixturesData, ParamGrid, TrainData
 from ._base import _BaseDataLoader
 
 OVER_UNDER = 2.5
 
 
 class DummySoccerDataLoader(_BaseDataLoader):
     """Dataloader for soccer dummy data.
@@ -58,14 +58,22 @@
 
         odds_cols_ (pd.Index):
             The columns of `O_train` and `O_fix`.
 
         target_cols_ (pd.Index):
             The columns used for the extraction of output and odds columns.
 
+        train_data_ (TrainData):
+            The tuple (X, Y, O) that represents the training data as extracted from
+            the method `extract_train_data`.
+
+        fixtures_data_ (FixturesData):
+            The tuple (X, Y, O) that represents the fixtures data as extracted from
+            the method `extract_fixtures_data`.
+
     Examples:
         >>> from sportsbet.datasets import DummySoccerDataLoader
         >>> import pandas as pd
         >>> # Get all available parameters to select the training data
         >>> DummySoccerDataLoader.get_all_params()
         [{'division': 1, 'year': 1998}, ...
         >>> # Select only the traning data for the Spanish league
@@ -394,15 +402,15 @@
     def _get_data(self: Self) -> pd.DataFrame:
         return self.DATA
 
     def extract_train_data(
         self: Self,
         drop_na_thres: float = 0.0,
         odds_type: str | None = None,
-    ) -> TrainingData:
+    ) -> TrainData:
         """Extract the training data.
 
         Read more in the [user guide][dataloader].
 
         It returns historical data that can be used to create a betting
         strategy based on heuristics or machine learning models.
```

### Comparing `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_data.py` & `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from functools import lru_cache
 
 import pandas as pd
 from sklearn.model_selection import ParameterGrid
 from typing_extensions import Self
 
-from ... import FixturesData, ParamGrid, TrainingData
+from ... import FixturesData, ParamGrid, TrainData
 from .._base import _BaseDataLoader
 from ._fd import _FDSoccerDataLoader
 from ._fte import _FTESoccerDataLoader
 from ._utils import OUTPUTS
 
 NAMES_MAPPING = {
     'SK Austria Klagenfurt': 'A. Klagenfurt',
@@ -396,14 +396,22 @@
 
         odds_cols_ (pd.Index):
             The columns of `O_train` and `O_fix`.
 
         target_cols_ (pd.Index):
             The columns used for the extraction of output and odds columns.
 
+        train_data_ (TrainData):
+            The tuple (X, Y, O) that represents the training data as extracted from
+            the method `extract_train_data`.
+
+        fixtures_data_ (FixturesData):
+            The tuple (X, Y, O) that represents the fixtures data as extracted from
+            the method `extract_fixtures_data`.
+
     Examples:
         >>> from sportsbet.datasets import SoccerDataLoader
         >>> import pandas as pd
         >>> # Get all available parameters to select the training data
         >>> SoccerDataLoader.get_all_params()
         [{'data_source': 'fivethirtyeight', 'division': 1, ...
         >>> # Select only the traning data for the French and Spanish leagues of 2020 year
@@ -484,15 +492,15 @@
         else:
             return pd.DataFrame()
 
     def extract_train_data(
         self: Self,
         drop_na_thres: float = 0.0,
         odds_type: str | None = None,
-    ) -> TrainingData:
+    ) -> TrainData:
         """Extract the training data.
 
         Read more in the [user guide][dataloader].
 
         It returns historical data that can be used to create a betting
         strategy based on heuristics or machine learning models.
 
@@ -524,20 +532,23 @@
             (X, Y, O):
                 Each of the components represent the training input data `X`, the
                 multi-output targets `Y` and the corresponding odds `O`, respectively.
         """
         X_train, Y_train, O_train = super().extract_train_data(drop_na_thres, odds_type)
         self.input_cols_ = pd.Index([col for col in self.input_cols_ if col != 'data_source'], dtype=object)
         X_train = X_train.reset_index().drop_duplicates(subset=self.input_cols_)
-        return (
+
+        self.train_data_ = (
             X_train.set_index('date')[self.input_cols_],
-            Y_train.take(X_train.index.to_list()),
-            O_train.take(X_train.index.to_list()) if O_train is not None else None,
+            Y_train.take(X_train.index.to_list()).reset_index(drop=True),
+            O_train.take(X_train.index.to_list()).reset_index(drop=True) if O_train is not None else None,
         )
 
+        return self.train_data_
+
     def extract_fixtures_data(self: Self) -> FixturesData:
         """Extract the fixtures data.
 
         Read more in the [user guide][dataloader].
 
         It returns fixtures data that can be used to make predictions for
         upcoming matches based on a betting strategy.
@@ -556,9 +567,8 @@
 
         Returns:
             (X, None, O):
                 Each of the components represent the fixtures input data `X`, the
                 multi-output targets `Y` equal to `None` and the
                 corresponding odds `O`, respectively.
         """
-        X_fix, Y_fix, O_fix = super().extract_fixtures_data()
-        return X_fix, Y_fix, O_fix
+        return super().extract_fixtures_data()
```

### Comparing `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fd.py` & `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fd.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,15 +515,15 @@
 
     @lru_cache  # noqa: B019
     def _get_data(self: Self) -> pd.DataFrame:
         # Training data
         data_container = []
         urls = _param_grid_to_csv_urls(self.param_grid_)
         for params, url in track(urls, description='Downloading training data', transient=True):
-            data = _read_csv(url).replace('#REF!', np.nan)
+            data = _read_csv(url).replace('^#', np.nan, regex=True)
             try:
                 data['Date'] = pd.to_datetime(data['Date'], format='%d/%m/%Y')
             except ValueError:
                 data['Date'] = pd.to_datetime(data['Date'], infer_datetime_format=True)
 
             if url.split('/')[-2] != 'new':
                 data = data.assign(
```

### Comparing `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_fte.py` & `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_fte.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.3.1/src/sportsbet/datasets/_soccer/_utils.py` & `sports-betting-0.4.0/src/sportsbet/datasets/_soccer/_utils.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.3.1/src/sportsbet/evaluation/_base.py` & `sports-betting-0.4.0/src/sportsbet/evaluation/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 # Author: Georgios Douzas <gdouzas@icloud.com>
 # License: MIT
 
 from __future__ import annotations
 
 from abc import ABCMeta
+from pathlib import Path
 
+import cloudpickle
 import numpy as np
 import pandas as pd
+from rich.progress import track
 from sklearn.base import BaseEstimator, ClassifierMixin, MultiOutputMixin
 from sklearn.model_selection import TimeSeriesSplit
 from sklearn.utils import check_consistent_length, check_scalar
 from sklearn.utils.validation import check_is_fitted
 from typing_extensions import Self
 from vectorbt import Portfolio
 
@@ -45,21 +48,32 @@
             (float, int),
             min_val=0.0,
             include_boundaries='neither',
         )
         self.init_cash_ = float(init_cash)
         return self
 
-    def _check_dates(self: Self, X: pd.DataFrame) -> pd.DatetimeIndex:
-        if isinstance(X, pd.DataFrame) and isinstance(X.index, pd.DatetimeIndex):
-            dates = X.index
-        else:
+    def _validate_data(
+        self: Self,
+        X: pd.DataFrame,
+        Y: pd.DataFrame,
+        O: pd.DataFrame,
+    ) -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
+        check_consistent_length(X, Y, O)
+        if not isinstance(X, pd.DataFrame) or not isinstance(X.index, pd.DatetimeIndex):
             error_msg = 'Input data `X` should be pandas dataframe with a date index.'
             raise TypeError(error_msg)
-        return dates
+        if not isinstance(Y, pd.DataFrame):
+            error_msg = 'Output data `Y` should be pandas dataframe.'
+            raise TypeError(error_msg)
+        if not isinstance(O, pd.DataFrame):
+            error_msg = 'Odds data `O` should be pandas dataframe.'
+            raise TypeError(error_msg)
+        indices = np.argsort(X.index)
+        return X.iloc[indices], Y.iloc[indices], O.iloc[indices]
 
     def _extract_portfolio(self: Self, prices: pd.DataFrame, orders: pd.DataFrame) -> Portfolio:
         """Extract portfolio."""
         return Portfolio.from_orders(prices, orders, freq='0.5D', cash_sharing=True, init_cash=self.init_cash_)
 
     @staticmethod
     def _extract_stats(portfolio: Portfolio, training_start: int, training_end: int) -> pd.DataFrame:
@@ -169,21 +183,21 @@
 
         Args:
             X:
                 The input data.
 
         Returns:
             Y:
-                The positive class probabilities.
+                The positive class labels.
         """
         check_is_fitted(self)
         decision_threshold = 0.5
         return self._predict_proba(X) > decision_threshold
 
-    def bet(self: Self, X: pd.DataFrame, O: pd.DataFrame) -> BoolData:  # noqa: E741
+    def bet(self: Self, X: pd.DataFrame, O: pd.DataFrame) -> BoolData:
         """Predict the value bets for the provided input data and odds.
 
         Args:
             X:
                 The input data.
 
             O:
@@ -197,38 +211,36 @@
             return np.array([], dtype=bool).reshape(0, O.shape[1])
         return self.predict_proba(X) * O > 1
 
     def backtest(
         self: Self,
         X: pd.DataFrame,
         Y: pd.DataFrame,
-        O: pd.DataFrame | None,  # noqa: E741
+        O: pd.DataFrame | None,
         tscv: TimeSeriesSplit | None = None,
-        init_cash: float | None = 1e3,
+        init_cash: float | None = None,
         refit: bool | None = True,
     ) -> Self:
         """Backtest the bettor.
 
         Args:
             X:
                 The input data. Each row of `X` represents information that is available
-                before the start of a specific match. The rows should be
-                sorted by an index named as `'date'`.
+                before the start of a specific match. The index should be of type
+                `datetime`, named as `'date'`.
 
             Y:
                 The multi-output targets. Each row of `Y` represents information
-                that is available after the end of a specific match. The column
+                that is available after the end of a specific event. The column
                 names follow the convention for the output data `Y` of the method
-                `extract_train_data`.
+                `extract_train_data` of dataloaders.
 
             O:
-                The odds data. Each row of `O` represents information
-                that is available after the end of a specific match. The column
-                names follow the convention for the output data `Y` of the method
-                `extract_train_data`.
+                The odds data. The column names follow the convention for the odds
+                data `O` of the method `extract_train_data` of dataloaders.
 
             tscv:
                 Provides train/test indices to split time series data samples
                 that are observed at fixed time intervals, in train/test sets. The
                 default value of the parameter is `None`.
 
             init_cash:
@@ -237,23 +249,26 @@
             refit:
                 Refit the bettor using the whole input data and multi-output targets.
 
         Returns:
             self:
                 The backtested bettor.
         """
-        if O is None:
+        if O is None or O.empty:
             return self
-        check_consistent_length(X, Y, O)
+
+        # Apply checks
+        X, Y, O = self._validate_data(X, Y, O)
         self._check_backtest_params(tscv, init_cash)
-        dates = self._check_dates(X)
+
+        dates = X.index
 
         # Calculate cross-validation stats
         results = []
-        for train_ind, test_ind in self.tscv_.split(X):
+        for train_ind, test_ind in track(list(self.tscv_.split(X)), description='Backtesting bettor', transient=True):
             # Fit bettor
             self.fit(X.iloc[train_ind], Y.iloc[train_ind])
 
             # Predict value bets
             value_bets = self.bet(X.iloc[test_ind], O.iloc[test_ind])
 
             # Calculate returns
@@ -295,27 +310,51 @@
                 .groupby('date')
                 .apply(lambda row: (row.iloc[0, :] == 2) & (row.iloc[1, :] == 0))  # noqa: PLR2004
             )
             orders[mask] = 0
 
             # Get portofolio from prices and orders
             portfolio = self._extract_portfolio(prices, orders)
-            results.append(
-                (
-                    self._extract_stats(portfolio, X.index[train_ind[0]], X.index[train_ind[-1]]),
-                    portfolio.plot_value,
-                ),
-            )
-        self.backtest_results_, plot_value_funcs = zip(*results)
-        self.backtest_results_ = pd.concat(self.backtest_results_, ignore_index=True)
-        self.backtest_plot_value_ = lambda ind: plot_value_funcs[ind]()
+            results.append(self._extract_stats(portfolio, X.index[train_ind[0]], X.index[train_ind[-1]]))
+        self.backtest_results_ = pd.concat(results, ignore_index=True)
 
         if refit:
             self.fit(X, Y)
 
         return self
 
     def _fit(self: Self, X: pd.DataFrame, Y: pd.DataFrame) -> Self:
         return self
 
     def _predict_proba(self: Self, X: pd.DataFrame) -> Data:
-        return np.array([], dtype=bool)
+        return np.array([], dtype=float)
+
+    def save(self: Self, path: str) -> Self:
+        """Save the bettor object.
+
+        Args:
+            path:
+                The path to save the object.
+
+        Returns:
+            self:
+                The bettor object.
+        """
+        with Path(path).open('wb') as file:
+            cloudpickle.dump(self, file)
+        return self
+
+
+def load_bettor(path: str) -> _BaseBettor:
+    """Load the bettor object.
+
+    Args:
+        path:
+            The path of the bettor pickled file.
+
+    Returns:
+        bettor:
+            The bettor object.
+    """
+    with Path(path).open('rb') as file:
+        bettor = cloudpickle.load(file)
+    return bettor
```

### Comparing `sports-betting-0.3.1/src/sportsbet/evaluation/_classifier.py` & `sports-betting-0.4.0/src/sportsbet/evaluation/_classifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, clone, is_classifier
 from sklearn.model_selection import TimeSeriesSplit
 from typing_extensions import Self
 
-from .. import Data
+from .. import BoolData, Data
 from ._base import _BaseBettor
 
 
 class ClassifierBettor(_BaseBettor):
     """Bettor based on a Scikit-Learn classifier.
 
     Read more in the [user guide][user-guide].
@@ -27,21 +27,21 @@
             A scikit-learn classifier object implementing `fit`, `score`
             and `predict_proba`.
 
     Attributes:
         tscv_ (TimeSeriesSplit):
             The checked value of time series cross-validator object. If `tscv` is `None`,
             it uses the default `TimeSeriesSplit` object.
+
         init_cash_:
             The checked value of initial cash. If `init_cash` is `None`, it uses the value
             of `1e3`.
+
         backtest_results_ (pd.DataFrame):
-            The backtesting resutsl.
-        backtest_plot_value_ (FigureWidget):
-            Figure widget that show the value of the portfolio over time.
+            The backtesting results.
 
     Examples:
         >>> from sklearn.tree import DecisionTreeClassifier
         >>> from sklearn.preprocessing import OneHotEncoder
         >>> from sklearn.impute import SimpleImputer
         >>> from sklearn.pipeline import make_pipeline
         >>> from sklearn.compose import make_column_transformer
@@ -101,19 +101,77 @@
                 The positive class probabilities.
         """
         return np.concatenate(
             [prob[:, -1].reshape(-1, 1) for prob in self.classifier_.predict_proba(X)],
             axis=1,
         )
 
+    def fit(self: Self, X: pd.DataFrame, Y: pd.DataFrame) -> Self:
+        """Fit the bettor to the input data and multi-output targets.
+
+        Args:
+            X:
+                The input data.
+
+            Y:
+                The multi-output targets.
+
+        Returns:
+            self:
+                The fitted bettor object.
+        """
+        return super().fit(X, Y)
+
+    def predict_proba(self: Self, X: pd.DataFrame) -> Data:
+        """Predict class probabilities for multi-output targets.
+
+        Args:
+            X:
+                The input data.
+
+        Returns:
+            Y:
+                The positive class probabilities.
+        """
+        return super().predict_proba(X)
+
+    def predict(self: Self, X: pd.DataFrame) -> BoolData:
+        """Predict class probabilities for multi-output targets.
+
+        Args:
+            X:
+                The input data.
+
+        Returns:
+            Y:
+                The positive class labels.
+        """
+        return super().predict(X)
+
+    def bet(self: Self, X: pd.DataFrame, O: pd.DataFrame) -> BoolData:
+        """Predict the value bets for the provided input data and odds.
+
+        Args:
+            X:
+                The input data.
+
+            O:
+                The odds data.
+
+        Returns:
+            B:
+                The value bets.
+        """
+        return super().bet(X, O)
+
     def backtest(
         self: Self,
         X: pd.DataFrame,
         Y: pd.DataFrame,
-        O: pd.DataFrame | None,  # noqa: E741
+        O: pd.DataFrame | None,
         tscv: TimeSeriesSplit | None = None,
         init_cash: float | None = 1e3,
         refit: bool | None = True,
     ) -> Self:
         """Backtest the bettor.
 
         Args:
```

### Comparing `sports-betting-0.3.1/tests/datasets/test_dummy.py` & `sports-betting-0.4.0/tests/datasets/test_dummy.py`

 * *Files identical despite different names*

### Comparing `sports-betting-0.3.1/tests/evaluation/test_classifier.py` & `sports-betting-0.4.0/tests/evaluation/test_classifier.py`

 * *Files identical despite different names*

