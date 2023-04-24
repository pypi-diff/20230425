# Comparing `tmp/numerblox-0.5.8.tar.gz` & `tmp/numerblox-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerblox-0.5.8.tar", last modified: Tue Apr 18 16:54:27 2023, max compression
+gzip compressed data, was "numerblox-0.5.9.tar", last modified: Mon Apr 24 22:27:33 2023, max compression
```

## Comparing `numerblox-0.5.8.tar` & `numerblox-0.5.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-18 16:54:27.747663 numerblox-0.5.8/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4767 2023-04-05 12:06:33.000000 numerblox-0.5.8/CONTRIBUTING.md
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11357 2023-04-05 12:06:33.000000 numerblox-0.5.8/LICENSE
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      111 2023-04-05 12:06:33.000000 numerblox-0.5.8/MANIFEST.in
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-18 16:54:27.747663 numerblox-0.5.8/PKG-INFO
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11651 2023-04-05 12:35:32.000000 numerblox-0.5.8/README.md
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-18 16:54:27.743662 numerblox-0.5.8/numerblox/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       22 2023-04-18 16:53:38.000000 numerblox-0.5.8/numerblox/__init__.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    68222 2023-04-18 16:53:38.000000 numerblox-0.5.8/numerblox/_modidx.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4073 2023-04-05 12:06:33.000000 numerblox-0.5.8/numerblox/_nbdev.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    22382 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/download.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    71551 2023-04-18 16:53:38.000000 numerblox-0.5.8/numerblox/evaluation.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      103 2023-04-05 12:06:33.000000 numerblox-0.5.8/numerblox/index.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      947 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/key.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      333 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/misc.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    26837 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/model.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     5985 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/model_pipeline.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     6929 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/numerframe.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15357 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/postprocessing.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    30218 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/preprocessing.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15925 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/submission.py
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-18 16:54:27.747663 numerblox-0.5.8/numerblox.egg-info/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/PKG-INFO
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      612 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/SOURCES.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/dependency_links.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       40 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/entry_points.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:40.000000 numerblox-0.5.8/numerblox.egg-info/not-zip-safe
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      194 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/requires.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       10 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/top_level.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     1071 2023-04-18 16:53:38.000000 numerblox-0.5.8/settings.ini
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       38 2023-04-18 16:54:27.747663 numerblox-0.5.8/setup.cfg
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     2537 2023-04-05 12:06:33.000000 numerblox-0.5.8/setup.py
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-24 22:27:33.625797 numerblox-0.5.9/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4767 2023-04-05 12:06:33.000000 numerblox-0.5.9/CONTRIBUTING.md
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11357 2023-04-05 12:06:33.000000 numerblox-0.5.9/LICENSE
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      111 2023-04-05 12:06:33.000000 numerblox-0.5.9/MANIFEST.in
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-24 22:27:33.625797 numerblox-0.5.9/PKG-INFO
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11651 2023-04-05 12:35:32.000000 numerblox-0.5.9/README.md
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-24 22:27:33.621797 numerblox-0.5.9/numerblox/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       22 2023-04-24 22:26:51.000000 numerblox-0.5.9/numerblox/__init__.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    68222 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/_modidx.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4073 2023-04-05 12:06:33.000000 numerblox-0.5.9/numerblox/_nbdev.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    22382 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/download.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    71601 2023-04-24 22:26:51.000000 numerblox-0.5.9/numerblox/evaluation.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      103 2023-04-05 12:06:33.000000 numerblox-0.5.9/numerblox/index.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      947 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/key.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      333 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/misc.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    26837 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/model.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     5985 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/model_pipeline.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     6929 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/numerframe.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15357 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/postprocessing.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    30218 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/preprocessing.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15925 2023-04-24 22:16:18.000000 numerblox-0.5.9/numerblox/submission.py
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-24 22:27:33.625797 numerblox-0.5.9/numerblox.egg-info/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-24 22:27:33.000000 numerblox-0.5.9/numerblox.egg-info/PKG-INFO
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      612 2023-04-24 22:27:33.000000 numerblox-0.5.9/numerblox.egg-info/SOURCES.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-24 22:27:33.000000 numerblox-0.5.9/numerblox.egg-info/dependency_links.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       40 2023-04-24 22:27:33.000000 numerblox-0.5.9/numerblox.egg-info/entry_points.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:40.000000 numerblox-0.5.9/numerblox.egg-info/not-zip-safe
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      194 2023-04-24 22:27:33.000000 numerblox-0.5.9/numerblox.egg-info/requires.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       10 2023-04-24 22:27:33.000000 numerblox-0.5.9/numerblox.egg-info/top_level.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     1071 2023-04-24 22:26:51.000000 numerblox-0.5.9/settings.ini
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       38 2023-04-24 22:27:33.625797 numerblox-0.5.9/setup.cfg
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     2537 2023-04-05 12:06:33.000000 numerblox-0.5.9/setup.py
```

### Comparing `numerblox-0.5.8/CONTRIBUTING.md` & `numerblox-0.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/LICENSE` & `numerblox-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/PKG-INFO` & `numerblox-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerblox
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tools for solid Numerai pipelines
 Home-page: https://github.com/crowdcent/numerblox/
 Author: Jason Rosenfeld, Carlo Lepelaars and contributors
 Author-email: support@crowdcent.com
 License: Apache Software License 2.0
 Keywords: Numerai,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `numerblox-0.5.8/README.md` & `numerblox-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/_modidx.py` & `numerblox-0.5.9/numerblox/_modidx.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/_nbdev.py` & `numerblox-0.5.9/numerblox/_nbdev.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/download.py` & `numerblox-0.5.9/numerblox/download.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/evaluation.py` & `numerblox-0.5.9/numerblox/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,25 +178,26 @@
         sharpe = mean / std
         return mean, std, sharpe
 
     def numerai_corr(
         self, dataf: pd.DataFrame, pred_col: str, target_col: str
     ) -> np.float64:
         """
-        Computes 'Numerai Corr'.
+        Computes 'Numerai Corr' aka 'Corrv2'.
         More info: https://forum.numer.ai/t/target-cyrus-new-primary-target/6303
 
         Assumes original target col as input (i.e. in [0, 1] range).
         """
         # Rank and gaussianize predictions
         ranked_preds = self._normalize_uniform(dataf[pred_col].fillna(0.5), 
                                                method="average")
         gauss_ranked_preds = stats.norm.ppf(ranked_preds)
         # Center target from [0...1] to [-0.5...0.5] range
-        centered_target = dataf[target_col] - 0.5
+        targets = dataf[target_col]
+        centered_target = targets - targets.mean()
         # Accentuate tails of predictions and targets
         preds_p15 = np.sign(gauss_ranked_preds) * np.abs(gauss_ranked_preds) ** 1.5
         target_p15 = np.sign(centered_target) * np.abs(centered_target) ** 1.5
         # Pearson correlation
         corr, _ = stats.pearsonr(preds_p15, target_p15)
         return corr
```

### Comparing `numerblox-0.5.8/numerblox/key.py` & `numerblox-0.5.9/numerblox/key.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/model.py` & `numerblox-0.5.9/numerblox/model.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/model_pipeline.py` & `numerblox-0.5.9/numerblox/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/numerframe.py` & `numerblox-0.5.9/numerblox/numerframe.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/postprocessing.py` & `numerblox-0.5.9/numerblox/postprocessing.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/preprocessing.py` & `numerblox-0.5.9/numerblox/preprocessing.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox/submission.py` & `numerblox-0.5.9/numerblox/submission.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/numerblox.egg-info/PKG-INFO` & `numerblox-0.5.9/numerblox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerblox
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tools for solid Numerai pipelines
 Home-page: https://github.com/crowdcent/numerblox/
 Author: Jason Rosenfeld, Carlo Lepelaars and contributors
 Author-email: support@crowdcent.com
 License: Apache Software License 2.0
 Keywords: Numerai,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `numerblox-0.5.8/numerblox.egg-info/SOURCES.txt` & `numerblox-0.5.9/numerblox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.8/settings.ini` & `numerblox-0.5.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 user = crowdcent
 description = Tools for solid Numerai pipelines
 keywords = Numerai, Machine Learning
 author = Jason Rosenfeld, Carlo Lepelaars and contributors
 author_email = support@crowdcent.com
 copyright = CrowdCent 2023
 branch = master
-version = 0.5.8
+version = 0.5.9
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 4
 requirements = jupyter eod wandb numpy scipy umap-learn pandas tqdm rich kaggle joblib pyarrow numerapi numerbay lightgbm catboost scikit-learn python-dateutil google-cloud-storage tensorflow pandas_ta
```

### Comparing `numerblox-0.5.8/setup.py` & `numerblox-0.5.9/setup.py`

 * *Files identical despite different names*

