# Comparing `tmp/ptwt-0.1.4.post2.tar.gz` & `tmp/ptwt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptwt-0.1.4.post2.tar", last modified: Tue Nov 15 12:22:31 2022, max compression
+gzip compressed data, was "ptwt-0.1.5.tar", last modified: Tue Apr 25 08:28:29 2023, max compression
```

## Comparing `ptwt-0.1.4.post2.tar` & `ptwt-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,41 @@
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2022-11-15 12:22:31.926517 ptwt-0.1.4.post2/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    14013 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/LICENSE
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8458 2022-11-15 12:22:31.926517 ptwt-0.1.4.post2/PKG-INFO
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     7244 2022-11-07 09:51:57.000000 ptwt-0.1.4.post2/README.rst
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1369 2022-11-15 12:22:31.926517 ptwt-0.1.4.post2/setup.cfg
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      115 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/setup.py
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2022-11-15 12:22:31.922516 ptwt-0.1.4.post2/src/
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2022-11-15 12:22:31.926517 ptwt-0.1.4.post2/src/ptwt/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      428 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/src/ptwt/__init__.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     3296 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/src/ptwt/_mackey_glass.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1485 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/src/ptwt/_util.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    11176 2022-10-24 11:20:48.000000 ptwt-0.1.4.post2/src/ptwt/continuous_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     9951 2022-11-07 09:53:32.000000 ptwt-0.1.4.post2/src/ptwt/conv_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     7576 2022-11-07 09:52:50.000000 ptwt-0.1.4.post2/src/ptwt/conv_transform_2.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     7749 2022-10-12 09:04:00.000000 ptwt-0.1.4.post2/src/ptwt/conv_transform_3.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    22874 2022-11-07 09:54:27.000000 ptwt-0.1.4.post2/src/ptwt/matmul_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    33291 2022-10-12 09:04:00.000000 ptwt-0.1.4.post2/src/ptwt/matmul_transform_2.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    19037 2022-11-07 09:54:51.000000 ptwt-0.1.4.post2/src/ptwt/packets.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    19427 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/src/ptwt/sparse_math.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      992 2022-11-15 12:20:22.000000 ptwt-0.1.4.post2/src/ptwt/version.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    10275 2022-06-08 12:13:31.000000 ptwt-0.1.4.post2/src/ptwt/wavelets_learnable.py
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2022-11-15 12:22:31.926517 ptwt-0.1.4.post2/src/ptwt.egg-info/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8458 2022-11-15 12:22:31.000000 ptwt-0.1.4.post2/src/ptwt.egg-info/PKG-INFO
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      534 2022-11-15 12:22:31.000000 ptwt-0.1.4.post2/src/ptwt.egg-info/SOURCES.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)        1 2022-11-15 12:22:31.000000 ptwt-0.1.4.post2/src/ptwt.egg-info/dependency_links.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)       40 2022-11-15 12:22:31.000000 ptwt-0.1.4.post2/src/ptwt.egg-info/requires.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)        5 2022-11-15 12:22:31.000000 ptwt-0.1.4.post2/src/ptwt.egg-info/top_level.txt
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.288498 ptwt-0.1.5/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    14013 2022-06-08 12:13:31.000000 ptwt-0.1.5/LICENSE
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8791 2023-04-25 08:28:29.288498 ptwt-0.1.5/PKG-INFO
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     7653 2023-04-25 08:12:55.000000 ptwt-0.1.5/README.rst
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1350 2023-04-25 08:28:29.288498 ptwt-0.1.5/setup.cfg
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      115 2022-06-08 12:13:31.000000 ptwt-0.1.5/setup.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/src/
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/src/ptwt/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      603 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/__init__.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1989 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/_util.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11257 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/continuous_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11636 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/conv_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     9066 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/conv_transform_2.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     9342 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/conv_transform_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    22734 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/matmul_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    32359 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/matmul_transform_2.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    16716 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/matmul_transform_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    21343 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/packets.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    13612 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/separable_conv_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    20237 2023-04-25 08:12:55.000000 ptwt-0.1.5/src/ptwt/sparse_math.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      986 2023-04-25 08:20:47.000000 ptwt-0.1.5/src/ptwt/version.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    10275 2022-06-08 12:13:31.000000 ptwt-0.1.5/src/ptwt/wavelets_learnable.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/src/ptwt.egg-info/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8791 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/PKG-INFO
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      875 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/SOURCES.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)        1 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/dependency_links.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)       63 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/requires.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)        5 2023-04-25 08:28:29.000000 ptwt-0.1.5/src/ptwt.egg-info/top_level.txt
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-04-25 08:28:29.284499 ptwt-0.1.5/tests/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8187 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_convolution_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     2637 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_convolution_fwt_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     3961 2022-10-24 11:21:37.000000 ptwt-0.1.5/tests/test_cwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     6477 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_jit.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     7206 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_matrix_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8091 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_matrix_fwt_2.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     3090 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_matrix_fwt_3.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    11918 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_packets.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     5702 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_separable_conv_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    10862 2023-04-25 08:12:55.000000 ptwt-0.1.5/tests/test_sparse_math.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1048 2022-06-08 12:13:31.000000 ptwt-0.1.5/tests/test_util.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1316 2022-06-08 12:13:31.000000 ptwt-0.1.5/tests/test_wavelet.py
```

### Comparing `ptwt-0.1.4.post2/LICENSE` & `ptwt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.4.post2/PKG-INFO` & `ptwt-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: ptwt
-Version: 0.1.4.post2
+Version: 0.1.5
 Summary: Differentiable and gpu enabled fast wavelet transforms in PyTorch
 Home-page: https://github.com/v0lta/PyTorch-Wavelet-Toolbox
 Download-URL: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
 Author: Moritz Wolter
 Author-email: moritz@wolter.tech
 Maintainer: Moritz Wolter
 Maintainer-email: moritz@wolter.tech
 License: EUPL-1.2
 Project-URL: Bug Tracker, https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
 Project-URL: Source Code, https://github.com/v0lta/PyTorch-Wavelet-Toolbox
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ********************************
 Pytorch Wavelet Toolbox (`ptwt`)
@@ -55,27 +53,30 @@
     :alt: Black code style
 
 .. image:: https://static.pepy.tech/personalized-badge/ptwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
  :target: https://pepy.tech/project/ptwt
 
 
 
+
 Welcome to the PyTorch wavelet toolbox. This package implements:
 
 - the fast wavelet transform (fwt) via ``wavedec`` and its inverse by providing the ``waverec`` function,
 - the two-dimensional fwt is called ``wavedec2`` the synthesis counterpart ``waverec2``,
 - ``wavedec3`` and ``waverec3`` cover the three-dimensional analysis and synthesis case,
-- ``MatrixWavedec`` and ``MatrixWaverec`` provide sparse-matrix-based fast wavelet transforms with boundary filters,
-- 2d sparse-matrix transforms with separable & non-separable boundary filters are available (experimental),
+- ``fswavedec2``, ``fswavedec3``, ``fswaverec2`` and ``fswaverec3`` support separable transformations.
+- ``MatrixWavedec`` and ``MatrixWaverec`` implement sparse-matrix-based fast wavelet transforms with boundary filters,
+- 2d sparse-matrix transforms with separable & non-separable boundary filters are available,
+- ``MatrixWavedec3`` and ``MatrixWaverec3`` allow separable 3D-fwt's with boundary filters.
 - ``cwt`` computes a one-dimensional continuous forward transform,
 - single and two-dimensional wavelet packet forward and backward transforms are available via the ``WaveletPacket`` and ``WaveletPacket2D`` objects,
 - finally, this package provides adaptive wavelet support (experimental).
 
-This toolbox supports pywt-wavelets. Complete documentation is available:
-https://pytorch-wavelet-toolbox.readthedocs.io/
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+Complete documentation is available at: https://pytorch-wavelet-toolbox.readthedocs.io/
 
 
 **Installation**
 
 Install the toolbox via pip or clone this repository. In order to use ``pip``, type:
 
 .. code-block:: sh
@@ -128,15 +129,15 @@
 
 .. code-block:: python
 
   import ptwt, pywt, torch
   import numpy as np
   import scipy.misc
 
-  face = np.transpose(scipy.misc.face(),
+  face = np.transpose(scipy.datasets.face(),
                           [2, 0, 1]).astype(np.float64)
   pytorch_face = torch.tensor(face)
   coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
                                   level=2, mode="constant")
   reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
   np.max(np.abs(face - reconstruction.squeeze(1).numpy()))
 
@@ -170,16 +171,16 @@
   # backward 
   matrix_waverec = ptwt.MatrixWaverec(pywt.Wavelet("haar"))
   rec = matrix_waverec(coeff)
   print(rec)
 
 
 The process for the 2d transforms ``MatrixWavedec2``, ``MatrixWaverec2`` works similarly.
-By default, a non-separable transformation is used.
-To use a separable transformation, pass ``separable=True`` to ``MatrixWavedec2`` and ``MatrixWaverec2``.
+By default, a separable transformation is used.
+To use a non-separable transformation, pass ``separable=False`` to ``MatrixWavedec2`` and ``MatrixWaverec2``.
 Separable transformations use a 1d transformation along both axes, which might be faster since fewer matrix entries
 have to be orthogonalized.
 
 
 **Adaptive** **Wavelets**
 
 Experimental code to train an adaptive wavelet layer in PyTorch is available in the ``examples`` folder. In addition to static wavelets
@@ -189,23 +190,26 @@
 - and optimizable orthogonal-wavelets are supported.
 
 See https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/network_compression/ for a complete implementation.
 
 
 **Testing**
 
-The ``tests`` folder contains multiple tests to allow independent verification of this toolbox. After cloning the
-repository, and moving into the main directory, and installing ``nox`` with ``pip install nox`` run:
+The ``tests`` folder contains multiple tests to allow independent verification of this toolbox.
+The GitHub workflow executes a subset of all tests for efficiency reasons. 
+After cloning the repository, moving into the main directory, and installing ``nox`` with ``pip install nox`` run
 
 .. code-block:: sh
 
   $ nox --session test
 
 
 
+to run all existing tests.
+
 Citation
 """"""""
 
 If you use this work in a scientific context please cite:
 
 .. code-block::
 
@@ -228,9 +232,7 @@
     title = {{Randbehandlung bei Wavelets für Faltungsnetzwerke}},
     type = {Bachelor's Thesis},
     annote = {Gbachelor},
     year = {2021},
     school = {Institut f\"ur Numerische Simulation, Universit\"at Bonn}
   }
 
-
-
```

### Comparing `ptwt-0.1.4.post2/README.rst` & `ptwt-0.1.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,30 @@
     :alt: Black code style
 
 .. image:: https://static.pepy.tech/personalized-badge/ptwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
  :target: https://pepy.tech/project/ptwt
 
 
 
+
 Welcome to the PyTorch wavelet toolbox. This package implements:
 
 - the fast wavelet transform (fwt) via ``wavedec`` and its inverse by providing the ``waverec`` function,
 - the two-dimensional fwt is called ``wavedec2`` the synthesis counterpart ``waverec2``,
 - ``wavedec3`` and ``waverec3`` cover the three-dimensional analysis and synthesis case,
-- ``MatrixWavedec`` and ``MatrixWaverec`` provide sparse-matrix-based fast wavelet transforms with boundary filters,
-- 2d sparse-matrix transforms with separable & non-separable boundary filters are available (experimental),
+- ``fswavedec2``, ``fswavedec3``, ``fswaverec2`` and ``fswaverec3`` support separable transformations.
+- ``MatrixWavedec`` and ``MatrixWaverec`` implement sparse-matrix-based fast wavelet transforms with boundary filters,
+- 2d sparse-matrix transforms with separable & non-separable boundary filters are available,
+- ``MatrixWavedec3`` and ``MatrixWaverec3`` allow separable 3D-fwt's with boundary filters.
 - ``cwt`` computes a one-dimensional continuous forward transform,
 - single and two-dimensional wavelet packet forward and backward transforms are available via the ``WaveletPacket`` and ``WaveletPacket2D`` objects,
 - finally, this package provides adaptive wavelet support (experimental).
 
-This toolbox supports pywt-wavelets. Complete documentation is available:
-https://pytorch-wavelet-toolbox.readthedocs.io/
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+Complete documentation is available at: https://pytorch-wavelet-toolbox.readthedocs.io/
 
 
 **Installation**
 
 Install the toolbox via pip or clone this repository. In order to use ``pip``, type:
 
 .. code-block:: sh
@@ -100,15 +103,15 @@
 
 .. code-block:: python
 
   import ptwt, pywt, torch
   import numpy as np
   import scipy.misc
 
-  face = np.transpose(scipy.misc.face(),
+  face = np.transpose(scipy.datasets.face(),
                           [2, 0, 1]).astype(np.float64)
   pytorch_face = torch.tensor(face)
   coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
                                   level=2, mode="constant")
   reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
   np.max(np.abs(face - reconstruction.squeeze(1).numpy()))
 
@@ -142,16 +145,16 @@
   # backward 
   matrix_waverec = ptwt.MatrixWaverec(pywt.Wavelet("haar"))
   rec = matrix_waverec(coeff)
   print(rec)
 
 
 The process for the 2d transforms ``MatrixWavedec2``, ``MatrixWaverec2`` works similarly.
-By default, a non-separable transformation is used.
-To use a separable transformation, pass ``separable=True`` to ``MatrixWavedec2`` and ``MatrixWaverec2``.
+By default, a separable transformation is used.
+To use a non-separable transformation, pass ``separable=False`` to ``MatrixWavedec2`` and ``MatrixWaverec2``.
 Separable transformations use a 1d transformation along both axes, which might be faster since fewer matrix entries
 have to be orthogonalized.
 
 
 **Adaptive** **Wavelets**
 
 Experimental code to train an adaptive wavelet layer in PyTorch is available in the ``examples`` folder. In addition to static wavelets
@@ -161,23 +164,26 @@
 - and optimizable orthogonal-wavelets are supported.
 
 See https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/network_compression/ for a complete implementation.
 
 
 **Testing**
 
-The ``tests`` folder contains multiple tests to allow independent verification of this toolbox. After cloning the
-repository, and moving into the main directory, and installing ``nox`` with ``pip install nox`` run:
+The ``tests`` folder contains multiple tests to allow independent verification of this toolbox.
+The GitHub workflow executes a subset of all tests for efficiency reasons. 
+After cloning the repository, moving into the main directory, and installing ``nox`` with ``pip install nox`` run
 
 .. code-block:: sh
 
   $ nox --session test
 
 
 
+to run all existing tests.
+
 Citation
 """"""""
 
 If you use this work in a scientific context please cite:
 
 .. code-block::
```

### Comparing `ptwt-0.1.4.post2/setup.cfg` & `ptwt-0.1.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ptwt
-version = 0.1.4.post2
+version = 0.1.5
 description = Differentiable and gpu enabled fast wavelet transforms in PyTorch
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/v0lta/PyTorch-Wavelet-Toolbox
 download_url = https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
 project_urls = 
 	Bug Tracker = https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
@@ -19,26 +19,28 @@
 	License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 
 [options]
 install_requires = 
 	PyWavelets
 	torch
-	scipy
+	scipy>=1.10
+	pooch
 	matplotlib
 	numpy
+	pytest
+	nox
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/_util.py` & `ptwt-0.1.5/src/ptwt/_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Utility methods to compute wavelet decompositions from a dataset."""
-from typing import Protocol, Sequence, Tuple, Union
+from typing import Optional, Protocol, Sequence, Tuple, Union
 
 import pywt
 import torch
 
 
 class Wavelet(Protocol):
     """Wavelet object interface, based on the pywt wavelet object."""
@@ -15,14 +15,18 @@
     rec_hi: Sequence[float]
     dec_len: int
     rec_len: int
     filter_bank: Tuple[
         Sequence[float], Sequence[float], Sequence[float], Sequence[float]
     ]
 
+    def __len__(self) -> int:
+        """Return the number of filter coefficients."""
+        return len(self.dec_lo)
+
 
 def _as_wavelet(wavelet: Union[Wavelet, str]) -> Wavelet:
     """Ensure the input argument to be a pywt wavelet compatible object.
 
     Args:
         wavelet (Wavelet or str): The input argument, which is either a
             pywt wavelet compatible object or a valid pywt wavelet name string.
@@ -33,18 +37,30 @@
     """
     if isinstance(wavelet, str):
         return pywt.Wavelet(wavelet)
     else:
         return wavelet
 
 
-def _is_boundary_mode_supported(boundary_mode: str) -> bool:
-    return boundary_mode == "qr" or boundary_mode == "gramschmidt"
+def _is_boundary_mode_supported(boundary_mode: Optional[str]) -> bool:
+    return boundary_mode in ["qr", "gramschmidt"]
+
+
+def _is_dtype_supported(dtype: torch.dtype) -> bool:
+    return dtype in [torch.float32, torch.float64]
 
 
 def _outer(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
     """Torch implementation of numpy's outer for 1d vectors."""
     a_flat = torch.reshape(a, [-1])
     b_flat = torch.reshape(b, [-1])
     a_mul = torch.unsqueeze(a_flat, dim=-1)
     b_mul = torch.unsqueeze(b_flat, dim=0)
     return a_mul * b_mul
+
+
+def _get_len(wavelet: Union[Tuple[torch.Tensor, ...], str, Wavelet]) -> int:
+    """Get number of filter coefficients for various wavelet data types."""
+    if isinstance(wavelet, tuple):
+        return wavelet[0].shape[0]
+    else:
+        return len(_as_wavelet(wavelet))
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/continuous_transform.py` & `ptwt-0.1.5/src/ptwt/continuous_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """PyTorch compatible cwt code.
 
-Based on https://github.com/PyWavelets/pywt/blob/master/pywt/_cwt.py
+This module is based on pywt's cwt implementation.
 """
 from typing import Any, Tuple, Union
 
 import numpy as np
 import torch
 from pywt import ContinuousWavelet, DiscreteContinuousWavelet, Wavelet
 from pywt._functions import scale2frequency
@@ -35,27 +35,27 @@
     Args:
         data (torch.Tensor): The input tensor of shape [batch_size, time].
         scales (torch.Tensor or np.array):
             The wavelet scales to use. One can use
             ``f = pywt.scale2frequency(wavelet, scale)/sampling_period`` to determine
             what physical frequency, ``f``. Here, ``f`` is in hertz when the
             ``sampling_period`` is given in seconds.
-            wavelet (str or Wavelet of ContinuousWavelet): The wavelet to work with.
         wavelet (ContinuousWavelet or str): The continuous wavelet to work with.
         sampling_period (float): Sampling period for the frequencies output (optional).
             The values computed for ``coefs`` are independent of the choice of
             ``sampling_period`` (i.e. ``scales`` is not scaled by the sampling
             period).
 
     Raises:
         ValueError: If a scale is too small for the input signal.
 
     Returns:
-        Tuple[torch.Tensor, np.ndarray]: A tuple with the transformation matrix
-            and frequencies in this order.
+        Tuple[torch.Tensor, np.ndarray]: The first tuple-element contains
+            the transformation matrix of shape [scales, batch, time].
+            The second element contains an array with frequency information.
 
     Example:
         >>> import torch, ptwt
         >>> import numpy as np
         >>> import scipy.signal as signal
         >>> t = np.linspace(-2, 2, 800, endpoint=False)
         >>> sig = signal.chirp(t, f0=1, f1=12, t1=2, method="linear")
@@ -70,24 +70,24 @@
     ):
         wavelet = DiscreteContinuousWavelet(wavelet)
     if type(scales) is torch.Tensor:
         scales = scales.numpy()
     elif np.isscalar(scales):
         scales = np.array([scales])
 
-    if isinstance(wavelet, _DifferentiableContinuousWavelet):
+    if isinstance(wavelet, torch.nn.Module):
         if data.is_cuda:
             wavelet.cuda()
 
     precision = 10
     int_psi, x = _integrate_wavelet(wavelet, precision=precision)
     if type(wavelet) is ContinuousWavelet:
         int_psi = np.conj(int_psi) if wavelet.complex_cwt else int_psi
         int_psi = torch.tensor(int_psi, device=data.device)
-    elif isinstance(wavelet, _DifferentiableContinuousWavelet):
+    elif isinstance(wavelet, torch.nn.Module):
         int_psi = torch.conj(int_psi) if wavelet.complex_cwt else int_psi
     else:
         int_psi = torch.tensor(int_psi, device=data.device)
         x = torch.tensor(x, device=data.device)
 
     # convert int_psi, x to the same precision as the data
     # x = np.asarray(x, dtype=data.cpu().numpy().real.dtype)
@@ -221,31 +221,37 @@
 
     else:  # biorthogonal wavelet
         _, psi_d, _, psi_r, x = functions_approximations
         step = x[1] - x[0]
         return _integrate(psi_d, step), _integrate(psi_r, step), x
 
 
+class _WaveletParameter(torch.nn.Parameter):
+    pass
+
+
 class _DifferentiableContinuousWavelet(
     torch.nn.Module, ContinuousWavelet  # type: ignore
 ):
     """A base class for learnable Continuous Wavelets."""
 
     def __init__(self, name: str):
         """Create a trainable shannon wavelet."""
         super().__init__()
         super(ContinuousWavelet, self).__init__()
 
         self.dtype = torch.float64
         # Use torch nn parameter
-        self.bandwidth_par = torch.nn.Parameter(
-            torch.sqrt(torch.tensor(self.bandwidth_frequency, dtype=self.dtype))
+        self.bandwidth_par = _WaveletParameter(
+            torch.sqrt(torch.tensor(self.bandwidth_frequency, dtype=self.dtype)),
+            requires_grad=True,
         )
-        self.center_par = torch.nn.Parameter(
-            torch.sqrt(torch.tensor(self.center_frequency, dtype=self.dtype))
+        self.center_par = _WaveletParameter(
+            torch.sqrt(torch.tensor(self.center_frequency, dtype=self.dtype)),
+            requires_grad=True,
         )
 
     def __call__(self, grid_values: torch.Tensor) -> torch.Tensor:
         """Return numerical values for the wavelet on a grid."""
         raise NotImplementedError
 
     @property
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/conv_transform.py` & `ptwt-0.1.5/src/ptwt/conv_transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,81 @@
-"""Fast wavelet transformation code with edge-padding."""
+"""Fast wavelet transformations based on torch.nn.functional.conv1d and its transpose.
+
+This module treats boundaries with edge-padding.
+"""
 # Created by moritz wolter, 14.04.20
 from typing import List, Optional, Sequence, Tuple, Union
 
 import pywt
 import torch
 
-from ._util import Wavelet, _as_wavelet
+from ._util import Wavelet, _as_wavelet, _get_len, _is_dtype_supported
+
+
+def _create_tensor(
+    filter: Sequence[float], flip: bool, device: torch.device, dtype: torch.dtype
+) -> torch.Tensor:
+    if flip:
+        if isinstance(filter, torch.Tensor):
+            return filter.flip(-1).unsqueeze(0).to(device=device, dtype=dtype)
+        else:
+            return torch.tensor(filter[::-1], device=device, dtype=dtype).unsqueeze(0)
+    else:
+        if isinstance(filter, torch.Tensor):
+            return filter.unsqueeze(0).to(device=device, dtype=dtype)
+        else:
+            return torch.tensor(filter, device=device, dtype=dtype).unsqueeze(0)
 
 
 def get_filter_tensors(
     wavelet: Union[Wavelet, str],
     flip: bool,
     device: Union[torch.device, str],
     dtype: torch.dtype = torch.float32,
 ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
     """Convert input wavelet to filter tensors.
 
     Args:
         wavelet (Wavelet or str): A pywt wavelet compatible object or
-                the name of a pywt wavelet.
-        flip (bool): If true filters are flipped.
-        device (torch.device) : PyTorch target device.
+            the name of a pywt wavelet.
+        flip (bool): Flip filters left-right, if true.
+        device (torch.device or str): PyTorch target device.
         dtype (torch.dtype): The data type sets the precision of the
                computation. Default: torch.float32.
 
     Returns:
         tuple: Tuple containing the four filter tensors
         dec_lo, dec_hi, rec_lo, rec_hi
 
     """
     wavelet = _as_wavelet(wavelet)
+    device = torch.device(device)
 
-    def _create_tensor(filter: Sequence[float]) -> torch.Tensor:
-        if flip:
-            if isinstance(filter, torch.Tensor):
-                return filter.flip(-1).unsqueeze(0).to(device)
-            else:
-                return torch.tensor(filter[::-1], device=device, dtype=dtype).unsqueeze(
-                    0
-                )
-        else:
-            if isinstance(filter, torch.Tensor):
-                return filter.unsqueeze(0).to(device)
-            else:
-                return torch.tensor(filter, device=device, dtype=dtype).unsqueeze(0)
-
-    dec_lo, dec_hi, rec_lo, rec_hi = wavelet.filter_bank
-    dec_lo_tensor = _create_tensor(dec_lo)
-    dec_hi_tensor = _create_tensor(dec_hi)
-    rec_lo_tensor = _create_tensor(rec_lo)
-    rec_hi_tensor = _create_tensor(rec_hi)
+    if isinstance(wavelet, tuple):
+        dec_lo, dec_hi, rec_lo, rec_hi = wavelet
+    else:
+        dec_lo, dec_hi, rec_lo, rec_hi = wavelet.filter_bank
+    dec_lo_tensor = _create_tensor(dec_lo, flip, device, dtype)
+    dec_hi_tensor = _create_tensor(dec_hi, flip, device, dtype)
+    rec_lo_tensor = _create_tensor(rec_lo, flip, device, dtype)
+    rec_hi_tensor = _create_tensor(rec_hi, flip, device, dtype)
     return dec_lo_tensor, dec_hi_tensor, rec_lo_tensor, rec_hi_tensor
 
 
 def _get_pad(data_len: int, filt_len: int) -> Tuple[int, int]:
     """Compute the required padding.
 
     Args:
         data_len (int): The length of the input vector.
-        filt_len (int): The length of the used filter.
+        filt_len (int): The size of the used filter.
 
     Returns:
-        tuple: The numbers to attach on the edges of the input.
+        Tuple: The first entry specifies how many numbers
+            to attach on the right. The second
+            entry covers the left side.
 
     """
     # pad to ensure we see all filter positions and
     # for pywt compatability.
     # convolution output length:
     # see https://arxiv.org/pdf/1603.07285.pdf section 2.3:
     # floor([data_len - filt_len]/2) + 1
@@ -84,19 +94,19 @@
     if data_len % 2 != 0:
         padr += 1
 
     return padr, padl
 
 
 def _translate_boundary_strings(pywt_mode: str) -> str:
-    """Translate pywt mode strings to pytorch mode strings.
+    """Translate pywt mode strings to PyTorch mode strings.
 
-    We support constant, zero, reflect and periodic.
-    Unfortunately "constant" has different meanings in the
-    pytorch and pywavelet communities.
+    We support constant, zero, reflect, and periodic.
+    Unfortunately, "constant" has different meanings in the
+    Pytorch and PyWavelet communities.
 
     Raises:
         ValueError: If the padding mode is not supported.
 
     """
     if pywt_mode == "constant":
         pt_mode = "replicate"
@@ -107,40 +117,44 @@
     elif pywt_mode == "periodic":
         pt_mode = "circular"
     else:
         raise ValueError("Padding mode not supported.")
     return pt_mode
 
 
-def fwt_pad(
+def _fwt_pad(
     data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str = "reflect"
 ) -> torch.Tensor:
     """Pad the input signal to make the fwt matrix work.
 
+    The padding assumes a future step will transform the last axis.
+
     Args:
         data (torch.Tensor): Input data [batch_size, 1, time]
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
-        mode (str): The desired way to pad.
-            Supported modes are "reflect", "zero", "constant" and "periodic".
+        mode (str): The desired way to pad. The following methods are supported::
+
+                "reflect", "zero", "constant", "periodic".
+
             Refection padding mirrors samples along the border.
             Zero padding pads zeros.
             Constant padding replicates border values.
-            periodic padding repeats samples in a cyclic fashing.
-            Defaults to reflect.
+            Periodic padding cyclically repeats samples.
+            This function defaults to reflect.
 
     Returns:
-        torch.Tensor: A pytorch tensor with the padded input data
+        torch.Tensor: A PyTorch tensor with the padded input data
 
     """
     wavelet = _as_wavelet(wavelet)
     # convert pywt to pytorch convention.
     mode = _translate_boundary_strings(mode)
 
-    padr, padl = _get_pad(data.shape[-1], len(wavelet.dec_lo))
+    padr, padl = _get_pad(data.shape[-1], _get_len(wavelet))
     data_pad = torch.nn.functional.pad(data, [padl, padr], mode=mode)
     return data_pad
 
 
 def _flatten_2d_coeff_lst(
     coeff_lst_2d: List[
         Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
@@ -168,39 +182,64 @@
             if flatten_tensors:
                 flat_coeff_lst.append(coeff.flatten())
             else:
                 flat_coeff_lst.append(coeff)
     return flat_coeff_lst
 
 
+def _adjust_padding_at_reconstruction(
+    res_ll_size: int, coeff_size: int, pad_end: int, pad_start: int
+) -> Tuple[int, int]:
+    pred_size = res_ll_size - (pad_start + pad_end)
+    next_size = coeff_size
+    if next_size == pred_size:
+        pass
+    elif next_size == pred_size - 1:
+        pad_end += 1
+    else:
+        raise AssertionError("padding error, please open an issue on github")
+    return pad_end, pad_start
+
+
 def wavedec(
     data: torch.Tensor,
     wavelet: Union[Wavelet, str],
-    level: Optional[int] = None,
     mode: str = "reflect",
+    level: Optional[int] = None,
 ) -> List[torch.Tensor]:
     """Compute the analysis (forward) 1d fast wavelet transform.
 
     Args:
         data (torch.Tensor): Input time series of shape [batch_size, 1, time]
                              1d inputs are interpreted as [time],
                              2d inputs are interpreted as [batch_size, time].
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
+            Please consider the output from ``pywt.wavelist(kind='discrete')``
+            for possible choices.
+        mode (str): The desired padding mode. Padding extends the signal along
+            the edges. Supported methods are::
+
+                "reflect", "zero", "constant", "periodic".
+
+            Defaults to "reflect".
         level (int): The scale level to be computed.
                                Defaults to None.
-        mode (str): The desired padding mode. Padding extends the singal along
-            the edges. Supported modes are "reflect", "zero", "constant"
-            and "periodic". Defaults to "reflect".
 
     Returns:
-        list: A list [cA_n, cD_n, cD_n-1, …, cD2, cD1]
+        list: A list::
+
+            [cA_n, cD_n, cD_n-1, …, cD2, cD1]
+
         containing the wavelet coefficients. A denotes
         approximation and D detail coefficients.
 
+    Raises:
+        ValueError: If the dtype of the input data tensor is unsupported.
+
     Example:
         >>> import torch
         >>> import ptwt, pywt
         >>> import numpy as np
         >>> # generate an input of even length.
         >>> data = np.array([0, 1, 2, 3, 4, 5, 5, 4, 3, 2, 1, 0])
         >>> data_torch = torch.from_numpy(data.astype(np.float32))
@@ -212,27 +251,30 @@
     if data.dim() == 1:
         # assume time series
         data = data.unsqueeze(0).unsqueeze(0)
     elif data.dim() == 2:
         # assume batched time series
         data = data.unsqueeze(1)
 
+    if not _is_dtype_supported(data.dtype):
+        raise ValueError(f"Input dtype {data.dtype} not supported")
+
     dec_lo, dec_hi, _, _ = get_filter_tensors(
         wavelet, flip=True, device=data.device, dtype=data.dtype
     )
     filt_len = dec_lo.shape[-1]
     filt = torch.stack([dec_lo, dec_hi], 0)
 
     if level is None:
         level = pywt.dwt_max_level(data.shape[-1], filt_len)
 
     result_lst = []
     res_lo = data
     for _ in range(level):
-        res_lo = fwt_pad(res_lo, wavelet, mode=mode)
+        res_lo = _fwt_pad(res_lo, wavelet, mode=mode)
         res = torch.nn.functional.conv1d(res_lo, filt, stride=2)
         res_lo, res_hi = torch.split(res, 1, 1)
         result_lst.append(res_hi.squeeze(1))
     result_lst.append(res_lo.squeeze(1))
     return result_lst[::-1]
 
 
@@ -243,48 +285,58 @@
         coeffs (list): The wavelet coefficient list produced by wavedec.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
 
     Returns:
         torch.Tensor: The reconstructed signal.
 
+    Raises:
+        ValueError: If the dtype of the coeffs tensor is unsupported or if the
+            coefficients have incompatible shapes, dtypes or devices.
+
     Example:
         >>> import torch
         >>> import ptwt, pywt
         >>> import numpy as np
         >>> # generate an input of even length.
         >>> data = np.array([0, 1, 2, 3, 4, 5, 5, 4, 3, 2, 1, 0])
         >>> data_torch = torch.from_numpy(data.astype(np.float32))
         >>> # invert the fast wavelet transform.
         >>> ptwt.waverec(ptwt.wavedec(data_torch, pywt.Wavelet('haar'),
         >>>                           mode='zero', level=2),
         >>>              pywt.Wavelet('haar'))
 
     """
+    torch_device = coeffs[0].device
+    torch_dtype = coeffs[0].dtype
+    if not _is_dtype_supported(torch_dtype):
+        raise ValueError(f"Input dtype {torch_dtype} not supported")
+
+    for coeff in coeffs[1:]:
+        if torch_device != coeff.device:
+            raise ValueError("coefficients must be on the same device")
+        elif torch_dtype != coeff.dtype:
+            raise ValueError("coefficients must have the same dtype")
+
     _, _, rec_lo, rec_hi = get_filter_tensors(
-        wavelet, flip=False, device=coeffs[-1].device, dtype=coeffs[-1].dtype
+        wavelet, flip=False, device=torch_device, dtype=torch_dtype
     )
     filt_len = rec_lo.shape[-1]
     filt = torch.stack([rec_lo, rec_hi], 0)
 
     res_lo = coeffs[0]
     for c_pos, res_hi in enumerate(coeffs[1:]):
         res_lo = torch.stack([res_lo, res_hi], 1)
         res_lo = torch.nn.functional.conv_transpose1d(res_lo, filt, stride=2).squeeze(1)
 
         # remove the padding
         padl = (2 * filt_len - 3) // 2
         padr = (2 * filt_len - 3) // 2
         if c_pos < len(coeffs) - 2:
-            pred_len = res_lo.shape[-1] - (padl + padr)
-            next_len = coeffs[c_pos + 2].shape[-1]
-            if next_len != pred_len:
-                padr += 1
-                pred_len = res_lo.shape[-1] - (padl + padr)
-                assert (
-                    next_len == pred_len
-                ), "padding error, please open an issue on github "
+            padr, padl = _adjust_padding_at_reconstruction(
+                res_lo.shape[-1], coeffs[c_pos + 2].shape[-1], padr, padl
+            )
         if padl > 0:
             res_lo = res_lo[..., padl:]
         if padr > 0:
             res_lo = res_lo[..., :-padr]
     return res_lo
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/conv_transform_2.py` & `ptwt-0.1.5/src/ptwt/conv_transform_2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,214 +1,265 @@
-"""This module implements two dimensional padded wavelet transforms."""
+"""This module implements two-dimensional padded wavelet transforms.
+
+The implementation relies on torch.nn.functional.conv2d and
+torch.nn.functional.conv_transpose2d under the hood.
+"""
 
 
 from typing import List, Optional, Tuple, Union
 
 import pywt
 import torch
 
-from ._util import Wavelet, _as_wavelet, _outer
-from .conv_transform import _get_pad, _translate_boundary_strings, get_filter_tensors
+from ._util import Wavelet, _as_wavelet, _get_len, _is_dtype_supported, _outer
+from .conv_transform import (
+    _adjust_padding_at_reconstruction,
+    _get_pad,
+    _translate_boundary_strings,
+    get_filter_tensors,
+)
 
 
 def construct_2d_filt(lo: torch.Tensor, hi: torch.Tensor) -> torch.Tensor:
-    """Construct two dimensional filters using outer products.
+    """Construct two-dimensional filters using outer products.
 
     Args:
         lo (torch.Tensor): Low-pass input filter.
         hi (torch.Tensor): High-pass input filter
 
     Returns:
-        torch.Tensor: Stacked 2d filters of dimension
-            [filt_no, 1, height, width].
-            The four filters are ordered ll, lh, hl, hh.
+        torch.Tensor: Stacked 2d-filters of dimension
+
+        [filt_no, 1, height, width].
+
+        The four filters are ordered ll, lh, hl, hh.
 
     """
     ll = _outer(lo, lo)
     lh = _outer(hi, lo)
     hl = _outer(lo, hi)
     hh = _outer(hi, hi)
     filt = torch.stack([ll, lh, hl, hh], 0)
     filt = filt.unsqueeze(1)
     return filt
 
 
-def fwt_pad2(
+def _fwt_pad2(
     data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str = "reflect"
 ) -> torch.Tensor:
     """Pad data for the 2d FWT.
 
+    This function pads along the last two axes.
+
     Args:
         data (torch.Tensor): Input data with 4 dimensions.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
         mode (str): The padding mode.
-            Supported modes are "reflect", "zero", "constant" and "periodic".
-            Defaults to reflect.
+            Supported modes are::
+
+                "reflect", "zero", "constant", "periodic".
+
+            "reflect" is the default mode.
 
     Returns:
         The padded output tensor.
 
     """
     mode = _translate_boundary_strings(mode)
 
     wavelet = _as_wavelet(wavelet)
-    padb, padt = _get_pad(data.shape[-2], len(wavelet.dec_lo))
-    padr, padl = _get_pad(data.shape[-1], len(wavelet.dec_lo))
+    padb, padt = _get_pad(data.shape[-2], _get_len(wavelet))
+    padr, padl = _get_pad(data.shape[-1], _get_len(wavelet))
     data_pad = torch.nn.functional.pad(data, [padl, padr, padt, padb], mode=mode)
     return data_pad
 
 
 def wavedec2(
     data: torch.Tensor,
     wavelet: Union[Wavelet, str],
-    level: Optional[int] = None,
     mode: str = "reflect",
+    level: Optional[int] = None,
 ) -> List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]:
-    """Non seperated two dimensional wavelet transform.
+    """Non separated two-dimensional wavelet transform.
 
     Args:
         data (torch.Tensor): The input data tensor with up to three dimensions.
             2d inputs are interpreted as [height, width],
             3d inputs are interpreted as [batch_size, height, width].
         wavelet (Wavelet or str): A pywt wavelet compatible object or
-            the name of a pywt wavelet.
+            the name of a pywt wavelet. Refer to the output of
+            ``pywt.wavelist(kind="discrete")`` for a list of possible choices.
+        mode (str): The padding mode. Options are::
+
+                "reflect", "zero", "constant", "periodic".
+
+            This function defaults to "reflect".
         level (int): The number of desired scales.
             Defaults to None.
-        mode (str): The padding mode. Options are
-            "reflect", "zero", "constant" and "periodic".
-            Defaults to "reflect".
 
     Returns:
         list: A list containing the wavelet coefficients.
-              The coefficients are in pywt order. That is:
-              [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
-              A denotes approximation, H horizontal, V vertical
-              and D diagonal coefficients.
+        The coefficients are in pywt order. That is::
+
+            [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
+
+        A denotes approximation, H horizontal, V vertical
+        and D diagonal coefficients.
 
     Raises:
-        ValueError: If the dimensionality of the input data tensor is unsupported.
+        ValueError: If the dimensionality or the dtype of the input data tensor
+            is unsupported.
 
     Example:
         >>> import torch
         >>> import ptwt, pywt
         >>> import numpy as np
-        >>> import scipy.misc
-        >>> face = np.transpose(scipy.misc.face(),
+        >>> from scipy import datasets
+        >>> face = np.transpose(datasets.face(),
         >>>                     [2, 0, 1]).astype(np.float64)
         >>> pytorch_face = torch.tensor(face)
         >>> coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
         >>>                              level=2, mode="zero")
 
     """
     if data.dim() == 2:
         data = data.unsqueeze(0).unsqueeze(0)
     elif data.dim() == 3:
+        # add a channel dimension for torch.
         data = data.unsqueeze(1)
     elif data.dim() == 4:
         raise ValueError(
             "Wavedec2 does not support four input dimensions. \
-             Optionally-batched two dimensional inputs work."
+             Optionally-batched two-dimensional inputs work."
         )
     elif data.dim() == 1:
         raise ValueError("Wavedec2 needs more than one input dimension to work.")
 
+    if not _is_dtype_supported(data.dtype):
+        raise ValueError(f"Input dtype {data.dtype} not supported")
+
     wavelet = _as_wavelet(wavelet)
     dec_lo, dec_hi, _, _ = get_filter_tensors(
         wavelet, flip=True, device=data.device, dtype=data.dtype
     )
     dec_filt = construct_2d_filt(lo=dec_lo, hi=dec_hi)
 
     if level is None:
         level = pywt.dwtn_max_level([data.shape[-1], data.shape[-2]], wavelet)
 
     result_lst: List[
         Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
     ] = []
     res_ll = data
     for _ in range(level):
-        res_ll = fwt_pad2(res_ll, wavelet, mode=mode)
+        res_ll = _fwt_pad2(res_ll, wavelet, mode=mode)
         res = torch.nn.functional.conv2d(res_ll, dec_filt, stride=2)
         res_ll, res_lh, res_hl, res_hh = torch.split(res, 1, 1)
-        result_lst.append((res_lh, res_hl, res_hh))
-    result_lst.append(res_ll)
+        to_append = (res_lh.squeeze(1), res_hl.squeeze(1), res_hh.squeeze(1))
+        result_lst.append(to_append)
+    result_lst.append(res_ll.squeeze(1))
     return result_lst[::-1]
 
 
 def waverec2(
     coeffs: List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
     wavelet: Union[Wavelet, str],
 ) -> torch.Tensor:
     """Reconstruct a signal from wavelet coefficients.
 
     Args:
         coeffs (list): The wavelet coefficient list produced by wavedec2.
+            The coefficients must be in pywt order. That is::
+
+            [cAn, (cHn, cVn, cDn), … (cH1, cV1, cD1)] .
+
+            A denotes approximation, H horizontal, V vertical,
+            and D diagonal coefficients.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
 
     Returns:
-        torch.Tensor: The reconstructed signal.
+        torch.Tensor: The reconstructed signal of shape [batch, height, width].
 
     Raises:
-        ValueError: If `coeffs` is not in the shape as it is returned from `wavedec2`.
+        ValueError: If `coeffs` is not in a shape as returned from `wavedec2` or
+            if the dtype is not supported.
 
     Example:
         >>> import ptwt, pywt, torch
         >>> import numpy as np
-        >>> import scipy.misc
-        >>> face = np.transpose(scipy.misc.face(),
+        >>> from scipy import datasets
+        >>> face = np.transpose(datasets.face(),
         >>>                     [2, 0, 1]).astype(np.float64)
         >>> pytorch_face = torch.tensor(face)
         >>> coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
         >>>                              level=2, mode="constant")
         >>> reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
 
     """
     wavelet = _as_wavelet(wavelet)
 
-    if not isinstance(coeffs[0], torch.Tensor):
+    res_ll = coeffs[0]
+    if not isinstance(res_ll, torch.Tensor):
         raise ValueError(
             "First element of coeffs must be the approximation coefficient tensor."
         )
 
+    torch_device = res_ll.device
+    torch_dtype = res_ll.dtype
+
+    if not _is_dtype_supported(torch_dtype):
+        raise ValueError(f"Input dtype {torch_dtype} not supported")
+
     _, _, rec_lo, rec_hi = get_filter_tensors(
-        wavelet, flip=False, device=coeffs[0].device, dtype=coeffs[0].dtype
+        wavelet, flip=False, device=torch_device, dtype=torch_dtype
     )
     filt_len = rec_lo.shape[-1]
     rec_filt = construct_2d_filt(lo=rec_lo, hi=rec_hi)
 
-    res_ll = coeffs[0]
-    for c_pos, res_lh_hl_hh in enumerate(coeffs[1:]):
-        res_ll = torch.cat(
-            [res_ll, res_lh_hl_hh[0], res_lh_hl_hh[1], res_lh_hl_hh[2]], 1
-        )
-        res_ll = torch.nn.functional.conv_transpose2d(res_ll, rec_filt, stride=2)
+    for c_pos, coeff_tuple in enumerate(coeffs[1:]):
+        if not isinstance(coeff_tuple, tuple) or len(coeff_tuple) != 3:
+            raise ValueError(
+                f"Unexpected detail coefficient type: {type(coeff_tuple)}. Detail "
+                "coefficients must be a 3-tuple of tensors as returned by "
+                "wavedec2."
+            )
+
+        curr_shape = res_ll.shape
+        for coeff in coeff_tuple:
+            if torch_device != coeff.device:
+                raise ValueError("coefficients must be on the same device")
+            elif torch_dtype != coeff.dtype:
+                raise ValueError("coefficients must have the same dtype")
+            elif coeff.shape != curr_shape:
+                raise ValueError(
+                    "All coefficients on each level must have the same shape"
+                )
+
+        res_lh, res_hl, res_hh = coeff_tuple
+
+        res_ll = torch.stack([res_ll, res_lh, res_hl, res_hh], 1)
+        res_ll = torch.nn.functional.conv_transpose2d(
+            res_ll, rec_filt, stride=2
+        ).squeeze(1)
 
         # remove the padding
         padl = (2 * filt_len - 3) // 2
         padr = (2 * filt_len - 3) // 2
         padt = (2 * filt_len - 3) // 2
         padb = (2 * filt_len - 3) // 2
         if c_pos < len(coeffs) - 2:
-            pred_len = res_ll.shape[-1] - (padl + padr)
-            next_len = coeffs[c_pos + 2][0].shape[-1]
-            pred_len2 = res_ll.shape[-2] - (padt + padb)
-            next_len2 = coeffs[c_pos + 2][0].shape[-2]
-            if next_len != pred_len:
-                padr += 1
-                pred_len = res_ll.shape[-1] - (padl + padr)
-                assert (
-                    next_len == pred_len
-                ), "padding error, please open an issue on github "
-            if next_len2 != pred_len2:
-                padb += 1
-                pred_len2 = res_ll.shape[-2] - (padt + padb)
-                assert (
-                    next_len2 == pred_len2
-                ), "padding error, please open an issue on github "
+            padr, padl = _adjust_padding_at_reconstruction(
+                res_ll.shape[-1], coeffs[c_pos + 2][0].shape[-1], padr, padl
+            )
+            padb, padt = _adjust_padding_at_reconstruction(
+                res_ll.shape[-2], coeffs[c_pos + 2][0].shape[-2], padb, padt
+            )
+
         if padt > 0:
             res_ll = res_ll[..., padt:, :]
         if padb > 0:
             res_ll = res_ll[..., :-padb, :]
         if padl > 0:
             res_ll = res_ll[..., padl:]
         if padr > 0:
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/conv_transform_3.py` & `ptwt-0.1.5/src/ptwt/conv_transform_3.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,39 @@
-"""Code for three dimensional padded transforms."""
+"""Code for three dimensional padded transforms.
 
-from typing import Dict, List, Optional, Union
+The functions here are based on torch.nn.functional.conv3d and it's transpose.
+"""
+
+from typing import Dict, List, Optional, Sequence, Union, cast
 
 import pywt
 import torch
 
-from ._util import Wavelet, _as_wavelet, _outer
-from .conv_transform import _get_pad, _translate_boundary_strings, get_filter_tensors
+from ._util import Wavelet, _as_wavelet, _get_len, _is_dtype_supported, _outer
+from .conv_transform import (
+    _adjust_padding_at_reconstruction,
+    _get_pad,
+    _translate_boundary_strings,
+    get_filter_tensors,
+)
 
 
 def _construct_3d_filt(lo: torch.Tensor, hi: torch.Tensor) -> torch.Tensor:
     """Construct three dimensional filters using outer products.
 
     Args:
         lo (torch.Tensor): Low-pass input filter.
         hi (torch.Tensor): High-pass input filter
 
     Returns:
-        torch.Tensor: Stacked 3d filters of dimension
-            [8, 1, length, height, width].
-            The four filters are ordered ll, lh, hl, hh.
+        torch.Tensor: Stacked 3d filters of dimension::
+
+        [8, 1, length, height, width].
+
+        The four filters are ordered ll, lh, hl, hh.
 
     """
     dim_size = lo.shape[-1]
     size = [dim_size] * 3
     lll = _outer(lo, _outer(lo, lo)).reshape(size)
     llh = _outer(lo, _outer(lo, hi)).reshape(size)
     lhl = _outer(lo, _outer(hi, lo)).reshape(size)
@@ -36,71 +46,87 @@
     filt = filt.unsqueeze(1)
     return filt
 
 
 def _fwt_pad3(
     data: torch.Tensor, wavelet: Union[Wavelet, str], mode: str
 ) -> torch.Tensor:
-    """Pad data for the 2d FWT.
+    """Pad data for the 3d-FWT.
+
+    This function pads the last three axes.
 
     Args:
         data (torch.Tensor): Input data with 4 dimensions.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
         mode (str): The padding mode. Supported modes are "zero".
 
     Returns:
         The padded output tensor.
 
     """
     mode = _translate_boundary_strings(mode)
 
     wavelet = _as_wavelet(wavelet)
-    pad_back, pad_front = _get_pad(data.shape[-3], len(wavelet.dec_lo))
-    pad_bottom, pad_top = _get_pad(data.shape[-2], len(wavelet.dec_lo))
-    pad_right, pad_left = _get_pad(data.shape[-1], len(wavelet.dec_lo))
+    pad_back, pad_front = _get_pad(data.shape[-3], _get_len(wavelet))
+    pad_bottom, pad_top = _get_pad(data.shape[-2], _get_len(wavelet))
+    pad_right, pad_left = _get_pad(data.shape[-1], _get_len(wavelet))
     data_pad = torch.nn.functional.pad(
         data, [pad_left, pad_right, pad_top, pad_bottom, pad_front, pad_back], mode=mode
     )
     return data_pad
 
 
 def wavedec3(
     data: torch.Tensor,
     wavelet: Union[Wavelet, str],
-    level: Optional[int] = None,
     mode: str = "zero",
+    level: Optional[int] = None,
 ) -> List[Union[torch.Tensor, Dict[str, torch.Tensor]]]:
-    """Compute a three dimensional wavelet transform.
+    """Compute a three-dimensional wavelet transform.
 
     Args:
         data (torch.Tensor): The input data of shape
             [batch_size, length, height, width]
-        wavelet (Union[Wavelet, str]): The wavelet to be used.
-        level (Optional[int]): The maximum decomposition level.
-            Defaults to None.
-        mode (str): The padding mode. Options are
+        wavelet (Union[Wavelet, str]): The wavelet to transform with.
+            ``pywt.wavelist(kind='discrete')`` lists possible choices.
+        mode (str): The padding mode. Possible options are
             "zero", "constant" or "periodic".
             Defaults to "zero".
+        level (Optional[int]): The maximum decomposition level.
+            This argument defaults to None.
 
     Returns:
         list: A list with the lll coefficients and dictionaries
-            with the filter order strings ("aad", "ada", "add",
-            "daa", "dad", "dda", "ddd") as keys.
+        with the filter order strings::
+
+        ("aad", "ada", "add", "daa", "dad", "dda", "ddd")
+
+        as keys. With a for the low pass or approximation filter and
+        d for the high-pass or detail filter.
 
     Raises:
-        ValueError: If the input has fewer than 3 dimensions.
+        ValueError: If the input has fewer than three dimensions or
+            if the dtype is not supported.
+
+    Example:
+        >>> import ptwt, torch
+        >>> data = torch.randn(5, 16, 16, 16)
+        >>> transformed = ptwt.wavedec3(data, "haar", level=2, mode="reflect")
 
     """
     if data.dim() < 3:
         raise ValueError("Three dimensional inputs required for 3d wavedec.")
     elif data.dim() == 3:
         # add batch dim.
         data = data.unsqueeze(0)
 
+    if not _is_dtype_supported(data.dtype):
+        raise ValueError(f"Input dtype {data.dtype} not supported")
+
     wavelet = _as_wavelet(wavelet)
     dec_lo, dec_hi, _, _ = get_filter_tensors(
         wavelet, flip=True, device=data.device, dtype=data.dtype
     )
     dec_filt = _construct_3d_filt(lo=dec_lo, hi=dec_hi)
 
     if level is None:
@@ -128,85 +154,110 @@
             }
         )
     result_lst.append(res_lll)
     return result_lst[::-1]
 
 
 def waverec3(
-    coeffs: List[Union[torch.Tensor, Dict[str, torch.Tensor]]],
+    coeffs: Sequence[Union[torch.Tensor, Dict[str, torch.Tensor]]],
     wavelet: Union[Wavelet, str],
 ) -> torch.Tensor:
     """Reconstruct a signal from wavelet coefficients.
 
     Args:
         coeffs (list): The wavelet coefficient list produced by wavedec3.
         wavelet (Wavelet or str): A pywt wavelet compatible object or
             the name of a pywt wavelet.
 
     Returns:
-        torch.Tensor: The reconstructed signal.
+        torch.Tensor: The reconstructed four-dimensional signal of shape
+        [batch, depth, height, width].
+
+    Raises:
+        ValueError: If `coeffs` is not in a shape as returned from `wavedec3` or
+            if the dtype is not supported.
+
+    Example:
+        >>> import ptwt, torch
+        >>> data = torch.randn(5, 16, 16, 16)
+        >>> transformed = ptwt.wavedec3(data, "haar", level=2, mode="reflect")
+        >>> reconstruction = ptwt.waverec3(transformed, "haar")
+
     """
     wavelet = _as_wavelet(wavelet)
     # the Union[tensor, dict] idea is coming from pywt. We don't change it here.
-    res_lll: torch.Tensor = coeffs[0]  # type: ignore
+    res_lll = coeffs[0]
+    if not isinstance(res_lll, torch.Tensor):
+        raise ValueError(
+            "First element of coeffs must be the approximation coefficient tensor."
+        )
+
+    torch_device = res_lll.device
+    torch_dtype = res_lll.dtype
+
+    if not _is_dtype_supported(torch_dtype):
+        if not _is_dtype_supported(torch_dtype):
+            raise ValueError(f"Input dtype {torch_dtype} not supported")
+
     _, _, rec_lo, rec_hi = get_filter_tensors(
-        wavelet, flip=False, device=res_lll.device, dtype=res_lll.dtype
+        wavelet, flip=False, device=torch_device, dtype=torch_dtype
     )
     filt_len = rec_lo.shape[-1]
     rec_filt = _construct_3d_filt(lo=rec_lo, hi=rec_hi)
 
-    for c_pos, coeff_dict in enumerate(coeffs[1:]):
+    coeff_dicts = cast(Sequence[Dict[str, torch.Tensor]], coeffs[1:])
+    for c_pos, coeff_dict in enumerate(coeff_dicts):
+        if not isinstance(coeff_dict, dict) or len(coeff_dict) != 7:
+            raise ValueError(
+                f"Unexpected detail coefficient type: {type(coeff_dict)}. Detail "
+                "coefficients must be a dict containing 7 tensors as returned by "
+                "wavedec3."
+            )
+        for coeff in coeff_dict.values():
+            if torch_device != coeff.device:
+                raise ValueError("coefficients must be on the same device")
+            elif torch_dtype != coeff.dtype:
+                raise ValueError("coefficients must have the same dtype")
+            elif res_lll.shape != coeff.shape:
+                raise ValueError(
+                    "All coefficients on each level must have the same shape"
+                )
         res_lll = torch.stack(
             [
                 res_lll,
-                coeff_dict["aad"],  # type: ignore
-                coeff_dict["ada"],  # type: ignore
-                coeff_dict["add"],  # type: ignore
-                coeff_dict["daa"],  # type: ignore
-                coeff_dict["dad"],  # type: ignore
-                coeff_dict["dda"],  # type: ignore
-                coeff_dict["ddd"],  # type: ignore
+                coeff_dict["aad"],
+                coeff_dict["ada"],
+                coeff_dict["add"],
+                coeff_dict["daa"],
+                coeff_dict["dad"],
+                coeff_dict["dda"],
+                coeff_dict["ddd"],
             ],
             1,
         )
         res_lll = torch.nn.functional.conv_transpose3d(res_lll, rec_filt, stride=2)
         res_lll = res_lll.squeeze(1)
 
         # remove the padding
         padfr = (2 * filt_len - 3) // 2
         padba = (2 * filt_len - 3) // 2
         padl = (2 * filt_len - 3) // 2
         padr = (2 * filt_len - 3) // 2
         padt = (2 * filt_len - 3) // 2
         padb = (2 * filt_len - 3) // 2
-        if c_pos < len(coeffs) - 2:
-            pred_len = res_lll.shape[-1] - (padl + padr)
-            next_len = coeffs[c_pos + 2]["aad"].shape[-1]  # type: ignore
-            pred_len2 = res_lll.shape[-2] - (padt + padb)
-            next_len2 = coeffs[c_pos + 2]["aad"].shape[-2]  # type: ignore
-            pred_len3 = res_lll.shape[-3] - (padfr + padba)
-            next_len3 = coeffs[c_pos + 2]["aad"].shape[-3]  # type: ignore
-            if next_len != pred_len:
-                padr += 1
-                pred_len = res_lll.shape[-1] - (padl + padr)
-                assert (
-                    next_len == pred_len
-                ), "padding error, please open an issue on github "
-            if next_len2 != pred_len2:
-                padb += 1
-                pred_len2 = res_lll.shape[-2] - (padt + padb)
-                assert (
-                    next_len2 == pred_len2
-                ), "padding error, please open an issue on github "
-            if next_len3 != pred_len3:
-                padba += 1
-                pred_len3 = res_lll.shape[-3] - (padba + padfr)
-                assert (
-                    next_len3 == pred_len3
-                ), "padding error, please open an issue on github "
+        if c_pos + 1 < len(coeff_dicts):
+            padr, padl = _adjust_padding_at_reconstruction(
+                res_lll.shape[-1], coeff_dicts[c_pos + 1]["aad"].shape[-1], padr, padl
+            )
+            padb, padt = _adjust_padding_at_reconstruction(
+                res_lll.shape[-2], coeff_dicts[c_pos + 1]["aad"].shape[-2], padb, padt
+            )
+            padba, padfr = _adjust_padding_at_reconstruction(
+                res_lll.shape[-3], coeff_dicts[c_pos + 1]["aad"].shape[-3], padba, padfr
+            )
         if padt > 0:
             res_lll = res_lll[..., padt:, :]
         if padb > 0:
             res_lll = res_lll[..., :-padb, :]
         if padl > 0:
             res_lll = res_lll[..., padl:]
         if padr > 0:
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/matmul_transform.py` & `ptwt-0.1.5/src/ptwt/matmul_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 # Created by moritz (wolter@cs.uni-bonn.de) at 14.04.20
 import sys
 from typing import List, Optional, Union
 
 import numpy as np
 import torch
 
-from ._util import Wavelet, _as_wavelet, _is_boundary_mode_supported
+from ._util import (
+    Wavelet,
+    _as_wavelet,
+    _is_boundary_mode_supported,
+    _is_dtype_supported,
+)
 from .conv_transform import get_filter_tensors
 from .sparse_math import (
     _orth_by_gram_schmidt,
     _orth_by_qr,
     cat_sparse_identity_matrix,
     construct_strided_conv_matrix,
 )
@@ -309,28 +314,32 @@
         elif input_signal.dim() != 2:
             raise ValueError(
                 f"Invalid input tensor shape {input_signal.size()}. "
                 "The input signal is expected to be of the form "
                 "[batch_size, length]."
             )
 
+        if not _is_dtype_supported(input_signal.dtype):
+            raise ValueError(f"Input dtype {input_signal.dtype} not supported")
+
         if input_signal.shape[-1] % 2 != 0:
             # odd length input
             # print('input length odd, padding a zero on the right')
             input_signal = torch.nn.functional.pad(input_signal, [0, 1])
 
         _, length = input_signal.shape
 
         re_build = False
         if self.input_length != length:
             self.input_length = length
             re_build = True
 
         if self.level is None:
-            self.level = int(np.log2(length))
+            wlen = len(self.wavelet)
+            self.level = int(np.log2(length / (wlen - 1)))
             re_build = True
         elif self.level <= 0:
             raise ValueError("level must be a positive integer.")
 
         if not self.fwt_matrix_list or re_build:
             self._construct_analysis_matrices(
                 device=input_signal.device, dtype=input_signal.dtype
@@ -563,46 +572,38 @@
 
         re_build = False
         if self.level != level or self.input_length != input_length:
             self.level = level
             self.input_length = input_length
             re_build = True
 
+        torch_device = coefficients[0].device
+        torch_dtype = coefficients[0].dtype
+        for coeff in coefficients[1:]:
+            if torch_device != coeff.device:
+                raise ValueError("coefficients must be on the same device")
+            elif torch_dtype != coeff.dtype:
+                raise ValueError("coefficients must have the same dtype")
+
+        if not _is_dtype_supported(torch_dtype):
+            raise ValueError(f"Input dtype {torch_dtype} not supported")
+
         if not self.ifwt_matrix_list or re_build:
             self._construct_synthesis_matrices(
-                device=coefficients[-1].device,
-                dtype=coefficients[-1].dtype,
+                device=torch_device,
+                dtype=torch_dtype,
             )
 
         # transpose the coefficients to handle the batch dimension efficiently.
         coefficients = [c.T for c in coefficients]
 
         lo = coefficients[0]
         for c_pos, hi in enumerate(coefficients[1:]):
-            torch_device = None
-            curr_shape: Optional[torch.Size] = None
-            dtype = None
-            for coeff in [lo, hi]:
-                if coeff is not None:
-                    if curr_shape is None:
-                        curr_shape = coeff.shape
-                        torch_device = coeff.device
-                        dtype = coeff.dtype
-                    elif curr_shape != coeff.shape:
-                        # TODO: Add check that coeffs are on the same device
-                        raise ValueError("coeffs must have the same shape")
-
-            if curr_shape is None:
-                raise ValueError(
-                    "At least one coefficient parameter must be specified."
-                )
-            if lo is None:
-                lo = torch.zeros(curr_shape, device=torch_device, dtype=dtype)
-            if hi is None:
-                hi = torch.zeros(curr_shape, device=torch_device, dtype=dtype)
+            if lo.shape != hi.shape:
+                raise ValueError("coefficients must have the same shape")
 
             lo = torch.cat([lo, hi], 0)
             lo = torch.sparse.mm(self.ifwt_matrix_list[::-1][c_pos], lo)
 
             # remove padding
             if c_pos < len(coefficients) - 2:
                 pred_len = lo.shape[0]
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/matmul_transform_2.py` & `ptwt-0.1.5/src/ptwt/matmul_transform_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 # Written by moritz ( @ wolter.tech ) in 2021
 import sys
 from typing import List, Optional, Tuple, Union, cast
 
 import numpy as np
 import torch
 
-from ._util import Wavelet, _as_wavelet, _is_boundary_mode_supported
+from ._util import (
+    Wavelet,
+    _as_wavelet,
+    _is_boundary_mode_supported,
+    _is_dtype_supported,
+)
 from .conv_transform import get_filter_tensors
 from .conv_transform_2 import construct_2d_filt
-from .matmul_transform import (
+from .matmul_transform import construct_boundary_a, construct_boundary_s, orthogonalize
+from .sparse_math import (
+    batch_mm,
     cat_sparse_identity_matrix,
-    construct_boundary_a,
-    construct_boundary_s,
-    orthogonalize,
+    construct_strided_conv2d_matrix,
 )
-from .sparse_math import batch_mm, construct_strided_conv2d_matrix
 
 
 def _construct_a_2(
     wavelet: Union[Wavelet, str],
     height: int,
     width: int,
     device: Union[torch.device, str],
@@ -111,15 +115,15 @@
     synthesis = torch.cat(
         [synthesis_ll, synthesis_lh, synthesis_hl, synthesis_hh], 0
     ).coalesce()
     indices = synthesis.indices()
     shape = synthesis.shape
     transpose_indices = torch.stack([indices[1, :], indices[0, :]])
     transpose_synthesis = torch.sparse_coo_tensor(
-        transpose_indices, synthesis.values(), size=(shape[1], shape[0])
+        transpose_indices, synthesis.values(), size=(shape[1], shape[0]), device=device
     )
     return transpose_synthesis
 
 
 def construct_boundary_a2(
     wavelet: Union[Wavelet, str],
     height: int,
@@ -136,15 +140,15 @@
         height (int): The height of the input matrix.
             Should be divisible by two.
         width (int): The width of the input matrix.
             Should be divisible by two.
         device (torch.device): Where to place the matrix. Either on
             the CPU or GPU.
         boundary (str): The method to use for matrix orthogonalization.
-            Choose qr or gramschmidt. Defaults to qr.
+            Choose "qr" or "gramschmidt". Defaults to "qr".
         dtype (torch.dtype, optional): The desired data-type for the matrix.
             Defaults to torch.float64.
 
     Returns:
         torch.Tensor: A sparse fwt matrix, with orthogonalized boundary
             wavelets.
     """
@@ -212,33 +216,34 @@
         property is equivalent.
 
     Note:
         Constructing the sparse fwt-matrix is expensive.
         For longer wavelets, high level transforms, and large
         input images this may take a while.
         The matrix is therefore constructed only once.
-        It can be accessed via the sparse_fwt_operator property.
+        In the non separable case, it can be accessed via
+        the sparse_fwt_operator property.
 
     Example:
         >>> import ptwt, torch, pywt
         >>> import numpy as np
-        >>> import scipy.misc
-        >>> face = scipy.misc.face()[:256, :256, :].astype(np.float32)
+        >>> from scipy import datasets
+        >>> face = datasets.face()[:256, :256, :].astype(np.float32)
         >>> pt_face = torch.tensor(face).permute([2, 0, 1])
         >>> matrixfwt = ptwt.MatrixWavedec2(pywt.Wavelet("haar"), level=2)
         >>> mat_coeff = matrixfwt(pt_face)
 
     """
 
     def __init__(
         self,
         wavelet: Union[Wavelet, str],
         level: Optional[int] = None,
         boundary: str = "qr",
-        separable: bool = False,
+        separable: bool = True,
     ):
         """Create a new matrix fwt object.
 
         Args:
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             level (int, optional): The level up to which to compute the fwt. If None,
@@ -248,17 +253,18 @@
                 Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's
                 dense qr implementation, it is fast but memory hungry.
                 The 'gramschmidt' option is sparse, memory efficient,
                 and slow.
                 Choose 'gramschmidt' if 'qr' runs out of memory.
                 Defaults to 'qr'.
             separable (bool): If this flag is set, a separable transformation
-                is used, i.e. a 1d transformation along each axis. This is significantly
-                faster than a non-separable transformation since only a small constant-
-                size part of the matrices must be orthogonalized. Defaults to False.
+                is used, i.e. a 1d transformation along each axis.
+                Matrix construction is significantly faster for separable
+                transformations since only a small constant-size part of the
+                matrices must be orthogonalized. Defaults to True.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
             ValueError: If the wavelet filters have different lenghts.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.level = level
@@ -267,16 +273,14 @@
         self.input_signal_shape: Optional[Tuple[int, int]] = None
         self.fwt_matrix_list: List[
             Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]
         ] = []
         self.pad_list: List[Tuple[bool, bool]] = []
         self.padded = False
 
-        # TODO: Allow separate wavelets and lengths for each axis in the separable case
-
         if not _is_boundary_mode_supported(self.boundary):
             raise NotImplementedError
 
         if self.wavelet.dec_len != self.wavelet.rec_len:
             raise ValueError("All filters must have the same length")
 
     @property
@@ -396,15 +400,19 @@
             input_signal (torch.Tensor): An input signal of shape
                 [batch_size, height, width].
                 2d inputs are interpreted as [height, width].
                 Inputs of the form [batch_size, 1, height, width] are squeezed.
 
         Returns:
             (list): The resulting coefficients per level stored in
-            a pywt style list.
+            a pywt style list. The list is ordered as::
+
+                (ll, (lh, hl, hh), ...)
+
+            with 'l' for low-pass and 'h' for high pass filters.
 
         Raises:
             ValueError: If the decomposition level is not a positive integer
                 or if the input signal has not the expected shape.
         """
         if input_signal.dim() == 2:
             # add batch dim to unbatched input
@@ -418,25 +426,31 @@
                 f"Invalid input tensor shape {input_signal.size()}. "
                 "The input signal is expected to be of the form "
                 "[batch_size, height, width]."
             )
 
         batch_size, height, width = input_signal.shape
 
+        if not _is_dtype_supported(input_signal.dtype):
+            raise ValueError(f"Input dtype {input_signal.dtype} not supported")
+
         re_build = False
         if (
             self.input_signal_shape is None
             or self.input_signal_shape[0] != height
             or self.input_signal_shape[1] != width
         ):
             self.input_signal_shape = height, width
             re_build = True
 
         if self.level is None:
-            self.level = int(np.min([np.log2(height), np.log2(width)]))
+            wlen = len(self.wavelet)
+            self.level = int(
+                np.min([np.log2(height / (wlen - 1)), np.log2(width / (wlen - 1))])
+            )
             re_build = True
         elif self.level <= 0:
             raise ValueError("level must be a positive integer.")
 
         if not self.fwt_matrix_list or re_build:
             self._construct_analysis_matrices(
                 device=input_signal.device, dtype=input_signal.dtype
@@ -462,15 +476,14 @@
                 ll = batch_mm(fwt_col_matrix, ll.transpose(-2, -1)).transpose(-2, -1)
                 ll = batch_mm(fwt_row_matrix, ll)
 
                 a_coeffs, d_coeffs = torch.split(ll, current_height // 2, dim=-2)
                 ll, lh = torch.split(a_coeffs, current_width // 2, dim=-1)
                 hl, hh = torch.split(d_coeffs, current_width // 2, dim=-1)
 
-                # TODO: Is the order consistent with the non-separable case?
                 split_list.append((lh, hl, hh))
             split_list.append(ll)
         else:
             ll = input_signal.transpose(-2, -1).reshape([batch_size, -1]).T
             for scale, fwt_matrix in enumerate(self.fwt_matrix_list):
                 fwt_matrix = cast(torch.Tensor, fwt_matrix)
                 pad = self.pad_list[scale]
@@ -515,51 +528,48 @@
             )
         return split_list[::-1]
 
 
 class MatrixWaverec2(object):
     """Synthesis or inverse matrix based-wavelet transformation object.
 
-    Note:
-        Constructing the fwt matrix is expensive.
-        The matrix is, therefore, constructed only
-        once and stored for later use.
-
     Example:
         >>> import ptwt, torch, pywt
         >>> import numpy as np
-        >>> import scipy.misc
-        >>> face = scipy.misc.face()[:256, :256, :].astype(np.float32)
+        >>> from scipy import datasets
+        >>> face = datasets.face()[:256, :256, :].astype(np.float32)
         >>> pt_face = torch.tensor(face).permute([2, 0, 1])
         >>> matrixfwt = ptwt.MatrixWavedec2(pywt.Wavelet("haar"), level=2)
         >>> mat_coeff = matrixfwt(pt_face)
         >>> matrixifwt = ptwt.MatrixWaverec2(pywt.Wavelet("haar"))
         >>> reconstruction = matrixifwt(mat_coeff)
     """
 
     def __init__(
         self,
         wavelet: Union[Wavelet, str],
         boundary: str = "qr",
-        separable: bool = False,
+        separable: bool = True,
     ):
         """Create the inverse matrix based fast wavelet transformation.
 
         Args:
             wavelet (Wavelet or str): A pywt wavelet compatible object or
                 the name of a pywt wavelet.
             boundary (str): The method used for boundary filter treatment.
                 Choose 'qr' or 'gramschmidt'. 'qr' relies on pytorch's dense qr
                 implementation, it is fast but memory hungry. The 'gramschmidt' option
                 is sparse, memory efficient, and slow. Choose 'gramschmidt' if 'qr' runs
                 out of memory. Defaults to 'qr'.
             separable (bool): If this flag is set, a separable transformation
                 is used, i.e. a 1d transformation along each axis. This is significantly
                 faster than a non-separable transformation since only a small constant-
-                size part of the matrices must be orthogonalized. Defaults to False.
+                size part of the matrices must be orthogonalized.
+                For invertability the analysis and synthesis values must be identical!
+                Defaults to True.
 
         Raises:
             NotImplementedError: If the selected `boundary` mode is not supported.
             ValueError: If the wavelet filters have different lenghts.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.boundary = boundary
@@ -569,16 +579,14 @@
             Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]
         ] = []
         self.level: Optional[int] = None
         self.input_signal_shape: Optional[Tuple[int, int]] = None
 
         self.padded = False
 
-        # TODO: Allow separate wavelets and lengths for each axis in the separable case
-
         if not _is_boundary_mode_supported(self.boundary):
             raise NotImplementedError
 
         if self.wavelet.dec_len != self.wavelet.rec_len:
             raise ValueError("All filters must have the same length")
 
     @property
@@ -675,60 +683,14 @@
                     device=device,
                     dtype=dtype,
                 )
                 self.ifwt_matrix_list.append(synthesis_matrix_2d)
             current_height = current_height // 2
             current_width = current_width // 2
 
-    def _process_coeffs(
-        self,
-        ll: torch.Tensor,
-        lh_hl_hh: Tuple[torch.Tensor, torch.Tensor, torch.Tensor],
-    ) -> Tuple[
-        Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor],
-        torch.Size,
-        torch.device,
-        torch.dtype,
-    ]:
-        if len(lh_hl_hh) != 3:
-            raise ValueError(
-                "Detail coefficients must be a 3-tuple of tensors as returned by "
-                "MatrixWavedec2."
-            )
-
-        lh, hl, hh = lh_hl_hh
-
-        torch_device = None
-        curr_shape = None
-        torch_dtype = None
-        for coeff in [ll, lh, hl, hh]:
-            if coeff is not None:
-                if curr_shape is None:
-                    curr_shape = coeff.shape
-                    torch_device = coeff.device
-                    torch_dtype = coeff.dtype
-                elif curr_shape != coeff.shape:
-                    # TODO: Add check that coeffs are on the same device
-                    raise ValueError(
-                        "All coeffs on each level must have the same shape"
-                    )
-
-        if torch_device is None or curr_shape is None or torch_dtype is None:
-            raise ValueError("At least one coefficient parameter must be specified.")
-
-        if ll is None:
-            ll = torch.zeros(curr_shape, device=torch_device, dtype=torch_dtype)
-        if lh is None:
-            lh = torch.zeros(curr_shape, device=torch_device, dtype=torch_dtype)
-        if hl is None:
-            hl = torch.zeros(curr_shape, device=torch_device, dtype=torch_dtype)
-        if hh is None:
-            hh = torch.zeros(curr_shape, device=torch_device, dtype=torch_dtype)
-        return (ll, lh, hl, hh), curr_shape, torch_device, torch_dtype
-
     def __call__(
         self,
         coefficients: List[
             Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
         ],
     ) -> torch.Tensor:
         """Compute the inverse matrix 2d fast wavelet transform.
@@ -758,37 +720,53 @@
             self.input_signal_shape = height, width
             re_build = True
 
         if self.level != level:
             self.level = level
             re_build = True
 
-        # TODO: handle coefficients[-1][0] == None
-        if not self.ifwt_matrix_list or re_build:
-            self._construct_synthesis_matrices(
-                device=coefficients[-1][0].device,
-                dtype=coefficients[-1][0].dtype,
-            )
-
-        batch_size = coefficients[-1][0].shape[0]
-        ll: torch.Tensor = coefficients[0]  # type: ignore
+        ll = coefficients[0]
         if not isinstance(ll, torch.Tensor):
             raise ValueError(
                 "First element of coeffs must be the approximation coefficient tensor."
             )
 
+        batch_size = ll.shape[0]
+        torch_device = ll.device
+        torch_dtype = ll.dtype
+
+        if not _is_dtype_supported(torch_dtype):
+            raise ValueError(f"Input dtype {torch_dtype} not supported")
+
+        if not self.ifwt_matrix_list or re_build:
+            self._construct_synthesis_matrices(
+                device=torch_device,
+                dtype=torch_dtype,
+            )
+
         for c_pos, coeff_tuple in enumerate(coefficients[1:]):
             if not isinstance(coeff_tuple, tuple) or len(coeff_tuple) != 3:
                 raise ValueError(
-                    (
-                        "Unexpected detail coefficient type: {}. Detail coefficients "
-                        "must be a 3-tuple of tensors as returned by MatrixWavedec2."
-                    ).format(type(coeff_tuple))
+                    f"Unexpected detail coefficient type: {type(coeff_tuple)}. Detail "
+                    "coefficients must be a 3-tuple of tensors as returned by "
+                    "MatrixWavedec2."
                 )
-            (ll, lh, hl, hh), curr_shape, _, _ = self._process_coeffs(ll, coeff_tuple)
+
+            curr_shape = ll.shape
+            for coeff in coeff_tuple:
+                if torch_device != coeff.device:
+                    raise ValueError("coefficients must be on the same device")
+                elif torch_dtype != coeff.dtype:
+                    raise ValueError("coefficients must have the same dtype")
+                elif coeff.shape != curr_shape:
+                    raise ValueError(
+                        "All coefficients on each level must have the same shape"
+                    )
+
+            lh, hl, hh = coeff_tuple
 
             if self.separable:
                 synthesis_matrix_rows, synthesis_matrix_cols = self.ifwt_matrix_list[
                     ::-1
                 ][c_pos]
                 a_coeffs = torch.cat((ll, lh), -1)
                 d_coeffs = torch.cat((hl, hh), -1)
@@ -806,22 +784,25 @@
                         lh.transpose(2, 1).reshape([batch_size, -1]),
                         hl.transpose(2, 1).reshape([batch_size, -1]),
                         hh.transpose(2, 1).reshape([batch_size, -1]),
                     ],
                     -1,
                 )
                 ifwt_mat = cast(torch.Tensor, self.ifwt_matrix_list[::-1][c_pos])
-                ll = torch.sparse.mm(ifwt_mat, ll.T)
+                ll = cast(torch.Tensor, torch.sparse.mm(ifwt_mat, ll.T))
 
-            pred_len = [s * 2 for s in curr_shape[-2:][::-1]]
             if not self.separable:
+                pred_len = [s * 2 for s in curr_shape[-2:]][::-1]
                 ll = ll.T.reshape([batch_size] + pred_len).transpose(2, 1)
+                pred_len = list(ll.shape[1:])
+            else:
+                pred_len = [s * 2 for s in curr_shape[-2:]]
             # remove the padding
             if c_pos < len(coefficients) - 2:
-                next_len = list(coefficients[c_pos + 2][0].shape[-2:])[::-1]
+                next_len = list(coefficients[c_pos + 2][0].shape[-2:])
                 if pred_len != next_len:
                     if pred_len[0] != next_len[0]:
                         ll = ll[:, :-1, :]
                     if pred_len[1] != next_len[1]:
                         ll = ll[:, :, :-1]
 
         return ll
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/packets.py` & `ptwt-0.1.5/src/ptwt/packets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 """Compute analysis wavelet packet representations."""
 # Created on Fri Apr 6 2021 by moritz (wolter@cs.uni-bonn.de)
 
 import collections
 from functools import partial
 from itertools import product
-from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple, Union, cast
 
+import numpy as np
 import pywt
 import torch
 
 from ._util import Wavelet, _as_wavelet
 from .conv_transform import wavedec, waverec
 from .conv_transform_2 import wavedec2, waverec2
 from .matmul_transform import MatrixWavedec, MatrixWaverec
 from .matmul_transform_2 import MatrixWavedec2, MatrixWaverec2
+from .separable_conv_transform import fswavedec2, fswaverec2
 
 if TYPE_CHECKING:
     BaseDict = collections.UserDict[str, torch.Tensor]
 else:
     BaseDict = collections.UserDict
 
 
+def _wpfreq(fs: float, level: int) -> List[float]:
+    """Compute the frequencies for a fully decomposed 1d packet tree.
+
+       The packet transform linearly subdivides all frequencies
+       from zero up to the Nyquist frequency.
+
+    Args:
+        fs (float): The sampling frequency.
+        level (int): The decomposition level.
+
+    Returns:
+        List[float]: The frequency bins of the packets in frequency order.
+    """
+    n = np.array(range(int(np.power(2.0, level))))
+    freqs = (fs / 2.0) * (n / (np.power(2.0, level)))
+    return list(freqs)
+
+
 class WaveletPacket(BaseDict):
     """One dimensional wavelet packets."""
 
     def __init__(
         self,
         data: Optional[torch.Tensor],
         wavelet: Union[Wavelet, str],
@@ -125,14 +145,20 @@
             self.maxlevel = pywt.dwt_max_level(self[""].shape[-1], self.wavelet.dec_len)
 
         for level in reversed(range(self.maxlevel)):
             for node in self.get_level(level):
                 data_a = self[node + "a"]
                 data_b = self[node + "d"]
                 rec = self._get_waverec(data_a.shape[-1])([data_a, data_b])
+                if level > 0:
+                    if rec.shape[-1] != self[node].shape[-1]:
+                        assert (
+                            rec.shape[-1] == self[node].shape[-1] + 1
+                        ), "padding error, please open an issue on github"
+                        rec = rec[..., :-1]
                 self[node] = rec
         return self
 
     def _get_wavedec(
         self,
         length: int,
     ) -> Callable[[torch.Tensor], List[torch.Tensor]]:
@@ -180,19 +206,14 @@
         else:
             return graycode_order
 
     def _recursive_dwt(self, data: torch.Tensor, level: int, path: str) -> None:
         if not self.maxlevel:
             raise AssertionError
 
-        # TODO: This is a workaround since the convolutional transforms insert a
-        #       squeezable dimension. We should adapt the wavedec code instead.
-        if data.dim() == 3:
-            data = data.squeeze(1)
-
         self.data[path] = data
         if level < self.maxlevel:
             res_lo, res_hi = self._get_wavedec(data.shape[-1])(data)
             self._recursive_dwt(res_lo, level + 1, path + "a")
             self._recursive_dwt(res_hi, level + 1, path + "d")
 
     def __getitem__(self, key: str) -> torch.Tensor:
@@ -250,17 +271,16 @@
             mode (str): A string indicating the desired padding mode.
                 If you select 'boundary', the sparse matrix backend is used.
                 Defaults to 'reflect'
             boundary_orthogonalization (str): The orthogonalization method
                 to use in the sparse matrix backend. Only used if `mode`
                 equals 'boundary'. Choose from 'qr' or 'gramschmidt'.
                 Defaults to 'qr'.
-            separable (bool): If true and the sparse matrix backend is selected,
-                a separable transform is performed, i.e. each image axis is
-                transformed separately. Defaults to False.
+            separable (bool): If true, a separable transform is performed,
+                i.e. each image axis is transformed separately. Defaults to False.
             maxlevel (int, optional): Value is passed on to `transform`.
                 The highest decomposition level to compute. If None, the maximum level
                 is determined from the input data shape. Defaults to None.
         """
         self.wavelet = _as_wavelet(wavelet)
         self.mode = mode
         self.boundary = boundary_orthogonalization
@@ -289,14 +309,18 @@
                 Defaults to None.
         """
         self.data = {}
         if maxlevel is None:
             maxlevel = pywt.dwt_max_level(min(data.shape[-2:]), self.wavelet.dec_len)
         self.maxlevel = maxlevel
 
+        if data.dim() == 2:
+            # add batch dim to unbatched input
+            data = data.unsqueeze(0)
+
         self._recursive_dwt2d(data, level=0, path="")
         return self
 
     def reconstruct(self) -> "WaveletPacket2D":
         """Recursively reconstruct the input starting from the leaf nodes.
 
         Note:
@@ -307,44 +331,45 @@
         if self.maxlevel is None:
             self.maxlevel = pywt.dwt_max_level(
                 min(self[""].shape[-2:]), self.wavelet.dec_len
             )
 
         for level in reversed(range(self.maxlevel)):
             for node in self.get_natural_order(level):
-                if self.mode == "boundary":
-                    data_a = self[node + "a"]
-                    data_h = self[node + "h"]
-                    data_v = self[node + "v"]
-                    data_d = self[node + "d"]
-                    rec = self._get_waverec(data_a.shape[-2:])(
-                        (data_a, (data_h, data_v, data_d))
-                    )
-                    self[node] = rec
-                else:
-                    data_a = self[node + "a"].unsqueeze(1)
-                    data_h = self[node + "h"].unsqueeze(1)
-                    data_v = self[node + "v"].unsqueeze(1)
-                    data_d = self[node + "d"].unsqueeze(1)
-                    rec = self._get_waverec(data_a.shape[-2:])(
-                        (data_a, (data_h, data_v, data_d))
-                    )
-                    self[node] = rec.squeeze(1)
+                data_a = self[node + "a"]
+                data_h = self[node + "h"]
+                data_v = self[node + "v"]
+                data_d = self[node + "d"]
+                rec = self._get_waverec(data_a.shape[-2:])(
+                    [data_a, (data_h, data_v, data_d)]
+                )
+                if level > 0:
+                    if rec.shape[-1] != self[node].shape[-1]:
+                        assert (
+                            rec.shape[-1] == self[node].shape[-1] + 1
+                        ), "padding error, please open an issue on github"
+                        rec = rec[..., :-1]
+                    if rec.shape[-2] != self[node].shape[-2]:
+                        assert (
+                            rec.shape[-2] == self[node].shape[-2] + 1
+                        ), "padding error, please open an issue on github"
+                        rec = rec[..., :-1, :]
+                self[node] = rec
         return self
 
     def get_natural_order(self, level: int) -> List[str]:
         """Get the natural ordering for a given decomposition level.
 
         Args:
             level (int): The decomposition level.
 
         Returns:
             list: A list with the filter order strings.
         """
-        return ["".join(p) for p in list(product(["a", "h", "v", "d"], repeat=level))]
+        return ["".join(p) for p in product(["a", "h", "v", "d"], repeat=level)]
 
     def _get_wavedec(
         self, shape: Tuple[int, ...]
     ) -> Callable[
         [torch.Tensor],
         List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
     ]:
@@ -355,45 +380,87 @@
                     self.wavelet,
                     level=1,
                     boundary=self.boundary,
                     separable=self.separable,
                 )
             fun = self.matrix_wavedec2_dict[shape]
             return fun
+        elif self.separable:
+            return self._transform_fsdict_to_tuple_func(
+                partial(fswavedec2, wavelet=self.wavelet, level=1, mode=self.mode)
+            )
         else:
             return partial(wavedec2, wavelet=self.wavelet, level=1, mode=self.mode)
 
     def _get_waverec(
         self, shape: Tuple[int, ...]
     ) -> Callable[
-        [Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
+        [List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]],
         torch.Tensor,
     ]:
         if self.mode == "boundary":
             shape = tuple(shape)
             if shape not in self.matrix_waverec2_dict.keys():
                 self.matrix_waverec2_dict[shape] = MatrixWaverec2(
                     self.wavelet,
                     boundary=self.boundary,
                     separable=self.separable,
                 )
-            fun = self.matrix_waverec2_dict[shape]
-            return fun  # type: ignore
+            return self.matrix_waverec2_dict[shape]
+        elif self.separable:
+            return self._transform_tuple_to_fsdict_func(
+                partial(fswaverec2, wavelet=self.wavelet)
+            )
         else:
             return partial(waverec2, wavelet=self.wavelet)
 
+    def _transform_fsdict_to_tuple_func(
+        self,
+        fs_dict_func: Callable[
+            [torch.Tensor], List[Union[torch.Tensor, Dict[str, torch.Tensor]]]
+        ],
+    ) -> Callable[
+        [torch.Tensor],
+        List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]],
+    ]:
+        def _tuple_func(
+            data: torch.Tensor,
+        ) -> List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]:
+            a_coeff, fsdict = fs_dict_func(data)
+            fsdict = cast(Dict[str, torch.Tensor], fsdict)
+            return [
+                cast(torch.Tensor, a_coeff),
+                (fsdict["ad"], fsdict["da"], fsdict["dd"]),
+            ]
+
+        return _tuple_func
+
+    def _transform_tuple_to_fsdict_func(
+        self,
+        fsdict_func: Callable[
+            [List[Union[torch.Tensor, Dict[str, torch.Tensor]]]], torch.Tensor
+        ],
+    ) -> Callable[
+        [List[Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]]],
+        torch.Tensor,
+    ]:
+        def _fsdict_func(
+            coeffs: List[
+                Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor, torch.Tensor]]
+            ]
+        ) -> torch.Tensor:
+            a, (h, v, d) = coeffs
+            return fsdict_func([cast(torch.Tensor, a), {"ad": h, "da": v, "dd": d}])
+
+        return _fsdict_func
+
     def _recursive_dwt2d(self, data: torch.Tensor, level: int, path: str) -> None:
         if not self.maxlevel:
             raise AssertionError
 
-        # TODO: This is a workaround since the convolutional transforms insert a
-        #       squeezable dimension. We should adapt the wavedec2 code instead.
-        if data.dim() == 4:
-            data = data.squeeze(1)
-
         self.data[path] = data
         if level < self.maxlevel:
             result_a, (result_h, result_v, result_d) = self._get_wavedec(
                 data.shape[-2:]
             )(data)
             # assert for type checking
             assert not isinstance(result_a, tuple)
@@ -448,15 +515,15 @@
         The code elements denote the filter application order. The filters
         are named following the pywt convention as:
         a - LL, low-low coefficients
         h - LH, low-high coefficients
         v - HL, high-low coefficients
         d - HH, high-high coefficients
     """
-    wp_natural_path = list(product(["a", "h", "v", "d"], repeat=level))
+    wp_natural_path = product(["a", "h", "v", "d"], repeat=level)
 
     def _get_graycode_order(level: int, x: str = "a", y: str = "d") -> List[str]:
         graycode_order = [x, y]
         for _ in range(level - 1):
             graycode_order = [x + path for path in graycode_order] + [
                 y + path for path in graycode_order[::-1]
             ]
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/sparse_math.py` & `ptwt-0.1.5/src/ptwt/sparse_math.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Efficiently construct fwt operations using sparse matrices."""
 # Written by moritz ( @ wolter.tech ) 17.09.21
+from itertools import product
 from typing import List
 
-import numpy as np
 import torch
 
 
 def _dense_kron(
     sparse_tensor_a: torch.Tensor, sparse_tensor_b: torch.Tensor
 ) -> torch.Tensor:
     """Faster than sparse_kron.
@@ -40,29 +40,32 @@
     Args:
         sparse_tensor_a (torch.Tensor): Sparse 2d-Tensor a of shape [m, n].
         sparse_tensor_b (torch.Tensor): Sparse 2d-Tensor b of shape [p, q].
 
     Returns:
         torch.Tensor: The resulting [mp, nq] tensor.
     """
-    if not sparse_tensor_a.is_coalesced():
-        sparse_tensor_a = sparse_tensor_a.coalesce()
-    if not sparse_tensor_b.is_coalesced():
-        sparse_tensor_b = sparse_tensor_b.coalesce()
+    assert sparse_tensor_a.device == sparse_tensor_b.device
+
+    sparse_tensor_a = sparse_tensor_a.coalesce()
+    sparse_tensor_b = sparse_tensor_b.coalesce()
     output_shape = (
         sparse_tensor_a.shape[0] * sparse_tensor_b.shape[0],
         sparse_tensor_a.shape[1] * sparse_tensor_b.shape[1],
     )
     nzz_a = len(sparse_tensor_a.values())
     nzz_b = len(sparse_tensor_b.values())
 
     # take care of the zero case.
     if nzz_a == 0 or nzz_b == 0:
         return torch.sparse_coo_tensor(
-            torch.zeros([2, 1]), torch.zeros([1]), size=output_shape
+            torch.zeros([2, 1]),
+            torch.zeros([1]),
+            size=output_shape,
+            device=sparse_tensor_a.device,
         )
 
     # expand A's entries into blocks
     row = sparse_tensor_a.indices()[0, :].repeat_interleave(nzz_b)
     col = sparse_tensor_a.indices()[1, :].repeat_interleave(nzz_b)
     data = sparse_tensor_a.values().repeat_interleave(nzz_b)
     row *= sparse_tensor_b.shape[0]
@@ -74,15 +77,18 @@
     col += sparse_tensor_b.indices()[1, :]
     row, col = row.reshape(-1), col.reshape(-1)
 
     # compute block entries
     data = data.reshape(-1, nzz_b) * sparse_tensor_b.values()
     data = data.reshape(-1)
     result = torch.sparse_coo_tensor(
-        torch.stack([row, col], 0), data, size=output_shape
+        torch.stack([row, col], 0),
+        data,
+        size=output_shape,
+        device=sparse_tensor_a.device,
     )
 
     return result
 
 
 def cat_sparse_identity_matrix(
     sparse_matrix: torch.Tensor, new_length: int
@@ -119,15 +125,17 @@
     extra_values = torch.ones(
         [new_length - sparse_matrix.shape[0]],
         dtype=sparse_matrix.dtype,
         device=sparse_matrix.device,
     )
     new_indices = torch.cat([sparse_matrix.coalesce().indices(), extra_indices], -1)
     new_values = torch.cat([sparse_matrix.coalesce().values(), extra_values], -1)
-    new_matrix = torch.sparse_coo_tensor(new_indices, new_values)
+    new_matrix = torch.sparse_coo_tensor(
+        new_indices, new_values, device=sparse_matrix.device
+    )
     return new_matrix
 
 
 def sparse_diag(
     diagonal: torch.Tensor, col_offset: int, rows: int, cols: int
 ) -> torch.Tensor:
     """Create a rows-by-cols sparse diagnoal-matrix.
@@ -163,15 +171,19 @@
         diagonal = diagonal[mask]
     if torch.max(diag_indices[1]) >= cols:
         mask = diag_indices[1] < cols
         diag_indices = diag_indices[:, mask]
         diagonal = diagonal[mask]
 
     diag = torch.sparse_coo_tensor(
-        diag_indices, diagonal, size=(rows, cols), dtype=diagonal.dtype
+        diag_indices,
+        diagonal,
+        size=(rows, cols),
+        dtype=diagonal.dtype,
+        device=diagonal.device,
     )
 
     return diag
 
 
 def sparse_replace_row(
     matrix: torch.Tensor, row_index: int, row: torch.Tensor
@@ -185,16 +197,15 @@
         row_index (int): The row to replace.
         row (torch.Tensor): The row to insert into the sparse matrix.
 
     Returns:
         torch.Tensor: A sparse matrix, with the new row inserted at
         row_index.
     """
-    if not matrix.is_coalesced():
-        matrix = matrix.coalesce()
+    matrix = matrix.coalesce()
     assert (
         matrix.shape[-1] == row.shape[-1]
     ), "matrix and replacement-row must share the same column number."
 
     # delete existing indices we dont want
     diag_indices = torch.arange(matrix.shape[0])
     diag = torch.ones_like(diag_indices)
@@ -202,16 +213,15 @@
     removal_matrix = torch.sparse_coo_tensor(
         torch.stack([diag_indices] * 2, 0),
         diag,
         size=matrix.shape,
         device=matrix.device,
         dtype=matrix.dtype,
     )
-    if not row.is_coalesced():
-        row = row.coalesce()
+    row = row.coalesce()
 
     addition_matrix = torch.sparse_coo_tensor(
         torch.stack((row.indices()[0, :] + row_index, row.indices()[1, :]), 0),
         row.values(),
         size=matrix.shape,
         device=matrix.device,
         dtype=matrix.dtype,
@@ -319,32 +329,31 @@
 
 def construct_conv_matrix(
     filter: torch.Tensor, input_rows: int, mode: str = "valid"
 ) -> torch.Tensor:
     """Construct a convolution matrix.
 
     Full, valid and same, padding are supported.
+    For reference see:
+    https://github.com/RoyiAvital/StackExchangeCodes/blob/\
+    master/StackOverflow/Q2080835/CreateConvMtxSparse.m
 
     Args:
         filter (torch.tensor): The 1d-filter to convolve with.
         input_rows (int): The number of columns in the input.
         mode (str): String indetifier for the desired padding.
             Choose 'full', 'valid' or 'same'.
             Defaults to valid.
 
     Returns:
         torch.Tensor: The sparse convolution tensor.
 
     Raises:
         ValueError: If the padding is not 'full', 'same' or 'valid'.
 
-    Note:
-        For reference see:
-        https://github.com/RoyiAvital/StackExchangeCodes/blob/\
-            master/StackOverflow/Q2080835/CreateConvMtxSparse.m
     """
     filter_length = len(filter)
 
     if mode == "full":
         start_row = 0
         stop_row = input_rows + filter_length - 1
     elif mode == "same" or mode == "sameshift":
@@ -354,30 +363,29 @@
         stop_row = start_row + input_rows - 1
     elif mode == "valid":
         start_row = filter_length - 1
         stop_row = input_rows - 1
     else:
         raise ValueError("unkown padding type.")
 
-    row_indices = []
-    column_indices = []
-    values = []
-    for column in range(0, input_rows):
-        for row in range(0, filter_length):
-            check_row = column + row
-            if (check_row >= start_row) and (check_row <= stop_row):
-                row_indices.append(row + column - start_row)
-                column_indices.append(column)
-                values.append(filter[row])
-    indices = torch.tensor(
-        np.stack([row_indices, column_indices]), device=filter.device
-    )
-    value_tensor = torch.stack(values)
+    product_lst = [
+        (row, col)
+        for col, row in product(range(input_rows), range(filter_length))
+        if row + col in range(start_row, stop_row + 1)
+    ]
+
+    row_indices = torch.tensor(
+        [row + col - start_row for row, col in product_lst], device=filter.device
+    )
+    col_indices = torch.tensor([col for row, col in product_lst], device=filter.device)
+    indices = torch.stack([row_indices, col_indices])
+    values = torch.stack([filter[row] for row, col in product_lst])
+
     return torch.sparse_coo_tensor(
-        indices, value_tensor, device=filter.device, dtype=filter.dtype
+        indices, values, device=filter.device, dtype=filter.dtype
     )
 
 
 def construct_conv2d_matrix(
     filter: torch.Tensor,
     input_rows: int,
     input_columns: int,
@@ -427,15 +435,15 @@
         raise ValueError("unknown conv mode.")
 
     block_matrix_list = []
     for i in range(matrix_block_number):
         block_matrix_list.append(construct_conv_matrix(filter[:, i], input_rows, mode))
 
     diag_values = torch.ones(
-        [int(np.min([kronecker_rows, input_columns]))],
+        min(kronecker_rows, input_columns),
         dtype=filter.dtype,
         device=filter.device,
     )
     diag = sparse_diag(diag_values, diag_index, kronecker_rows, input_columns)
     sparse_conv_matrix = kron(diag, block_matrix_list[0])
 
     for block_matrix in block_matrix_list[1:]:
@@ -571,7 +579,27 @@
     batch_size = matrix_batch.shape[0]
     if matrix.shape[1] != matrix_batch.shape[1]:
         raise ValueError("Matrix shapes not compatible.")
 
     # Stack the vector batch into columns. (b, n, k) -> (n, b, k) -> (n, b*k)
     vectors = matrix_batch.transpose(0, 1).reshape(matrix.shape[1], -1)
     return matrix.mm(vectors).reshape(matrix.shape[0], batch_size, -1).transpose(1, 0)
+
+
+def _batch_dim_mm(
+    matrix: torch.Tensor, batch_tensor: torch.Tensor, dim: int
+) -> torch.Tensor:
+    """Multiply batch_tensor with matrix along the dimensions specified in dim.
+
+    Args:
+        matrix (torch.Tensor): A matrix of shape [m, n]
+        batch_tensor (torch.Tensor): A tensor with a selected dim of length n.
+        dim (int): The position of the desired dimension.
+
+    Returns:
+        torch.Tensor: The multiplication result.
+    """
+    dim_length = batch_tensor.shape[dim]
+    permuted_tensor = batch_tensor.transpose(dim, -1)
+    permuted_shape = permuted_tensor.shape
+    res = torch.sparse.mm(matrix, permuted_tensor.reshape(-1, dim_length).T).T
+    return res.reshape(list(permuted_shape[:-1]) + [matrix.shape[0]]).transpose(-1, dim)
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/version.py` & `ptwt-0.1.5/src/ptwt/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.1.4.post2"
+VERSION = "0.1.5"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`ptwt` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `ptwt-0.1.4.post2/src/ptwt/wavelets_learnable.py` & `ptwt-0.1.5/src/ptwt/wavelets_learnable.py`

 * *Files identical despite different names*

### Comparing `ptwt-0.1.4.post2/src/ptwt.egg-info/PKG-INFO` & `ptwt-0.1.5/src/ptwt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: ptwt
-Version: 0.1.4.post2
+Version: 0.1.5
 Summary: Differentiable and gpu enabled fast wavelet transforms in PyTorch
 Home-page: https://github.com/v0lta/PyTorch-Wavelet-Toolbox
 Download-URL: https://github.com/v0lta/PyTorch-Wavelet-Toolbox/releases
 Author: Moritz Wolter
 Author-email: moritz@wolter.tech
 Maintainer: Moritz Wolter
 Maintainer-email: moritz@wolter.tech
 License: EUPL-1.2
 Project-URL: Bug Tracker, https://github.com/v0lta/PyTorch-Wavelet-Toolbox/issues
 Project-URL: Source Code, https://github.com/v0lta/PyTorch-Wavelet-Toolbox
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ********************************
 Pytorch Wavelet Toolbox (`ptwt`)
@@ -55,27 +53,30 @@
     :alt: Black code style
 
 .. image:: https://static.pepy.tech/personalized-badge/ptwt?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
  :target: https://pepy.tech/project/ptwt
 
 
 
+
 Welcome to the PyTorch wavelet toolbox. This package implements:
 
 - the fast wavelet transform (fwt) via ``wavedec`` and its inverse by providing the ``waverec`` function,
 - the two-dimensional fwt is called ``wavedec2`` the synthesis counterpart ``waverec2``,
 - ``wavedec3`` and ``waverec3`` cover the three-dimensional analysis and synthesis case,
-- ``MatrixWavedec`` and ``MatrixWaverec`` provide sparse-matrix-based fast wavelet transforms with boundary filters,
-- 2d sparse-matrix transforms with separable & non-separable boundary filters are available (experimental),
+- ``fswavedec2``, ``fswavedec3``, ``fswaverec2`` and ``fswaverec3`` support separable transformations.
+- ``MatrixWavedec`` and ``MatrixWaverec`` implement sparse-matrix-based fast wavelet transforms with boundary filters,
+- 2d sparse-matrix transforms with separable & non-separable boundary filters are available,
+- ``MatrixWavedec3`` and ``MatrixWaverec3`` allow separable 3D-fwt's with boundary filters.
 - ``cwt`` computes a one-dimensional continuous forward transform,
 - single and two-dimensional wavelet packet forward and backward transforms are available via the ``WaveletPacket`` and ``WaveletPacket2D`` objects,
 - finally, this package provides adaptive wavelet support (experimental).
 
-This toolbox supports pywt-wavelets. Complete documentation is available:
-https://pytorch-wavelet-toolbox.readthedocs.io/
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+Complete documentation is available at: https://pytorch-wavelet-toolbox.readthedocs.io/
 
 
 **Installation**
 
 Install the toolbox via pip or clone this repository. In order to use ``pip``, type:
 
 .. code-block:: sh
@@ -128,15 +129,15 @@
 
 .. code-block:: python
 
   import ptwt, pywt, torch
   import numpy as np
   import scipy.misc
 
-  face = np.transpose(scipy.misc.face(),
+  face = np.transpose(scipy.datasets.face(),
                           [2, 0, 1]).astype(np.float64)
   pytorch_face = torch.tensor(face)
   coefficients = ptwt.wavedec2(pytorch_face, pywt.Wavelet("haar"),
                                   level=2, mode="constant")
   reconstruction = ptwt.waverec2(coefficients, pywt.Wavelet("haar"))
   np.max(np.abs(face - reconstruction.squeeze(1).numpy()))
 
@@ -170,16 +171,16 @@
   # backward 
   matrix_waverec = ptwt.MatrixWaverec(pywt.Wavelet("haar"))
   rec = matrix_waverec(coeff)
   print(rec)
 
 
 The process for the 2d transforms ``MatrixWavedec2``, ``MatrixWaverec2`` works similarly.
-By default, a non-separable transformation is used.
-To use a separable transformation, pass ``separable=True`` to ``MatrixWavedec2`` and ``MatrixWaverec2``.
+By default, a separable transformation is used.
+To use a non-separable transformation, pass ``separable=False`` to ``MatrixWavedec2`` and ``MatrixWaverec2``.
 Separable transformations use a 1d transformation along both axes, which might be faster since fewer matrix entries
 have to be orthogonalized.
 
 
 **Adaptive** **Wavelets**
 
 Experimental code to train an adaptive wavelet layer in PyTorch is available in the ``examples`` folder. In addition to static wavelets
@@ -189,23 +190,26 @@
 - and optimizable orthogonal-wavelets are supported.
 
 See https://github.com/v0lta/PyTorch-Wavelet-Toolbox/tree/main/examples/network_compression/ for a complete implementation.
 
 
 **Testing**
 
-The ``tests`` folder contains multiple tests to allow independent verification of this toolbox. After cloning the
-repository, and moving into the main directory, and installing ``nox`` with ``pip install nox`` run:
+The ``tests`` folder contains multiple tests to allow independent verification of this toolbox.
+The GitHub workflow executes a subset of all tests for efficiency reasons. 
+After cloning the repository, moving into the main directory, and installing ``nox`` with ``pip install nox`` run
 
 .. code-block:: sh
 
   $ nox --session test
 
 
 
+to run all existing tests.
+
 Citation
 """"""""
 
 If you use this work in a scientific context please cite:
 
 .. code-block::
 
@@ -228,9 +232,7 @@
     title = {{Randbehandlung bei Wavelets für Faltungsnetzwerke}},
     type = {Bachelor's Thesis},
     annote = {Gbachelor},
     year = {2021},
     school = {Institut f\"ur Numerische Simulation, Universit\"at Bonn}
   }
 
-
-
```

### Comparing `ptwt-0.1.4.post2/src/ptwt.egg-info/SOURCES.txt` & `ptwt-0.1.5/src/ptwt.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 LICENSE
 README.rst
 setup.cfg
 setup.py
 src/ptwt/__init__.py
-src/ptwt/_mackey_glass.py
 src/ptwt/_util.py
 src/ptwt/continuous_transform.py
 src/ptwt/conv_transform.py
 src/ptwt/conv_transform_2.py
 src/ptwt/conv_transform_3.py
 src/ptwt/matmul_transform.py
 src/ptwt/matmul_transform_2.py
+src/ptwt/matmul_transform_3.py
 src/ptwt/packets.py
+src/ptwt/separable_conv_transform.py
 src/ptwt/sparse_math.py
 src/ptwt/version.py
 src/ptwt/wavelets_learnable.py
 src/ptwt.egg-info/PKG-INFO
 src/ptwt.egg-info/SOURCES.txt
 src/ptwt.egg-info/dependency_links.txt
 src/ptwt.egg-info/requires.txt
-src/ptwt.egg-info/top_level.txt
+src/ptwt.egg-info/top_level.txt
+tests/test_convolution_fwt.py
+tests/test_convolution_fwt_3.py
+tests/test_cwt.py
+tests/test_jit.py
+tests/test_matrix_fwt.py
+tests/test_matrix_fwt_2.py
+tests/test_matrix_fwt_3.py
+tests/test_packets.py
+tests/test_separable_conv_fwt.py
+tests/test_sparse_math.py
+tests/test_util.py
+tests/test_wavelet.py
```

