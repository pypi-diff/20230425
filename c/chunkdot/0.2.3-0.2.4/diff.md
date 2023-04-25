# Comparing `tmp/chunkdot-0.2.3.tar.gz` & `tmp/chunkdot-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkdot-0.2.3.tar", max compression
+gzip compressed data, was "chunkdot-0.2.4.tar", max compression
```

## Comparing `chunkdot-0.2.3.tar` & `chunkdot-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2839 2023-04-25 01:44:32.276253 chunkdot-0.2.3/README.md
--rw-r--r--   0        0        0      131 2023-04-25 01:45:35.545225 chunkdot-0.2.3/chunkdot/__init__.py
--rw-r--r--   0        0        0     3032 2023-04-24 10:44:08.694869 chunkdot-0.2.3/chunkdot/chunkdot.py
--rw-r--r--   0        0        0     7681 2023-04-24 10:44:18.808767 chunkdot-0.2.3/chunkdot/chunkdot_sparse.py
--rw-r--r--   0        0        0     3966 2023-04-24 10:47:15.290030 chunkdot-0.2.3/chunkdot/cosine_similarity_top_k.py
--rw-r--r--   0        0        0     4094 2023-04-24 10:34:50.140798 chunkdot-0.2.3/chunkdot/numba_argpartition.py
--rw-r--r--   0        0        0     4702 2023-04-24 10:34:50.142160 chunkdot-0.2.3/chunkdot/utils.py
--rw-r--r--   0        0        0     1141 2023-04-25 01:45:34.533039 chunkdot-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 chunkdot-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2869 2023-04-25 01:47:51.729168 chunkdot-0.2.4/README.md
+-rw-r--r--   0        0        0      131 2023-04-25 01:49:13.433855 chunkdot-0.2.4/chunkdot/__init__.py
+-rw-r--r--   0        0        0     3032 2023-04-24 10:44:08.694869 chunkdot-0.2.4/chunkdot/chunkdot.py
+-rw-r--r--   0        0        0     7681 2023-04-24 10:44:18.808767 chunkdot-0.2.4/chunkdot/chunkdot_sparse.py
+-rw-r--r--   0        0        0     3966 2023-04-24 10:47:15.290030 chunkdot-0.2.4/chunkdot/cosine_similarity_top_k.py
+-rw-r--r--   0        0        0     4094 2023-04-24 10:34:50.140798 chunkdot-0.2.4/chunkdot/numba_argpartition.py
+-rw-r--r--   0        0        0     4702 2023-04-24 10:34:50.142160 chunkdot-0.2.4/chunkdot/utils.py
+-rw-r--r--   0        0        0     1141 2023-04-25 01:49:11.535003 chunkdot-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 chunkdot-0.2.4/PKG-INFO
```

### Comparing `chunkdot-0.2.3/README.md` & `chunkdot-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ChunkDot
 
-Multi-threaded matrix multiplication and cosine similarity calculations. Appropriate for calculating the K most similar items for a large number of items by chunking the item matrix representation (embeddings) and using Numba to accelerate the calculations.
+Multi-threaded matrix multiplication and cosine similarity calculations for dense and sparse matrices. Appropriate for calculating the K most similar items for a large number of items by chunking the item matrix representation (embeddings) and using Numba to accelerate the calculations.
 
 ## Related blog posts
 
 - [Cosine Similarity for 1 Trillion Pairs of Vectors
 ](https://pub.towardsai.net/cosine-similarity-for-1-trillion-pairs-of-vectors-11f6a1ed6458)
 - [Bulk Similarity Calculations for Sparse Embeddings
 ](https://pub.towardsai.net/scale-up-bulk-similarity-calculations-for-sparse-embeddings-fb3ecb624727)
```

### Comparing `chunkdot-0.2.3/chunkdot/chunkdot.py` & `chunkdot-0.2.4/chunkdot/chunkdot.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.3/chunkdot/chunkdot_sparse.py` & `chunkdot-0.2.4/chunkdot/chunkdot_sparse.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.3/chunkdot/cosine_similarity_top_k.py` & `chunkdot-0.2.4/chunkdot/cosine_similarity_top_k.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.3/chunkdot/numba_argpartition.py` & `chunkdot-0.2.4/chunkdot/numba_argpartition.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.3/chunkdot/utils.py` & `chunkdot-0.2.4/chunkdot/utils.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.2.3/pyproject.toml` & `chunkdot-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chunkdot"
-version = "0.2.3"
+version = "0.2.4"
 description = "Multi-threaded matrix multiplication and cosine similarity calculations."
 authors = ["Rodrigo Agundez <rragundez@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/rragundez/chunkdot"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
```

### Comparing `chunkdot-0.2.3/PKG-INFO` & `chunkdot-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chunkdot
-Version: 0.2.3
+Version: 0.2.4
 Summary: Multi-threaded matrix multiplication and cosine similarity calculations.
 Home-page: https://github.com/rragundez/chunkdot
 Author: Rodrigo Agundez
 Author-email: rragundez@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,15 +19,15 @@
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/rragundez/chunkdot
 Description-Content-Type: text/markdown
 
 # ChunkDot
 
-Multi-threaded matrix multiplication and cosine similarity calculations. Appropriate for calculating the K most similar items for a large number of items by chunking the item matrix representation (embeddings) and using Numba to accelerate the calculations.
+Multi-threaded matrix multiplication and cosine similarity calculations for dense and sparse matrices. Appropriate for calculating the K most similar items for a large number of items by chunking the item matrix representation (embeddings) and using Numba to accelerate the calculations.
 
 ## Related blog posts
 
 - [Cosine Similarity for 1 Trillion Pairs of Vectors
 ](https://pub.towardsai.net/cosine-similarity-for-1-trillion-pairs-of-vectors-11f6a1ed6458)
 - [Bulk Similarity Calculations for Sparse Embeddings
 ](https://pub.towardsai.net/scale-up-bulk-similarity-calculations-for-sparse-embeddings-fb3ecb624727)
```

