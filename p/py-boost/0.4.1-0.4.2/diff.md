# Comparing `tmp/py_boost-0.4.1.tar.gz` & `tmp/py_boost-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_boost-0.4.1.tar", max compression
+gzip compressed data, was "py_boost-0.4.2.tar", max compression
```

## Comparing `py_boost-0.4.1.tar` & `py_boost-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11361 2023-03-21 17:55:59.930672 py_boost-0.4.1/LICENSE
--rw-r--r--   0        0        0     3636 2023-03-21 17:55:59.930672 py_boost-0.4.1/README.md
--rw-r--r--   0        0        0     1301 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/callbacks/__init__.py
--rw-r--r--   0        0        0     8542 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/callbacks/callback.py
--rw-r--r--   0        0        0      234 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/cv/__init__.py
--rw-r--r--   0        0        0     9356 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/cv/adaptive_es.py
--rw-r--r--   0        0        0     4199 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/cv/base.py
--rw-r--r--   0        0        0     7012 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/cv/cluster_tree.py
--rw-r--r--   0        0        0      120 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/__init__.py
--rw-r--r--   0        0        0    27174 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/base.py
--rw-r--r--   0        0        0    13160 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/boosting.py
--rw-r--r--   0        0        0      457 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/losses/__init__.py
--rw-r--r--   0        0        0     6266 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/losses/losses.py
--rw-r--r--   0        0        0     9368 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/losses/metrics.py
--rw-r--r--   0        0        0     3783 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/losses/multiclass_metrics.py
--rw-r--r--   0        0        0     4691 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/sketch_boost.py
--rw-r--r--   0        0        0    26445 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/tree.py
--rw-r--r--   0        0        0    28118 2023-03-21 17:55:59.930672 py_boost-0.4.1/py_boost/gpu/utils.py
--rw-r--r--   0        0        0       52 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/multioutput/__init__.py
--rw-r--r--   0        0        0     7943 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/multioutput/sketching.py
--rw-r--r--   0        0        0     2362 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/multioutput/target_splitter.py
--rw-r--r--   0        0        0       29 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/quantization/__init__.py
--rw-r--r--   0        0        0     3028 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/quantization/base.py
--rw-r--r--   0        0        0     4061 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/quantization/utils.py
--rw-r--r--   0        0        0       50 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/sampling/__init__.py
--rw-r--r--   0        0        0     6275 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/sampling/bagging.py
--rw-r--r--   0        0        0       35 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/utils/__init__.py
--rw-r--r--   0        0        0     5823 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/utils/logging.py
--rw-r--r--   0        0        0    10338 2023-03-21 17:55:59.934671 py_boost-0.4.1/py_boost/utils/tl_wrapper.py
--rw-r--r--   0        0        0     1083 2023-03-21 17:55:59.934671 py_boost-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 py_boost-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11361 2023-04-25 08:31:35.388767 py_boost-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3636 2023-04-25 08:31:35.388767 py_boost-0.4.2/README.md
+-rw-r--r--   0        0        0     1301 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/callbacks/__init__.py
+-rw-r--r--   0        0        0     8542 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/callbacks/callback.py
+-rw-r--r--   0        0        0      234 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/cv/__init__.py
+-rw-r--r--   0        0        0     9356 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/cv/adaptive_es.py
+-rw-r--r--   0        0        0     4199 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/cv/base.py
+-rw-r--r--   0        0        0     7012 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/cv/cluster_tree.py
+-rw-r--r--   0        0        0      120 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/__init__.py
+-rw-r--r--   0        0        0    27174 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/base.py
+-rw-r--r--   0        0        0    13160 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/boosting.py
+-rw-r--r--   0        0        0      457 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/losses/__init__.py
+-rw-r--r--   0        0        0     6266 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/losses/losses.py
+-rw-r--r--   0        0        0     9368 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/losses/metrics.py
+-rw-r--r--   0        0        0     3783 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/losses/multiclass_metrics.py
+-rw-r--r--   0        0        0     4691 2023-04-25 08:31:35.388767 py_boost-0.4.2/py_boost/gpu/sketch_boost.py
+-rw-r--r--   0        0        0    26445 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/gpu/tree.py
+-rw-r--r--   0        0        0    28118 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/gpu/utils.py
+-rw-r--r--   0        0        0       52 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/multioutput/__init__.py
+-rw-r--r--   0        0        0     7943 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/multioutput/sketching.py
+-rw-r--r--   0        0        0     2362 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/multioutput/target_splitter.py
+-rw-r--r--   0        0        0       29 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/quantization/__init__.py
+-rw-r--r--   0        0        0     3028 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/quantization/base.py
+-rw-r--r--   0        0        0     4061 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/quantization/utils.py
+-rw-r--r--   0        0        0       50 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/sampling/__init__.py
+-rw-r--r--   0        0        0     6275 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/sampling/bagging.py
+-rw-r--r--   0        0        0       35 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/utils/__init__.py
+-rw-r--r--   0        0        0     5823 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/utils/logging.py
+-rw-r--r--   0        0        0    10338 2023-04-25 08:31:35.392767 py_boost-0.4.2/py_boost/utils/tl_wrapper.py
+-rw-r--r--   0        0        0     1247 2023-04-25 08:45:40.268077 py_boost-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5184 1970-01-01 00:00:00.000000 py_boost-0.4.2/PKG-INFO
```

### Comparing `py_boost-0.4.1/LICENSE` & `py_boost-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/README.md` & `py_boost-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/__init__.py` & `py_boost-0.4.2/py_boost/__init__.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/callbacks/callback.py` & `py_boost-0.4.2/py_boost/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/cv/adaptive_es.py` & `py_boost-0.4.2/py_boost/cv/adaptive_es.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/cv/base.py` & `py_boost-0.4.2/py_boost/cv/base.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/cv/cluster_tree.py` & `py_boost-0.4.2/py_boost/cv/cluster_tree.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/base.py` & `py_boost-0.4.2/py_boost/gpu/base.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/boosting.py` & `py_boost-0.4.2/py_boost/gpu/boosting.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/losses/losses.py` & `py_boost-0.4.2/py_boost/gpu/losses/losses.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/losses/metrics.py` & `py_boost-0.4.2/py_boost/gpu/losses/metrics.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/losses/multiclass_metrics.py` & `py_boost-0.4.2/py_boost/gpu/losses/multiclass_metrics.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/sketch_boost.py` & `py_boost-0.4.2/py_boost/gpu/sketch_boost.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/tree.py` & `py_boost-0.4.2/py_boost/gpu/tree.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/gpu/utils.py` & `py_boost-0.4.2/py_boost/gpu/utils.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/multioutput/sketching.py` & `py_boost-0.4.2/py_boost/multioutput/sketching.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/multioutput/target_splitter.py` & `py_boost-0.4.2/py_boost/multioutput/target_splitter.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/quantization/base.py` & `py_boost-0.4.2/py_boost/quantization/base.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/quantization/utils.py` & `py_boost-0.4.2/py_boost/quantization/utils.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/sampling/bagging.py` & `py_boost-0.4.2/py_boost/sampling/bagging.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/utils/logging.py` & `py_boost-0.4.2/py_boost/utils/logging.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/py_boost/utils/tl_wrapper.py` & `py_boost-0.4.2/py_boost/utils/tl_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_boost-0.4.1/pyproject.toml` & `py_boost-0.4.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Py-Boost"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python based GBDT"
 
 authors = ["Vakhrushev Anton <btbpanda@gmail.com>",
            "Iosipoi Leonid",
            "Sergey Kupriyanov"]
            
 readme = "README.md"
@@ -30,16 +30,22 @@
 
 scikit-learn = ">=1"
 numpy = "*"
 joblib = "*"
 numba = "*"
 
 pandas = ">=1"
-treelite = ">=3"
-treelite_runtime = ">=3"
+treelite = [
+    {version = "<3.2,>=3", python = "<3.8"},
+    {version = "^3", python = ">=3.8"}
+]
+treelite_runtime = [
+    {version = "<3.2,>=3", python = "<3.8"},
+    {version = "^3", python = ">=3.8"}
+]
 tqdm = ">=4.64.1"
 
 importlib-metadata = {version = "^1.0", python = "<3.8"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_boost-0.4.1/PKG-INFO` & `py_boost-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-boost
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python based GBDT
 Home-page: https://github.com/AILab-MLTools/Py-Boost
 Author: Vakhrushev Anton
 Author-email: btbpanda@gmail.com
 Requires-Python: >=3.7,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -24,16 +24,18 @@
 Requires-Dist: importlib-metadata (>=1.0,<2.0) ; python_version < "3.8"
 Requires-Dist: joblib
 Requires-Dist: numba
 Requires-Dist: numpy
 Requires-Dist: pandas (>=1)
 Requires-Dist: scikit-learn (>=1)
 Requires-Dist: tqdm (>=4.64.1)
-Requires-Dist: treelite (>=3)
-Requires-Dist: treelite_runtime (>=3)
+Requires-Dist: treelite (>=3,<3.2) ; python_version < "3.8"
+Requires-Dist: treelite (>=3,<4) ; python_version >= "3.8"
+Requires-Dist: treelite_runtime (>=3,<3.2) ; python_version < "3.8"
+Requires-Dist: treelite_runtime (>=3,<4) ; python_version >= "3.8"
 Project-URL: Repository, https://github.com/AILab-MLTools/Py-Boost
 Description-Content-Type: text/markdown
 
 # Py-boost: a research tool for exploring GBDTs
 
 Modern gradient boosting toolkits are very complex and are written in low-level programming languages. As a result,
```

