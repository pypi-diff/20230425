# Comparing `tmp/graphix-0.2.0.tar.gz` & `tmp/graphix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphix-0.2.0.tar", last modified: Sat Mar 18 14:02:52 2023, max compression
+gzip compressed data, was "graphix-0.2.1.tar", last modified: Tue Apr 25 07:36:33 2023, max compression
```

## Comparing `graphix-0.2.0.tar` & `graphix-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-03-18 14:02:52.883152 graphix-0.2.0/
--rw-r--r--   0 sunami     (501) staff       (20)    10761 2022-09-29 19:21:12.000000 graphix-0.2.0/LICENSE
--rw-r--r--   0 sunami     (501) staff       (20)       94 2022-12-15 06:51:32.000000 graphix-0.2.0/MANIFEST.in
--rw-r--r--   0 sunami     (501) staff       (20)     4970 2023-03-18 14:02:52.882985 graphix-0.2.0/PKG-INFO
--rw-r--r--   0 sunami     (501) staff       (20)     4036 2023-02-18 20:39:43.000000 graphix-0.2.0/README.md
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-03-18 14:02:52.876566 graphix-0.2.0/docs/
--rw-r--r--   0 sunami     (501) staff       (20)    10244 2023-02-17 11:09:17.000000 graphix-0.2.0/docs/.DS_Store
--rw-r--r--   0 sunami     (501) staff       (20)      638 2022-12-02 15:18:40.000000 graphix-0.2.0/docs/Makefile
--rw-r--r--   0 sunami     (501) staff       (20)      804 2022-12-02 15:18:40.000000 graphix-0.2.0/docs/make.bat
--rw-r--r--   0 sunami     (501) staff       (20)     1294 2023-01-09 01:14:11.000000 graphix-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-03-18 14:02:52.879827 graphix-0.2.0/graphix/
--rw-r--r--   0 sunami     (501) staff       (20)      243 2022-12-15 06:51:32.000000 graphix-0.2.0/graphix/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)     7451 2023-01-14 13:01:46.000000 graphix-0.2.0/graphix/clifford.py
--rw-r--r--   0 sunami     (501) staff       (20)    18838 2022-12-15 11:43:28.000000 graphix-0.2.0/graphix/gflow.py
--rw-r--r--   0 sunami     (501) staff       (20)    13678 2023-01-14 13:01:46.000000 graphix-0.2.0/graphix/graphsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     2463 2023-03-01 11:13:38.000000 graphix-0.2.0/graphix/ops.py
--rw-r--r--   0 sunami     (501) staff       (20)    43805 2023-03-16 06:55:48.000000 graphix-0.2.0/graphix/pattern.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-03-18 14:02:52.881152 graphix-0.2.0/graphix/sim/
--rw-r--r--   0 sunami     (501) staff       (20)        0 2022-12-12 11:17:35.000000 graphix-0.2.0/graphix/sim/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)    11313 2023-03-01 11:13:38.000000 graphix-0.2.0/graphix/sim/statevec.py
--rw-r--r--   0 sunami     (501) staff       (20)    25419 2023-03-01 11:13:38.000000 graphix-0.2.0/graphix/sim/tensornet.py
--rw-r--r--   0 sunami     (501) staff       (20)     2269 2023-03-01 11:13:38.000000 graphix-0.2.0/graphix/simulator.py
--rw-r--r--   0 sunami     (501) staff       (20)    37241 2023-03-16 06:55:32.000000 graphix-0.2.0/graphix/transpiler.py
--rw-r--r--   0 sunami     (501) staff       (20)       22 2023-03-16 06:55:56.000000 graphix-0.2.0/graphix/version.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-03-18 14:02:52.880513 graphix-0.2.0/graphix.egg-info/
--rw-r--r--   0 sunami     (501) staff       (20)     4970 2023-03-18 14:02:52.000000 graphix-0.2.0/graphix.egg-info/PKG-INFO
--rw-r--r--   0 sunami     (501) staff       (20)      651 2023-03-18 14:02:52.000000 graphix-0.2.0/graphix.egg-info/SOURCES.txt
--rw-r--r--   0 sunami     (501) staff       (20)        1 2023-03-18 14:02:52.000000 graphix-0.2.0/graphix.egg-info/dependency_links.txt
--rw-r--r--   0 sunami     (501) staff       (20)       85 2023-03-18 14:02:52.000000 graphix-0.2.0/graphix.egg-info/requires.txt
--rw-r--r--   0 sunami     (501) staff       (20)        8 2023-03-18 14:02:52.000000 graphix-0.2.0/graphix.egg-info/top_level.txt
--rw-r--r--   0 sunami     (501) staff       (20)       81 2022-12-15 06:51:32.000000 graphix-0.2.0/pyproject.toml
--rw-r--r--   0 sunami     (501) staff       (20)       38 2023-03-18 14:02:52.883200 graphix-0.2.0/setup.cfg
--rw-r--r--   0 sunami     (501) staff       (20)     1488 2022-12-21 06:16:27.000000 graphix-0.2.0/setup.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-03-18 14:02:52.882742 graphix-0.2.0/tests/
--rw-r--r--   0 sunami     (501) staff       (20)     2904 2023-01-14 13:01:46.000000 graphix-0.2.0/tests/test_clifford.py
--rw-r--r--   0 sunami     (501) staff       (20)     3624 2022-12-15 11:43:28.000000 graphix-0.2.0/tests/test_gflow.py
--rw-r--r--   0 sunami     (501) staff       (20)     3974 2022-12-15 11:43:28.000000 graphix-0.2.0/tests/test_graphsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     5758 2023-03-16 06:55:48.000000 graphix-0.2.0/tests/test_pattern.py
--rw-r--r--   0 sunami     (501) staff       (20)    15835 2023-03-01 11:13:38.000000 graphix-0.2.0/tests/test_tnsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     5102 2023-01-14 13:01:46.000000 graphix-0.2.0/tests/test_transpiler.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.241831 graphix-0.2.1/
+-rw-r--r--   0 ss         (501) staff       (20)    10766 2023-04-25 07:26:44.000000 graphix-0.2.1/LICENSE
+-rw-r--r--   0 ss         (501) staff       (20)       94 2022-12-15 06:51:32.000000 graphix-0.2.1/MANIFEST.in
+-rw-r--r--   0 ss         (501) staff       (20)     5510 2023-04-25 07:36:33.241436 graphix-0.2.1/PKG-INFO
+-rw-r--r--   0 ss         (501) staff       (20)     4576 2023-04-25 07:20:26.000000 graphix-0.2.1/README.md
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.214418 graphix-0.2.1/docs/
+-rw-r--r--   0 ss         (501) staff       (20)      638 2022-12-02 15:18:40.000000 graphix-0.2.1/docs/Makefile
+-rw-r--r--   0 ss         (501) staff       (20)      804 2022-12-02 15:18:40.000000 graphix-0.2.1/docs/make.bat
+-rw-r--r--   0 ss         (501) staff       (20)     1294 2023-01-09 01:14:11.000000 graphix-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.226204 graphix-0.2.1/graphix/
+-rw-r--r--   0 ss         (501) staff       (20)      247 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/__init__.py
+-rw-r--r--   0 ss         (501) staff       (20)     7451 2023-01-14 13:01:46.000000 graphix-0.2.1/graphix/clifford.py
+-rw-r--r--   0 ss         (501) staff       (20)     4173 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/generator.py
+-rw-r--r--   0 ss         (501) staff       (20)    13035 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/gflow.py
+-rw-r--r--   0 ss         (501) staff       (20)    13678 2023-01-14 13:01:46.000000 graphix-0.2.1/graphix/graphsim.py
+-rw-r--r--   0 ss         (501) staff       (20)     2463 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/ops.py
+-rw-r--r--   0 ss         (501) staff       (20)    46518 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/pattern.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.232022 graphix-0.2.1/graphix/sim/
+-rw-r--r--   0 ss         (501) staff       (20)        0 2022-12-12 11:17:35.000000 graphix-0.2.1/graphix/sim/__init__.py
+-rw-r--r--   0 ss         (501) staff       (20)    11313 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/sim/statevec.py
+-rw-r--r--   0 ss         (501) staff       (20)    25419 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/sim/tensornet.py
+-rw-r--r--   0 ss         (501) staff       (20)     2269 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/simulator.py
+-rw-r--r--   0 ss         (501) staff       (20)    37241 2023-03-16 06:55:32.000000 graphix-0.2.1/graphix/transpiler.py
+-rw-r--r--   0 ss         (501) staff       (20)       22 2023-04-25 06:52:17.000000 graphix-0.2.1/graphix/version.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.229563 graphix-0.2.1/graphix.egg-info/
+-rw-r--r--   0 ss         (501) staff       (20)     5510 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/PKG-INFO
+-rw-r--r--   0 ss         (501) staff       (20)      681 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/SOURCES.txt
+-rw-r--r--   0 ss         (501) staff       (20)        1 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/dependency_links.txt
+-rw-r--r--   0 ss         (501) staff       (20)       85 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/requires.txt
+-rw-r--r--   0 ss         (501) staff       (20)        8 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/top_level.txt
+-rw-r--r--   0 ss         (501) staff       (20)       81 2022-12-15 06:51:32.000000 graphix-0.2.1/pyproject.toml
+-rw-r--r--   0 ss         (501) staff       (20)       38 2023-04-25 07:36:33.241956 graphix-0.2.1/setup.cfg
+-rw-r--r--   0 ss         (501) staff       (20)     1488 2022-12-21 06:16:27.000000 graphix-0.2.1/setup.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.240319 graphix-0.2.1/tests/
+-rw-r--r--   0 ss         (501) staff       (20)     2904 2023-01-14 13:01:46.000000 graphix-0.2.1/tests/test_clifford.py
+-rw-r--r--   0 ss         (501) staff       (20)     2963 2023-04-07 01:21:59.000000 graphix-0.2.1/tests/test_generator.py
+-rw-r--r--   0 ss         (501) staff       (20)     2479 2023-04-07 01:21:59.000000 graphix-0.2.1/tests/test_gflow.py
+-rw-r--r--   0 ss         (501) staff       (20)     3974 2022-12-15 11:43:28.000000 graphix-0.2.1/tests/test_graphsim.py
+-rw-r--r--   0 ss         (501) staff       (20)     7565 2023-04-07 01:21:59.000000 graphix-0.2.1/tests/test_pattern.py
+-rw-r--r--   0 ss         (501) staff       (20)    15835 2023-03-01 11:13:38.000000 graphix-0.2.1/tests/test_tnsim.py
+-rw-r--r--   0 ss         (501) staff       (20)     5102 2023-01-14 13:01:46.000000 graphix-0.2.1/tests/test_transpiler.py
```

### Comparing `graphix-0.2.0/LICENSE` & `graphix-0.2.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   Copyright 2022 Shinichi Sunami
+   Copyright 2022-2023 Shinichi Sunami
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `graphix-0.2.0/PKG-INFO` & `graphix-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.0
+Version: 0.2.1
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -18,43 +18,44 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="600">
+<img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
 [![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
 ![PyPI](https://img.shields.io/pypi/v/graphix)
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg)](https://unitary.fund/)
+[![DOI](https://zenodo.org/badge/573466585.svg)](https://zenodo.org/badge/latestdoi/573466585)
 
-**Graphix** is an open-source library to optimize and simulate measurement-based quantum computing (MBQC). 
+**Graphix** is a measurement-based quantum computing (MBQC) compiler, which makes it easier to generate, optimize and simulate MBQC *measurement patterns*.
 
 ## Feature
 
 - We integrate an efficient [graph state simulator](https://graphix.readthedocs.io/en/latest/lc-mbqc.html) as an optimization routine of MBQC *measurement pattern*, with which we can classically [preprocess all Pauli measurements](https://graphix.readthedocs.io/en/latest/tutorial.html#performing-pauli-measurements) (corresponding to the elimination of all Clifford gates in the gate network - c.f. [Gottesman-Knill theorem](https://en.wikipedia.org/wiki/Gottesman–Knill_theorem)), significantly reducing the required size of graph state to run the computation.
-- We implement Matrix Product State (MPS) simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
+- We implement tensor-network simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
 - Our pattern-based construction and optimization routines are suitable for high-level optimization to run quantum algorithms on MBQC quantum hardware with minimal resource state size requirements. We plan to add quantum hardware emulators (and quantum hardware) as pattern execution backends.
 
 ## Installation
 Install `graphix` with `pip`:
 
 ```bash
 $ pip install graphix
 ```
 
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
-  - Using MPS simulator: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_mps.ipynb)
+  - Using tensor-network simulator backend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_tn.ipynb)
   - QAOA circuit: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qaoa.ipynb)
 
 - Read the [tutorial](https://graphix.readthedocs.io/en/latest/tutorial.html) for more comprehensive guide.
 
 - For theoretical background, read our quick introduction into [MBQC](https://graphix.readthedocs.io/en/latest/intro.html) and [LC-MBQC](https://graphix.readthedocs.io/en/latest/lc-mbqc.html).
 
 ## Citing
@@ -67,24 +68,32 @@
 [^1]: Following the release of this arXiv preprint, we were made aware of a previous work by [Backens et al.](https://quantum-journal.org/papers/q-2021-03-25-421/) where Pauli measurement elimination method for MBQC was developed in the context of circuit optimization. 
 Many thanks for letting us know about this work, we will properly mention this work in the next version of our paper.
 
 ## Contributing
 
 We use [GitHub issues](https://github.com/TeamGraphix/graphix/issues) for tracking requests and bugs. 
 
+## Discord Server
+
+Please visit [Unitary Fund's Discord server](https://discord.com/servers/unitary-fund-764231928676089909), where you can find a channel for `graphix` to ask questions.
+
 ## Core Contributors
 
 Dr. Shinichi Sunami (University of Oxford)
 
 Masato Fukushima (University of Tokyo, Fixstars Amplify)
 
 ## Acknowledgements
 
 We are proud to be supported by [unitary fund microgrant program](https://unitary.fund/grants.html). 
 
+<p><a href="https://unitary.fund/grants.html">
+<img src="https://user-images.githubusercontent.com/33350509/233384863-654485cf-b7d0-449e-8868-265c6fea2ced.png" alt="unitary-fund" width="150"/>
+</a></p>
+
 Special thanks to Fixstars Amplify:
 
 <p><a href="https://amplify.fixstars.com/en/">
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/imgs/fam_logo.png" alt="amplify" width="200"/>
 </a></p>
```

### Comparing `graphix-0.2.0/README.md` & `graphix-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
 00000010: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6561  //github.com/Tea
 00000020: 6d47 7261 7068 6978 2f67 7261 7068 6978  mGraphix/graphix
 00000030: 2f72 6177 2f6d 6173 7465 722f 646f 6373  /raw/master/docs
 00000040: 2f6c 6f67 6f2f 626c 6163 6b5f 7769 7468  /logo/black_with
 00000050: 5f6e 616d 652e 706e 6722 2061 6c74 3d22  _name.png" alt="
-00000060: 6c6f 676f 2220 7769 6474 683d 2236 3030  logo" width="600
+00000060: 6c6f 676f 2220 7769 6474 683d 2235 3530  logo" width="550
 00000070: 223e 0a0a 5b21 5b44 6f63 756d 656e 7461  ">..[![Documenta
 00000080: 7469 6f6e 2053 7461 7475 735d 2868 7474  tion Status](htt
 00000090: 7073 3a2f 2f72 6561 6474 6865 646f 6373  ps://readthedocs
 000000a0: 2e6f 7267 2f70 726f 6a65 6374 732f 6772  .org/projects/gr
 000000b0: 6170 6869 782f 6261 6467 652f 3f76 6572  aphix/badge/?ver
 000000c0: 7369 6f6e 3d6c 6174 6573 7429 5d28 6874  sion=latest)](ht
 000000d0: 7470 733a 2f2f 6772 6170 6869 782e 7265  tps://graphix.re
@@ -29,225 +29,258 @@
 000001c0: 7829 0a5b 215b 556e 6974 6172 7920 4675  x).[![Unitary Fu
 000001d0: 6e64 5d28 6874 7470 733a 2f2f 696d 672e  nd](https://img.
 000001e0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
 000001f0: 2f53 7570 706f 7274 6564 2532 3042 792d  /Supported%20By-
 00000200: 554e 4954 4152 5925 3230 4655 4e44 2d62  UNITARY%20FUND-b
 00000210: 7269 6768 7467 7265 656e 2e73 7667 295d  rightgreen.svg)]
 00000220: 2868 7474 7073 3a2f 2f75 6e69 7461 7279  (https://unitary
-00000230: 2e66 756e 642f 290a 0a2a 2a47 7261 7068  .fund/)..**Graph
-00000240: 6978 2a2a 2069 7320 616e 206f 7065 6e2d  ix** is an open-
-00000250: 736f 7572 6365 206c 6962 7261 7279 2074  source library t
-00000260: 6f20 6f70 7469 6d69 7a65 2061 6e64 2073  o optimize and s
-00000270: 696d 756c 6174 6520 6d65 6173 7572 656d  imulate measurem
-00000280: 656e 742d 6261 7365 6420 7175 616e 7475  ent-based quantu
-00000290: 6d20 636f 6d70 7574 696e 6720 284d 4251  m computing (MBQ
-000002a0: 4329 2e20 0a0a 2323 2046 6561 7475 7265  C). ..## Feature
-000002b0: 0a0a 2d20 5765 2069 6e74 6567 7261 7465  ..- We integrate
-000002c0: 2061 6e20 6566 6669 6369 656e 7420 5b67   an efficient [g
-000002d0: 7261 7068 2073 7461 7465 2073 696d 756c  raph state simul
-000002e0: 6174 6f72 5d28 6874 7470 733a 2f2f 6772  ator](https://gr
-000002f0: 6170 6869 782e 7265 6164 7468 6564 6f63  aphix.readthedoc
-00000300: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6c  s.io/en/latest/l
-00000310: 632d 6d62 7163 2e68 746d 6c29 2061 7320  c-mbqc.html) as 
-00000320: 616e 206f 7074 696d 697a 6174 696f 6e20  an optimization 
-00000330: 726f 7574 696e 6520 6f66 204d 4251 4320  routine of MBQC 
-00000340: 2a6d 6561 7375 7265 6d65 6e74 2070 6174  *measurement pat
-00000350: 7465 726e 2a2c 2077 6974 6820 7768 6963  tern*, with whic
-00000360: 6820 7765 2063 616e 2063 6c61 7373 6963  h we can classic
-00000370: 616c 6c79 205b 7072 6570 726f 6365 7373  ally [preprocess
-00000380: 2061 6c6c 2050 6175 6c69 206d 6561 7375   all Pauli measu
-00000390: 7265 6d65 6e74 735d 2868 7474 7073 3a2f  rements](https:/
-000003a0: 2f67 7261 7068 6978 2e72 6561 6474 6865  /graphix.readthe
-000003b0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-000003c0: 742f 7475 746f 7269 616c 2e68 746d 6c23  t/tutorial.html#
-000003d0: 7065 7266 6f72 6d69 6e67 2d70 6175 6c69  performing-pauli
-000003e0: 2d6d 6561 7375 7265 6d65 6e74 7329 2028  -measurements) (
-000003f0: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00000400: 2074 6865 2065 6c69 6d69 6e61 7469 6f6e   the elimination
-00000410: 206f 6620 616c 6c20 436c 6966 666f 7264   of all Clifford
-00000420: 2067 6174 6573 2069 6e20 7468 6520 6761   gates in the ga
-00000430: 7465 206e 6574 776f 726b 202d 2063 2e66  te network - c.f
-00000440: 2e20 5b47 6f74 7465 736d 616e 2d4b 6e69  . [Gottesman-Kni
-00000450: 6c6c 2074 6865 6f72 656d 5d28 6874 7470  ll theorem](http
-00000460: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00000470: 2e6f 7267 2f77 696b 692f 476f 7474 6573  .org/wiki/Gottes
-00000480: 6d61 6ee2 8093 4b6e 696c 6c5f 7468 656f  man...Knill_theo
-00000490: 7265 6d29 292c 2073 6967 6e69 6669 6361  rem)), significa
-000004a0: 6e74 6c79 2072 6564 7563 696e 6720 7468  ntly reducing th
-000004b0: 6520 7265 7175 6972 6564 2073 697a 6520  e required size 
-000004c0: 6f66 2067 7261 7068 2073 7461 7465 2074  of graph state t
-000004d0: 6f20 7275 6e20 7468 6520 636f 6d70 7574  o run the comput
-000004e0: 6174 696f 6e2e 0a2d 2057 6520 696d 706c  ation..- We impl
-000004f0: 656d 656e 7420 4d61 7472 6978 2050 726f  ement Matrix Pro
-00000500: 6475 6374 2053 7461 7465 2028 4d50 5329  duct State (MPS)
-00000510: 2073 696d 756c 6174 696f 6e20 6f66 204d   simulation of M
-00000520: 4251 4320 7769 7468 2077 6869 6368 2074  BQC with which t
-00000530: 686f 7573 616e 6473 206f 6620 7175 6269  housands of qubi
-00000540: 7473 2028 6772 6170 6820 6e6f 6465 7329  ts (graph nodes)
-00000550: 2063 616e 2062 6520 7369 6d75 6c61 7465   can be simulate
-00000560: 6420 7769 7468 206d 6f64 6573 7420 636f  d with modest co
-00000570: 6d70 7574 696e 6720 7265 736f 7572 6365  mputing resource
-00000580: 7320 2865 2e67 2e20 6c61 7074 6f70 292c  s (e.g. laptop),
-00000590: 2077 6974 686f 7574 2061 7070 726f 7869   without approxi
-000005a0: 6d61 7469 6f6e 2e0a 2d20 4f75 7220 7061  mation..- Our pa
-000005b0: 7474 6572 6e2d 6261 7365 6420 636f 6e73  ttern-based cons
-000005c0: 7472 7563 7469 6f6e 2061 6e64 206f 7074  truction and opt
-000005d0: 696d 697a 6174 696f 6e20 726f 7574 696e  imization routin
-000005e0: 6573 2061 7265 2073 7569 7461 626c 6520  es are suitable 
-000005f0: 666f 7220 6869 6768 2d6c 6576 656c 206f  for high-level o
-00000600: 7074 696d 697a 6174 696f 6e20 746f 2072  ptimization to r
-00000610: 756e 2071 7561 6e74 756d 2061 6c67 6f72  un quantum algor
-00000620: 6974 686d 7320 6f6e 204d 4251 4320 7175  ithms on MBQC qu
-00000630: 616e 7475 6d20 6861 7264 7761 7265 2077  antum hardware w
-00000640: 6974 6820 6d69 6e69 6d61 6c20 7265 736f  ith minimal reso
-00000650: 7572 6365 2073 7461 7465 2073 697a 6520  urce state size 
-00000660: 7265 7175 6972 656d 656e 7473 2e20 5765  requirements. We
-00000670: 2070 6c61 6e20 746f 2061 6464 2071 7561   plan to add qua
-00000680: 6e74 756d 2068 6172 6477 6172 6520 656d  ntum hardware em
-00000690: 756c 6174 6f72 7320 2861 6e64 2071 7561  ulators (and qua
-000006a0: 6e74 756d 2068 6172 6477 6172 6529 2061  ntum hardware) a
-000006b0: 7320 7061 7474 6572 6e20 6578 6563 7574  s pattern execut
-000006c0: 696f 6e20 6261 636b 656e 6473 2e0a 0a23  ion backends...#
-000006d0: 2320 496e 7374 616c 6c61 7469 6f6e 0a49  # Installation.I
-000006e0: 6e73 7461 6c6c 2060 6772 6170 6869 7860  nstall `graphix`
-000006f0: 2077 6974 6820 6070 6970 603a 0a0a 6060   with `pip`:..``
-00000700: 6062 6173 680a 2420 7069 7020 696e 7374  `bash.$ pip inst
-00000710: 616c 6c20 6772 6170 6869 780a 6060 600a  all graphix.```.
-00000720: 0a23 2320 4e65 7874 2053 7465 7073 0a0a  .## Next Steps..
-00000730: 2d20 5765 2068 6176 6520 6120 6665 7720  - We have a few 
-00000740: 5b64 656d 6f73 5d28 6874 7470 733a 2f2f  [demos](https://
-00000750: 6772 6170 6869 782e 7265 6164 7468 6564  graphix.readthed
-00000760: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000770: 2f67 616c 6c65 7279 2f69 6e64 6578 2e68  /gallery/index.h
-00000780: 746d 6c29 2073 686f 7769 6e67 2062 6173  tml) showing bas
-00000790: 6963 2075 7361 6765 7320 6f66 2060 4772  ic usages of `Gr
-000007a0: 6170 6869 7860 2e0a 2d20 596f 7520 6361  aphix`..- You ca
-000007b0: 6e20 7275 6e20 6465 6d6f 7320 6f6e 2079  n run demos on y
-000007c0: 6f75 7220 6272 6f77 7365 723a 0a20 202d  our browser:.  -
-000007d0: 2050 7265 7072 6f63 6573 7369 6e67 2043   Preprocessing C
-000007e0: 6c69 6666 6f72 6420 6761 7465 733a 205b  lifford gates: [
-000007f0: 215b 4269 6e64 6572 5d28 6874 7470 733a  ![Binder](https:
-00000800: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f62  //mybinder.org/b
-00000810: 6164 6765 5f6c 6f67 6f2e 7376 6729 5d28  adge_logo.svg)](
-00000820: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-00000830: 2e6f 7267 2f76 322f 6768 2f54 6561 6d47  .org/v2/gh/TeamG
-00000840: 7261 7068 6978 2f67 7261 7068 6978 2d65  raphix/graphix-e
-00000850: 7861 6d70 6c65 732f 4845 4144 3f6c 6162  xamples/HEAD?lab
-00000860: 7061 7468 3d64 6575 7473 6368 2d6a 6f7a  path=deutsch-joz
-00000870: 7361 2e69 7079 6e62 290a 2020 2d20 5573  sa.ipynb).  - Us
-00000880: 696e 6720 4d50 5320 7369 6d75 6c61 746f  ing MPS simulato
-00000890: 723a 205b 215b 4269 6e64 6572 5d28 6874  r: [![Binder](ht
-000008a0: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
-000008b0: 7267 2f62 6164 6765 5f6c 6f67 6f2e 7376  rg/badge_logo.sv
-000008c0: 6729 5d28 6874 7470 733a 2f2f 6d79 6269  g)](https://mybi
-000008d0: 6e64 6572 2e6f 7267 2f76 322f 6768 2f54  nder.org/v2/gh/T
-000008e0: 6561 6d47 7261 7068 6978 2f67 7261 7068  eamGraphix/graph
-000008f0: 6978 2d65 7861 6d70 6c65 732f 4845 4144  ix-examples/HEAD
-00000900: 3f6c 6162 7061 7468 3d71 6674 5f77 6974  ?labpath=qft_wit
-00000910: 685f 6d70 732e 6970 796e 6229 0a20 202d  h_mps.ipynb).  -
-00000920: 2051 414f 4120 6369 7263 7569 743a 205b   QAOA circuit: [
-00000930: 215b 4269 6e64 6572 5d28 6874 7470 733a  ![Binder](https:
-00000940: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f62  //mybinder.org/b
-00000950: 6164 6765 5f6c 6f67 6f2e 7376 6729 5d28  adge_logo.svg)](
-00000960: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-00000970: 2e6f 7267 2f76 322f 6768 2f54 6561 6d47  .org/v2/gh/TeamG
-00000980: 7261 7068 6978 2f67 7261 7068 6978 2d65  raphix/graphix-e
-00000990: 7861 6d70 6c65 732f 4845 4144 3f6c 6162  xamples/HEAD?lab
-000009a0: 7061 7468 3d71 616f 612e 6970 796e 6229  path=qaoa.ipynb)
-000009b0: 0a0a 2d20 5265 6164 2074 6865 205b 7475  ..- Read the [tu
-000009c0: 746f 7269 616c 5d28 6874 7470 733a 2f2f  torial](https://
-000009d0: 6772 6170 6869 782e 7265 6164 7468 6564  graphix.readthed
-000009e0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000009f0: 2f74 7574 6f72 6961 6c2e 6874 6d6c 2920  /tutorial.html) 
-00000a00: 666f 7220 6d6f 7265 2063 6f6d 7072 6568  for more compreh
-00000a10: 656e 7369 7665 2067 7569 6465 2e0a 0a2d  ensive guide...-
-00000a20: 2046 6f72 2074 6865 6f72 6574 6963 616c   For theoretical
-00000a30: 2062 6163 6b67 726f 756e 642c 2072 6561   background, rea
-00000a40: 6420 6f75 7220 7175 6963 6b20 696e 7472  d our quick intr
-00000a50: 6f64 7563 7469 6f6e 2069 6e74 6f20 5b4d  oduction into [M
-00000a60: 4251 435d 2868 7474 7073 3a2f 2f67 7261  BQC](https://gra
-00000a70: 7068 6978 2e72 6561 6474 6865 646f 6373  phix.readthedocs
-00000a80: 2e69 6f2f 656e 2f6c 6174 6573 742f 696e  .io/en/latest/in
-00000a90: 7472 6f2e 6874 6d6c 2920 616e 6420 5b4c  tro.html) and [L
-00000aa0: 432d 4d42 5143 5d28 6874 7470 733a 2f2f  C-MBQC](https://
-00000ab0: 6772 6170 6869 782e 7265 6164 7468 6564  graphix.readthed
-00000ac0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000ad0: 2f6c 632d 6d62 7163 2e68 746d 6c29 2e0a  /lc-mbqc.html)..
-00000ae0: 0a23 2320 4369 7469 6e67 0a0a 3e20 532e  .## Citing..> S.
-00000af0: 2053 756e 616d 6920 616e 6420 4d2e 2046   Sunami and M. F
-00000b00: 756b 7573 6869 6d61 2e20 2247 7261 7068  ukushima. "Graph
-00000b10: 6978 3a20 6f70 7469 6d69 7a69 6e67 2061  ix: optimizing a
-00000b20: 6e64 2073 696d 756c 6174 696e 6720 6d65  nd simulating me
-00000b30: 6173 7572 656d 656e 742d 6261 7365 6420  asurement-based 
-00000b40: 7175 616e 7475 6d20 636f 6d70 7574 6174  quantum computat
-00000b50: 696f 6e20 6f6e 206c 6f63 616c 2d43 6c69  ion on local-Cli
-00000b60: 6666 6f72 6420 6465 636f 7261 7465 6420  fford decorated 
-00000b70: 6772 6170 6822 2c20 0a3e 205b 6172 5869  graph", .> [arXi
-00000b80: 763a 3232 3132 2e31 3139 3735 5d28 6874  v:2212.11975](ht
-00000b90: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00000ba0: 6162 732f 3232 3132 2e31 3139 3735 2920  abs/2212.11975) 
-00000bb0: 2832 3032 3229 2e0a 0a55 7064 6174 6520  (2022)...Update 
-00000bc0: 6f6e 2074 6865 2070 6170 6572 3a20 5b5e  on the paper: [^
-00000bd0: 315d 0a0a 5b5e 315d 3a20 466f 6c6c 6f77  1]..[^1]: Follow
-00000be0: 696e 6720 7468 6520 7265 6c65 6173 6520  ing the release 
-00000bf0: 6f66 2074 6869 7320 6172 5869 7620 7072  of this arXiv pr
-00000c00: 6570 7269 6e74 2c20 7765 2077 6572 6520  eprint, we were 
-00000c10: 6d61 6465 2061 7761 7265 206f 6620 6120  made aware of a 
-00000c20: 7072 6576 696f 7573 2077 6f72 6b20 6279  previous work by
-00000c30: 205b 4261 636b 656e 7320 6574 2061 6c2e   [Backens et al.
-00000c40: 5d28 6874 7470 733a 2f2f 7175 616e 7475  ](https://quantu
-00000c50: 6d2d 6a6f 7572 6e61 6c2e 6f72 672f 7061  m-journal.org/pa
-00000c60: 7065 7273 2f71 2d32 3032 312d 3033 2d32  pers/q-2021-03-2
-00000c70: 352d 3432 312f 2920 7768 6572 6520 5061  5-421/) where Pa
-00000c80: 756c 6920 6d65 6173 7572 656d 656e 7420  uli measurement 
-00000c90: 656c 696d 696e 6174 696f 6e20 6d65 7468  elimination meth
-00000ca0: 6f64 2066 6f72 204d 4251 4320 7761 7320  od for MBQC was 
-00000cb0: 6465 7665 6c6f 7065 6420 696e 2074 6865  developed in the
-00000cc0: 2063 6f6e 7465 7874 206f 6620 6369 7263   context of circ
-00000cd0: 7569 7420 6f70 7469 6d69 7a61 7469 6f6e  uit optimization
-00000ce0: 2e20 0a4d 616e 7920 7468 616e 6b73 2066  . .Many thanks f
-00000cf0: 6f72 206c 6574 7469 6e67 2075 7320 6b6e  or letting us kn
-00000d00: 6f77 2061 626f 7574 2074 6869 7320 776f  ow about this wo
-00000d10: 726b 2c20 7765 2077 696c 6c20 7072 6f70  rk, we will prop
-00000d20: 6572 6c79 206d 656e 7469 6f6e 2074 6869  erly mention thi
-00000d30: 7320 776f 726b 2069 6e20 7468 6520 6e65  s work in the ne
-00000d40: 7874 2076 6572 7369 6f6e 206f 6620 6f75  xt version of ou
-00000d50: 7220 7061 7065 722e 0a0a 2323 2043 6f6e  r paper...## Con
-00000d60: 7472 6962 7574 696e 670a 0a57 6520 7573  tributing..We us
-00000d70: 6520 5b47 6974 4875 6220 6973 7375 6573  e [GitHub issues
-00000d80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000d90: 2e63 6f6d 2f54 6561 6d47 7261 7068 6978  .com/TeamGraphix
-00000da0: 2f67 7261 7068 6978 2f69 7373 7565 7329  /graphix/issues)
-00000db0: 2066 6f72 2074 7261 636b 696e 6720 7265   for tracking re
-00000dc0: 7175 6573 7473 2061 6e64 2062 7567 732e  quests and bugs.
-00000dd0: 200a 0a23 2320 436f 7265 2043 6f6e 7472   ..## Core Contr
-00000de0: 6962 7574 6f72 730a 0a44 722e 2053 6869  ibutors..Dr. Shi
-00000df0: 6e69 6368 6920 5375 6e61 6d69 2028 556e  nichi Sunami (Un
-00000e00: 6976 6572 7369 7479 206f 6620 4f78 666f  iversity of Oxfo
-00000e10: 7264 290a 0a4d 6173 6174 6f20 4675 6b75  rd)..Masato Fuku
-00000e20: 7368 696d 6120 2855 6e69 7665 7273 6974  shima (Universit
-00000e30: 7920 6f66 2054 6f6b 796f 2c20 4669 7873  y of Tokyo, Fixs
-00000e40: 7461 7273 2041 6d70 6c69 6679 290a 0a23  tars Amplify)..#
-00000e50: 2320 4163 6b6e 6f77 6c65 6467 656d 656e  # Acknowledgemen
-00000e60: 7473 0a0a 5765 2061 7265 2070 726f 7564  ts..We are proud
-00000e70: 2074 6f20 6265 2073 7570 706f 7274 6564   to be supported
-00000e80: 2062 7920 5b75 6e69 7461 7279 2066 756e   by [unitary fun
-00000e90: 6420 6d69 6372 6f67 7261 6e74 2070 726f  d microgrant pro
-00000ea0: 6772 616d 5d28 6874 7470 733a 2f2f 756e  gram](https://un
-00000eb0: 6974 6172 792e 6675 6e64 2f67 7261 6e74  itary.fund/grant
-00000ec0: 732e 6874 6d6c 292e 200a 0a53 7065 6369  s.html). ..Speci
-00000ed0: 616c 2074 6861 6e6b 7320 746f 2046 6978  al thanks to Fix
-00000ee0: 7374 6172 7320 416d 706c 6966 793a 0a0a  stars Amplify:..
-00000ef0: 3c70 3e3c 6120 6872 6566 3d22 6874 7470  <p><a href="http
-00000f00: 733a 2f2f 616d 706c 6966 792e 6669 7873  s://amplify.fixs
-00000f10: 7461 7273 2e63 6f6d 2f65 6e2f 223e 0a3c  tars.com/en/">.<
-00000f20: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000f30: 2f67 6974 6875 622e 636f 6d2f 5465 616d  /github.com/Team
-00000f40: 4772 6170 6869 782f 6772 6170 6869 782f  Graphix/graphix/
-00000f50: 7261 772f 6d61 7374 6572 2f64 6f63 732f  raw/master/docs/
-00000f60: 696d 6773 2f66 616d 5f6c 6f67 6f2e 706e  imgs/fam_logo.pn
-00000f70: 6722 2061 6c74 3d22 616d 706c 6966 7922  g" alt="amplify"
-00000f80: 2077 6964 7468 3d22 3230 3022 2f3e 0a3c   width="200"/>.<
-00000f90: 2f61 3e3c 2f70 3e0a 0a0a 2323 204c 6963  /a></p>...## Lic
-00000fa0: 656e 7365 0a0a 5b41 7061 6368 6520 4c69  ense..[Apache Li
-00000fb0: 6365 6e73 6520 322e 305d 284c 4943 454e  cense 2.0](LICEN
-00000fc0: 5345 290a                                SE).
+00000230: 2e66 756e 642f 290a 5b21 5b44 4f49 5d28  .fund/).[![DOI](
+00000240: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+00000250: 7267 2f62 6164 6765 2f35 3733 3436 3635  rg/badge/5734665
+00000260: 3835 2e73 7667 295d 2868 7474 7073 3a2f  85.svg)](https:/
+00000270: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
+00000280: 652f 6c61 7465 7374 646f 692f 3537 3334  e/latestdoi/5734
+00000290: 3636 3538 3529 0a0a 2a2a 4772 6170 6869  66585)..**Graphi
+000002a0: 782a 2a20 6973 2061 206d 6561 7375 7265  x** is a measure
+000002b0: 6d65 6e74 2d62 6173 6564 2071 7561 6e74  ment-based quant
+000002c0: 756d 2063 6f6d 7075 7469 6e67 2028 4d42  um computing (MB
+000002d0: 5143 2920 636f 6d70 696c 6572 2c20 7768  QC) compiler, wh
+000002e0: 6963 6820 6d61 6b65 7320 6974 2065 6173  ich makes it eas
+000002f0: 6965 7220 746f 2067 656e 6572 6174 652c  ier to generate,
+00000300: 206f 7074 696d 697a 6520 616e 6420 7369   optimize and si
+00000310: 6d75 6c61 7465 204d 4251 4320 2a6d 6561  mulate MBQC *mea
+00000320: 7375 7265 6d65 6e74 2070 6174 7465 726e  surement pattern
+00000330: 732a 2e0a 0a23 2320 4665 6174 7572 650a  s*...## Feature.
+00000340: 0a2d 2057 6520 696e 7465 6772 6174 6520  .- We integrate 
+00000350: 616e 2065 6666 6963 6965 6e74 205b 6772  an efficient [gr
+00000360: 6170 6820 7374 6174 6520 7369 6d75 6c61  aph state simula
+00000370: 746f 725d 2868 7474 7073 3a2f 2f67 7261  tor](https://gra
+00000380: 7068 6978 2e72 6561 6474 6865 646f 6373  phix.readthedocs
+00000390: 2e69 6f2f 656e 2f6c 6174 6573 742f 6c63  .io/en/latest/lc
+000003a0: 2d6d 6271 632e 6874 6d6c 2920 6173 2061  -mbqc.html) as a
+000003b0: 6e20 6f70 7469 6d69 7a61 7469 6f6e 2072  n optimization r
+000003c0: 6f75 7469 6e65 206f 6620 4d42 5143 202a  outine of MBQC *
+000003d0: 6d65 6173 7572 656d 656e 7420 7061 7474  measurement patt
+000003e0: 6572 6e2a 2c20 7769 7468 2077 6869 6368  ern*, with which
+000003f0: 2077 6520 6361 6e20 636c 6173 7369 6361   we can classica
+00000400: 6c6c 7920 5b70 7265 7072 6f63 6573 7320  lly [preprocess 
+00000410: 616c 6c20 5061 756c 6920 6d65 6173 7572  all Pauli measur
+00000420: 656d 656e 7473 5d28 6874 7470 733a 2f2f  ements](https://
+00000430: 6772 6170 6869 782e 7265 6164 7468 6564  graphix.readthed
+00000440: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000450: 2f74 7574 6f72 6961 6c2e 6874 6d6c 2370  /tutorial.html#p
+00000460: 6572 666f 726d 696e 672d 7061 756c 692d  erforming-pauli-
+00000470: 6d65 6173 7572 656d 656e 7473 2920 2863  measurements) (c
+00000480: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
+00000490: 7468 6520 656c 696d 696e 6174 696f 6e20  the elimination 
+000004a0: 6f66 2061 6c6c 2043 6c69 6666 6f72 6420  of all Clifford 
+000004b0: 6761 7465 7320 696e 2074 6865 2067 6174  gates in the gat
+000004c0: 6520 6e65 7477 6f72 6b20 2d20 632e 662e  e network - c.f.
+000004d0: 205b 476f 7474 6573 6d61 6e2d 4b6e 696c   [Gottesman-Knil
+000004e0: 6c20 7468 656f 7265 6d5d 2868 7474 7073  l theorem](https
+000004f0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00000500: 6f72 672f 7769 6b69 2f47 6f74 7465 736d  org/wiki/Gottesm
+00000510: 616e e280 934b 6e69 6c6c 5f74 6865 6f72  an...Knill_theor
+00000520: 656d 2929 2c20 7369 676e 6966 6963 616e  em)), significan
+00000530: 746c 7920 7265 6475 6369 6e67 2074 6865  tly reducing the
+00000540: 2072 6571 7569 7265 6420 7369 7a65 206f   required size o
+00000550: 6620 6772 6170 6820 7374 6174 6520 746f  f graph state to
+00000560: 2072 756e 2074 6865 2063 6f6d 7075 7461   run the computa
+00000570: 7469 6f6e 2e0a 2d20 5765 2069 6d70 6c65  tion..- We imple
+00000580: 6d65 6e74 2074 656e 736f 722d 6e65 7477  ment tensor-netw
+00000590: 6f72 6b20 7369 6d75 6c61 7469 6f6e 206f  ork simulation o
+000005a0: 6620 4d42 5143 2077 6974 6820 7768 6963  f MBQC with whic
+000005b0: 6820 7468 6f75 7361 6e64 7320 6f66 2071  h thousands of q
+000005c0: 7562 6974 7320 2867 7261 7068 206e 6f64  ubits (graph nod
+000005d0: 6573 2920 6361 6e20 6265 2073 696d 756c  es) can be simul
+000005e0: 6174 6564 2077 6974 6820 6d6f 6465 7374  ated with modest
+000005f0: 2063 6f6d 7075 7469 6e67 2072 6573 6f75   computing resou
+00000600: 7263 6573 2028 652e 672e 206c 6170 746f  rces (e.g. lapto
+00000610: 7029 2c20 7769 7468 6f75 7420 6170 7072  p), without appr
+00000620: 6f78 696d 6174 696f 6e2e 0a2d 204f 7572  oximation..- Our
+00000630: 2070 6174 7465 726e 2d62 6173 6564 2063   pattern-based c
+00000640: 6f6e 7374 7275 6374 696f 6e20 616e 6420  onstruction and 
+00000650: 6f70 7469 6d69 7a61 7469 6f6e 2072 6f75  optimization rou
+00000660: 7469 6e65 7320 6172 6520 7375 6974 6162  tines are suitab
+00000670: 6c65 2066 6f72 2068 6967 682d 6c65 7665  le for high-leve
+00000680: 6c20 6f70 7469 6d69 7a61 7469 6f6e 2074  l optimization t
+00000690: 6f20 7275 6e20 7175 616e 7475 6d20 616c  o run quantum al
+000006a0: 676f 7269 7468 6d73 206f 6e20 4d42 5143  gorithms on MBQC
+000006b0: 2071 7561 6e74 756d 2068 6172 6477 6172   quantum hardwar
+000006c0: 6520 7769 7468 206d 696e 696d 616c 2072  e with minimal r
+000006d0: 6573 6f75 7263 6520 7374 6174 6520 7369  esource state si
+000006e0: 7a65 2072 6571 7569 7265 6d65 6e74 732e  ze requirements.
+000006f0: 2057 6520 706c 616e 2074 6f20 6164 6420   We plan to add 
+00000700: 7175 616e 7475 6d20 6861 7264 7761 7265  quantum hardware
+00000710: 2065 6d75 6c61 746f 7273 2028 616e 6420   emulators (and 
+00000720: 7175 616e 7475 6d20 6861 7264 7761 7265  quantum hardware
+00000730: 2920 6173 2070 6174 7465 726e 2065 7865  ) as pattern exe
+00000740: 6375 7469 6f6e 2062 6163 6b65 6e64 732e  cution backends.
+00000750: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000760: 6e0a 496e 7374 616c 6c20 6067 7261 7068  n.Install `graph
+00000770: 6978 6020 7769 7468 2060 7069 7060 3a0a  ix` with `pip`:.
+00000780: 0a60 6060 6261 7368 0a24 2070 6970 2069  .```bash.$ pip i
+00000790: 6e73 7461 6c6c 2067 7261 7068 6978 0a60  nstall graphix.`
+000007a0: 6060 0a0a 2323 204e 6578 7420 5374 6570  ``..## Next Step
+000007b0: 730a 0a2d 2057 6520 6861 7665 2061 2066  s..- We have a f
+000007c0: 6577 205b 6465 6d6f 735d 2868 7474 7073  ew [demos](https
+000007d0: 3a2f 2f67 7261 7068 6978 2e72 6561 6474  ://graphix.readt
+000007e0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+000007f0: 6573 742f 6761 6c6c 6572 792f 696e 6465  est/gallery/inde
+00000800: 782e 6874 6d6c 2920 7368 6f77 696e 6720  x.html) showing 
+00000810: 6261 7369 6320 7573 6167 6573 206f 6620  basic usages of 
+00000820: 6047 7261 7068 6978 602e 0a2d 2059 6f75  `Graphix`..- You
+00000830: 2063 616e 2072 756e 2064 656d 6f73 206f   can run demos o
+00000840: 6e20 796f 7572 2062 726f 7773 6572 3a0a  n your browser:.
+00000850: 2020 2d20 5072 6570 726f 6365 7373 696e    - Preprocessin
+00000860: 6720 436c 6966 666f 7264 2067 6174 6573  g Clifford gates
+00000870: 3a20 5b21 5b42 696e 6465 725d 2868 7474  : [![Binder](htt
+00000880: 7073 3a2f 2f6d 7962 696e 6465 722e 6f72  ps://mybinder.or
+00000890: 672f 6261 6467 655f 6c6f 676f 2e73 7667  g/badge_logo.svg
+000008a0: 295d 2868 7474 7073 3a2f 2f6d 7962 696e  )](https://mybin
+000008b0: 6465 722e 6f72 672f 7632 2f67 682f 5465  der.org/v2/gh/Te
+000008c0: 616d 4772 6170 6869 782f 6772 6170 6869  amGraphix/graphi
+000008d0: 782d 6578 616d 706c 6573 2f48 4541 443f  x-examples/HEAD?
+000008e0: 6c61 6270 6174 683d 6465 7574 7363 682d  labpath=deutsch-
+000008f0: 6a6f 7a73 612e 6970 796e 6229 0a20 202d  jozsa.ipynb).  -
+00000900: 2055 7369 6e67 2074 656e 736f 722d 6e65   Using tensor-ne
+00000910: 7477 6f72 6b20 7369 6d75 6c61 746f 7220  twork simulator 
+00000920: 6261 636b 656e 643a 205b 215b 4269 6e64  backend: [![Bind
+00000930: 6572 5d28 6874 7470 733a 2f2f 6d79 6269  er](https://mybi
+00000940: 6e64 6572 2e6f 7267 2f62 6164 6765 5f6c  nder.org/badge_l
+00000950: 6f67 6f2e 7376 6729 5d28 6874 7470 733a  ogo.svg)](https:
+00000960: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f76  //mybinder.org/v
+00000970: 322f 6768 2f54 6561 6d47 7261 7068 6978  2/gh/TeamGraphix
+00000980: 2f67 7261 7068 6978 2d65 7861 6d70 6c65  /graphix-example
+00000990: 732f 4845 4144 3f6c 6162 7061 7468 3d71  s/HEAD?labpath=q
+000009a0: 6674 5f77 6974 685f 746e 2e69 7079 6e62  ft_with_tn.ipynb
+000009b0: 290a 2020 2d20 5141 4f41 2063 6972 6375  ).  - QAOA circu
+000009c0: 6974 3a20 5b21 5b42 696e 6465 725d 2868  it: [![Binder](h
+000009d0: 7474 7073 3a2f 2f6d 7962 696e 6465 722e  ttps://mybinder.
+000009e0: 6f72 672f 6261 6467 655f 6c6f 676f 2e73  org/badge_logo.s
+000009f0: 7667 295d 2868 7474 7073 3a2f 2f6d 7962  vg)](https://myb
+00000a00: 696e 6465 722e 6f72 672f 7632 2f67 682f  inder.org/v2/gh/
+00000a10: 5465 616d 4772 6170 6869 782f 6772 6170  TeamGraphix/grap
+00000a20: 6869 782d 6578 616d 706c 6573 2f48 4541  hix-examples/HEA
+00000a30: 443f 6c61 6270 6174 683d 7161 6f61 2e69  D?labpath=qaoa.i
+00000a40: 7079 6e62 290a 0a2d 2052 6561 6420 7468  pynb)..- Read th
+00000a50: 6520 5b74 7574 6f72 6961 6c5d 2868 7474  e [tutorial](htt
+00000a60: 7073 3a2f 2f67 7261 7068 6978 2e72 6561  ps://graphix.rea
+00000a70: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000a80: 6174 6573 742f 7475 746f 7269 616c 2e68  atest/tutorial.h
+00000a90: 746d 6c29 2066 6f72 206d 6f72 6520 636f  tml) for more co
+00000aa0: 6d70 7265 6865 6e73 6976 6520 6775 6964  mprehensive guid
+00000ab0: 652e 0a0a 2d20 466f 7220 7468 656f 7265  e...- For theore
+00000ac0: 7469 6361 6c20 6261 636b 6772 6f75 6e64  tical background
+00000ad0: 2c20 7265 6164 206f 7572 2071 7569 636b  , read our quick
+00000ae0: 2069 6e74 726f 6475 6374 696f 6e20 696e   introduction in
+00000af0: 746f 205b 4d42 5143 5d28 6874 7470 733a  to [MBQC](https:
+00000b00: 2f2f 6772 6170 6869 782e 7265 6164 7468  //graphix.readth
+00000b10: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00000b20: 7374 2f69 6e74 726f 2e68 746d 6c29 2061  st/intro.html) a
+00000b30: 6e64 205b 4c43 2d4d 4251 435d 2868 7474  nd [LC-MBQC](htt
+00000b40: 7073 3a2f 2f67 7261 7068 6978 2e72 6561  ps://graphix.rea
+00000b50: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000b60: 6174 6573 742f 6c63 2d6d 6271 632e 6874  atest/lc-mbqc.ht
+00000b70: 6d6c 292e 0a0a 2323 2043 6974 696e 670a  ml)...## Citing.
+00000b80: 0a3e 2053 2e20 5375 6e61 6d69 2061 6e64  .> S. Sunami and
+00000b90: 204d 2e20 4675 6b75 7368 696d 612e 2022   M. Fukushima. "
+00000ba0: 4772 6170 6869 783a 206f 7074 696d 697a  Graphix: optimiz
+00000bb0: 696e 6720 616e 6420 7369 6d75 6c61 7469  ing and simulati
+00000bc0: 6e67 206d 6561 7375 7265 6d65 6e74 2d62  ng measurement-b
+00000bd0: 6173 6564 2071 7561 6e74 756d 2063 6f6d  ased quantum com
+00000be0: 7075 7461 7469 6f6e 206f 6e20 6c6f 6361  putation on loca
+00000bf0: 6c2d 436c 6966 666f 7264 2064 6563 6f72  l-Clifford decor
+00000c00: 6174 6564 2067 7261 7068 222c 200a 3e20  ated graph", .> 
+00000c10: 5b61 7258 6976 3a32 3231 322e 3131 3937  [arXiv:2212.1197
+00000c20: 355d 2868 7474 7073 3a2f 2f61 7278 6976  5](https://arxiv
+00000c30: 2e6f 7267 2f61 6273 2f32 3231 322e 3131  .org/abs/2212.11
+00000c40: 3937 3529 2028 3230 3232 292e 0a0a 5570  975) (2022)...Up
+00000c50: 6461 7465 206f 6e20 7468 6520 7061 7065  date on the pape
+00000c60: 723a 205b 5e31 5d0a 0a5b 5e31 5d3a 2046  r: [^1]..[^1]: F
+00000c70: 6f6c 6c6f 7769 6e67 2074 6865 2072 656c  ollowing the rel
+00000c80: 6561 7365 206f 6620 7468 6973 2061 7258  ease of this arX
+00000c90: 6976 2070 7265 7072 696e 742c 2077 6520  iv preprint, we 
+00000ca0: 7765 7265 206d 6164 6520 6177 6172 6520  were made aware 
+00000cb0: 6f66 2061 2070 7265 7669 6f75 7320 776f  of a previous wo
+00000cc0: 726b 2062 7920 5b42 6163 6b65 6e73 2065  rk by [Backens e
+00000cd0: 7420 616c 2e5d 2868 7474 7073 3a2f 2f71  t al.](https://q
+00000ce0: 7561 6e74 756d 2d6a 6f75 726e 616c 2e6f  uantum-journal.o
+00000cf0: 7267 2f70 6170 6572 732f 712d 3230 3231  rg/papers/q-2021
+00000d00: 2d30 332d 3235 2d34 3231 2f29 2077 6865  -03-25-421/) whe
+00000d10: 7265 2050 6175 6c69 206d 6561 7375 7265  re Pauli measure
+00000d20: 6d65 6e74 2065 6c69 6d69 6e61 7469 6f6e  ment elimination
+00000d30: 206d 6574 686f 6420 666f 7220 4d42 5143   method for MBQC
+00000d40: 2077 6173 2064 6576 656c 6f70 6564 2069   was developed i
+00000d50: 6e20 7468 6520 636f 6e74 6578 7420 6f66  n the context of
+00000d60: 2063 6972 6375 6974 206f 7074 696d 697a   circuit optimiz
+00000d70: 6174 696f 6e2e 200a 4d61 6e79 2074 6861  ation. .Many tha
+00000d80: 6e6b 7320 666f 7220 6c65 7474 696e 6720  nks for letting 
+00000d90: 7573 206b 6e6f 7720 6162 6f75 7420 7468  us know about th
+00000da0: 6973 2077 6f72 6b2c 2077 6520 7769 6c6c  is work, we will
+00000db0: 2070 726f 7065 726c 7920 6d65 6e74 696f   properly mentio
+00000dc0: 6e20 7468 6973 2077 6f72 6b20 696e 2074  n this work in t
+00000dd0: 6865 206e 6578 7420 7665 7273 696f 6e20  he next version 
+00000de0: 6f66 206f 7572 2070 6170 6572 2e0a 0a23  of our paper...#
+00000df0: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00000e00: 5765 2075 7365 205b 4769 7448 7562 2069  We use [GitHub i
+00000e10: 7373 7565 735d 2868 7474 7073 3a2f 2f67  ssues](https://g
+00000e20: 6974 6875 622e 636f 6d2f 5465 616d 4772  ithub.com/TeamGr
+00000e30: 6170 6869 782f 6772 6170 6869 782f 6973  aphix/graphix/is
+00000e40: 7375 6573 2920 666f 7220 7472 6163 6b69  sues) for tracki
+00000e50: 6e67 2072 6571 7565 7374 7320 616e 6420  ng requests and 
+00000e60: 6275 6773 2e20 0a0a 2323 2044 6973 636f  bugs. ..## Disco
+00000e70: 7264 2053 6572 7665 720a 0a50 6c65 6173  rd Server..Pleas
+00000e80: 6520 7669 7369 7420 5b55 6e69 7461 7279  e visit [Unitary
+00000e90: 2046 756e 6427 7320 4469 7363 6f72 6420   Fund's Discord 
+00000ea0: 7365 7276 6572 5d28 6874 7470 733a 2f2f  server](https://
+00000eb0: 6469 7363 6f72 642e 636f 6d2f 7365 7276  discord.com/serv
+00000ec0: 6572 732f 756e 6974 6172 792d 6675 6e64  ers/unitary-fund
+00000ed0: 2d37 3634 3233 3139 3238 3637 3630 3839  -764231928676089
+00000ee0: 3930 3929 2c20 7768 6572 6520 796f 7520  909), where you 
+00000ef0: 6361 6e20 6669 6e64 2061 2063 6861 6e6e  can find a chann
+00000f00: 656c 2066 6f72 2060 6772 6170 6869 7860  el for `graphix`
+00000f10: 2074 6f20 6173 6b20 7175 6573 7469 6f6e   to ask question
+00000f20: 732e 0a0a 2323 2043 6f72 6520 436f 6e74  s...## Core Cont
+00000f30: 7269 6275 746f 7273 0a0a 4472 2e20 5368  ributors..Dr. Sh
+00000f40: 696e 6963 6869 2053 756e 616d 6920 2855  inichi Sunami (U
+00000f50: 6e69 7665 7273 6974 7920 6f66 204f 7866  niversity of Oxf
+00000f60: 6f72 6429 0a0a 4d61 7361 746f 2046 756b  ord)..Masato Fuk
+00000f70: 7573 6869 6d61 2028 556e 6976 6572 7369  ushima (Universi
+00000f80: 7479 206f 6620 546f 6b79 6f2c 2046 6978  ty of Tokyo, Fix
+00000f90: 7374 6172 7320 416d 706c 6966 7929 0a0a  stars Amplify)..
+00000fa0: 2323 2041 636b 6e6f 776c 6564 6765 6d65  ## Acknowledgeme
+00000fb0: 6e74 730a 0a57 6520 6172 6520 7072 6f75  nts..We are prou
+00000fc0: 6420 746f 2062 6520 7375 7070 6f72 7465  d to be supporte
+00000fd0: 6420 6279 205b 756e 6974 6172 7920 6675  d by [unitary fu
+00000fe0: 6e64 206d 6963 726f 6772 616e 7420 7072  nd microgrant pr
+00000ff0: 6f67 7261 6d5d 2868 7474 7073 3a2f 2f75  ogram](https://u
+00001000: 6e69 7461 7279 2e66 756e 642f 6772 616e  nitary.fund/gran
+00001010: 7473 2e68 746d 6c29 2e20 0a0a 3c70 3e3c  ts.html). ..<p><
+00001020: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001030: 756e 6974 6172 792e 6675 6e64 2f67 7261  unitary.fund/gra
+00001040: 6e74 732e 6874 6d6c 223e 0a3c 696d 6720  nts.html">.<img 
+00001050: 7372 633d 2268 7474 7073 3a2f 2f75 7365  src="https://use
+00001060: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
+00001070: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f33  sercontent.com/3
+00001080: 3333 3530 3530 392f 3233 3333 3834 3836  3350509/23338486
+00001090: 332d 3635 3434 3835 6366 2d62 3764 302d  3-654485cf-b7d0-
+000010a0: 3434 3965 2d38 3836 382d 3236 3563 3666  449e-8868-265c6f
+000010b0: 6561 3263 6564 2e70 6e67 2220 616c 743d  ea2ced.png" alt=
+000010c0: 2275 6e69 7461 7279 2d66 756e 6422 2077  "unitary-fund" w
+000010d0: 6964 7468 3d22 3135 3022 2f3e 0a3c 2f61  idth="150"/>.</a
+000010e0: 3e3c 2f70 3e0a 0a53 7065 6369 616c 2074  ></p>..Special t
+000010f0: 6861 6e6b 7320 746f 2046 6978 7374 6172  hanks to Fixstar
+00001100: 7320 416d 706c 6966 793a 0a0a 3c70 3e3c  s Amplify:..<p><
+00001110: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001120: 616d 706c 6966 792e 6669 7873 7461 7273  amplify.fixstars
+00001130: 2e63 6f6d 2f65 6e2f 223e 0a3c 696d 6720  .com/en/">.<img 
+00001140: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00001150: 6875 622e 636f 6d2f 5465 616d 4772 6170  hub.com/TeamGrap
+00001160: 6869 782f 6772 6170 6869 782f 7261 772f  hix/graphix/raw/
+00001170: 6d61 7374 6572 2f64 6f63 732f 696d 6773  master/docs/imgs
+00001180: 2f66 616d 5f6c 6f67 6f2e 706e 6722 2061  /fam_logo.png" a
+00001190: 6c74 3d22 616d 706c 6966 7922 2077 6964  lt="amplify" wid
+000011a0: 7468 3d22 3230 3022 2f3e 0a3c 2f61 3e3c  th="200"/>.</a><
+000011b0: 2f70 3e0a 0a0a 2323 204c 6963 656e 7365  /p>...## License
+000011c0: 0a0a 5b41 7061 6368 6520 4c69 6365 6e73  ..[Apache Licens
+000011d0: 6520 322e 305d 284c 4943 454e 5345 290a  e 2.0](LICENSE).
```

### Comparing `graphix-0.2.0/docs/Makefile` & `graphix-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/docs/make.bat` & `graphix-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/docs/requirements.txt` & `graphix-0.2.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/clifford.py` & `graphix-0.2.1/graphix/clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/gflow.py` & `graphix-0.2.1/graphix/gflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,113 +11,14 @@
 
 """
 
 import networkx as nx
 import numpy as np
 import z3
 import copy
-from graphix.pattern import Pattern
-
-
-def generate_from_graph(graph, angles, inputs, outputs, timeout=100):
-    r"""Generate the measurement pattern from open graph and measurement angles.
-
-    This function takes an open graph G = (nodes, edges, input, outputs),
-    specified by networks.Graph and two lists specifying input and output nodes.
-    Currently we support XY-plane measurements.
-
-    Searches for the flow in the open graph using :func:`flow` and if found,
-    construct the measurement pattern according to the theorem 1 of [NJP 9, 250 (2007)].
-
-    Then, if no flow was found, searches for gflow using :func:`gflow`,
-    from which measurement pattern can be constructed from theorem 2 of [NJP 9, 250 (2007)].
-
-    The constructed measurement pattern deterministically realize the unitary embedding
-
-    .. math::
-
-        U = \left( \prod_i \langle +_{\alpha_i} |_i \right) E_G N_{I^C},
-
-    where the measurements (bras) with always :math:`\langle+|` bases determined by the measurement
-    angles :math:`\alpha_i` are applied to the measuring nodes,
-    i.e. the randomness of the measurement is eliminated by the added byproduct commands.
-
-    .. seealso:: :func:`flow` :func:`gflow` :class:`graphix.pattern.Pattern`
-
-    Parameters
-    ----------
-    graph : networkx.Graph
-        graph on which MBQC should be performed
-    angles : dict
-        measurement angles for each nodes on the graph (unit of pi), except output nodes
-    inputs : list
-        list of node indices for input nodes
-    outputs : list
-        list of node indices for output nodes
-    timeout : int
-        optional argument for flow and gflow search depth
-
-    Returns
-    -------
-    pattern : graphix.pattern.Pattern object
-        constructed pattern.
-    """
-    assert len(inputs) == len(outputs)
-    measuring_nodes = list(set(graph.nodes) - set(outputs) - set(inputs))
-
-    # search for flow first
-    f, l_k = flow(graph, set(inputs), set(outputs), timeout=timeout)
-    if f:
-        # flow found
-        depth, layers = get_layers(l_k)
-        pattern = Pattern(len(inputs))
-        pattern.seq = [["N", i] for i in inputs]
-        for i in set(graph.nodes) - set(inputs):
-            pattern.seq.append(["N", i])
-        for e in graph.edges:
-            pattern.seq.append(["E", e])
-        measured = []
-        for i in range(depth, 0, -1):  # i from depth, depth-1, ... 1
-            for j in layers[i]:
-                measured.append(j)
-                pattern.seq.append(["M", j, "XY", angles[j], [], []])
-                for k in set(graph.neighbors(f[j])) - set([j]):
-                    if k not in measured:
-                        pattern.seq.append(["Z", k, [j]])
-                pattern.seq.append(["X", f[j], [j]])
-        pattern.output_nodes = outputs
-        pattern.Nnode = len(graph.nodes)
-    else:
-        # no flow found - we try gflow
-        g, l_k = gflow(graph, set(inputs), set(outputs), timeout=timeout)
-        if g:
-            # gflow found
-            depth, layers = get_layers(l_k)
-            pattern = Pattern(len(inputs))
-            pattern.seq = [["N", i] for i in inputs]
-            for i in set(graph.nodes) - set(inputs):
-                pattern.seq.append(["N", i])
-            for e in graph.edges:
-                pattern.seq.append(["E", e])
-            remaining = set(measuring_nodes)
-            for i in range(depth, 0, -1):  # i from depth, depth-1, ... 1
-                for j in layers[i]:
-                    pattern.seq.append(["M", j, "XY", angles[j], [], []])
-                    remaining = remaining - set([j])
-                    odd_neighbors = find_odd_neighbor(graph, remaining, set(g[j]))
-                    for k in odd_neighbors:
-                        pattern.seq.append(["Z", k, [j]])
-                    for k in set(g[j]) - set([j]):
-                        pattern.seq.append(["X", k, [j]])
-            pattern.output_nodes = outputs
-            pattern.Nnode = len(graph.nodes)
-        else:
-            raise ValueError("no flow or gflow found")
-
-    return pattern
 
 
 def solvebool(A, b):
     """solves linear equations of booleans
 
     Solves Ax=b, where A is n*m matrix and b is 1*m array, both of booleans.
     for example, for A=[[0,1,1],[1,0,1]] and b=[1,0], we solve:
@@ -168,15 +69,15 @@
     if s.check() == z3.sat:  # there's solution
         ans = s.model()
         return np.array([ans[p[i]] for i in range(A.shape[1])])
     else:  # no solution found
         return False
 
 
-def gflow(g, v_in, v_out, meas_plane=None, timeout=100):
+def gflow(g, v_in, v_out, meas_plane=None, timeout=1000):
     """Optimum generalized flow finding algorithm
 
     For open graph g with input and output, this returns optimum gflow.
 
     gflow consist of function g(i) where i is the qubit labels,
     and strict partial ordering < or layers labels l_k where each element
     specify the order of qubits to be measured to maintain determinism in MBQC.
@@ -282,15 +183,14 @@
     v_correct_list = list(v_correct)
 
     index_0 = [[index_list.index(i)] for i in iter(v_rem)]  # for slicing rows
     index_1 = [index_list.index(i) for i in iter(v_correct)]  # for slicing columns
 
     # if index_0 or index_1 is blank, skip the calculation below
     if len(index_0) * len(index_1):
-
         gamma_sub = gamma[index_0, index_1]
 
         for u in iter(v_rem):
             if meas_plane[u] == "Z":
                 c_set = c_set | {u}
                 g[u] = set()
                 l_k[u] = k
@@ -318,15 +218,15 @@
     else:
         finished = False
         exist = True
 
     return v_out | c_set, g, l_k, finished, exist
 
 
-def flow(g, v_in, v_out, meas_plane=None, timeout=100):
+def flow(g, v_in, v_out, meas_plane=None, timeout=10000):
     """Causal flow finding algorithm
 
     For open graph g with input and output, this returns causal flow.
 
     For more detail of causal flow, see Danos and Kashefi, PRA 74, 052310 (2006).
 
     Original algorithm by Mhalla and Perdrix,
@@ -557,71 +457,7 @@
         components of each layer
     """
     d = get_min_depth(l_k)
     layers = {k: [] for k in range(d + 1)}
     for i in l_k.keys():
         layers[l_k[i]].append(i)
     return d, layers
-
-
-def get_meas_plane(pattern):
-    """get measurement plane from the pattern.
-    Parameter
-    -------
-    pattern: graphix.pattern.Pattern object
-
-    Return
-    -------
-    meas_plane: dict of str
-        list of strs representing measurement plane for each node.
-    """
-    meas_plane = dict()
-    XYtoXZ_list = [
-        6,
-        8,
-        11,
-        12,
-        20,
-        21,
-        22,
-        23,
-    ]  # clifford indices that change meas plane from xy to xz
-    for cmd in pattern.seq:
-        if cmd[0] == "M":
-            if len(cmd) == 7:
-                if cmd[6] in XYtoXZ_list:
-                    meas_plane[cmd[1]] = "XZ"
-                else:
-                    meas_plane[cmd[1]] = cmd[2]
-            else:
-                meas_plane[cmd[1]] = cmd[2]
-    return meas_plane
-
-
-def get_measurement_order_from_gflow(pattern):
-    """Returns a list containing the node indices,
-    in the order of measurements which can be performed with minimum depth.
-    Input must be a simple connected graph for the gflow-finding algorithm to work.
-
-    Returns
-    -------
-    meas_order : list
-        list of node indices in the order of measurements
-    """
-    nodes, edges = pattern.get_graph()
-    G = nx.Graph()
-    G.add_nodes_from(nodes)
-    G.add_edges_from(edges)
-    isolated = list(nx.isolates(G))
-    if isolated:
-        raise ValueError("The input graph must be connected")
-    meas_plane = get_meas_plane(pattern)
-    g, l_k = gflow(G, set(), set(pattern.output_nodes), meas_plane=meas_plane)
-    if not g:
-        raise ValueError("No gflow found")
-    k, layers = get_layers(l_k)
-    meas_order = []
-    while k > 0:
-        for node in layers[k]:
-            meas_order.append(node)
-        k -= 1
-    return meas_order
```

### Comparing `graphix-0.2.0/graphix/graphsim.py` & `graphix-0.2.1/graphix/graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/ops.py` & `graphix-0.2.1/graphix/ops.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/pattern.py` & `graphix-0.2.1/graphix/pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """MBQC pattern according to Measurement Calculus
 ref: V. Danos, E. Kashefi and P. Panangaden. J. ACM 54.2 8 (2007)
 """
 import numpy as np
 import networkx as nx
 from graphix.simulator import PatternSimulator
 from graphix.graphsim import GraphState
-from graphix.clifford import CLIFFORD_CONJ, CLIFFORD_TO_QASM3, CLIFFORD_MUL
+from graphix.gflow import flow, gflow, get_layers
+from graphix.clifford import (
+    CLIFFORD_CONJ,
+    CLIFFORD_TO_QASM3,
+    CLIFFORD_MUL,
+    CLIFFORD_MEASURE,
+)
 from copy import deepcopy
 
 
 class Pattern:
     """
     MBQC pattern class
 
@@ -95,15 +101,14 @@
         """arrange the order of output_nodes.
 
         Parameters
         ----------
         output_nodes: list of int
             output nodes order determined by user. each index corresponds to that of logical qubits.
         """
-        assert set(self.output_nodes) == set(output_nodes)
         self.output_nodes = output_nodes
 
     def __repr__(self):
         return f"graphix.pattern.Pattern object with {len(self.seq)} commands and {self.width} output qubits"
 
     def print_pattern(self, lim=40, filter=None):
         """print the pattern sequence (Pattern.seq).
@@ -538,41 +543,41 @@
     def _get_dependency(self):
         """Get dependency (byproduct correction & dependent measurement)
         structure of nodes in the graph (resource) state, according to the pattern.
         This is used to determine the optimum measurement order.
 
         Returns
         -------
-        dependency : dict of sets
+        dependency : dict of set
             index is node number. all nodes in the each set must be measured before measuring
         """
         nodes, _ = self.get_graph()
         dependency = {i: set() for i in nodes}
         for cmd in self.seq:
             if cmd[0] == "M":
                 dependency[cmd[1]] = dependency[cmd[1]] | set(cmd[4]) | set(cmd[5])
             elif cmd[0] == "X":
                 dependency[cmd[1]] = dependency[cmd[1]] | set(cmd[2])
             elif cmd[0] == "Z":
                 dependency[cmd[1]] = dependency[cmd[1]] | set(cmd[2])
         return dependency
 
     def update_dependency(self, measured, dependency):
-        """Update dependency function. remove measured nodes from dependency.
+        """Remove measured nodes from the 'dependency'.
 
         Parameters
         ----------
-        measured: set
+        measured: set of int
             measured nodes.
-        dependency: dict of sets
+        dependency: dict of set
             which is produced by `_get_dependency`
 
         Returns
         --------
-        dependency: dict of sets
+        dependency: dict of set
             updated dependency information
         """
         for i in dependency.keys():
             dependency[i] -= measured
         return dependency
 
     def get_layers(self):
@@ -580,15 +585,15 @@
         kth layer must be measured before measuring k+1th layer
         and nodes in the same layer can be measured simultaneously.
 
         Returns
         -------
         depth : int
             depth of graph
-        layers : dict of sets
+        layers : dict of set
             nodes grouped by layer index(k)
         """
         dependency = self._get_dependency()
         measured = self.results.keys()
         dependency = self.update_dependency(measured, dependency)
         not_measured = set()
         for cmd in self.seq:
@@ -605,53 +610,51 @@
             dependency = self.update_dependency(l_k[k], dependency)
             not_measured -= l_k[k]
             k += 1
             depth = k
         return depth, l_k
 
     def _measurement_order_depth(self):
-        """Obtain the measurement order which reduces the depth of
-        pattern execution.
+        """Obtain a measurement order which reduces the depth of a pattern.
 
         Returns
         -------
-        meas_order: list of ints
+        meas_order: list of int
             optimal measurement order for parallel computing
         """
         d, l_k = self.get_layers()
         meas_order = []
         for i in range(d):
             for node in l_k[i]:
                 meas_order.append(node)
         return meas_order
 
     def connected_edges(self, node, edges):
         """Search not activated edges connected to the specified node
 
         Returns
         -------
-        connected: set of taples
+        connected: set of taple
                 set of connected edges
         """
         connected = set()
         for edge in edges:
             if edge[0] == node:
                 connected = connected | {edge}
             elif edge[1] == node:
                 connected = connected | {edge}
         return connected
 
     def _measurement_order_space(self):
-        """Determine the optimal measurement order
-         which minimize the `max_space` of the pattern.
+        """Determine measurement order that heuristically optimises the max_space of a pattern
 
         Returns
         -------
-        meas_order: list of ints
-            optimal measurement order for classical simulation
+        meas_order: list of int
+            sub-optimal measurement order for classical simulation
         """
         nodes, edges = self.get_graph()
         nodes = set(nodes)
         edges = set(edges)
         not_measured = nodes - set(self.output_nodes)
         dependency = self._get_dependency()
         dependency = self.update_dependency(self.results.keys(), dependency)
@@ -670,56 +673,132 @@
             assert next_node > -1
             meas_order.append(next_node)
             dependency = self.update_dependency({next_node}, dependency)
             not_measured -= {next_node}
             edges -= removable_edges
         return meas_order
 
+    def get_measurement_order_from_flow(self):
+        """Return a measurement order generated from flow. If a graph has flow, the minimum 'max_space' of a pattern is guaranteed to width+1.
+
+        Returns
+        -------
+        meas_order: list of int
+            measurement order
+        """
+        nodes, edges = self.get_graph()
+        G = nx.Graph()
+        G.add_nodes_from(nodes)
+        G.add_edges_from(edges)
+        vin = {i for i in range(self.width)}
+        vout = set(self.output_nodes)
+        f, l_k = flow(G, vin, vout)
+        if f is None:
+            return None
+        depth, layer = get_layers(l_k)
+        meas_order = []
+        for i in range(depth):
+            k = depth - i
+            nodes = layer[k]
+            meas_order += nodes
+        return meas_order
+
+    def get_measurement_order_from_gflow(self):
+        """Returns a list containing the node indices,
+        in the order of measurements which can be performed with minimum depth.
+
+        Returns
+        -------
+        meas_order : list of int
+            measurement order
+        """
+        nodes, edges = self.get_graph()
+        G = nx.Graph()
+        G.add_nodes_from(nodes)
+        G.add_edges_from(edges)
+        isolated = list(nx.isolates(G))
+        if isolated:
+            raise ValueError("The input graph must be connected")
+        meas_plane = self.get_meas_plane()
+        g, l_k = gflow(G, set(), set(self.output_nodes), meas_plane=meas_plane)
+        if not g:
+            raise ValueError("No gflow found")
+        k, layers = get_layers(l_k)
+        meas_order = []
+        while k > 0:
+            for node in layers[k]:
+                meas_order.append(node)
+            k -= 1
+        return meas_order
+
     def sort_measurement_commands(self, meas_order):
         """Convert measurement order to sequence of measurement commands
 
         Parameters
-        --------
-        meas_order: list of ints
+        ----------
+        meas_order: list of int
             optimal measurement order.
 
         Returns
-        --------
-        meas_flow: list of commands
+        -------
+        meas_cmds: list of command
             sorted measurement commands
         """
-        meas_flow = []
+        meas_cmds = []
         for i in meas_order:
             target = 0
             while True:
                 if (self.seq[target][0] == "M") & (self.seq[target][1] == i):
-                    meas_flow.append(self.seq[target])
+                    meas_cmds.append(self.seq[target])
                     break
                 target += 1
-        return meas_flow
+        return meas_cmds
 
-    def get_measurement_order(self):
-        """Returns the list containing the node indices,
+    def get_measurement_commands(self):
+        """Returns the list containing the measurement commands,
         in the order of measurements
 
         Returns
         -------
-        meas_flow : list
-            list of node indices in the order of meaurements
+        meas_cmds : list
+            list of measurement commands in the order of meaurements
         """
         if not self.is_standard():
             self.standardize()
-        meas_flow = []
+        meas_cmds = []
         ind = self._find_op_to_be_moved("M")
         if ind == "end":
             return []
         while self.seq[ind][0] == "M":
-            meas_flow.append(self.seq[ind])
+            meas_cmds.append(self.seq[ind])
             ind += 1
-        return meas_flow
+        return meas_cmds
+
+    def get_meas_plane(self):
+        """get measurement plane from the pattern.
+
+        Returns
+        -------
+        meas_plane: dict of str
+            list of str representing measurement plane for each node.
+        """
+        meas_plane = dict()
+        order = ["X", "Y", "Z"]
+        for cmd in self.seq:
+            if cmd[0] == "M":
+                mplane = cmd[2]
+                if len(cmd) == 7:
+                    converted_mplane = ""
+                    clifford_measure = CLIFFORD_MEASURE[cmd[6]]
+                    for axis in mplane:
+                        converted = order[clifford_measure[order.index(axis)][0]]
+                        converted_mplane += converted
+                    mplane = "".join(sorted(converted_mplane))
+                meas_plane[cmd[1]] = mplane
+        return meas_plane
 
     def get_graph(self):
         """returns the list of nodes and edges from the command sequence,
         extracted from 'N' and 'E' commands.
 
         Returns
         -------
@@ -737,23 +816,24 @@
         return node_list, edge_list
 
     def get_isolated_nodes(self):
         """Get isolated nodes.
 
         Returns
         -------
-        set of int :
+        isolated_nodes : set of int
             set of the isolated nodes
         """
         nodes, edges = self.get_graph()
         node_set = set(nodes)
         connected_node_set = set()
         for edge in edges:
             connected_node_set |= set(edge)
-        return node_set - connected_node_set
+        isolated_nodes = node_set - connected_node_set
+        return isolated_nodes
 
     def get_vops(self, conj=False, include_identity=False):
         """Get local-Clifford decorations from measurement or Clifford commands.
 
         Parameters
         ----------
             conj (False) : bool, optional
@@ -852,23 +932,25 @@
         """Optimize the pattern to minimize the max_space property of
         the pattern i.e. the optimized pattern has significantly
         reduced space requirement (memory space for classical simulation,
         and maximum simultaneously prepared qubits for quantum hardwares).
         """
         if not self.is_standard():
             self.standardize()
-        meas_order = self._measurement_order_space()
+        meas_order = self.get_measurement_order_from_flow()
+        if meas_order is None:
+            meas_order = self._measurement_order_space()
         self._reorder_pattern(self.sort_measurement_commands(meas_order))
 
     def _reorder_pattern(self, meas_commands):
         """internal method to reorder the command sequence
 
         Parameters
         ----------
-        meas_commands : list of commands
+        meas_commands : list of command
             list of measurement ('M') commands
         """
         prepared = []
         measured = []
         new = []
         for cmd in meas_commands:
             node = cmd[1]
@@ -1111,15 +1193,15 @@
     Returns
     -------
     pauli_node : list
         list of node indices
     """
     if not pattern.is_standard():
         pattern.standardize()
-    m_commands = pattern.get_measurement_order()
+    m_commands = pattern.get_measurement_commands()
     pauli_node = []
     # Nodes that are non-Pauli measured, or pauli measured but depends on pauli measurement
     non_pauli_node = []
     for cmd in m_commands:
         if cmd[2] == "XY":
             if cmd[3] in [-1, 0, 1]:  # Not affected by t dependency
                 t_cond = np.any(np.isin(cmd[5], np.array(non_pauli_node, dtype=object)))
```

### Comparing `graphix-0.2.0/graphix/sim/statevec.py` & `graphix-0.2.1/graphix/sim/statevec.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/sim/tensornet.py` & `graphix-0.2.1/graphix/sim/tensornet.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/simulator.py` & `graphix-0.2.1/graphix/simulator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix/transpiler.py` & `graphix-0.2.1/graphix/transpiler.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/graphix.egg-info/PKG-INFO` & `graphix-0.2.1/graphix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.0
+Version: 0.2.1
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -18,43 +18,44 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="600">
+<img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
 [![Documentation Status](https://readthedocs.org/projects/graphix/badge/?version=latest)](https://graphix.readthedocs.io/en/latest/?badge=latest)
 ![GitHub](https://img.shields.io/github/license/TeamGraphix/graphix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
 ![PyPI](https://img.shields.io/pypi/v/graphix)
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg)](https://unitary.fund/)
+[![DOI](https://zenodo.org/badge/573466585.svg)](https://zenodo.org/badge/latestdoi/573466585)
 
-**Graphix** is an open-source library to optimize and simulate measurement-based quantum computing (MBQC). 
+**Graphix** is a measurement-based quantum computing (MBQC) compiler, which makes it easier to generate, optimize and simulate MBQC *measurement patterns*.
 
 ## Feature
 
 - We integrate an efficient [graph state simulator](https://graphix.readthedocs.io/en/latest/lc-mbqc.html) as an optimization routine of MBQC *measurement pattern*, with which we can classically [preprocess all Pauli measurements](https://graphix.readthedocs.io/en/latest/tutorial.html#performing-pauli-measurements) (corresponding to the elimination of all Clifford gates in the gate network - c.f. [Gottesman-Knill theorem](https://en.wikipedia.org/wiki/Gottesman–Knill_theorem)), significantly reducing the required size of graph state to run the computation.
-- We implement Matrix Product State (MPS) simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
+- We implement tensor-network simulation of MBQC with which thousands of qubits (graph nodes) can be simulated with modest computing resources (e.g. laptop), without approximation.
 - Our pattern-based construction and optimization routines are suitable for high-level optimization to run quantum algorithms on MBQC quantum hardware with minimal resource state size requirements. We plan to add quantum hardware emulators (and quantum hardware) as pattern execution backends.
 
 ## Installation
 Install `graphix` with `pip`:
 
 ```bash
 $ pip install graphix
 ```
 
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
-  - Using MPS simulator: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_mps.ipynb)
+  - Using tensor-network simulator backend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qft_with_tn.ipynb)
   - QAOA circuit: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=qaoa.ipynb)
 
 - Read the [tutorial](https://graphix.readthedocs.io/en/latest/tutorial.html) for more comprehensive guide.
 
 - For theoretical background, read our quick introduction into [MBQC](https://graphix.readthedocs.io/en/latest/intro.html) and [LC-MBQC](https://graphix.readthedocs.io/en/latest/lc-mbqc.html).
 
 ## Citing
@@ -67,24 +68,32 @@
 [^1]: Following the release of this arXiv preprint, we were made aware of a previous work by [Backens et al.](https://quantum-journal.org/papers/q-2021-03-25-421/) where Pauli measurement elimination method for MBQC was developed in the context of circuit optimization. 
 Many thanks for letting us know about this work, we will properly mention this work in the next version of our paper.
 
 ## Contributing
 
 We use [GitHub issues](https://github.com/TeamGraphix/graphix/issues) for tracking requests and bugs. 
 
+## Discord Server
+
+Please visit [Unitary Fund's Discord server](https://discord.com/servers/unitary-fund-764231928676089909), where you can find a channel for `graphix` to ask questions.
+
 ## Core Contributors
 
 Dr. Shinichi Sunami (University of Oxford)
 
 Masato Fukushima (University of Tokyo, Fixstars Amplify)
 
 ## Acknowledgements
 
 We are proud to be supported by [unitary fund microgrant program](https://unitary.fund/grants.html). 
 
+<p><a href="https://unitary.fund/grants.html">
+<img src="https://user-images.githubusercontent.com/33350509/233384863-654485cf-b7d0-449e-8868-265c6fea2ced.png" alt="unitary-fund" width="150"/>
+</a></p>
+
 Special thanks to Fixstars Amplify:
 
 <p><a href="https://amplify.fixstars.com/en/">
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/imgs/fam_logo.png" alt="amplify" width="200"/>
 </a></p>
```

### Comparing `graphix-0.2.0/graphix.egg-info/SOURCES.txt` & `graphix-0.2.1/graphix.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-docs/.DS_Store
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 graphix/__init__.py
 graphix/clifford.py
+graphix/generator.py
 graphix/gflow.py
 graphix/graphsim.py
 graphix/ops.py
 graphix/pattern.py
 graphix/simulator.py
 graphix/transpiler.py
 graphix/version.py
@@ -21,12 +21,13 @@
 graphix.egg-info/dependency_links.txt
 graphix.egg-info/requires.txt
 graphix.egg-info/top_level.txt
 graphix/sim/__init__.py
 graphix/sim/statevec.py
 graphix/sim/tensornet.py
 tests/test_clifford.py
+tests/test_generator.py
 tests/test_gflow.py
 tests/test_graphsim.py
 tests/test_pattern.py
 tests/test_tnsim.py
 tests/test_transpiler.py
```

### Comparing `graphix-0.2.0/setup.py` & `graphix-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/tests/test_clifford.py` & `graphix-0.2.1/tests/test_clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/tests/test_gflow.py` & `graphix-0.2.1/tests/test_gflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import unittest
 import networkx as nx
-from graphix.gflow import gflow, flow, generate_from_graph
-import tests.random_circuit as rc
+from graphix.gflow import gflow, flow
 import numpy as np
 
 
 class TestGflow(unittest.TestCase):
     def test_flow(self):
         nodes = [i for i in range(9)]
         edges = [(0, 3), (1, 4), (2, 5), (1, 3), (2, 4), (3, 6), (4, 7), (5, 8)]
@@ -47,15 +46,15 @@
             (4, 5),
             (7, 8),
             (2, 5),
             (5, 8),
             (8, 10),
             (10, 12),
         ]
-        input = set()
+        input = {1, 2}
         output = {11, 12}
         G = nx.Graph()
         G.add_nodes_from(nodes)
         G.add_edges_from(edges)
         f, l_k = flow(G, input, output)
         self.assertIsNone(f)
         self.assertIsNone(l_k)
@@ -82,37 +81,10 @@
         G = nx.Graph()
         G.add_nodes_from(nodes)
         G.add_edges_from(edges)
         g, l_k = gflow(G, input, output)
         self.assertIsNone(g)
         self.assertIsNone(l_k)
 
-    def test_pattern_generation_flow(self):
-        nqubits = 3
-        depth = 2
-        pairs = [(0, 1), (1, 2)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        # transpile into graph
-        pattern = circuit.transpile()
-        pattern.standardize()
-        pattern.shift_signals()
-        # get the graph and generate pattern again with flow algorithm
-        nodes, edges = pattern.get_graph()
-        g = nx.Graph()
-        g.add_nodes_from(nodes)
-        g.add_edges_from(edges)
-        input = [0, 1, 2]
-        angles = dict()
-        for cmd in pattern.get_measurement_order():
-            angles[cmd[1]] = cmd[3]
-        pattern2 = generate_from_graph(g, angles, input, pattern.output_nodes)
-        # check that the new one runs and returns correct result
-        pattern2.standardize()
-        pattern2.shift_signals()
-        pattern2.minimize_space()
-        state = circuit.simulate_statevector()
-        state_mbqc = pattern2.simulate_pattern()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `graphix-0.2.0/tests/test_graphsim.py` & `graphix-0.2.1/tests/test_graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/tests/test_pattern.py` & `graphix-0.2.1/tests/test_pattern.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 import numpy as np
 import tests.random_circuit as rc
 from graphix.transpiler import Circuit
+from graphix.pattern import Pattern
 
 
 class TestPattern(unittest.TestCase):
     def test_standardize(self):
         nqubits = 2
         depth = 1
         pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
@@ -23,14 +24,37 @@
         circuit = rc.generate_gate(nqubits, depth, pairs)
         pattern = circuit.transpile()
         pattern.minimize_space()
         state = circuit.simulate_statevector()
         state_mbqc = pattern.simulate_pattern()
         np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
+    def test_minimize_space_with_gflow(self):
+        nqubits = 5
+        depth = 5
+        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
+        circuit = rc.generate_gate(nqubits, depth, pairs)
+        pattern = circuit.transpile()
+        pattern.shift_signals()
+        pattern.perform_pauli_measurements()
+        pattern.minimize_space()
+        state = circuit.simulate_statevector()
+        state_mbqc = pattern.simulate_pattern()
+        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
+
+    def test_minimize_space_graph_maxspace_with_flow(self):
+        max_qubits = 20
+        for nqubits in range(2, max_qubits):
+            depth = 5
+            pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
+            circuit = rc.generate_gate(nqubits, depth, pairs)
+            pattern = circuit.transpile()
+            pattern.minimize_space()
+            np.testing.assert_equal(pattern.max_space(), nqubits + 1)
+
     def test_parallelize_pattern(self):
         nqubits = 2
         depth = 1
         pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
         circuit = rc.generate_gate(nqubits, depth, pairs)
         pattern = circuit.transpile()
         pattern.parallelize_pattern()
@@ -127,14 +151,35 @@
 
         isolated_nodes = pattern.get_isolated_nodes()
         # 48-node is the isolated and output node.
         isolated_nodes_ref = {48}
 
         np.testing.assert_equal(isolated_nodes, isolated_nodes_ref)
 
+    def test_get_meas_plane(self):
+        preset_meas_plane = ["XY", "XY", "XY", "YZ", "YZ", "YZ", "XZ", "XZ", "XZ"]
+        vop_list = [0, 5, 6]  # [identity, S gate, H gate]
+        pattern = Pattern(len(preset_meas_plane))
+        pattern.set_output_nodes([i for i in range(len(preset_meas_plane))])
+        for i in range(len(preset_meas_plane)):
+            pattern.add(["M", i, preset_meas_plane[i], 0, [], [], vop_list[i % 3]])
+        ref_meas_plane = {
+            0: "XY",
+            1: "XY",
+            2: "YZ",
+            3: "YZ",
+            4: "XZ",
+            5: "XY",
+            6: "XZ",
+            7: "YZ",
+            8: "XZ",
+        }
+        meas_plane = pattern.get_meas_plane()
+        np.testing.assert_equal(meas_plane, ref_meas_plane)
+
 
 def cp(circuit, theta, control, target):
     """Controlled rotation gate, decomposed"""
     circuit.rz(control, theta / 2)
     circuit.rz(target, theta / 2)
     circuit.cnot(control, target)
     circuit.rz(target, -1 * theta / 2)
```

### Comparing `graphix-0.2.0/tests/test_tnsim.py` & `graphix-0.2.1/tests/test_tnsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.0/tests/test_transpiler.py` & `graphix-0.2.1/tests/test_transpiler.py`

 * *Files identical despite different names*

