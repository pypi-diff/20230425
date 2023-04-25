# Comparing `tmp/speechtotext-python-0.3.6.tar.gz` & `tmp/speechtotext-python-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechtotext-python-0.3.6.tar", last modified: Mon Apr 24 09:28:16 2023, max compression
+gzip compressed data, was "speechtotext-python-0.3.7.tar", last modified: Tue Apr 25 07:26:48 2023, max compression
```

## Comparing `speechtotext-python-0.3.6.tar` & `speechtotext-python-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.371530 speechtotext-python-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:28:16.371530 speechtotext-python-0.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4109 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/speechtotext/
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3603 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/speechtotext/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/speechtotext_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 09:28:16.000000 speechtotext-python-0.3.6/speechtotext_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:28:16.367530 speechtotext-python-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-24 09:27:00.000000 speechtotext-python-0.3.6/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4099 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.590268 speechtotext-python-0.3.7/speechtotext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6847 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/speechtotext/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.590268 speechtotext-python-0.3.7/speechtotext_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 07:26:48.000000 speechtotext-python-0.3.7/speechtotext_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:26:48.594268 speechtotext-python-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-25 07:24:54.000000 speechtotext-python-0.3.7/tests/test_metrics.py
```

### Comparing `speechtotext-python-0.3.6/LICENSE` & `speechtotext-python-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `speechtotext-python-0.3.6/PKG-INFO` & `speechtotext-python-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `speechtotext-python-0.3.6/setup.py` & `speechtotext-python-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	'deepgram-sdk', 'azure-cognitiveservices-speech', 
 	'speechmatics-python==1.6.4', 'pydub', 'docstring_parser'
 ]
 
 # What packages are optional?
 EXTRAS = {
 	'docs': ['Sphinx>=6.1.3', 'sphinx-markdown-builder>=0.5.5', 'sphinx_autodoc_typehints>=1.22', 
-			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine', 'pytest']
+			 'sphinx-press-theme>=0.8.0', 'sphinx_favicon', 'twine']
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
```

### Comparing `speechtotext-python-0.3.6/speechtotext/datasets.py` & `speechtotext-python-0.3.7/speechtotext/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 			return None
 
 class SampleDataset(DatasetBare):
 	"""Sample of dataset.
 	"""    
 	def __init__(self, df: pd.core.frame.DataFrame, path_to_dir: str, name: str, file_ext: str = ".wav"):
 		super().__init__(path_to_dir, name, file_ext)
-		self.dataset = df
+		self.dataset: pd.core.frame.DataFrame = df
 
 class Dataset(DatasetBare):
 	"""Class to extract data from the dataset folder.
 	"""    
 	def __init__(self, path_to_dir:str, name: str, file_ext:str=".wav"):  
 		super().__init__(path_to_dir, name, file_ext)
 		self.load_transcript()
@@ -117,24 +117,24 @@
 		"""     
 		file_path = f"{self.path_to_dir}/transcripts.txt"
 
 		df= pd.read_csv(file_path, sep="|", header=None)
 		df = df.iloc[:, 0:2] 
 		df.columns = ["id", "text"]
 		df['id'] = df['id'].apply(lambda id :get_file_name_without_extention(id) )
-		self.dataset = df
+		self.dataset: pd.core.frame.DataFrame = df
 
 	def get_n_samples(self, number_of_samples:int) -> SampleDataset:
 		"""Get n random samples.
 
 		Args:
 			number_of_samples (int): Number of random samples.
 
 		Returns:
 			SampleDataset: Dataset with the samples.
 		"""     
 		if number_of_samples > self.number_of_samples():
 			print("number larger then samples in dataset. Using full dataset")
-			number_of_samples = self.dataset.number_of_samples()
+			number_of_samples = self.number_of_samples()
 		df = self.dataset.sample(n=number_of_samples)
 
 		return SampleDataset(df, self.path_to_dir, self.name, self.file_ext)
```

### Comparing `speechtotext-python-0.3.6/speechtotext/functions.py` & `speechtotext-python-0.3.7/speechtotext/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,30 +51,31 @@
 
 	Args:
 		text (str): Uncleaned string.
 
 	Returns:
 		str: Cleaned string.
 	"""    
-	return re.sub(REGEX_STRING_PARSE, '', text)
+	return re.sub(REGEX_STRING_PARSE, '', text).rstrip()
 
 def join_benchmark_results(results: list[pd.core.frame.DataFrame], set_index=True) -> pd.core.frame.DataFrame:
 	"""Join Benchmark results.
 
 	Args:
 			results (list[pd.core.frame.DataFrame]): Results of benchmarks.
 			set_index (bool, optional): Set True if ["model_name", "audio_ID"] can be set as index. Defaults to True.
 
 	Returns:
 			pd.core.frame.DataFrame: Dataframe with results of all benchmarks.
 	"""
 	df = pd.concat(results)
 	if set_index:
 		df = df.set_index(["model_name", "audio_ID"])
-	return df
+		return df
+	return df.reset_index(drop=True)
 
 def separate_benchmark_results_by_model(dataframe: pd.core.frame.DataFrame) -> dict[str, pd.core.frame.DataFrame]:
 	"""Seperate benchmark results for each model.
 
 	Args:
 			dataframe pd.core.frame.DataFrame: Dataframe with results of all benchmarks.
```

### Comparing `speechtotext-python-0.3.6/speechtotext_python.egg-info/PKG-INFO` & `speechtotext-python-0.3.7/speechtotext_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speechtotext-python
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python package to benchmark speech2text models.
 Home-page: https://github.com/jarneamerlinck/speechtotext
 Author: Jarne Amerlinck
 Author-email: jarneamerlinck@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

