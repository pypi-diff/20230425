# Comparing `tmp/mentpy-0.1.0a2.tar.gz` & `tmp/mentpy-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentpy-0.1.0a2.tar", last modified: Fri Mar 17 22:49:25 2023, max compression
+gzip compressed data, was "mentpy-0.1.0a3.tar", last modified: Tue Apr 25 08:51:38 2023, max compression
```

## Comparing `mentpy-0.1.0a2.tar` & `mentpy-0.1.0a3.tar`

### file list

```diff
@@ -1,49 +1,64 @@
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.314034 mentpy-0.1.0a2/
--rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a2/LICENSE
--rw-r--r--   0 luismantilla   (501) staff       (20)     2944 2023-03-17 22:49:25.313891 mentpy-0.1.0a2/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     2627 2023-03-17 22:26:53.000000 mentpy-0.1.0a2/README.md
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.306535 mentpy-0.1.0a2/mentpy/
--rw-r--r--   0 luismantilla   (501) staff       (20)      285 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/__init__.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.308038 mentpy-0.1.0a2/mentpy/gradients/
--rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/gradients/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2016 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/gradients/finite_difference.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.308471 mentpy-0.1.0a2/mentpy/noise/
--rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/noise/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/noise/base_noise.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.309051 mentpy-0.1.0a2/mentpy/operators/
--rw-r--r--   0 luismantilla   (501) staff       (20)       76 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/operators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      665 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/operators/gates.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     4322 2023-03-17 21:39:04.000000 mentpy-0.1.0a2/mentpy/operators/pauliop.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.310141 mentpy-0.1.0a2/mentpy/optimizers/
--rw-r--r--   0 luismantilla   (501) staff       (20)       86 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/optimizers/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3058 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/optimizers/adam.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/optimizers/base_optimizer.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/optimizers/bp_tools.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/optimizers/sgd.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.311476 mentpy-0.1.0a2/mentpy/simulators/
--rw-r--r--   0 luismantilla   (501) staff       (20)      195 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/simulators/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2331 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/simulators/base_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1218 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/simulators/cirq_simulators.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2377 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/simulators/pattern_simulator.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3369 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/simulators/pennylane_simulators.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     1222 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/simulators/qiskit_simulators.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.312441 mentpy-0.1.0a2/mentpy/states/
--rw-r--r--   0 luismantilla   (501) staff       (20)      209 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/states/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    14599 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/states/flow.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2839 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/states/graphstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     8502 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/states/mbqcstate.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3112 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/states/templates.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.313584 mentpy-0.1.0a2/mentpy/utils/
--rw-r--r--   0 luismantilla   (501) staff       (20)      113 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/utils/__init__.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     6888 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/utils/expressivity.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     3182 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/utils/flow_space.py
--rw-r--r--   0 luismantilla   (501) staff       (20)     2691 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/utils/generate_data.py
--rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/utils/lc_equivalence.py
--rw-r--r--   0 luismantilla   (501) staff       (20)      160 2023-03-17 21:21:26.000000 mentpy-0.1.0a2/mentpy/utils/lie_algebra.py
-drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-03-17 22:49:25.307542 mentpy-0.1.0a2/mentpy.egg-info/
--rw-r--r--   0 luismantilla   (501) staff       (20)     2944 2023-03-17 22:49:25.000000 mentpy-0.1.0a2/mentpy.egg-info/PKG-INFO
--rw-r--r--   0 luismantilla   (501) staff       (20)     1037 2023-03-17 22:49:25.000000 mentpy-0.1.0a2/mentpy.egg-info/SOURCES.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-03-17 22:49:25.000000 mentpy-0.1.0a2/mentpy.egg-info/dependency_links.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-03-17 22:49:25.000000 mentpy-0.1.0a2/mentpy.egg-info/top_level.txt
--rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-03-17 22:49:25.314092 mentpy-0.1.0a2/setup.cfg
--rw-r--r--   0 luismantilla   (501) staff       (20)      430 2023-03-17 22:47:19.000000 mentpy-0.1.0a2/setup.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.460457 mentpy-0.1.0a3/
+-rw-r--r--   0 luismantilla   (501) staff       (20)    35149 2023-03-17 11:11:29.000000 mentpy-0.1.0a3/LICENSE
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-25 08:51:38.460282 mentpy-0.1.0a3/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3093 2023-04-08 10:02:59.000000 mentpy-0.1.0a3/README.md
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.444218 mentpy-0.1.0a3/mentpy/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      283 2023-04-16 02:10:35.000000 mentpy-0.1.0a3/mentpy/__init__.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.446183 mentpy-0.1.0a3/mentpy/gradients/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       33 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/gradients/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2016 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/gradients/finite_difference.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.448140 mentpy-0.1.0a3/mentpy/mbqc/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      343 2023-04-16 02:07:08.000000 mentpy-0.1.0a3/mentpy/mbqc/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    16348 2023-04-16 05:41:03.000000 mentpy-0.1.0a3/mentpy/mbqc/flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    25108 2023-04-21 10:07:34.000000 mentpy-0.1.0a3/mentpy/mbqc/mbqcircuit.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.449951 mentpy-0.1.0a3/mentpy/mbqc/states/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      149 2023-04-16 02:07:17.000000 mentpy-0.1.0a3/mentpy/mbqc/states/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      163 2023-04-15 11:17:22.000000 mentpy-0.1.0a3/mentpy/mbqc/states/aklt.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      195 2023-04-15 11:17:22.000000 mentpy-0.1.0a3/mentpy/mbqc/states/cluster.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2976 2023-04-16 05:41:03.000000 mentpy-0.1.0a3/mentpy/mbqc/states/graphstate.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7359 2023-04-18 08:22:14.000000 mentpy-0.1.0a3/mentpy/mbqc/templates.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.450531 mentpy-0.1.0a3/mentpy/noise/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       34 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/noise/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      173 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/noise/base_noise.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.452204 mentpy-0.1.0a3/mentpy/operators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      236 2023-04-21 07:24:47.000000 mentpy-0.1.0a3/mentpy/operators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2822 2023-04-21 09:50:33.000000 mentpy-0.1.0a3/mentpy/operators/controlled_ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1567 2023-04-16 01:27:43.000000 mentpy-0.1.0a3/mentpy/operators/gates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     7820 2023-04-21 10:14:40.000000 mentpy-0.1.0a3/mentpy/operators/ment.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5354 2023-04-15 10:49:22.000000 mentpy-0.1.0a3/mentpy/operators/pauliop.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.453816 mentpy-0.1.0a3/mentpy/optimizers/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      245 2023-04-25 08:17:14.000000 mentpy-0.1.0a3/mentpy/optimizers/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3054 2023-03-22 20:56:41.000000 mentpy-0.1.0a3/mentpy/optimizers/adam.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      632 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/optimizers/base_optimizer.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      379 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/optimizers/bp_tools.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3121 2023-04-25 08:49:44.000000 mentpy-0.1.0a3/mentpy/optimizers/rcd.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2637 2023-04-15 23:00:30.000000 mentpy-0.1.0a3/mentpy/optimizers/sgd.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.456594 mentpy-0.1.0a3/mentpy/simulators/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      281 2023-04-16 02:18:15.000000 mentpy-0.1.0a3/mentpy/simulators/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2143 2023-04-18 08:22:14.000000 mentpy-0.1.0a3/mentpy/simulators/base_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1156 2023-04-18 08:22:14.000000 mentpy-0.1.0a3/mentpy/simulators/cirq_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    13040 2023-04-21 10:14:40.000000 mentpy-0.1.0a3/mentpy/simulators/np_simulator_dm.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    14376 2023-04-19 21:51:28.000000 mentpy-0.1.0a3/mentpy/simulators/np_simulator_sv.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     2668 2023-04-18 19:39:18.000000 mentpy-0.1.0a3/mentpy/simulators/pattern_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     5854 2023-04-21 09:50:33.000000 mentpy-0.1.0a3/mentpy/simulators/pennylane_simulator.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1255 2023-04-21 09:50:33.000000 mentpy-0.1.0a3/mentpy/simulators/qiskit_simulators.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.458685 mentpy-0.1.0a3/mentpy/utils/
+-rw-r--r--   0 luismantilla   (501) staff       (20)      140 2023-04-16 02:10:19.000000 mentpy-0.1.0a3/mentpy/utils/__init__.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     6674 2023-04-16 02:23:18.000000 mentpy-0.1.0a3/mentpy/utils/expressivity.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3183 2023-04-16 01:51:56.000000 mentpy-0.1.0a3/mentpy/utils/flow_space.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     4466 2023-04-16 01:44:39.000000 mentpy-0.1.0a3/mentpy/utils/generate_data.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)    10395 2023-03-17 21:21:26.000000 mentpy-0.1.0a3/mentpy/utils/lc_equivalence.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3313 2023-04-16 01:44:39.000000 mentpy-0.1.0a3/mentpy/utils/lie_algebra.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.445427 mentpy-0.1.0a3/mentpy.egg-info/
+-rw-r--r--   0 luismantilla   (501) staff       (20)     3373 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/PKG-INFO
+-rw-r--r--   0 luismantilla   (501) staff       (20)     1409 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        1 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       49 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/requires.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)        7 2023-04-25 08:51:38.000000 mentpy-0.1.0a3/mentpy.egg-info/top_level.txt
+-rw-r--r--   0 luismantilla   (501) staff       (20)       38 2023-04-25 08:51:38.460516 mentpy-0.1.0a3/setup.cfg
+-rw-r--r--   0 luismantilla   (501) staff       (20)      553 2023-04-21 10:24:58.000000 mentpy-0.1.0a3/setup.py
+drwxr-xr-x   0 luismantilla   (501) staff       (20)        0 2023-04-25 08:51:38.459863 mentpy-0.1.0a3/tests/
+-rw-r--r--   0 luismantilla   (501) staff       (20)       58 2023-04-16 01:51:49.000000 mentpy-0.1.0a3/tests/test_flow.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)       64 2023-04-16 01:52:08.000000 mentpy-0.1.0a3/tests/test_graph_state.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      579 2023-04-16 01:52:23.000000 mentpy-0.1.0a3/tests/test_mbqc_templates.py
+-rw-r--r--   0 luismantilla   (501) staff       (20)      999 2023-04-19 21:51:31.000000 mentpy-0.1.0a3/tests/test_simulators.py
```

### Comparing `mentpy-0.1.0a2/LICENSE` & `mentpy-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a2/PKG-INFO` & `mentpy-0.1.0a3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 :warning: **This library is under development.**
 
-# ![MentPy: A Measurement-Based Quantum computing simulator.](./docs/_static/logo.png)
+<p align="center">
+  <img src="./docs/_static/logo.png" alt="MentPy: A Measurement-Based Quantum computing simulator." width="70%">
+</p>
 
 <div align=center>
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/v/mentpy"></a>
   <!-- <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/pyversions/mentpy"></a> -->
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/wheel/mentpy"></a>
   <a href='https://mentpy.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/mentpy/badge/?version=latest' alt='Documentation Status' />
@@ -33,37 +33,45 @@
 
 The `MentPy` library is an open-source software for simulations of 
 measurement-based quantum computing circuits. Currently, this package is under 
 development and is not ready for public use.
 
 ## Installation
 
-The `MentPy` library can be installed using `pip`:
+The `MentPy` library can be installed using `pip` with
+
+```bash
+pip install mentpy
+```
+
+or directly from the source code for the latest version with
 
 ```bash
 pip install git+https://github.com/BestQuark/mentpy.git
 ```
 
 ## Usage
-
+To simulate a measurement pattern, you can use the `mp.PatternSimulator`.
 ```python
 import mentpy as mp
 
-st = mp.templates.grid_cluster(4,2)
+st = mp.templates.grid_cluster(2,4)
 ps = mp.PatternSimulator(st)
 output = ps(np.random.rand(len(st.outputc)))
 ```
 
+For visualization of circuits, you can use the `mp.draw(st)` function
+
+![image](https://user-images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-bf59557b0875.png)
+
 ## Documentation
 
-The documentation for `MentPy` can be found [here](./docs).
+The documentation for `MentPy` can be found <a href="https://mentpy.readthedocs.io/en/latest/" target="_blank">here</a>.
 
 ## Contributing
 
 We welcome contributions to `MentPy`! Please see our [contributing guidelines](./CONTRIBUTING.md) for more information.
 
 ## License
 
 `MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
 
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a2 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a3 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
-Author: Luis Mantilla Author-email: luismantilla99@outlook.com License: UNKNOWN
-Platform: UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE
-:warning: **This library is under development.** # ![MentPy: A Measurement-
-Based Quantum computing simulator.](./docs/_static/logo.png)
+Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
+Content-Type: text/markdown License-File: LICENSE :warning: **This library is
+under development.**
+          [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
 The `MentPy` library is an open-source software for simulations of measurement-
 based quantum computing circuits. Currently, this package is under development
 and is not ready for public use. ## Installation The `MentPy` library can be
-installed using `pip`: ```bash pip install git+https://github.com/BestQuark/
-mentpy.git ``` ## Usage ```python import mentpy as mp st =
-mp.templates.grid_cluster(4,2) ps = mp.PatternSimulator(st) output = ps
-(np.random.rand(len(st.outputc))) ``` ## Documentation The documentation for
-`MentPy` can be found [here](./docs). ## Contributing We welcome contributions
-to `MentPy`! Please see our [contributing guidelines](./CONTRIBUTING.md) for
-more information. ## License `MentPy` is licensed under the [GNU General Public
-License v3.0](./LICENSE).
+installed using `pip` with ```bash pip install mentpy ``` or directly from the
+source code for the latest version with ```bash pip install git+https://
+github.com/BestQuark/mentpy.git ``` ## Usage To simulate a measurement pattern,
+you can use the `mp.PatternSimulator`. ```python import mentpy as mp st =
+mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st) output = ps
+(np.random.rand(len(st.outputc))) ``` For visualization of circuits, you can
+use the `mp.draw(st)` function ![image](https://user-
+images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-
+bf59557b0875.png) ## Documentation The documentation for `MentPy` can be found
+here. ## Contributing We welcome contributions to `MentPy`! Please see our
+[contributing guidelines](./CONTRIBUTING.md) for more information. ## License
+`MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
```

### Comparing `mentpy-0.1.0a2/mentpy/gradients/finite_difference.py` & `mentpy-0.1.0a3/mentpy/gradients/finite_difference.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a2/mentpy/operators/pauliop.py` & `mentpy-0.1.0a3/mentpy/operators/pauliop.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 GF = galois.GF(2)
 
 
 class PauliOp:
     """Class for representing Pauli operators as matrices and strings.
 
-    Args
-    ----
+    Parameters
+    ----------
     op: Union[np.ndarray, str, List[str]]
         The Pauli operator to be represented. Can be a matrix, a string, or a list of strings.
 
     Examples
     --------
     Create a Pauli operator from a matrix
 
@@ -83,20 +83,27 @@
             self._array = [self]
         else:
             self._array = [PauliOp(op) for op in self.txt.split("\n")]
 
     def __repr__(self):
         return self.txt
 
+    def __len__(self):
+        return self.mat.shape[0]
+
     def __getitem__(self, key):
         paulis = self._array[key]
         if isinstance(key, slice):
             return PauliOp(";".join([pauli.txt for pauli in paulis]))
         return paulis
 
+    def __contains__(self, item: "PauliOp"):
+        # check item.mat rows are in self.mat rows
+        return np.prod((self.mat[:, None] == item.mat).all(axis=2).any(axis=0))
+
     def _mat_to_txt(self, op):
         n_qubits = op.shape[1] // 2
         txt = ""
         for i in range(op.shape[0]):
             for j in range(op.shape[1] // 2):
                 if op[i, j] == 1 and op[i, j + n_qubits] == 0:
                     txt += "X"
@@ -125,21 +132,52 @@
                 elif char == "Y":
                     mat[i, j] = 1
                     mat[i, j + n_qubits] = 1
         return GF(mat)
 
     def commutator(self, other):
         """Returns the commutator of two Pauli operators."""
-        return self.mat + other.mat
+        return PauliOp(self.mat + other.mat)
 
     def symplectic_prod(self, other):
         """Returns the symplectic product of two Pauli operators."""
         x1 = self.mat[:, : self.mat.shape[1] // 2]
         x2 = other.mat[:, : other.mat.shape[1] // 2]
         z1 = self.mat[:, self.mat.shape[1] // 2 :]
         z2 = other.mat[:, other.mat.shape[1] // 2 :]
         return x1 @ z2.T + z1 @ x2.T
 
     def append(self, other):
-        """Appends a Pauli operator to the end of another Pauli operator."""
-        self.mat = np.vstack((self.mat, other.mat))
-        self.txt = self._mat_to_txt(self.mat)
+        """Appends a Pauli operator to the end of another Pauli operator.
+
+        Examples
+        --------
+        .. ipython:: python
+
+            op1 = mp.PauliOp('XIZ;IZI')
+            op2 = mp.PauliOp('XZZ')
+            op1.append(op2)
+            print(op1)
+        """
+        new_mat = np.vstack((self.mat, other.mat))
+        self.__init__(new_mat)
+
+    def get_subset(self, indices):
+        """Returns a subset of the Pauli operator.
+
+        Parameters
+        ----------
+        indices: List[int]
+            The indices of the Pauli operators to be returned.
+
+        Examples
+        --------
+        .. ipython:: python
+
+            op = mp.PauliOp('XIZ;ZII;IIZ;IZI')
+            print(op.get_subset([0, 2]))
+        """
+        if max(indices) >= self.mat.shape[1] // 2:
+            raise ValueError("Index out of range")
+
+        indices += [i + self.mat.shape[1] // 2 for i in indices]
+        return PauliOp(self.mat[:, indices])
```

### Comparing `mentpy-0.1.0a2/mentpy/optimizers/adam.py` & `mentpy-0.1.0a3/mentpy/optimizers/adam.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         opt = mp.optimizers.AdamOptimizer()
         print(opt)
 
 
     See Also
     --------
     :class:`mp.optimizers.SGDOptimizer`
-    
+
     Group
     -----
     optimizers
     """
 
     def __init__(self, step_size=0.1, b1=0.9, b2=0.999, eps=10**-8) -> None:
         """Initialize the Adam optimizer."""
```

### Comparing `mentpy-0.1.0a2/mentpy/optimizers/base_optimizer.py` & `mentpy-0.1.0a3/mentpy/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a2/mentpy/optimizers/sgd.py` & `mentpy-0.1.0a3/mentpy/optimizers/sgd.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :class:`mp.optimizers.AdamOptimizer`
 
     Group
     -----
     optimizers
     """
 
-    def __init__(self, step_size=0.1, momentum=0.9, nesterov=False) -> None:
+    def __init__(self, step_size=0.1, momentum=0.0, nesterov=False) -> None:
         """Initialize the SGD optimizer."""
         self.step_size = step_size
         self.momentum = momentum
         self.nesterov = nesterov
 
     def optimize(self, f, x0, num_iters=100, callback=None, verbose=False, **kwargs):
         """Optimize a function f using the SGD optimizer."""
```

### Comparing `mentpy-0.1.0a2/mentpy/simulators/base_simulator.py` & `mentpy-0.1.0a3/mentpy/simulators/base_simulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,85 @@
 import abc
 import numpy as np
 from typing import Union, List, Tuple, Optional
 
-from mentpy.states.mbqcstate import MBQCState
+from mentpy.mbqc.mbqcircuit import MBQCircuit
 
 
 class BaseSimulator(abc.ABC):
     """Base class for simulators.
 
     Note
     ----
     This class should not be used directly. Instead, use one of the subclasses.
 
     Args
     ----
-    mbqcstate: mp.MBQCState
-        The MBQC state used for the simulation.
+    mbqcircuit: mp.MBQCircuit
+        The MBQC circuit used for the simulation.
     input_state: np.ndarray
         The input state of the simulator.
 
     See Also
     --------
     :class:`mp.PatternSimulator`, :class:`mp.PennylaneSimulator`, :class:`mp.CirqSimulator`
 
     Group
     -----
     simulators
     """
 
-    def __init__(self, mbqcstate: MBQCState, input_state: np.ndarray = None) -> None:
-        self._mbqcstate = mbqcstate
+    def __init__(
+        self,
+        mbqcircuit: MBQCircuit,
+        input_state: np.ndarray = None,
+    ) -> None:
+        self._mbqcirc = mbqcircuit
         self._input_state = input_state
 
     @property
-    def mbqcstate(self) -> MBQCState:
-        """The MBQC state used for the simulation."""
-        return self._mbqcstate
+    def mbqcircuit(self) -> MBQCircuit:
+        """The MBQC circuit used for the simulation."""
+        return self._mbqcirc
 
     @property
     def input_state(self) -> np.ndarray:
         """The input state of the simulator."""
         return self._input_state
 
     @input_state.setter
     def input_state(self, input_state: np.ndarray):
         """Sets the input state of the simulator."""
         self._input_state = input_state
 
-    def __call__(
-        self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
-    ):
-        return self.measure_pattern(angles, planes, **kwargs)
+    def __call__(self, angles: List[float], **kwargs):
+        return self.run(angles, **kwargs)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__} for {self.mbqcstate}"
+        return f"{self.__class__.__name__} for {self.mbqcircuit}"
 
     @abc.abstractmethod
-    def measure(self, angle: float, plane: str = "XY", **kwargs):
+    def measure(self, angle: float, **kwargs):
         """Measures the state of the system.
 
-        Args
-        ----
+        Parameters
+        ----------
         angle: float
             The angle of measurement.
-        plane: str
-            The plane of measurement.
         """
         pass
 
     @abc.abstractmethod
-    def measure_pattern(
-        self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
-    ) -> Tuple[List[int], np.ndarray]:
+    def run(self, parameters: List[float], **kwargs) -> Tuple[List[int], np.ndarray]:
         """Measures the state of the system.
 
-        Args
-        ----
-        angles: List[float]
-            The angles of measurement.
-        planes: List[str]
-            The planes of measurement.
+        Parameters
+        ----------
+        parameters: List[float]
+            The parameters of the MBQC circuit (if any).
         """
         pass
 
     @abc.abstractmethod
     def reset(self, input_state=None):
         """Resets the simulator to the initial state."""
         pass
```

### Comparing `mentpy-0.1.0a2/mentpy/simulators/cirq_simulators.py` & `mentpy-0.1.0a3/mentpy/simulators/qiskit_simulators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from typing import Union, List, Tuple, Optional
 import numpy as np
 
-from mentpy.states.mbqcstate import MBQCState
+from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
 
 
-class CirqSimulator(BaseSimulator):
-    """Simulator for measuring patterns of MBQC states.
+class QiskitSimulator(BaseSimulator):
+    """Simulator for measuring patterns of MBQC circuits.
     Note
     ----
-    This is a placeholder for the Cirq simulator. It is not yet implemented.
+    This is a placeholder for the Qiskit simulator. It is not yet implemented.
 
     Args
     ----
-    mbqcstate: mp.MBQCState
-        The MBQC state used for the simulation.
+    mbqcircuit: mp.MBQCircuit
+        The MBQC circuit used for the simulation.
     simulator: str
         The simulator to use.
     input_state: np.ndarray
         The input state of the simulator.
 
     See Also
     --------
     :class:`mp.PatternSimulator`, :class:`mp.PennylaneSimulator`
 
     Group
     -----
     simulators
     """
 
-    def __init__(self, mbqcstate: MBQCState, input_state: np.ndarray = None) -> None:
-        super().__init__(mbqcstate, input_state)
+    def __init__(self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None) -> None:
+
+        super().__init__(mbqcircuit, input_state)
+
+        raise NotImplementedError
 
     def measure(self, angle: float, plane: str = "XY", **kwargs):
         raise NotImplementedError
 
-    def measure_pattern(
+    def run(
         self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
     ) -> Tuple[List[int], np.ndarray]:
         raise NotImplementedError
 
     def reset(self, input_state: np.ndarray = None):
         raise NotImplementedError
```

### Comparing `mentpy-0.1.0a2/mentpy/simulators/pattern_simulator.py` & `mentpy-0.1.0a3/mentpy/simulators/pattern_simulator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,88 @@
 from typing import Union, List, Tuple, Optional
 import numpy as np
 
-from mentpy.states.mbqcstate import MBQCState
+from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
-from mentpy.simulators.pennylane_simulators import *
-from mentpy.simulators.cirq_simulators import *
+from mentpy.simulators.pennylane_simulator import *
+from mentpy.simulators.np_simulator_dm import *
+from mentpy.simulators.np_simulator_sv import *
+
+# from mentpy.simulators.cirq_simulator import *
+# from mentpy.simulators.qiskit_simulator import *
 
 __all__ = ["PatternSimulator"]
 
 
 class PatternSimulator:
-    """Simulator for measuring patterns of MBQC states.
+    """Simulator for measuring patterns of MBQC circuits.
 
-    Args
-    ----
-    mbqcstate: mp.MBQCState
-        The MBQC state used for the simulation.
+    Parameters
+    ----------
+    mbqcircuit: mp.MBQCircuit
+        The MBQC circuit used for the simulation.
     simulator: str
         The simulator to use. Currently only 'pennylane-default.qubit' is supported.
 
     See Also
     --------
     :class:`mp.PennylaneSimulator`, :class:`mp.CirqSimulator`
 
     Group
     -----
     simulators
     """
 
     def __init__(
         self,
-        mbqcstate: MBQCState,
+        mbqcircuit: MBQCircuit,
         input_state: np.ndarray = None,
-        simulator="pennylane-default.qubit",
+        simulator="pennylane",
         *args,
         **kwargs,
     ) -> None:
 
         supported_simulators = {
-            "pennylane-default.qubit": PennylaneSimulator,
-            "cirq": CirqSimulator,
+            "pennylane": PennylaneSimulator,
+            # "cirq": CirqSimulator,
+            # "qiskit": QiskitSimulator,
+            "numpy-dm": NumpySimulatorDM,
+            "numpy-sv": NumpySimulatorSV,
         }
 
         if simulator not in supported_simulators:
             raise ValueError(
                 f"Simulator {simulator} not supported. Supported simulators are {supported_simulators.keys()}"
             )
 
         if input_state is None:
             input_state = 1
-            for i in range(len(mbqcstate.input_nodes)):
+            for i in range(len(mbqcircuit.input_nodes)):
                 input_state = np.kron(input_state, np.array([1, 1]) / np.sqrt(2))
+        else:
+            if not isinstance(input_state, np.ndarray):
+                raise TypeError(
+                    f"Input state must be a numpy array, not {type(input_state)}"
+                )
 
         self.simulator = supported_simulators[simulator](
-            mbqcstate, input_state, *args, **kwargs
+            mbqcircuit, input_state, *args, **kwargs
         )
 
     def __getattr__(self, name):
         return getattr(self.simulator, name)
 
-    def __call__(
-        self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
-    ):
-        return self.measure_pattern(angles, planes, **kwargs)
+    def __call__(self, angles: List[float], **kwargs):
+        return self.run(angles, **kwargs)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} ({self.simulator!r})"
 
-    def measure(self, angle: float, plane: str = "XY", **kwargs):
-        return self.simulator.measure(angle, plane, **kwargs)
+    def measure(self, angle: float, **kwargs):
+        return self.simulator.measure(angle, **kwargs)
+
+    def run(self, angles: List[float], **kwargs) -> Tuple[List[int], np.ndarray]:
 
-    def measure_pattern(
-        self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
-    ) -> Tuple[List[int], np.ndarray]:
-        return self.simulator.measure_pattern(angles, planes, **kwargs)
+        return self.simulator.run(angles, **kwargs)
 
     def reset(self, input_state: np.ndarray = None):
         return self.simulator.reset(input_state)
```

### Comparing `mentpy-0.1.0a2/mentpy/simulators/qiskit_simulators.py` & `mentpy-0.1.0a3/mentpy/simulators/cirq_simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 from typing import Union, List, Tuple, Optional
 import numpy as np
 
-from mentpy.states.mbqcstate import MBQCState
+from mentpy.mbqc.mbqcircuit import MBQCircuit
 from mentpy.simulators.base_simulator import BaseSimulator
 
 
-class QiskitSimulator(BaseSimulator):
-    """Simulator for measuring patterns of MBQC states.
+class CirqSimulator(BaseSimulator):
+    """Simulator for measuring patterns of MBQC circuits.
     Note
     ----
-    This is a placeholder for the Qiskit simulator. It is not yet implemented.
+    This is a placeholder for the Cirq simulator. It is not yet implemented.
 
-    Args
-    ----
-    mbqcstate: mp.MBQCState
-        The MBQC state used for the simulation.
+    Parameters
+    ----------
+    mbqcircuit: mp.MBQCircuit
+        The MBQC circuit used for the simulation.
     simulator: str
         The simulator to use.
     input_state: np.ndarray
         The input state of the simulator.
 
     See Also
     --------
     :class:`mp.PatternSimulator`, :class:`mp.PennylaneSimulator`
 
     Group
     -----
     simulators
     """
 
-    def __init__(self, mbqcstate: MBQCState, input_state: np.ndarray = None) -> None:
-        super().__init__(mbqcstate, input_state)
+    def __init__(self, mbqcircuit: MBQCircuit, input_state: np.ndarray = None) -> None:
+        super().__init__(mbqcircuit, input_state)
 
-    def measure(self, angle: float, plane: str = "XY", **kwargs):
+    def measure(self, angle: float, **kwargs):
         raise NotImplementedError
 
-    def measure_pattern(
-        self, angles: List[float], planes: Union[List[str], str] = "XY", **kwargs
-    ) -> Tuple[List[int], np.ndarray]:
+    def run(self, angles: List[float], **kwargs) -> Tuple[List[int], np.ndarray]:
         raise NotImplementedError
 
     def reset(self, input_state: np.ndarray = None):
         raise NotImplementedError
```

### Comparing `mentpy-0.1.0a2/mentpy/states/flow.py` & `mentpy-0.1.0a3/mentpy/mbqc/flow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,43 @@
+# Author: Luis Mantilla
+# Github: BestQuark
 """This is the Flow module. It deals with the flow of a given graph state"""
 import math
 import numpy as np
 import networkx as nx
 
-from mentpy.states import GraphState
+from mentpy.mbqc import GraphState
 from typing import List
 import warnings
 
 import galois
 
+## Not used in main MBQC module
+
 
 def find_flow(graph: GraphState, input_nodes, output_nodes, sanity_check=True):
     r"""Finds the generalized flow of graph state if allowed.
 
     Implementation of https://arxiv.org/pdf/quant-ph/0603072.pdf.
 
     Returns
     -------
     The flow function ``flow`` and the partial order function.
 
-    Examples
-    --------
-    Find the flow of a graph state :math:`|G\rangle`.
-
-    .. ipython:: python
-
-        g = nx.Graph()
-        g.add_edges_from([(0,1), (1,2), (2,3), (3, 4)])
-        state = mtp.MBQCGraph(g, input_nodes = [0], output_nodes = [4])
-        flow, partial_order = mtp.find_flow(state)
-        print("Flow of node 1: ", flow(1))
-        print("Partial order: ", partial_order)
-
     Group
     -----
     states
     """
+    # raise deprecated warning
+    warnings.warn(
+        "The function find_flow is deprecated. Use find_cflow instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+
     n_input, n_output = len(input_nodes), len(output_nodes)
     inp = input_nodes
     outp = output_nodes
     if n_input != n_output:
         raise ValueError(
             f"Cannot find flow or gflow. Input ({n_input}) and output ({n_output}) nodes have different size."
         )
@@ -294,177 +292,254 @@
                     print(f"{i} ≮ {k}")
     return conds
 
 
 ### This section implements causal flow
 
 
-def causal_flow(graph: GraphState, input_nodes, output_nodes) -> object:
+def find_cflow(graph: GraphState, input_nodes, output_nodes) -> object:
     """Finds the causal flow of a ``MBQCGraph`` if it exists.
     Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
     """
+    if len(input_nodes) != len(output_nodes):
+        raise ValueError(
+            f"Cannot find flow or gflow. Input ({len(input_nodes)}) and output ({len(output_nodes)}) nodes have different size."
+        )
+
     l = {}
+    g = {}
+    past = {}
+    C_set = set()
 
-    for v in output_nodes:
+    graph_extended = graph.copy()
+    max_node = max(graph.nodes()) + 1
+    input_nodes_extended = [max_node + i for i in range(len(input_nodes))]
+    graph_extended.add_edges_from(
+        [(input_nodes_extended[i], input_nodes[i]) for i in range(len(input_nodes))]
+    )
+
+    for v in graph_extended.nodes():
         l[v] = 0
+        past[v] = 0
+
+    for v in set(output_nodes) - set(input_nodes_extended):
+        past[v] = len(
+            set(graph_extended.neighbors(v))
+            & (set(graph_extended.nodes() - set(output_nodes)))
+        )
+        if past[v] == 1:
+            C_set = C_set.union({v})
 
-    result, flow = causal_flow_aux(
-        graph,
-        set(input_nodes),
+    flow, l = causal_flow_aux(
+        graph_extended,
+        set(input_nodes_extended),
         set(output_nodes),
-        set(output_nodes) - set(input_nodes),
+        C_set,
+        past,
         1,
+        g,
         l,
     )
 
-    if not result:
-        raise UserWarning("No causal flow exists for this graph.")
+    flow = {k: v for k, v in flow.items() if k not in input_nodes_extended}
+    ln = {k: v for k, v in l.items() if k not in input_nodes_extended}
+
+    if len(flow) != len(graph.nodes()) - len(output_nodes):
+        return None, None, None
 
-    # return flow and partial order
-    return lambda x: flow[x], lambda u, v: l[u] > l[v]
+    return lambda x: flow[x], lambda u, v: ln[u] > ln[v], max(flow.values())
 
 
-def causal_flow_aux(graph: GraphState, inputs, outputs, C, k, l) -> object:
+def causal_flow_aux(graph: GraphState, inputs, outputs, C, past, k, g, l) -> object:
     """Aux function for causal_flow"""
     V = set(graph.nodes())
-    out_prime = set()
     C_prime = set()
-    g = {}
 
     for _, v in enumerate(C):
         # get intersection of neighbors of v and (V \ output nodes
         intersection = set(graph.neighbors(v)) & (V - outputs)
         if len(intersection) == 1:
             u = intersection.pop()
             g[u] = v
-            l[v] = k
-            out_prime.add(u)
-            C_prime.add(v)
+            l[u] = k
+            outputs.add(u)
+            if u not in inputs:
+                past[u] = len(set(graph.neighbors(u)) & (V - outputs))
+                if past[u] == 1:
+                    C_prime.add(u)
+            for w in set(graph.neighbors(u)):
+                if past[w] > 0:
+                    past[w] -= 1
+                    if past[w] == 1:
+                        C_prime.add(w)
+
+    if len(C_prime) == 0:
+        return g, l
 
-    if len(out_prime) == 0:
-        if set(outputs) == V:
-            return True, l
-        else:
-            return False, l
     else:
         return causal_flow_aux(
             graph,
             inputs,
-            outputs | out_prime,
-            (C - C_prime) | ((out_prime & V) - inputs),
+            outputs,
+            C_prime,
+            past,
             k + 1,
+            g,
             l,
         )
 
 
-### This section is for GFlow ###
-
-# def gflow(state: MBQCGraph) -> object:
-#     """Finds the generalized flow of a ``MBQCGraph`` if it exists.
-#    Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
-#    """
-#     gamma = nx.adjacency_matrix(state.graph).toarray()
-#     l = {}
-#     g = {}
-
-#     for v in state.output_nodes:
-#         l[v] = 0
-
-
-#     result, flow, g = gflowaux(set(state.graph.nodes()), gamma, set(state.input_nodes), set(state.output_nodes), 1, l, g)
-
-#     return lambda x: flow[x], lambda u, v: l[u] > l[v], lambda u: g[u]
-
-# def gflowaux(V, gamma, inputs, outputs, k, l, g) -> object:
-#     """Aux function for gflow"""
-#     GF = galois.GF(2)
-#     node_mapping = {i: node for i, node in enumerate(V)}
-
-#     C = set()
-#     for u in V-outputs:
-#         # submatrix = gamma[np.ix_(list(V-outputs), list(outputs - inputs))]
-#         # get submatrix with rows corresponding to V-outputs and columns corresponding to outputs - inputs
-#         # but use the node_mapping to get the correct indices
-#         submatrix = np.zeros((len(V-outputs), len(outputs - inputs)), dtype=int)
-#         for i, v in enumerate(V-outputs):
-#             for j, w in enumerate(outputs - inputs):
-#                 submatrix[i, j] = gamma[node_mapping[v], node_mapping[w]]
-
-#         iu = np.zeros(len(V-outputs), dtype=int)
-#         iu[list(V-outputs).index(u)] = 1
-#         # use node_mapping to get the correct index
-
-#         submatrix, iu = GF(submatrix), GF(np.array([iu]).T)
-#         #solve submatrix @ X = iu using galois in mod2
-#         sys = np.hstack((submatrix, iu))
-#         row_reduced = sys.row_reduce()
-
-#         # FILL HERE TO GET SOLUTION
-
-
-#         # check if solution is a valid solution
-#         if np.linalg.norm(submatrix @ solution - iu) <= 1e-5:
-#             l[u] = k
-#             C.add(u)
-#             g[u] = solution
-
-#     if len(C) == 0:
-#         return True, l, g
-#     else:
-#         return gflowaux(V, gamma, inputs, outputs | C, k+1, l, g)
-
-
-# def _check_if_gflow(state: MBQCGraph, gflow, partial_order) -> bool:
-#     """Checks if gflow satisfies conditions on state."""
+### This section implements generalized flow
 
 
 def find_gflow(graph: GraphState, input_nodes, output_nodes) -> object:
     """Finds the generalized flow of a ``MBQCGraph`` if it exists.
     Retrieved from https://arxiv.org/pdf/0709.2670v1.pdf.
     """
-    gamma = nx.adjacency_matrix(graph).toarray()
+    graph_extended = graph.copy()
+    max_node = max(graph.nodes()) + 1
+    input_nodes_extended = [max_node + i for i in range(len(input_nodes))]
+    graph_extended.add_edges_from(
+        [(input_nodes_extended[i], input_nodes[i]) for i in range(len(input_nodes))]
+    )
+
+    gamma = nx.adjacency_matrix(graph_extended).toarray()
+
     l = {}
     g = {}
 
     for v in output_nodes:
         l[v] = 0
 
-    result, flow, g = gflowaux(
-        graph, gamma, set(input_nodes), set(output_nodes) - set(input_nodes), 1, l, g
+    result, g, l = gflowaux(
+        graph_extended,
+        gamma,
+        set(input_nodes_extended),
+        set(output_nodes) - set(input_nodes_extended),
+        1,
+        g,
+        l,
     )
 
     if result == False:
         warnings.warn("No gflow exists for this graph.", UserWarning, stacklevel=2)
+        return None, None, None
+
+    gn = {i: g[i] for i in set(graph.nodes()) - set(output_nodes)}
+    ln = {i: l[i] for i in graph.nodes()}
+
+    return lambda x: gn[x], lambda u, v: ln[u] > ln[v], max(ln.values())
 
-    return lambda x: flow[x], lambda u, v: l[u] > l[v], lambda u: g[u]
 
+def gf2_matrix_solve(A, b):
+    A = A % 2
+    b = b % 2
+    sol, _, _, _ = np.linalg.lstsq(A, b, rcond=None)
+    return (sol.round() % 2).astype(int)
 
-def gflowaux(graph: GraphState, gamma, inputs, outputs, k, l, g) -> object:
+
+def gflowaux(graph: GraphState, gamma, inputs, outputs, k, g, l) -> object:
     """Aux function for gflow"""
     out_prime = set()
+    mapping = graph.index_mapping()
     GF = galois.GF(2)
     V = set(graph.nodes())
     C = set()
-    for u in V - outputs:
-        submatrix = GF(np.zeros((len(V - outputs), len(outputs)), dtype=int))
-        b = GF(np.zeros((len(V - outputs), 1), dtype=int))
-        b[list(V - outputs).index(u)] = 1
-        syst = np.hstack((submatrix, b))
-        row_reduced = GF(syst).row_reduce()
-        solution = GF(np.zeros((len(outputs), 1), dtype=int))
-        for i, v in enumerate(outputs):
-            if row_reduced[i, i] == 1:
-                solution[i] = row_reduced[i, -1]
+    vmol = list(V - outputs)
+    for u in vmol:
+        submatrix = np.zeros((len(vmol), len(outputs - inputs)), dtype=int)
+        for i, v in enumerate(vmol):
+            for j, w in enumerate(outputs - inputs):
+                submatrix[i, j] = gamma[mapping[v], mapping[w]]
+
+        b = np.zeros((len(vmol), 1), dtype=int)
+        b[vmol.index(u)] = 1
+        solution = gf2_matrix_solve(submatrix, b)
 
+        # Check if solution is a valid solution
         if np.linalg.norm(submatrix @ solution - b) <= 1e-5:
             l[u] = k
             C.add(u)
             g[u] = solution
 
     if len(C) == 0:
         if set(outputs) == V:
-            return True, l, g
+            return True, g, l
         else:
-            return False, l, g
+            return False, g, l
+
+    else:
+        return gflowaux(graph, gamma, inputs, outputs | C, k + 1, g, l)
+
 
+## This section implements PauliFlow
+
+
+def find_pflow(
+    graph: GraphState, input_nodes, output_nodes, basis="XY", testing=False
+) -> object:
+    """Implementation of pauli flow algorithm in https://arxiv.org/pdf/2109.05654v1.pdf"""
+
+    if not testing:
+        raise NotImplementedError("This algorithm is not yet implemented.")
+
+    if type(basis) == str:
+        basis = {v: basis for v in graph.nodes()}
+    elif type(basis) != dict:
+        raise TypeError("Basis must be a string or a dictionary.")
+
+    lx = set()
+    ly = set()
+    lz = set()
+    d = {}
+    p = {}
+
+    gamma = nx.adjacency_matrix(graph).toarray()
+
+    for v in graph.nodes():
+        if v in output_nodes:
+            d[v] = 0
+        if basis[v] == "X":
+            lx = lx.add(v)
+        elif basis[v] == "Y":
+            ly = ly.add(v)
+        elif basis[v] == "Z":
+            lz = lz.add(v)
+
+    return pflowaux(graph, gamma, input_nodes, basis, set(), output_nodes, 0, d, p)
+
+
+def pflowaux(graph: GraphState, gamma, inputs, plane, A, B, k, d, p) -> object:
+    """Aux function for pflow"""
+    C = set()
+    mapping = graph.index_mapping()
+    for u in set(graph.nodes()) - set(B):
+        submatrix1, submatrix2, submatrix3 = None, None, None
+        solution1, solution2, solution3 = None, None, None
+        if plane[u] in ["XY", "X", "Y"]:
+            submatrix1 = 0  # TODO
+            solution1 = 0  # TODO
+        if plane[u] in ["XZ", "X", "Z"]:
+            submatrix2 = 0  # TODO
+            solution2 = 0  # TODO
+        if plane[u] in ["YZ", "Y", "Z"]:
+            submatrix3 = 0  # TODO
+            solution3 = 0  # TODO
+
+        if (
+            (solution1 is not None)
+            or (solution2 is not None)
+            or (solution3 is not None)
+        ):
+            C.add(u)
+            sol = solution1 or solution2 or solution3
+            p[u] = sol
+            d[u] = k
+
+    if len(C) == 0 and k > 0:
+        if set(B) == set(graph.nodes()):
+            return True, p, d
+        else:
+            return False, set(), set()
     else:
-        return gflowaux(graph, gamma, inputs, outputs | C, k + 1, l, g)
+        B = B.union(C)
+        return pflowaux(graph, gamma, inputs, plane, B, B, k + 1, d, p)
```

### Comparing `mentpy-0.1.0a2/mentpy/states/graphstate.py` & `mentpy-0.1.0a3/mentpy/mbqc/states/graphstate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Author: Luis Mantilla
+# Github: BestQuark
 import numpy as np
 from mentpy.operators import PauliOp
 import networkx as nx
 from typing import Optional, List
 
 __all__ = ["GraphState", "entanglement_entropy"]
 
@@ -17,49 +19,54 @@
 
         g = mp.GraphState()
         g.add_edges_from([(0,1), (1,2), (2,3), (3, 4)])
         print(g)
 
     See Also
     --------
-    :class:`mentpy.state.mbqcstate.MBQCState`
+    :class:`mentpy.mbqc.MBQCircuit`
 
     Group
     -----
     states
     """
 
     def __init__(self, *args, **kwargs):
+        """Initialize a graph state. See networkx.Graph for more information."""
         super().__init__(*args, **kwargs)
 
     def __repr__(self):
         return f"GraphState with {self.number_of_nodes()} nodes and {self.number_of_edges()} edges."
 
     def __len__(self):
         return self.number_of_nodes()
 
     def __eq__(self, other):
         return nx.is_isomorphic(self, other)
-    
+
+    def index_mapping(self):
+        """Return a mapping of the nodes to their indices."""
+        return {v: i for i, v in enumerate(self.nodes())}
+
     def stabilizers(self):
         """
         Generate the stabilizers of a graph state.
-        
+
         Examples
         --------
         Calculate the stabilizers of a 1D cluster state :math:`|G>` of five qubits
 
         .. ipython:: python
             :okwarning:
 
             g = mp.GraphState()
             g.add_edges_from([(0,1), (1,2), (2,3), (3, 4)])
             print(g.stabilizers())
         """
-        return graphstate_stabs(self)
+        return _get_stabilizers(self)
 
 
 def lc_reduce(graph: GraphState):
     """Reduce graph state
 
     Group
     -----
@@ -91,24 +98,18 @@
         for v in subRegionA:
             G = nx.contracted_nodes(G, subRegionB[0], v)
         subRegionB = subRegionB[0]
 
     return nx.minimum_cut(G, subRegionA, subRegionB)[0]
 
 
-def graphstate_stabs(graph: GraphState) -> List[PauliOp]:
+def _get_stabilizers(graph: GraphState) -> List[PauliOp]:
     """Generate the stabilizers of a graph state.
 
-    Examples
-    --------
-    Calculate the stabilizers of a 1D cluster state :math:`|G>` of five qubits
-    
     Group
     -----
     states
     """
     z_mat = nx.adjacency_matrix(graph).todense()
     x_mat = np.eye(graph.number_of_nodes(), dtype=int)
 
     return PauliOp(np.hstack((x_mat, z_mat)))
-
-
```

### Comparing `mentpy-0.1.0a2/mentpy/utils/expressivity.py` & `mentpy-0.1.0a3/mentpy/utils/expressivity.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,42 +3,41 @@
 import networkx as nx
 
 from scipy.spatial import distance
 from scipy.special import kl_div, rel_entr
 
 import pennylane as qml
 
-from mentpy.states import MBQCState
+from mentpy.mbqc import MBQCircuit
 from mentpy.simulators import PatternSimulator
 from mentpy.utils.lc_equivalence import are_lc_equivalent
-from mentpy.utils.generate_data import generate_random_input_states
+from mentpy.utils.generate_data import generate_haar_random_states
 from mentpy.utils.flow_space import FlowSpace
 
 
 def haar_probability_density_of_fidelities(F: float, n_qubits: int):
     r"""Returns the probability density function of fidelities
     :math:`P_{Haar}(F) = (N-1)(1-F)^{N-2}` where :math:`N = 2^{n}` is
     the dimension of the Hilbert space.
 
     Args
     ----
     F (float): Fidelity. Must be between :math:`0` and :math:`1`.
     n_qubits (int): Number of qubits. Must be greater than or equal to 1.
-    n_bins (int): Number of bins used in the histogram
 
     Returns
     -------
     :math:`P_{Haar}(F) = (N-1)(1-F)^{N-2}`  where  :math:`N = 2^{n}`
     """
     N = int(2**n_qubits)
     return (N - 1) * ((1 - F) ** (N - 2))
 
 
 def expressivity_with_histogram(
-    graph_state_circuit: MBQCState,
+    graph_state_circuit: MBQCircuit,
     n_samples: int = 10000,
     n_bins: int = 1000,
     method: str = "KL",
 ):
     r"""Returns the expressivity calculated using the Kullback-Leiber entropy
 
     Args
@@ -81,21 +80,21 @@
     elif method == "JS":
         expressivity = distance.jensenshannon(discrete_prob_data, discrete_prob_haar)
 
     return expressivity
 
 
 def sample_probability_density_of_fidelities(
-    graph_state_circuit: MBQCState, n_samples=1000, backend="pennylane"
+    graph_state_circuit: MBQCircuit, n_samples=1000, backend="pennylane"
 ):
     r"""Calculates samples of the probability of fidelities of the given graph state circuit"""
 
     pattern_simulator = PatternSimulator(graph_state_circuit)
-    random_input_states = generate_random_input_states(
-        pattern_simulator.state, n_samples
+    random_input_states = generate_haar_random_states(
+        len(graph_state_circuit.input_nodes), n_samples
     )
     fidelities = []
 
     if backend == "pennylane":
         qmlcircuit = pattern_simulator.graphstate_to_circuit()
         for random_st in random_input_states:
             random_pattern = (
@@ -125,16 +124,14 @@
 def digraph_expressivity_of_flow_space(flow_space: FlowSpace, method="KL", **kwargs):
     """Returns digraph given the expressivity of a ``FlowSpace`` object.
 
     Args
     ----
         flow_space (FlowSpace): Graph for which we will calculate the expressivity
         method (str): 'KL' for Kullback-Leiber entropy, 'RE' for relative entropy.
-        n_samples (int): Number of samples to calculate fidelity histogram. 10000 is default.
-        n_bins (int): Number of bins of fidelity histogram. 1000 is default.
     """
 
     expr_digraph = nx.DiGraph()
     for node in flow_space.flow_graph_space.nodes():
         graph_circuit = flow_space.flow_graph_space.nodes[node]["mbqc_circuit"]
         expr = expressivity_with_histogram(graph_circuit, method=method, **kwargs)
         expr_digraph.add_node(node, expr=expr, mbqc_circuit=graph_circuit)
```

### Comparing `mentpy-0.1.0a2/mentpy/utils/flow_space.py` & `mentpy-0.1.0a3/mentpy/utils/flow_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from mentpy.states import MBQCState
+from mentpy.mbqc import MBQCircuit
 
 import networkx as nx
 import itertools
 
 
 class FlowSpace:
     r"""The flow space graph of a MBQCGraph.
@@ -10,15 +10,15 @@
     Each node corresponds to a possible graph over ``len(graph_state)`` qubits.
     Each edge between nodes represent going from one graph to another via adding or removing edges.
 
     .. note::  ``flow_space()`` will only work for MBQCGraph with less
     than 8 qubits.
     """
 
-    def __init__(self, graph_state: MBQCState, allow_any_size_graphs: bool = False):
+    def __init__(self, graph_state: MBQCircuit, allow_any_size_graphs: bool = False):
         """Creates the flow graph space of a graph state circuit."""
 
         if len(graph_state) > 7 and (not allow_any_size_graphs):
             raise UserWarning(
                 f"Expected a graph_state of size 7 or less, but {len(graph_state)} "
                 "was given."
             )
@@ -59,15 +59,15 @@
         subgraph of all graphs without flow."""
 
         graphs_list = list(self.generator_all_graphs())
         graph_space = nx.Graph()
         wflow = []
         woflow = []
         for ind, g in enumerate(graphs_list):
-            gs = MBQCState(
+            gs = MBQCircuit(
                 g, input_nodes=self.input_nodes, output_nodes=self.output_nodes
             )
 
             fl = gs.flow
 
             if fl is not None:
                 graph_space.add_node(ind, flow=True, mbqc_circuit=gs)
```

### Comparing `mentpy-0.1.0a2/mentpy/utils/lc_equivalence.py` & `mentpy-0.1.0a3/mentpy/utils/lc_equivalence.py`

 * *Files identical despite different names*

### Comparing `mentpy-0.1.0a2/mentpy.egg-info/PKG-INFO` & `mentpy-0.1.0a3/mentpy.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mentpy
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A Python library for simulating MBQC circuits
 Home-page: https://github.com/BestQuark/mentpy
 Author: Luis Mantilla
 Author-email: luismantilla99@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 :warning: **This library is under development.**
 
-# ![MentPy: A Measurement-Based Quantum computing simulator.](./docs/_static/logo.png)
+<p align="center">
+  <img src="./docs/_static/logo.png" alt="MentPy: A Measurement-Based Quantum computing simulator." width="70%">
+</p>
 
 <div align=center>
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/v/mentpy"></a>
   <!-- <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/pyversions/mentpy"></a> -->
   <a href="https://pypi.org/project/mentpy"><img src="https://img.shields.io/pypi/wheel/mentpy"></a>
   <a href='https://mentpy.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/mentpy/badge/?version=latest' alt='Documentation Status' />
@@ -33,37 +33,45 @@
 
 The `MentPy` library is an open-source software for simulations of 
 measurement-based quantum computing circuits. Currently, this package is under 
 development and is not ready for public use.
 
 ## Installation
 
-The `MentPy` library can be installed using `pip`:
+The `MentPy` library can be installed using `pip` with
+
+```bash
+pip install mentpy
+```
+
+or directly from the source code for the latest version with
 
 ```bash
 pip install git+https://github.com/BestQuark/mentpy.git
 ```
 
 ## Usage
-
+To simulate a measurement pattern, you can use the `mp.PatternSimulator`.
 ```python
 import mentpy as mp
 
-st = mp.templates.grid_cluster(4,2)
+st = mp.templates.grid_cluster(2,4)
 ps = mp.PatternSimulator(st)
 output = ps(np.random.rand(len(st.outputc)))
 ```
 
+For visualization of circuits, you can use the `mp.draw(st)` function
+
+![image](https://user-images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-bf59557b0875.png)
+
 ## Documentation
 
-The documentation for `MentPy` can be found [here](./docs).
+The documentation for `MentPy` can be found <a href="https://mentpy.readthedocs.io/en/latest/" target="_blank">here</a>.
 
 ## Contributing
 
 We welcome contributions to `MentPy`! Please see our [contributing guidelines](./CONTRIBUTING.md) for more information.
 
 ## License
 
 `MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
 
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a2 Summary: A Python library
+Metadata-Version: 2.1 Name: mentpy Version: 0.1.0a3 Summary: A Python library
 for simulating MBQC circuits Home-page: https://github.com/BestQuark/mentpy
-Author: Luis Mantilla Author-email: luismantilla99@outlook.com License: UNKNOWN
-Platform: UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE
-:warning: **This library is under development.** # ![MentPy: A Measurement-
-Based Quantum computing simulator.](./docs/_static/logo.png)
+Author: Luis Mantilla Author-email: luismantilla99@outlook.com Description-
+Content-Type: text/markdown License-File: LICENSE :warning: **This library is
+under development.**
+          [MentPy: A Measurement-Based Quantum computing simulator.]
   [https://img.shields.io/pypi/v/mentpy]  [https://img.shields.io/pypi/wheel/
     mentpy] [Documentation_Status]  [https://img.shields.io/twitter/follow/
                  mentpy?label=mentpy&style=flat&logo=twitter]
 The `MentPy` library is an open-source software for simulations of measurement-
 based quantum computing circuits. Currently, this package is under development
 and is not ready for public use. ## Installation The `MentPy` library can be
-installed using `pip`: ```bash pip install git+https://github.com/BestQuark/
-mentpy.git ``` ## Usage ```python import mentpy as mp st =
-mp.templates.grid_cluster(4,2) ps = mp.PatternSimulator(st) output = ps
-(np.random.rand(len(st.outputc))) ``` ## Documentation The documentation for
-`MentPy` can be found [here](./docs). ## Contributing We welcome contributions
-to `MentPy`! Please see our [contributing guidelines](./CONTRIBUTING.md) for
-more information. ## License `MentPy` is licensed under the [GNU General Public
-License v3.0](./LICENSE).
+installed using `pip` with ```bash pip install mentpy ``` or directly from the
+source code for the latest version with ```bash pip install git+https://
+github.com/BestQuark/mentpy.git ``` ## Usage To simulate a measurement pattern,
+you can use the `mp.PatternSimulator`. ```python import mentpy as mp st =
+mp.templates.grid_cluster(2,4) ps = mp.PatternSimulator(st) output = ps
+(np.random.rand(len(st.outputc))) ``` For visualization of circuits, you can
+use the `mp.draw(st)` function ![image](https://user-
+images.githubusercontent.com/52287586/230715389-bf280971-c841-437d-8772-
+bf59557b0875.png) ## Documentation The documentation for `MentPy` can be found
+here. ## Contributing We welcome contributions to `MentPy`! Please see our
+[contributing guidelines](./CONTRIBUTING.md) for more information. ## License
+`MentPy` is licensed under the [GNU General Public License v3.0](./LICENSE).
```

### Comparing `mentpy-0.1.0a2/mentpy.egg-info/SOURCES.txt` & `mentpy-0.1.0a3/mentpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 LICENSE
 README.md
 setup.py
 mentpy/__init__.py
 mentpy.egg-info/PKG-INFO
 mentpy.egg-info/SOURCES.txt
 mentpy.egg-info/dependency_links.txt
+mentpy.egg-info/requires.txt
 mentpy.egg-info/top_level.txt
 mentpy/gradients/__init__.py
 mentpy/gradients/finite_difference.py
+mentpy/mbqc/__init__.py
+mentpy/mbqc/flow.py
+mentpy/mbqc/mbqcircuit.py
+mentpy/mbqc/templates.py
+mentpy/mbqc/states/__init__.py
+mentpy/mbqc/states/aklt.py
+mentpy/mbqc/states/cluster.py
+mentpy/mbqc/states/graphstate.py
 mentpy/noise/__init__.py
 mentpy/noise/base_noise.py
 mentpy/operators/__init__.py
+mentpy/operators/controlled_ment.py
 mentpy/operators/gates.py
+mentpy/operators/ment.py
 mentpy/operators/pauliop.py
 mentpy/optimizers/__init__.py
 mentpy/optimizers/adam.py
 mentpy/optimizers/base_optimizer.py
 mentpy/optimizers/bp_tools.py
+mentpy/optimizers/rcd.py
 mentpy/optimizers/sgd.py
 mentpy/simulators/__init__.py
 mentpy/simulators/base_simulator.py
-mentpy/simulators/cirq_simulators.py
+mentpy/simulators/cirq_simulator.py
+mentpy/simulators/np_simulator_dm.py
+mentpy/simulators/np_simulator_sv.py
 mentpy/simulators/pattern_simulator.py
-mentpy/simulators/pennylane_simulators.py
+mentpy/simulators/pennylane_simulator.py
 mentpy/simulators/qiskit_simulators.py
-mentpy/states/__init__.py
-mentpy/states/flow.py
-mentpy/states/graphstate.py
-mentpy/states/mbqcstate.py
-mentpy/states/templates.py
 mentpy/utils/__init__.py
 mentpy/utils/expressivity.py
 mentpy/utils/flow_space.py
 mentpy/utils/generate_data.py
 mentpy/utils/lc_equivalence.py
-mentpy/utils/lie_algebra.py
+mentpy/utils/lie_algebra.py
+tests/test_flow.py
+tests/test_graph_state.py
+tests/test_mbqc_templates.py
+tests/test_simulators.py
```

