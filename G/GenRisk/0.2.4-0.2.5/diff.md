# Comparing `tmp/GenRisk-0.2.4.tar.gz` & `tmp/GenRisk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenRisk-0.2.4.tar", last modified: Mon Apr 24 15:18:02 2023, max compression
+gzip compressed data, was "GenRisk-0.2.5.tar", last modified: Tue Apr 25 07:23:54 2023, max compression
```

## Comparing `GenRisk-0.2.4.tar` & `GenRisk-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 15:18:02.652490 GenRisk-0.2.4/
--rw-r--r--   0 raldisi    (501) staff       (20)     1068 2021-07-21 16:39:45.000000 GenRisk-0.2.4/LICENSE
--rw-r--r--   0 raldisi    (501) staff       (20)     4394 2023-04-24 15:18:02.652768 GenRisk-0.2.4/PKG-INFO
--rw-r--r--   0 raldisi    (501) staff       (20)     3155 2023-03-15 14:48:24.000000 GenRisk-0.2.4/README.md
--rw-r--r--   0 raldisi    (501) staff       (20)      103 2021-10-18 09:34:04.000000 GenRisk-0.2.4/pyproject.toml
--rw-r--r--   0 raldisi    (501) staff       (20)     1193 2023-04-24 15:18:02.653676 GenRisk-0.2.4/setup.cfg
--rw-r--r--   0 raldisi    (501) staff       (20)      115 2021-07-21 16:39:45.000000 GenRisk-0.2.4/setup.py
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 15:18:02.636895 GenRisk-0.2.4/src/
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 15:18:02.642946 GenRisk-0.2.4/src/GenRisk.egg-info/
--rw-r--r--   0 raldisi    (501) staff       (20)     4394 2023-04-24 15:18:02.000000 GenRisk-0.2.4/src/GenRisk.egg-info/PKG-INFO
--rw-r--r--   0 raldisi    (501) staff       (20)      556 2023-04-24 15:18:02.000000 GenRisk-0.2.4/src/GenRisk.egg-info/SOURCES.txt
--rw-r--r--   0 raldisi    (501) staff       (20)        1 2023-04-24 15:18:02.000000 GenRisk-0.2.4/src/GenRisk.egg-info/dependency_links.txt
--rw-r--r--   0 raldisi    (501) staff       (20)       46 2023-04-24 15:18:02.000000 GenRisk-0.2.4/src/GenRisk.egg-info/entry_points.txt
--rw-r--r--   0 raldisi    (501) staff       (20)        1 2021-10-18 14:25:34.000000 GenRisk-0.2.4/src/GenRisk.egg-info/not-zip-safe
--rw-r--r--   0 raldisi    (501) staff       (20)      309 2023-04-24 15:18:02.000000 GenRisk-0.2.4/src/GenRisk.egg-info/requires.txt
--rw-r--r--   0 raldisi    (501) staff       (20)        8 2023-04-24 15:18:02.000000 GenRisk-0.2.4/src/GenRisk.egg-info/top_level.txt
-drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-24 15:18:02.651661 GenRisk-0.2.4/src/genrisk/
--rw-r--r--   0 raldisi    (501) staff       (20)       32 2021-07-21 16:39:45.000000 GenRisk-0.2.4/src/genrisk/__init__.py
--rw-r--r--   0 raldisi    (501) staff       (20)      154 2021-10-12 12:05:52.000000 GenRisk-0.2.4/src/genrisk/__main__.py
--rw-r--r--   0 raldisi    (501) staff       (20)     6945 2023-04-04 12:13:50.000000 GenRisk-0.2.4/src/genrisk/association_analysis.py
--rw-r--r--   0 raldisi    (501) staff       (20)    30612 2023-04-03 19:36:08.000000 GenRisk-0.2.4/src/genrisk/cli.py
--rw-r--r--   0 raldisi    (501) staff       (20)     9589 2023-04-24 11:43:57.000000 GenRisk-0.2.4/src/genrisk/gene_scoring.py
--rw-r--r--   0 raldisi    (501) staff       (20)     3374 2022-08-20 08:52:58.000000 GenRisk-0.2.4/src/genrisk/helpers.py
--rw-r--r--   0 raldisi    (501) staff       (20)    15514 2023-04-24 13:17:29.000000 GenRisk-0.2.4/src/genrisk/pipeline.py
--rw-r--r--   0 raldisi    (501) staff       (20)     7913 2023-04-03 19:34:00.000000 GenRisk-0.2.4/src/genrisk/prediction_models.py
--rw-r--r--   0 raldisi    (501) staff       (20)     2838 2022-02-04 09:26:13.000000 GenRisk-0.2.4/src/genrisk/prs_scoring.py
--rw-r--r--   0 raldisi    (501) staff       (20)     5615 2023-03-22 14:17:27.000000 GenRisk-0.2.4/src/genrisk/utils.py
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-25 07:23:54.057235 GenRisk-0.2.5/
+-rw-r--r--   0 raldisi    (501) staff       (20)     1068 2021-07-21 16:39:45.000000 GenRisk-0.2.5/LICENSE
+-rw-r--r--   0 raldisi    (501) staff       (20)     4394 2023-04-25 07:23:54.057525 GenRisk-0.2.5/PKG-INFO
+-rw-r--r--   0 raldisi    (501) staff       (20)     3155 2023-03-15 14:48:24.000000 GenRisk-0.2.5/README.md
+-rw-r--r--   0 raldisi    (501) staff       (20)      103 2021-10-18 09:34:04.000000 GenRisk-0.2.5/pyproject.toml
+-rw-r--r--   0 raldisi    (501) staff       (20)     1192 2023-04-25 07:23:54.058481 GenRisk-0.2.5/setup.cfg
+-rw-r--r--   0 raldisi    (501) staff       (20)      115 2021-07-21 16:39:45.000000 GenRisk-0.2.5/setup.py
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-25 07:23:54.042239 GenRisk-0.2.5/src/
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-25 07:23:54.047468 GenRisk-0.2.5/src/GenRisk.egg-info/
+-rw-r--r--   0 raldisi    (501) staff       (20)     4394 2023-04-25 07:23:53.000000 GenRisk-0.2.5/src/GenRisk.egg-info/PKG-INFO
+-rw-r--r--   0 raldisi    (501) staff       (20)      556 2023-04-25 07:23:53.000000 GenRisk-0.2.5/src/GenRisk.egg-info/SOURCES.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)        1 2023-04-25 07:23:53.000000 GenRisk-0.2.5/src/GenRisk.egg-info/dependency_links.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)       46 2023-04-25 07:23:53.000000 GenRisk-0.2.5/src/GenRisk.egg-info/entry_points.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)        1 2021-10-18 14:25:34.000000 GenRisk-0.2.5/src/GenRisk.egg-info/not-zip-safe
+-rw-r--r--   0 raldisi    (501) staff       (20)      308 2023-04-25 07:23:53.000000 GenRisk-0.2.5/src/GenRisk.egg-info/requires.txt
+-rw-r--r--   0 raldisi    (501) staff       (20)        8 2023-04-25 07:23:53.000000 GenRisk-0.2.5/src/GenRisk.egg-info/top_level.txt
+drwxr-xr-x   0 raldisi    (501) staff       (20)        0 2023-04-25 07:23:54.056255 GenRisk-0.2.5/src/genrisk/
+-rw-r--r--   0 raldisi    (501) staff       (20)       32 2021-07-21 16:39:45.000000 GenRisk-0.2.5/src/genrisk/__init__.py
+-rw-r--r--   0 raldisi    (501) staff       (20)      154 2021-10-12 12:05:52.000000 GenRisk-0.2.5/src/genrisk/__main__.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     6945 2023-04-04 12:13:50.000000 GenRisk-0.2.5/src/genrisk/association_analysis.py
+-rw-r--r--   0 raldisi    (501) staff       (20)    30612 2023-04-03 19:36:08.000000 GenRisk-0.2.5/src/genrisk/cli.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     9589 2023-04-24 11:43:57.000000 GenRisk-0.2.5/src/genrisk/gene_scoring.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     3374 2022-08-20 08:52:58.000000 GenRisk-0.2.5/src/genrisk/helpers.py
+-rw-r--r--   0 raldisi    (501) staff       (20)    15514 2023-04-24 13:17:29.000000 GenRisk-0.2.5/src/genrisk/pipeline.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     7913 2023-04-03 19:34:00.000000 GenRisk-0.2.5/src/genrisk/prediction_models.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     2838 2022-02-04 09:26:13.000000 GenRisk-0.2.5/src/genrisk/prs_scoring.py
+-rw-r--r--   0 raldisi    (501) staff       (20)     5615 2023-03-22 14:17:27.000000 GenRisk-0.2.5/src/genrisk/utils.py
```

### Comparing `GenRisk-0.2.4/LICENSE` & `GenRisk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/PKG-INFO` & `GenRisk-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenRisk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Comprehensive genetic risk assessment
 Home-page: https://github.com/AldisiRana/genrisk
 Author: Rana Aldisi
 Author-email: aldisi.rana@gmail.com
 License: MIT
 Description: # GenRisk
```

### Comparing `GenRisk-0.2.4/README.md` & `GenRisk-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/setup.cfg` & `GenRisk-0.2.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GenRisk
-version = 0.2.4
+version = 0.2.5
 description = Comprehensive genetic risk assessment
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AldisiRana/genrisk
 author = Rana Aldisi
 author_email = aldisi.rana@gmail.com
 license = MIT
@@ -19,27 +19,27 @@
 	genetics
 	scoring
 	risk
 	comprehensive
 
 [options]
 install_requires = 
-	pandas==1.5.3
-	numpy==1.20.3
-	click==7.1.2
+	pandas>=1.5.3
+	numpy>=1.21.5
+	click>=7.1.2
 	statsmodels==0.13.5
-	scikit-learn==0.23.2
+	scikit-learn==1.2.0
 	scipy==1.5.4
 	tqdm==4.64.1
 	pycaret==3.0.0
 	qmplot==0.3.2
-	matplotlib==3.5.3
+	matplotlib>=3.6.0
 	seaborn==0.12.2
-	setuptools==1.2.0
-	joblib==1.0.1
+	setuptools>=1.2.0
+	joblib==1.2.0
 	adjustText
 	pybiomart
 zip_safe = false
 python_requires = >= 3.7.5
 packages = find:
 package_dir = 
 	= src
```

### Comparing `GenRisk-0.2.4/src/GenRisk.egg-info/PKG-INFO` & `GenRisk-0.2.5/src/GenRisk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenRisk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Comprehensive genetic risk assessment
 Home-page: https://github.com/AldisiRana/genrisk
 Author: Rana Aldisi
 Author-email: aldisi.rana@gmail.com
 License: MIT
 Description: # GenRisk
```

### Comparing `GenRisk-0.2.4/src/GenRisk.egg-info/SOURCES.txt` & `GenRisk-0.2.5/src/GenRisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/association_analysis.py` & `GenRisk-0.2.5/src/genrisk/association_analysis.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/cli.py` & `GenRisk-0.2.5/src/genrisk/cli.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/gene_scoring.py` & `GenRisk-0.2.5/src/genrisk/gene_scoring.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/helpers.py` & `GenRisk-0.2.5/src/genrisk/helpers.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/pipeline.py` & `GenRisk-0.2.5/src/genrisk/pipeline.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/prediction_models.py` & `GenRisk-0.2.5/src/genrisk/prediction_models.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/prs_scoring.py` & `GenRisk-0.2.5/src/genrisk/prs_scoring.py`

 * *Files identical despite different names*

### Comparing `GenRisk-0.2.4/src/genrisk/utils.py` & `GenRisk-0.2.5/src/genrisk/utils.py`

 * *Files identical despite different names*

