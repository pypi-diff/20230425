# Comparing `tmp/chunkdot-0.2.1.tar.gz` & `tmp/chunkdot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkdot-0.2.1.tar", max compression
+gzip compressed data, was "chunkdot-0.2.2.tar", max compression
```

## Comparing `chunkdot-0.2.1.tar` & `chunkdot-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2048 2023-04-18 03:28:46.747971 chunkdot-0.2.1/README.md
--rw-r--r--   0        0        0      131 2023-04-18 03:29:23.762631 chunkdot-0.2.1/chunkdot/__init__.py
--rw-r--r--   0        0        0     2364 2023-04-18 03:25:54.012135 chunkdot-0.2.1/chunkdot/chunkdot.py
--rw-r--r--   0        0        0     7094 2023-04-18 03:25:54.013225 chunkdot-0.2.1/chunkdot/chunkdot_sparse.py
--rw-r--r--   0        0        0     3693 2023-04-18 03:25:54.014044 chunkdot-0.2.1/chunkdot/cosine_similarity_top_k.py
--rw-r--r--   0        0        0     4094 2023-03-08 12:19:56.965969 chunkdot-0.2.1/chunkdot/numba_argpartition.py
--rw-r--r--   0        0        0     4700 2023-04-18 03:25:54.015437 chunkdot-0.2.1/chunkdot/utils.py
--rw-r--r--   0        0        0     1115 2023-04-18 03:29:22.744575 chunkdot-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 chunkdot-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2514 2023-04-24 11:00:37.358458 chunkdot-0.2.2/README.md
+-rw-r--r--   0        0        0      131 2023-04-24 23:00:29.818046 chunkdot-0.2.2/chunkdot/__init__.py
+-rw-r--r--   0        0        0     3032 2023-04-24 10:44:08.694869 chunkdot-0.2.2/chunkdot/chunkdot.py
+-rw-r--r--   0        0        0     7681 2023-04-24 10:44:18.808767 chunkdot-0.2.2/chunkdot/chunkdot_sparse.py
+-rw-r--r--   0        0        0     3966 2023-04-24 10:47:15.290030 chunkdot-0.2.2/chunkdot/cosine_similarity_top_k.py
+-rw-r--r--   0        0        0     4094 2023-04-24 10:34:50.140798 chunkdot-0.2.2/chunkdot/numba_argpartition.py
+-rw-r--r--   0        0        0     4702 2023-04-24 10:34:50.142160 chunkdot-0.2.2/chunkdot/utils.py
+-rw-r--r--   0        0        0     1141 2023-04-24 23:00:28.842449 chunkdot-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 chunkdot-0.2.2/PKG-INFO
```

### Comparing `chunkdot-0.2.1/chunkdot/chunkdot_sparse.py` & `chunkdot-0.2.2/chunkdot/chunkdot_sparse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import math
+
 import numpy as np
 from numba import njit, prange
-from scipy.sparse import csr_matrix, rand as srand
-from chunkdot.utils import to_sparse
+from numba_progress import ProgressBar
+from scipy.sparse import csr_matrix
+from scipy.sparse import rand as srand
 
+from chunkdot.utils import to_sparse
 
 LOGGER = logging.getLogger(__name__)
 
 
 def warm_up_chunkdot_sparse():
     """Make a dummy run of the "chunkdot" function to compile it."""
     matrix = srand(10000, 100, density=0.01, format="csr")
@@ -83,36 +86,38 @@
         data[left_i:right_i],
         indices[left_i:right_i],
         indptr[start_row : end_row + 1] - indptr[start_row],
     )
 
 
 @njit(parallel=True)
-def _chunkdot_sparse_rowwise(
+def _chunkdot_sparse_rowwise(  # pylint: disable=too-many-arguments
     matrix_left_data,
     matrix_left_indices,
     matrix_left_indptr,
     left_n_rows,
     matrix_right_data,
     matrix_right_indices,
     matrix_right_indptr,
     right_n_cols,
     top_k,
     chunk_size,
+    progress_bar=None,
 ):
     """Parallelize the sparse matrix multiplication by converting the left matrix into chunks."""
     # pylint: disable=duplicate-code
     abs_top_k = abs(top_k)
     n_non_zero = left_n_rows * abs_top_k
     all_values, all_indices = (
         np.zeros(n_non_zero, dtype="float64"),
         np.empty(n_non_zero, dtype="int64"),
     )
     # Round up since the in the last iteration chunk <= chunk_size
-    for i in prange(0, math.ceil(left_n_rows / chunk_size)):  # pylint: disable=not-an-iterable
+    num_iterations = math.ceil(left_n_rows / chunk_size)
+    for i in prange(0, num_iterations):  # pylint: disable=not-an-iterable
         start_row_i, end_row_i = i * chunk_size, (i + 1) * chunk_size
         data, indices, indptr = slice_csr_sparse(
             matrix_left_data, matrix_left_indices, matrix_left_indptr, start_row_i, end_row_i
         )
         chunk_m = sparse_dot(
             data,
             indices,
@@ -125,31 +130,37 @@
         )
         to_sparse(
             chunk_m,
             top_k,
             all_values[start_row_i * abs_top_k : end_row_i * abs_top_k],
             all_indices[start_row_i * abs_top_k : end_row_i * abs_top_k],
         )
+        if progress_bar is not None:
+            progress_bar.update(1)
     # standard CSR form representation
     all_indptr = np.arange(0, abs_top_k * (1 + left_n_rows), abs_top_k)
     return all_values, all_indices, all_indptr
 
 
-def chunkdot_sparse(matrix_left, matrix_right, top_k, chunk_size, return_type="float64"):
+def chunkdot_sparse(
+    matrix_left, matrix_right, top_k, chunk_size, return_type="float64", show_progress=False
+):
     """Parallelize sparse matrix multiplication by converting the left matrix into chunks.
 
     Args:
         matrix_left (scipy.sparse.csr_matrix): The left sparse matrix in the matrix multiplication
             operation.
         matrix_right (scipy.sparse.csr_matrix): The right sparse matrix in the matrix
             multiplication operation.
         top_k (int): Keep only the biggest K values per row in the resulting matrix.
         chunk_size (int): The number of rows in the matrix_left to use per parallelized
             calculation.
         return_type (str): The return type of the matrix elements.
+        show_progress (bool): Whether to show tqdm-like progress bar
+            for parallel chunking
 
     Returns:
         scipy.sparse.csr_matrix: The result of the matrix multiplication as a CSR sparse matrix.
     """
     left_n_rows = matrix_left.shape[0]
     right_n_cols = matrix_right.shape[1]
     if matrix_left.shape[1] != matrix_right.shape[0]:
@@ -164,22 +175,29 @@
         matrix_left = matrix_left.tocsr()
 
     right_format = matrix_right.getformat()
     if right_format != "csr":
         LOGGER.debug(f"Converting right matrix format from {right_format.upper()} to CSR.")
         matrix_right = matrix_right.tocsr()
 
+    num_iterations = math.ceil(left_n_rows / chunk_size)
+    progress_bar = ProgressBar(total=num_iterations) if show_progress else None
     values, indices, indptr = _chunkdot_sparse_rowwise(
         matrix_left.data,
         matrix_left.indices,
         matrix_left.indptr,
         left_n_rows,
         matrix_right.data,
         matrix_right.indices,
         matrix_right.indptr,
         right_n_cols,
         top_k,
         chunk_size,
+        progress_bar=progress_bar,
     )
+
+    if progress_bar:
+        progress_bar.close()
+
     return csr_matrix(
         (values.astype(return_type), indices, indptr), shape=(left_n_rows, right_n_cols)
     )
```

### Comparing `chunkdot-0.2.1/chunkdot/cosine_similarity_top_k.py` & `chunkdot-0.2.2/chunkdot/cosine_similarity_top_k.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+from typing import Union
+
 import numpy as np
+
 from scipy import sparse
+
 from chunkdot.chunkdot import chunkdot
 from chunkdot.chunkdot_sparse import chunkdot_sparse
 from chunkdot.utils import get_chunk_size_per_thread
 
 
 def cosine_similarity_top_k(
-    embeddings: np.ndarray,
+    embeddings: Union[np.ndarray, sparse.spmatrix],
     top_k: int,
     normalize: bool = True,
     max_memory: int = None,
     force_memory: bool = False,
+    show_progress: bool = False,
 ):
     """Calculate cosine similarity and only keep the K most similar items for each item.
 
     Args:
         embeddings (np.array or scipy.sparse matrix): 2D object containing the items embeddings,
             of shape number of items x embedding dimension.
         top_k (int): The amount of similar items per item to return.
@@ -25,14 +30,16 @@
             Default None.
         force_memory (bool): Use max_memory even if it is bigger than the memory
             available. This can be desired if the cosine similarity calculation is used many times
             within the same Python process, such that objects are garbage collected but memory is
             not marked as available to the OS. In this case is advised to set max_memory
             to chunkdot.utils.get_memory_available at the start of your Python process.
             Default False.
+        show_progress (bool): Whether to show tqdm-like progress bar
+            on chunked matrix multiplications. False by default.
 
     Returns:
         scipy.sparse.csr_matrix: Sparse matrix containing non-zero values only for the K most
             similar items per item.
 
     Raises:
         ValueError:
@@ -70,14 +77,18 @@
     if abs_top_k >= n_rows:
         raise ValueError(
             f"The number of requested similar items (top_k={abs_top_k}) must be less than the "
             f"total number of items (embeddings.shape[0]={n_rows})"
         )
 
     chunk_size_per_thread = get_chunk_size_per_thread(n_rows, abs_top_k, max_memory, force_memory)
+
     if sparse.issparse(embeddings):
         similarities = chunkdot_sparse(
-            embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type
+            embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type, show_progress
         )
     else:
-        similarities = chunkdot(embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type)
+        similarities = chunkdot(
+            embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type, show_progress
+        )
+
     return similarities
```

### Comparing `chunkdot-0.2.1/chunkdot/numba_argpartition.py` & `chunkdot-0.2.2/chunkdot/numba_argpartition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: skip-file
 
-from numba.extending import overload, register_jitable
 import numpy as np
-from numba.np.arraymath import _asarray, valid_kths, nan_aware_less_than
 from numba import types
+from numba.extending import overload, register_jitable
+from numba.np.arraymath import _asarray, nan_aware_less_than, valid_kths
 
 
 def _partition_factory(pivotimpl, argpartition=False):
     def _partition(A, low, high, I=None):
         mid = (low + high) >> 1
         # NOTE: the pattern of swaps below for the pivot choice and the
         # partitioning gives good results (i.e. regular O(n log n))
```

### Comparing `chunkdot-0.2.1/chunkdot/utils.py` & `chunkdot-0.2.2/chunkdot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import math
 import warnings
-import psutil
+
 import numba
 from numba import njit
 import numpy as np
+import psutil
+
 from chunkdot import numba_argpartition  # pylint: disable=unused-import
 
 LOGGER = logging.getLogger(__name__)
 
 
 # Noting to parallelize in this function. It will raise an error if setting parallel to True since
 # the calling functions are already being parallelized.
```

### Comparing `chunkdot-0.2.1/pyproject.toml` & `chunkdot-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chunkdot"
-version = "0.2.1"
+version = "0.2.2"
 description = "Multi-threaded matrix multiplication and cosine similarity calculations."
 authors = ["Rodrigo Agundez <rragundez@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/rragundez/chunkdot"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
@@ -13,14 +13,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 numba = "^0.56.4"
 numpy = "^1.23"
 scipy = "^1.10.1"
+numba-progress = "^0.0.4"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 scikit-learn = "^1.2.1"
 matplotlib = "^3.7.1"
 black = "^23.1.0"
 pylint = "^2.16.4"
```

### Comparing `chunkdot-0.2.1/PKG-INFO` & `chunkdot-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: chunkdot
-Version: 0.2.1
+Version: 0.2.2
 Summary: Multi-threaded matrix multiplication and cosine similarity calculations.
 Home-page: https://github.com/rragundez/chunkdot
 Author: Rodrigo Agundez
 Author-email: rragundez@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numba-progress (>=0.0.4,<0.0.5)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/rragundez/chunkdot
 Description-Content-Type: text/markdown
 
 # ChunkDot
 
@@ -44,14 +45,23 @@
 # most dissimilar items using 20GB
 cosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)
 ```
 ```
 <100000x100000 sparse matrix of type '<class 'numpy.float64'>'
  with 5000000 stored elements in Compressed Sparse Row format>
 ```
+```python
+# with progress bar
+cosine_similarity_top_k(embeddings, top_k=50, show_progress=True)
+```
+```
+100%|███████████████████████████████████████████████████████████████| 129.0/129 [01:04<00:00,  1.80it/s]
+<100000x100000 sparse matrix of type '<class 'numpy.float64'>'
+  with 5000000 stored elements in Compressed Sparse Row format>
+```
 
 Execution time
 ```python
 from timeit import timeit
 import numpy as np
 from chunkdot import cosine_similarity_top_k
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

