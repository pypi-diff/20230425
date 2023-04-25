# Comparing `tmp/clarabel-0.4.1-cp37-abi3-win_amd64.whl.zip` & `tmp/clarabel-0.5.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 317077 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4461 b- defN 23-Mar-08 20:55 clarabel-0.4.1.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Mar-08 20:55 clarabel-0.4.1.dist-info/WHEEL
--rw-r--r--  4.6 unx    11558 b- defN 23-Mar-08 20:55 clarabel-0.4.1.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx      115 b- defN 23-Mar-08 20:55 clarabel/__init__.py
--rwxr-xr-x  4.6 unx   781312 b- defN 23-Mar-08 20:55 clarabel/clarabel.pyd
--rw-r--r--  4.6 unx      472 b- defN 23-Mar-08 20:55 clarabel-0.4.1.dist-info/RECORD
-6 files, 798014 bytes uncompressed, 316231 bytes compressed:  60.4%
+Zip file size: 331269 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     4398 b- defN 23-Apr-25 08:50 clarabel-0.5.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-25 08:50 clarabel-0.5.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11558 b- defN 23-Apr-25 08:50 clarabel-0.5.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx      160 b- defN 23-Apr-25 08:50 clarabel/__init__.py
+-rwxr-xr-x  4.6 unx   825344 b- defN 23-Apr-25 08:50 clarabel/clarabel.pyd
+-rw-r--r--  4.6 unx      472 b- defN 23-Apr-25 08:50 clarabel-0.5.0.dist-info/RECORD
+6 files, 842028 bytes uncompressed, 330423 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: clarabel-0.4.1.dist-info/METADATA
+Filename: clarabel-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: clarabel-0.4.1.dist-info/WHEEL
+Filename: clarabel-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: clarabel-0.4.1.dist-info/license_files/LICENSE.md
+Filename: clarabel-0.5.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: clarabel/__init__.py
 Comment: 
 
 Filename: clarabel/clarabel.pyd
 Comment: 
 
-Filename: clarabel-0.4.1.dist-info/RECORD
+Filename: clarabel-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clarabel/__init__.py

```diff
@@ -1,5 +1,8 @@
-from .clarabel import *
-
-__doc__ = clarabel.__doc__
-if hasattr(clarabel, "__all__"):
-    __all__ = clarabel.__all__
+from .clarabel import *
+
+__doc__ = clarabel.__doc__
+if hasattr(clarabel, "__all__"):
+    __all__ = clarabel.__all__
+
+clarabel.force_load_blas_lapack()
+
```

## Comparing `clarabel-0.4.1.dist-info/METADATA` & `clarabel-0.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: clarabel
-Version: 0.4.1
+Version: 0.5.0
 Classifier: Programming Language :: Rust
 Requires-Dist: numpy
 Requires-Dist: scipy
 License-File: LICENSE.md
 Summary: Clarabel Conic Interior Point Solver for Rust / Python
-Keywords: convex,optimization,QP,LP,SOCP
+Keywords: convex,optimization,QP,LP,SOCP,SDP,conic
 Author: Paul Goulart <paul.goulart@eng.ox.ac.uk>
 Author-email: Paul Goulart <paul.goulart@eng.ox.ac.uk>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/oxfordcontrol/Clarabel.rs
 
@@ -22,15 +22,15 @@
 Interior Point Conic Optimization for Rust and Python
 </h1>
 <p align="center">
    <a href="https://github.com/oxfordcontrol/Clarabel.rs/actions"><img src="https://github.com/oxfordcontrol/Clarabel.rs/workflows/ci/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/oxfordcontrol/Clarabel.rs"><img src="https://codecov.io/gh/oxfordcontrol/Clarabel.rs/branch/main/graph/badge.svg"></a>
   <a href="https://oxfordcontrol.github.io/ClarabelDocs/stable"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
-  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.4.1-blue.svg"></a>
+  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.5.0-blue.svg"></a>
 </p>
 
 <p align="center">
   <a href="#features">Features</a> •
   <a href="#installation">Installation</a> •
   <a href="#license-">License</a> •
   <a href="https://oxfordcontrol.github.io/ClarabelDocs/stable">Documentation</a>
@@ -59,15 +59,15 @@
 __For more information see the Clarabel Documentation ([stable](https://oxfordcontrol.github.io/ClarabelDocs/stable) |  [dev](https://oxfordcontrol.github.io/ClarabelDocs/dev)).__
 
 Clarabel is also available in a Julia implementation.  See [here](https://github.com/oxfordcontrol/Clarabel.jl).
  
 
 ## Features
 
-* __Versatile__: Clarabel.rs solves linear programs (LPs), quadratic programs (QPs) and second-order cone programs (SOCPs).   It also solves problems with exponential and power cone constraints.  Future versions will provide support for problems involving positive semidefinite cone constraints.
+* __Versatile__: Clarabel.rs solves linear programs (LPs), quadratic programs (QPs), second-order cone programs (SOCPs) and semidefinite programs (SDPs). It also solves problems with exponential and power cone constraints.
 * __Quadratic objectives__: Unlike interior point solvers based on the standard homogeneous self-dual embedding (HSDE), Clarabel.rs handles quadratic objectives without requiring any epigraphical reformulation of the objective.   It can therefore be significantly faster than other HSDE-based solvers for problems with quadratic objective functions.
 * __Infeasibility detection__: Infeasible problems are detected using a homogeneous embedding technique.
 * __Open Source__: Our code is available on [GitHub](https://github.com/oxfordcontrol/Clarabel.rs) and distributed under the Apache 2.0 License
 
 # Installation
 
 Clarabel can be imported to Cargo based Rust projects by adding
```

### html2text {}

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1 Name: clarabel Version: 0.4.1 Classifier: Programming
+Metadata-Version: 2.1 Name: clarabel Version: 0.5.0 Classifier: Programming
 Language :: Rust Requires-Dist: numpy Requires-Dist: scipy License-File:
 LICENSE.md Summary: Clarabel Conic Interior Point Solver for Rust / Python
-Keywords: convex,optimization,QP,LP,SOCP Author: Paul Goulart
+Keywords: convex,optimization,QP,LP,SOCP,SDP,conic Author: Paul Goulart
 goulart@eng.ox.ac.uk> Author-email: Paul Goulart
 goulart@eng.ox.ac.uk> License: Apache-2.0 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Source
 Code, https://github.com/oxfordcontrol/Clarabel.rs
    ****** [https://github.com/oxfordcontrol/ClarabelDocs/blob/main/docs/src/
    assets/logo-banner-light-rs.png#gh-light-mode-only] [https://github.com/
     oxfordcontrol/ClarabelDocs/blob/main/docs/src/assets/logo-banner-dark-
                           rs.png#gh-dark-mode-only]
          Interior Point Conic Optimization for Rust and Python ******
           [https://github.com/oxfordcontrol/Clarabel.rs/workflows/ci/
 badge.svg?branch=main] [https://codecov.io/gh/oxfordcontrol/Clarabel.rs/branch/
    main/graph/badge.svg] [https://img.shields.io/badge/Documentation-stable-
    purple.svg] [https://img.shields.io/badge/License-Apache%202.0-blue.svg]
-            [https://img.shields.io/badge/Release-v0.4.1-blue.svg]
+            [https://img.shields.io/badge/Release-v0.5.0-blue.svg]
             Features â¢ Installation â¢ License â¢ Documentation
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver
 for convex optimization problems using a novel homogeneous embedding.
 Clarabel.rs solves the following problem: $$ \begin{array}{r} \text{minimize} &
 \frac{1}{2}x^T P x + q^T x\\\\[2ex] \text{subject to} & Ax + s = b \\\\[1ex] &
 s \in \mathcal{K} \end{array} $$ with decision variables $x \in \mathbb{R}^n$,
 $s \in \mathbb{R}^m$ and data matrices $P=P^\top \succeq 0$, $q \in \mathbb
 {R}^n$, $A \in \mathbb{R}^{m \times n}$, and $b \in \mathbb{R}^m$. The convex
 set $\mathcal{K}$ is a composition of convex cones. __For more information see
 the Clarabel Documentation ([stable](https://oxfordcontrol.github.io/
 ClarabelDocs/stable) | [dev](https://oxfordcontrol.github.io/ClarabelDocs/
 dev)).__ Clarabel is also available in a Julia implementation. See [here]
 (https://github.com/oxfordcontrol/Clarabel.jl). ## Features * __Versatile__:
-Clarabel.rs solves linear programs (LPs), quadratic programs (QPs) and second-
-order cone programs (SOCPs). It also solves problems with exponential and power
-cone constraints. Future versions will provide support for problems involving
-positive semidefinite cone constraints. * __Quadratic objectives__: Unlike
-interior point solvers based on the standard homogeneous self-dual embedding
-(HSDE), Clarabel.rs handles quadratic objectives without requiring any
-epigraphical reformulation of the objective. It can therefore be significantly
-faster than other HSDE-based solvers for problems with quadratic objective
-functions. * __Infeasibility detection__: Infeasible problems are detected
-using a homogeneous embedding technique. * __Open Source__: Our code is
-available on [GitHub](https://github.com/oxfordcontrol/Clarabel.rs) and
+Clarabel.rs solves linear programs (LPs), quadratic programs (QPs), second-
+order cone programs (SOCPs) and semidefinite programs (SDPs). It also solves
+problems with exponential and power cone constraints. * __Quadratic
+objectives__: Unlike interior point solvers based on the standard homogeneous
+self-dual embedding (HSDE), Clarabel.rs handles quadratic objectives without
+requiring any epigraphical reformulation of the objective. It can therefore be
+significantly faster than other HSDE-based solvers for problems with quadratic
+objective functions. * __Infeasibility detection__: Infeasible problems are
+detected using a homogeneous embedding technique. * __Open Source__: Our code
+is available on [GitHub](https://github.com/oxfordcontrol/Clarabel.rs) and
 distributed under the Apache 2.0 License # Installation Clarabel can be
 imported to Cargo based Rust projects by adding ```rust [dependencies] clarabel
 = "0" ``` to the project's `Cargo.toml` file. To install from source, see the
 [Rust Installation Documentation](https://oxfordcontrol.github.io/ClarabelDocs/
 stable/rust/installation_rs/). To use the Python interface to the solver: ```
 pip install clarabel ``` To install the Python interface from source, see the
 [Python Installation Documentation](https://oxfordcontrol.github.io/
```

## Comparing `clarabel-0.4.1.dist-info/license_files/LICENSE.md` & `clarabel-0.5.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

