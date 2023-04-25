# Comparing `tmp/kooplearn-0.1.8.tar.gz` & `tmp/kooplearn-0.1.9.tar.gz`

## Comparing `kooplearn-0.1.8.tar` & `kooplearn-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 kooplearn-0.1.8/docs/_source/conf.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 kooplearn-0.1.8/docs/_source/index.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 kooplearn-0.1.8/docs/_source/installation.rst
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 kooplearn-0.1.8/docs/_source/kooplearn.rst
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kooplearn-0.1.8/docs/_source/modules.rst
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/__about__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/__init__.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/_keops_utils.py
--rw-r--r--   0        0        0    26347 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/estimators.py
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/kernels.py
--rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/utils.py
--rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 kooplearn-0.1.8/kooplearn/__deprecated__/KernelRidge.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 kooplearn-0.1.8/tests/test_QR_decomposition.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 kooplearn-0.1.8/tests/test_check_estimators.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 kooplearn-0.1.8/tests/test_noisy_logistic_map.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 kooplearn-0.1.8/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kooplearn-0.1.8/README.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 kooplearn-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kooplearn-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 kooplearn-0.1.9/docs/_source/conf.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 kooplearn-0.1.9/docs/_source/index.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 kooplearn-0.1.9/docs/_source/installation.rst
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 kooplearn-0.1.9/docs/_source/kooplearn.rst
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 kooplearn-0.1.9/docs/_source/modules.rst
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/__about__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/__init__.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/_keops_utils.py
+-rw-r--r--   0        0        0    26390 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/estimators.py
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/kernels.py
+-rw-r--r--   0        0        0    10446 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/utils.py
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 kooplearn-0.1.9/kooplearn/__deprecated__/KernelRidge.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kooplearn-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 kooplearn-0.1.9/tests/test_QR_decomposition.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 kooplearn-0.1.9/tests/test_check_estimators.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 kooplearn-0.1.9/tests/test_noisy_logistic_map.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 kooplearn-0.1.9/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kooplearn-0.1.9/README.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 kooplearn-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kooplearn-0.1.9/PKG-INFO
```

### Comparing `kooplearn-0.1.8/docs/_source/conf.py` & `kooplearn-0.1.9/docs/_source/conf.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/docs/_source/kooplearn.rst` & `kooplearn-0.1.9/docs/_source/kooplearn.rst`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/kooplearn/_keops_utils.py` & `kooplearn-0.1.9/kooplearn/_keops_utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/kooplearn/estimators.py` & `kooplearn-0.1.9/kooplearn/estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,16 +276,17 @@
             V = sqrt_inv_dim*self.V_
             U = sqrt_inv_dim*self.U_
             
             C = K_vt_Y@V
             D = (K_tv_X.T@U).T
             E = (V.T)@(self.K_Y_@V)
 
-            M = K_v_Y -(C@D + (D.T)@(C.T)) + (val_dim**(-1))*((D.T)@E@(D))
-            return np.sqrt(np.linalg.norm((val_dim**(-1))*M, ord=2))
+            M = (val_dim**(-1))*(K_v_Y -(C@D + (D.T)@(C.T)) + (val_dim**(-1))*((D.T)@E@(D)))
+            sigma_1_sq = np.max(np.linalg.eigvalsh(M))
+            return np.sqrt(sigma_1_sq)
         else:
             raise ValueError(f"Accepted norms are 'HS' (Hilbert-Schmidt) or 'op' (Operator norm), while '{norm}' was provided.")
     def _more_tags(self):
         return {
             'multioutput_only': True,
             'non_deterministic': True,
             'poor_score': True,
```

### Comparing `kooplearn-0.1.8/kooplearn/kernels.py` & `kooplearn-0.1.9/kooplearn/kernels.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/kooplearn/utils.py` & `kooplearn-0.1.9/kooplearn/utils.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/kooplearn/__deprecated__/KernelRidge.py` & `kooplearn-0.1.9/kooplearn/__deprecated__/KernelRidge.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/tests/test_QR_decomposition.py` & `kooplearn-0.1.9/tests/test_QR_decomposition.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/tests/test_check_estimators.py` & `kooplearn-0.1.9/tests/test_check_estimators.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/tests/test_noisy_logistic_map.py` & `kooplearn-0.1.9/tests/test_noisy_logistic_map.py`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/.gitignore` & `kooplearn-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/pyproject.toml` & `kooplearn-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kooplearn-0.1.8/PKG-INFO` & `kooplearn-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kooplearn
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python package implementing ML algorithms to learn the Koopman operator
 Project-URL: Documentation, https://github.com/unknown/kooplearn#readme
 Project-URL: Issues, https://github.com/unknown/kooplearn/issues
 Project-URL: Source, https://github.com/unknown/kooplearn
 Author-email: Pietro Novelli <pietro.novelli@iit.it>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

