# Comparing `tmp/ratinabox-1.5.1.tar.gz` & `tmp/ratinabox-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratinabox-1.5.1.tar", last modified: Fri Apr 21 16:39:02 2023, max compression
+gzip compressed data, was "ratinabox-1.6.0.tar", last modified: Mon Apr 24 17:06:25 2023, max compression
```

## Comparing `ratinabox-1.5.1.tar` & `ratinabox-1.6.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.128712 ratinabox-1.5.1/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.5.1/LICENSE
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 16:39:02.128826 ratinabox-1.5.1/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)    24627 2023-04-11 18:06:50.000000 ratinabox-1.5.1/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.5.1/pyproject.toml
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.122072 ratinabox-1.5.1/ratinabox/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    41547 2023-04-21 16:30:58.000000 ratinabox-1.5.1/ratinabox/Agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    32289 2023-04-21 16:31:04.000000 ratinabox-1.5.1/ratinabox/Environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    81263 2023-04-21 16:29:55.000000 ratinabox-1.5.1/ratinabox/Neurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.5.1/ratinabox/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.5.1/ratinabox/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.124333 ratinabox-1.5.1/ratinabox/contribs/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/FieldOfViewNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/PhasePrecessingPlaceCells.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/PlaneWaveNeurons.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.5.1/ratinabox/contribs/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.5.1/ratinabox/contribs/STDPFeedForwardLayer.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-04-21 14:28:51.000000 ratinabox-1.5.1/ratinabox/contribs/SuccessorFeatures.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/ThetaSequenceAgent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7270 2023-04-21 14:50:52.000000 ratinabox-1.5.1/ratinabox/contribs/ValueNeuron.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.5.1/ratinabox/contribs/__init__.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.125370 ratinabox-1.5.1/ratinabox/data/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.5.1/ratinabox/data/README.md
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.5.1/ratinabox/data/__init__.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.5.1/ratinabox/data/rat.png
--rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.5.1/ratinabox/data/sargolini.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.5.1/ratinabox/data/tanni.npz
--rw-r--r--   0 tomgeorge   (501) staff       (20)    34247 2023-04-21 16:38:02.000000 ratinabox-1.5.1/ratinabox/utils.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.122836 ratinabox-1.5.1/ratinabox.egg-info/
--rw-r--r--   0 tomgeorge   (501) staff       (20)    25321 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/PKG-INFO
--rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/SOURCES.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/dependency_links.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/requires.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-21 16:39:02.000000 ratinabox-1.5.1/ratinabox.egg-info/top_level.txt
--rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-21 16:39:02.129134 ratinabox-1.5.1/setup.cfg
--rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.5.1/setup.py
-drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-21 16:39:02.128611 ratinabox-1.5.1/tests/
--rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.5.1/tests/test_advanced.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.5.1/tests/test_agent.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.5.1/tests/test_environment.py
--rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.5.1/tests/test_neurons.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-24 17:06:25.398680 ratinabox-1.6.0/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1068 2022-12-19 16:05:16.000000 ratinabox-1.6.0/LICENSE
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-04-24 17:06:25.398817 ratinabox-1.6.0/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    26607 2023-04-24 16:38:06.000000 ratinabox-1.6.0/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       88 2023-01-09 17:15:52.000000 ratinabox-1.6.0/pyproject.toml
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-24 17:06:25.389239 ratinabox-1.6.0/ratinabox/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    42379 2023-04-24 16:38:06.000000 ratinabox-1.6.0/ratinabox/Agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    32366 2023-04-24 16:38:06.000000 ratinabox-1.6.0/ratinabox/Environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    82493 2023-04-24 16:38:06.000000 ratinabox-1.6.0/ratinabox/Neurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      560 2022-07-22 03:47:47.000000 ratinabox-1.6.0/ratinabox/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3820 2023-04-06 16:54:27.000000 ratinabox-1.6.0/ratinabox/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-24 17:06:25.391684 ratinabox-1.6.0/ratinabox/contribs/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     8800 2023-04-23 10:24:42.000000 ratinabox-1.6.0/ratinabox/contribs/FieldOfViewNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     5782 2023-04-23 10:24:42.000000 ratinabox-1.6.0/ratinabox/contribs/PhasePrecessingPlaceCells.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3930 2023-04-23 10:24:42.000000 ratinabox-1.6.0/ratinabox/contribs/PlaneWaveNeurons.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1298 2022-10-06 19:21:04.000000 ratinabox-1.6.0/ratinabox/contribs/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3822 2023-01-06 11:05:05.000000 ratinabox-1.6.0/ratinabox/contribs/STDPFeedForwardLayer.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3402 2023-04-24 16:38:06.000000 ratinabox-1.6.0/ratinabox/contribs/SuccessorFeatures.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    15029 2023-04-23 10:24:42.000000 ratinabox-1.6.0/ratinabox/contribs/ThetaSequenceAgent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7522 2023-04-24 16:38:06.000000 ratinabox-1.6.0/ratinabox/contribs/ValueNeuron.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      193 2023-03-07 14:55:23.000000 ratinabox-1.6.0/ratinabox/contribs/__init__.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-24 17:06:25.393254 ratinabox-1.6.0/ratinabox/data/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     2736 2022-10-19 17:17:32.000000 ratinabox-1.6.0/ratinabox/data/README.md
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-09 10:55:06.000000 ratinabox-1.6.0/ratinabox/data/__init__.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     3357 2023-04-06 16:54:27.000000 ratinabox-1.6.0/ratinabox/data/rat.png
+-rw-r--r--   0 tomgeorge   (501) staff       (20)   715694 2022-08-10 04:16:33.000000 ratinabox-1.6.0/ratinabox/data/sargolini.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)  5272574 2022-10-19 17:17:32.000000 ratinabox-1.6.0/ratinabox/data/tanni.npz
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    34247 2023-04-23 10:24:42.000000 ratinabox-1.6.0/ratinabox/utils.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-24 17:06:25.390177 ratinabox-1.6.0/ratinabox.egg-info/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)    27301 2023-04-24 17:06:25.000000 ratinabox-1.6.0/ratinabox.egg-info/PKG-INFO
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      907 2023-04-24 17:06:25.000000 ratinabox-1.6.0/ratinabox.egg-info/SOURCES.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        1 2023-04-24 17:06:25.000000 ratinabox-1.6.0/ratinabox.egg-info/dependency_links.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       46 2023-04-24 17:06:25.000000 ratinabox-1.6.0/ratinabox.egg-info/requires.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       10 2023-04-24 17:06:25.000000 ratinabox-1.6.0/ratinabox.egg-info/top_level.txt
+-rw-r--r--   0 tomgeorge   (501) staff       (20)      930 2023-04-24 17:06:25.399195 ratinabox-1.6.0/setup.cfg
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       69 2023-02-09 16:01:18.000000 ratinabox-1.6.0/setup.py
+drwxr-xr-x   0 tomgeorge   (501) staff       (20)        0 2023-04-24 17:06:25.398552 ratinabox-1.6.0/tests/
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     7884 2023-04-12 13:21:00.000000 ratinabox-1.6.0/tests/test_advanced.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)       13 2023-01-04 16:37:04.000000 ratinabox-1.6.0/tests/test_agent.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)     1257 2023-02-02 11:38:49.000000 ratinabox-1.6.0/tests/test_environment.py
+-rw-r--r--   0 tomgeorge   (501) staff       (20)        0 2023-01-04 16:37:04.000000 ratinabox-1.6.0/tests/test_neurons.py
```

### Comparing `ratinabox-1.5.1/LICENSE` & `ratinabox-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/PKG-INFO` & `ratinabox-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: ratinabox
-Version: 1.5.1
-Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
-Author: Tom George
-Author-email: tomgeorge1@btinternet.com
-License: MIT
-Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
-Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
-Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
-Platform: any
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # RatInABox 
 ![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
 [**Install**](#installing-and-importing) | [**Demos**](#get-started) | [**Features**](#feature-run-down) | [**Contributions and Questions**](#contribute) | [**Cite**](#cite)
 
@@ -41,14 +22,15 @@
     * `GridCells`
     * `BoundaryVectorCells` (egocentric or allocentric)
     * `ObjectVectorCells`
     * `VelocityCells`
     * `SpeedCells`
     * `HeadDirectionCells`
     * `FeedForwardLayer` (a generic class analagous to a feedforward layer in a deep neural network)
+    * `SuccessorFeatures` 
     * ...
 
 The top animation shows an example use case: an `Agent` randomly explores a 2D `Environment` with a wall. Three populations of `Neurons` (`PlaceCells`, `GridCells`, `BoundaryVectorCells`) fire according to the receptive fields shown. All data is saved into the history for downstream use. `RatInABox` is fully continuous is space; this means that position and neuronal firing rates are calculated rapidly online with float precision rather than pre-calculated over a discretised mesh. `RatInABox` is flexibly discretised in time; `dt` can be set by the user (defaulting to 10 ms) depending on requirements.
 
 
 ## Key features
 * **Non-specific**: Trajectories can be randomly generated, imported, or adaptively controlled making `RatInABox` a powerful engine for many tasks involving continuous motion (e.g. control theory or [reinforcement learning](#policy-control)). 
@@ -97,44 +79,46 @@
 * [1- or 2-dimensions](#1--or-2-dimensions) 
 
 (ii) the [`Agent`](#ii-agent-features)
 * [Random motion](#random-motion-model)
 * [Importing trajectories](#importing-trajectories)
 * [Policy control](#policy-control)
 * [Wall repelling](#wall-repelling)
+* [Multiple Agents](#multiple-agents)
 * [Advanced `Agent` classes](#advanced-agent-classes)
 
 (iii) the [`Neurons`](#iii-neurons-features).
 * [Cell types](#multiple-cell-types) 
 * [Noise](#noise)
 * [Spikes vs rates](#spiking)
 * [Plotting rate maps](#rate-maps)
 * [Place cell models](#place-cell-models) 
 * [Place cell geometry](#geometry-of-placecells)
 * [Egocentric encodings](#egocentric-encodings)
+* [Successor features and reinforcement learning](#successor-features-and-reinforcement-learning)
 * [Deep neural networks](#more-complex-neuron-types-and-networks-of-neurons)
 
 (iv) [Figures and animations plotting](#iv-figures-and-animations)
 
 Specific details can be found in the [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3). 
 
 
 
 ### (i) `Environment` features
-#### Walls 
+#### **Walls**
 Arbitrarily add walls to the environment to produce arbitrarily complex mazes:
 ```python 
 Environment.add_wall([[x0,y0],[x1,y1]])
 ```
 Here are some easy to make examples.
 
 <img src=".images/readme/walls.png" width=1000>
 
 
-#### Complex `Environment`s: Polygons, curves, and holes
+#### **Complex `Environment`s: Polygons, curves, and holes**
 By default, `Environments` in RatInABox are square (or rectangular if `aspect != 1`). It is possible to create arbitrary environment shapes using the `"boundary"` parameter at initialisation. 
 
 One can all add holes to the `Environment` using the `"holes"` parameter at initialisation. Positions sampled from the Environment (e.g. at initialisation) won't be inside holes.
 
 Any curved environments can be made by creating a boundary of many small walls (uyse sparingly, walls may slow down computations)
 
 ```python 
@@ -157,39 +141,39 @@
 ```
 
 
 <img src=".images/readme/complex_envs.png" width=1000>
 
 
 
-#### Boundary conditions 
+#### **Boundary conditions**
 Boundary conditions (for default square/rectangular environments) can be "periodic" or "solid". Place cells and the motion of the Agent will respect these boundaries accordingly. 
 ```python
 Env = Environment(
     params = {'boundary_conditions':'periodic'} #or 'solid' (default)
 ) 
 ```
 
 <img src=".images/readme/boundary_conditions.png" width=500>
 
-#### 1- or 2-dimensions 
+#### **1- or 2-dimensions**
 `RatInABox` supports 1- or 2-dimensional `Environment`s. Almost all applicable features and plotting functions work in both. The following figure shows 1 minute of exploration of an `Agent` in a 1D environment with periodic boundary conditions spanned by 10 place cells. 
 ```python 
 Env = Environment(
     params = {'dimensionality':'1D'} #or '2D' (default)
 ) 
 ```
 
 <img src=".images/readme/one_dimension.png" width=500>
 
 
 
 ### (ii) `Agent` features
 
-#### Random motion model
+#### **Random motion model**
 By defaut the `Agent` follows a random motion policy.  Random motion is stochastic but smooth. The speed (and rotational speed, if in 2D) of an Agent take constrained random walks governed by Ornstein-Uhlenbeck processes. You can change the means, variance and coherence times of these processes to control the shape of the trajectory. Default parameters are fit to real rat locomotion data from Sargolini et al. (2006): 
 
 <img src=".images/readme/riab_vs_sargolini.gif" width=500>
 
 The default parameters can be changed to obtain different style trajectories. The following set of trajectories were generated by modifying the rotational speed parameter `Agent.rotational_velocity_std`:
 
 ```python
@@ -198,68 +182,76 @@
 Agent.rotation_velocity_std = 120 * np.pi/180 #radians 
 Agent.rotational_velocity_coherence_time = 0.08
 ```
 
 <img src=".images/readme/motion_model.png" width=800>
 
 
-#### Importing trajectories
+#### **Importing trajectories**
 `RatInABox` supports importing external trajectory data (rather than using the in built random motion policy). Imported data can be of low temporal resolution. It will be smoothly upsampled using a cubic splines interpolation technique. We provide a 10 minute trajectory from the open-source data set of Sargolini et al. (2006) ready to import. In the following figure blue shows (low resolution) trajectory data imported into an `Agent` and purple shows the smoothly upsampled trajectory taken by the `Agent` during exploration. 
 ```python
 Agent.import_trajectory(dataset='sargolini')
 #or 
 Agent.import_trajectory(times=array_of_times,
                         positions=array_of_positions)
 
 ```
 
 <img src=".images/readme/imported_trajectory.png" width=200>
 
-#### Policy control 
+#### **Policy control**
 By default the movement policy is an random and uncontrolled (e.g. displayed above). It is possible, however, to manually pass a "drift_velocity" to the Agent on each `Agent.update()` step. This 'closes the loop' allowing, for example, Actor-Critic systems to control the Agent policy. As a demonstration that this method can be used to control the agent's movement we set a radial drift velocity to encourage circular motion. We also use RatInABox to perform a simple model-free RL task and find a reward hidden behind a wall (the full script is given as an example script [here](./demos/reinforcement_learning_example.ipynb))
 ```python
 Agent.update(drift_velocity=drift_velocity)
 ```
 
 <img src=".images/readme/motion.gif" width=600>
 
-#### Wall repelling 
+#### **Wall repelling**
 Under the random motion policy, walls in the environment mildly "repel" the `Agent`. Coupled with the finite turning speed this replicates an effect (known as thigmotaxis, sometimes linked to anxiety) where the `Agent` is biased to over-explore near walls and corners (as shown in these heatmaps) matching real rodent behaviour. It can be turned up or down with the `thigmotaxis` parameter.
 ```python 
 Αgent.thigmotaxis = 0.8 #1 = high thigmotaxis (left plot), 0 = low (right)
 ```
 
 <img src=".images/readme/wall_repel.png" width=900>
 
+#### **Multiple `Agent`s**
+There is nothing to stop multiple `Agent`s being added to the same `Environment`. When plotting/animating trajectories set the kwarg `plot_all_agents=True` to visualise all `Agent`s simultaneously. 
+
+The following animation shows three `Agent`s in an `Environment`. Drift velocities are set so that `Agent`s weally locally attract one another creating "interactive" behaviour.
+
+<img src=".images/readme/multi_agents.gif" width=350>
 
-#### Advanced `Agent` classes
+
+#### **Advanced `Agent` classes**
 One can make more advanced Agent classes, for example `ThetaSequenceAgent()` where the position "sweeps" (blue) over the position of an underlying true (regular) `Agent()` (purple), highly reminiscent of theta sequences observed when one decodes position from the hippocampal populaton code on sub-theta (10 Hz) timescales. This class can be found in the [`contribs`](./ratinabox/contribs/) directory. 
 
 <img src=".images/readme/theta_sequences.gif" width=350>
 
 
 ### (iii) `Neurons` features 
 
-#### Multiple cell types: 
-We provide a list of premade `Neurons` subclasses. These include: 
+#### **Multiple cell types:**
+We provide a list of premade `Neurons` subclasses. These include (but are not limited to): 
 
 * `PlaceCells` 
 * `GridCells`
 * `BoundaryVectorCells` (can be egocentric or allocentric)
 * `ObjectVectorCells` (can be used as visual cues, i.e. only fire when `Agent` is looking towards them)
 * `HeadDirectionCells`
 * `VelocityCells`
 * `SpeedCells`
 * `FeedForwardLayer` - calculates activated weighted sum of inputs from a provide list of input `Neurons` layers.
 * `FieldOfViewNeurons` - Egocentric encoding of what the `Agent` can see 
+* `SuccessorFeatures` - Learns the successor features for a set of features under teh current motion policy
 
-This last class, `FeedForwardLayer` deserves special mention. Instead of its firing rate being determined explicitly by the state of the `Agent` it summates synaptic inputs from a provided list of input layers (which can be any `Neurons` subclass). This layer is the building block for how more complex networks can be studied using `RatInABox`. 
+`FeedForwardLayer` deserves special mention. Instead of its firing rate being determined explicitly by the state of the `Agent` it summates synaptic inputs from a provided list of input layers (which can be any `Neurons` subclass). This layer is the building block for how more complex networks can be studied using `RatInABox`. 
 
 
-#### Noise 
+#### **Noise** 
 Use the `Neurons.noise_std` and `Neurons.noise_coherence_time` parameters to control the amount of noise (Hz) and autocorrelation timescale of the noise (seconds). For example (work with all `Neurons` classes, not just `PlaceCells`): 
 
 ```python
 PCs = PlaceCells(Ag,params={
     'noise_std':0.1, #defaults to 0 i.e. no noise
     'noise_coherence_time':0.5, #autocorrelation timescale of additive noise vector 
 })
@@ -272,27 +264,27 @@
 ```
 Neurons.plot_ratemap(spikes=True)
 ```
 
 <img src=".images/readme/spikes.png" width="1000">
 
 
-#### Rate maps 
+#### **Rate maps**
 `PlaceCells`, `GridCells` and allocentric `BoundaryVectorCells` (among others) have firing rates which depend exclusively on the position of the agent. These rate maps can be displayed by querying their firing rate at an array of positions spanning the environment, then plotting. This process is done for you using the function `Neurons.plot_rate_map()`. 
 
 More generally, however, cells firing is not only determined by position but potentially other factors (e.g. velocity, or historical effects if the layer is part of a recurrent network). In these cases the above method of plotting rate maps will necessarily fail. A more robust way to display the receptive field is to plot a heatmap of the positions of the Agent has visited where each positions contribution to a bin is weighted by the firing rate observed at that position. Over time, as coverage become complete, the firing fields become visible.
 ```
 Neurons.plot_rate_map() #attempts to plot "ground truth" rate map 
 Neurons.plot_rate_map(method="history") #plots rate map by firing-rate-weighted position heatmap
 ``` 
 
 <img src=".images/readme/rate_map.png" width=600>
 
 
-#### Place cell models
+#### **Place cell models**
 
 Place cells come in multiple types (given by `params['description']`), or it would be easy to write your own:
 * `"gaussian"`: normal gaussian place cell 
 * `"gaussian_threshold"`: gaussian thresholded at 1 sigma
 * `"diff_of_gaussians"`: gaussian(sigma) - gaussian(1.5 sigma)
 * `"top_hat"`: circular receptive field, max firing rate within, min firing rate otherwise
 * `"one_hot"`: the closest palce cell to any given location is established. This and only this cell fires. 
@@ -302,21 +294,21 @@
 <img src=".images/readme/placecellmodels.png" width=800>
 
 These place cells (with the exception of `"one_hot"`s) can all be made to phase precess by instead initialising them with the `PhasePrecessingPlaceCells()` class currently residing in the `contribs` folder. This figure shows example output data. 
 
 <img src=".images/readme/phaseprecession.png" width=500>
 
 
-#### Geometry of `PlaceCells` 
+#### **Geometry of `PlaceCells`** 
 Choose how you want `PlaceCells` to interact with walls in the `Environment`. We provide three types of geometries.  
 
 <img src=".images/readme/wall_geometry.png" width=900>
 
 
-#### Egocentric encodings
+#### **Egocentric encodings**
 Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric. `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. With an adequately defined field of view these can make, for example, "whisker cells". 
 
 ```python
 FoV_BVCs = FieldOfViewNeurons(Ag)
 FoV_OVCs = FieldOfViewNeurons(Ag,params={
     'cell_type':'OVC',
     })
@@ -324,37 +316,43 @@
     "FoV_angles":[75,105],
     "FoV_distance":[0.1,0.2],
     "spatial_resolution":0.02,})
 ```
 
 <img src=".images/readme/field_of_view.gif" width=600>
 
+#### **Successor Features and Reinforcement Learning**
+A dedicated `Neurons` class called `SuccessorFeatures` learns the successor features for a given feature set under teh current policy. See [this demo](./demos/successor_features_example.ipynb) for more info. 
+<img src=".images/demos/SF_development.gif" width=600>
+
+`SuccessorFeatures` are a specific instance of a more general class of neurons called `ValueNeuron`s which learn value function for any reward density under the `Agent`s motion policy. This can be used to do reinforcement learning tasks such as finding rewards hidden behind walls etc as shown in [this demo](./demos/reinforcement_learning_example.ipynb). 
 
+Finally, we are working on making an OpenAI `Gym` environment wrapper for `RatInABox`. This should be available soon, keep an eye on [this issue](https://github.com/TomGeorge1234/RatInABox/issues/30). 
 
-#### More complex Neuron types and networks of Neurons
-We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here](./demos/path_integration_example.ipynb) and [here](./demos/reinforcement_learning_example.ipynb). 
+#### **More complex Neuron types and networks of Neurons**
+We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here (path integration)](./demos/path_integration_example.ipynb), [here (reinforcement learning)](./demos/reinforcement_learning_example.ipynb) and [here (successor features)](./demos/successor_features_example.ipynb). 
 
 
 
 ### (iv) Figures and animations 
 `RatInABox` is built to be highly visual. It is easy to plot or animate data and save these plots/animations. Here are some tips
 
-#### Saving
+#### **Saving**
 * `ratinabox.figure_directory` a global variable specifying the directory into which figures/animations will be saved 
 * `ratinabox.utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within the figure directory  as both `".svg"` and `".png"` (`".mp4"` or `".gif"`). The current time will be appended to the `fig_name` so you won't ever overwrite. 
 
 
-#### Saving (but automatically)
+#### **Saving (but automatically)**
 * Setting `ratinabox.autosave_plots = True` means RatInABox figure will be automatically saved in the figure directory without having to indvidually call the `utils` function above. 
 
-#### Styling
+#### **Styling**
 * `ratinabox.stylize_plots()` this call sets some global matplotlib rcParams to make plots look pretty/exactly like they do in this repo
 
 
-#### Most important plotting functions
+#### **Most important plotting functions**
 The most important plotting functions are (see source code for the available arguments/kwargs):
 
 ```python
 Environment.plot_environment() #visualises current environment with walls and objects
 Agent.plot_trajectory() #plots trajectory
 Agent.animate_trajectory() #animate trajectory
 Neurons.plot_rate_map() # plots the rate map of the neurons at all positions
@@ -388,14 +386,15 @@
 ```
 * [extensive_example.ipynb](./demos/extensive_example.ipynb): a more involved tutorial. More complex enivornment, more complex cell types and more complex plots are used. 
 * [list_of_plotting_functions.md](./demos/list_of_plotting_fuctions.md): All the types of plots available for are listed and explained. 
 * [readme_figures.ipynb](./demos/readme_figures.ipynb): (Almost) all plots/animations shown in the root readme are produced from this script (plus some minor formatting done afterwards in powerpoint).
 * [paper_figures.ipynb](./demos/paper_figures.ipynb): (Almost) all plots/animations shown in the paper are produced from this script (plus some major formatting done afterwards in powerpoint).
 * [decoding_position_example.ipynb](./demos/decoding_position_example.ipynb): Postion is decoded from neural data generated with RatInABox. Place cells, grid cell and boundary vector cells are compared. 
 * [reinforcement_learning_example.ipynb](./demos/reinforcement_learning_example.ipynb): RatInABox is use to construct, train and visualise a small two-layer network capable of model free reinforcement learning in order to find a reward hidden behind a wall. 
+* [successor_features_example.ipynb](./successor_features_example.ipynb): RatInABox is use to learn and visualise successor features under random and biased motion policies.
 * [path_integration_example.ipynb](./demos/path_integration_example.ipynb): RatInABox is use to construct, train and visualise a large multi-layer network capable of learning a "ring attractor" capable of path integrating a position estimate using only velocity inputs.
 
 ## Contribute 
 `RatInABox` is an open source project, and we actively encourage community contributions, for example bug fixes, new cells types, new features, new plotting functions, new motion datasets, documentation, citations of relevant work, or additional experiment notebooks. Typically the best way to go about this is by opening an issue or feel free to make a pull request. 
 
 We have a dedicated [contribs](./ratinabox/contribs/) directory where you can safely add awesome scripts and new `Neurons` classes etc.
 
@@ -418,8 +417,8 @@
 }
 ```
 
 Formatted:
 ```
 Tom M George, William de Cothi, Claudia Clopath, Kimberly Stachenfeld, Caswell Barry. "RatInABox: A toolkit for modelling locomotion and neuronal activity in continuous environments" (2022).
 ``` 
-The research paper corresponding to the above citation can be found [here](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3).
+The research paper corresponding to the above citation can be found [here](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3).
```

### Comparing `ratinabox-1.5.1/README.md` & `ratinabox-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: ratinabox
+Version: 1.6.0
+Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
+Author: Tom George
+Author-email: tomgeorge1@btinternet.com
+License: MIT
+Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
+Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
+Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
+Platform: any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # RatInABox 
 ![Tests](https://github.com/TomGeorge1234/RatInABox/actions/workflows/test.yml/badge.svg)   [![PyPI version](https://badge.fury.io/py/ratinabox.svg)](https://badge.fury.io/py/ratinabox) [![Downloads](https://static.pepy.tech/badge/ratinabox)](https://pepy.tech/project/ratinabox)
 
 `RatInABox` (see [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3)) is a toolkit for generating locomotion trajectories and complementary neural data for spatially and/or velocity selective cell types in complex continuous environments. 
 
 [**Install**](#installing-and-importing) | [**Demos**](#get-started) | [**Features**](#feature-run-down) | [**Contributions and Questions**](#contribute) | [**Cite**](#cite)
 
@@ -22,14 +41,15 @@
     * `GridCells`
     * `BoundaryVectorCells` (egocentric or allocentric)
     * `ObjectVectorCells`
     * `VelocityCells`
     * `SpeedCells`
     * `HeadDirectionCells`
     * `FeedForwardLayer` (a generic class analagous to a feedforward layer in a deep neural network)
+    * `SuccessorFeatures` 
     * ...
 
 The top animation shows an example use case: an `Agent` randomly explores a 2D `Environment` with a wall. Three populations of `Neurons` (`PlaceCells`, `GridCells`, `BoundaryVectorCells`) fire according to the receptive fields shown. All data is saved into the history for downstream use. `RatInABox` is fully continuous is space; this means that position and neuronal firing rates are calculated rapidly online with float precision rather than pre-calculated over a discretised mesh. `RatInABox` is flexibly discretised in time; `dt` can be set by the user (defaulting to 10 ms) depending on requirements.
 
 
 ## Key features
 * **Non-specific**: Trajectories can be randomly generated, imported, or adaptively controlled making `RatInABox` a powerful engine for many tasks involving continuous motion (e.g. control theory or [reinforcement learning](#policy-control)). 
@@ -78,44 +98,46 @@
 * [1- or 2-dimensions](#1--or-2-dimensions) 
 
 (ii) the [`Agent`](#ii-agent-features)
 * [Random motion](#random-motion-model)
 * [Importing trajectories](#importing-trajectories)
 * [Policy control](#policy-control)
 * [Wall repelling](#wall-repelling)
+* [Multiple Agents](#multiple-agents)
 * [Advanced `Agent` classes](#advanced-agent-classes)
 
 (iii) the [`Neurons`](#iii-neurons-features).
 * [Cell types](#multiple-cell-types) 
 * [Noise](#noise)
 * [Spikes vs rates](#spiking)
 * [Plotting rate maps](#rate-maps)
 * [Place cell models](#place-cell-models) 
 * [Place cell geometry](#geometry-of-placecells)
 * [Egocentric encodings](#egocentric-encodings)
+* [Successor features and reinforcement learning](#successor-features-and-reinforcement-learning)
 * [Deep neural networks](#more-complex-neuron-types-and-networks-of-neurons)
 
 (iv) [Figures and animations plotting](#iv-figures-and-animations)
 
 Specific details can be found in the [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3). 
 
 
 
 ### (i) `Environment` features
-#### Walls 
+#### **Walls**
 Arbitrarily add walls to the environment to produce arbitrarily complex mazes:
 ```python 
 Environment.add_wall([[x0,y0],[x1,y1]])
 ```
 Here are some easy to make examples.
 
 <img src=".images/readme/walls.png" width=1000>
 
 
-#### Complex `Environment`s: Polygons, curves, and holes
+#### **Complex `Environment`s: Polygons, curves, and holes**
 By default, `Environments` in RatInABox are square (or rectangular if `aspect != 1`). It is possible to create arbitrary environment shapes using the `"boundary"` parameter at initialisation. 
 
 One can all add holes to the `Environment` using the `"holes"` parameter at initialisation. Positions sampled from the Environment (e.g. at initialisation) won't be inside holes.
 
 Any curved environments can be made by creating a boundary of many small walls (uyse sparingly, walls may slow down computations)
 
 ```python 
@@ -138,39 +160,39 @@
 ```
 
 
 <img src=".images/readme/complex_envs.png" width=1000>
 
 
 
-#### Boundary conditions 
+#### **Boundary conditions**
 Boundary conditions (for default square/rectangular environments) can be "periodic" or "solid". Place cells and the motion of the Agent will respect these boundaries accordingly. 
 ```python
 Env = Environment(
     params = {'boundary_conditions':'periodic'} #or 'solid' (default)
 ) 
 ```
 
 <img src=".images/readme/boundary_conditions.png" width=500>
 
-#### 1- or 2-dimensions 
+#### **1- or 2-dimensions**
 `RatInABox` supports 1- or 2-dimensional `Environment`s. Almost all applicable features and plotting functions work in both. The following figure shows 1 minute of exploration of an `Agent` in a 1D environment with periodic boundary conditions spanned by 10 place cells. 
 ```python 
 Env = Environment(
     params = {'dimensionality':'1D'} #or '2D' (default)
 ) 
 ```
 
 <img src=".images/readme/one_dimension.png" width=500>
 
 
 
 ### (ii) `Agent` features
 
-#### Random motion model
+#### **Random motion model**
 By defaut the `Agent` follows a random motion policy.  Random motion is stochastic but smooth. The speed (and rotational speed, if in 2D) of an Agent take constrained random walks governed by Ornstein-Uhlenbeck processes. You can change the means, variance and coherence times of these processes to control the shape of the trajectory. Default parameters are fit to real rat locomotion data from Sargolini et al. (2006): 
 
 <img src=".images/readme/riab_vs_sargolini.gif" width=500>
 
 The default parameters can be changed to obtain different style trajectories. The following set of trajectories were generated by modifying the rotational speed parameter `Agent.rotational_velocity_std`:
 
 ```python
@@ -179,68 +201,76 @@
 Agent.rotation_velocity_std = 120 * np.pi/180 #radians 
 Agent.rotational_velocity_coherence_time = 0.08
 ```
 
 <img src=".images/readme/motion_model.png" width=800>
 
 
-#### Importing trajectories
+#### **Importing trajectories**
 `RatInABox` supports importing external trajectory data (rather than using the in built random motion policy). Imported data can be of low temporal resolution. It will be smoothly upsampled using a cubic splines interpolation technique. We provide a 10 minute trajectory from the open-source data set of Sargolini et al. (2006) ready to import. In the following figure blue shows (low resolution) trajectory data imported into an `Agent` and purple shows the smoothly upsampled trajectory taken by the `Agent` during exploration. 
 ```python
 Agent.import_trajectory(dataset='sargolini')
 #or 
 Agent.import_trajectory(times=array_of_times,
                         positions=array_of_positions)
 
 ```
 
 <img src=".images/readme/imported_trajectory.png" width=200>
 
-#### Policy control 
+#### **Policy control**
 By default the movement policy is an random and uncontrolled (e.g. displayed above). It is possible, however, to manually pass a "drift_velocity" to the Agent on each `Agent.update()` step. This 'closes the loop' allowing, for example, Actor-Critic systems to control the Agent policy. As a demonstration that this method can be used to control the agent's movement we set a radial drift velocity to encourage circular motion. We also use RatInABox to perform a simple model-free RL task and find a reward hidden behind a wall (the full script is given as an example script [here](./demos/reinforcement_learning_example.ipynb))
 ```python
 Agent.update(drift_velocity=drift_velocity)
 ```
 
 <img src=".images/readme/motion.gif" width=600>
 
-#### Wall repelling 
+#### **Wall repelling**
 Under the random motion policy, walls in the environment mildly "repel" the `Agent`. Coupled with the finite turning speed this replicates an effect (known as thigmotaxis, sometimes linked to anxiety) where the `Agent` is biased to over-explore near walls and corners (as shown in these heatmaps) matching real rodent behaviour. It can be turned up or down with the `thigmotaxis` parameter.
 ```python 
 Αgent.thigmotaxis = 0.8 #1 = high thigmotaxis (left plot), 0 = low (right)
 ```
 
 <img src=".images/readme/wall_repel.png" width=900>
 
+#### **Multiple `Agent`s**
+There is nothing to stop multiple `Agent`s being added to the same `Environment`. When plotting/animating trajectories set the kwarg `plot_all_agents=True` to visualise all `Agent`s simultaneously. 
+
+The following animation shows three `Agent`s in an `Environment`. Drift velocities are set so that `Agent`s weally locally attract one another creating "interactive" behaviour.
+
+<img src=".images/readme/multi_agents.gif" width=350>
 
-#### Advanced `Agent` classes
+
+#### **Advanced `Agent` classes**
 One can make more advanced Agent classes, for example `ThetaSequenceAgent()` where the position "sweeps" (blue) over the position of an underlying true (regular) `Agent()` (purple), highly reminiscent of theta sequences observed when one decodes position from the hippocampal populaton code on sub-theta (10 Hz) timescales. This class can be found in the [`contribs`](./ratinabox/contribs/) directory. 
 
 <img src=".images/readme/theta_sequences.gif" width=350>
 
 
 ### (iii) `Neurons` features 
 
-#### Multiple cell types: 
-We provide a list of premade `Neurons` subclasses. These include: 
+#### **Multiple cell types:**
+We provide a list of premade `Neurons` subclasses. These include (but are not limited to): 
 
 * `PlaceCells` 
 * `GridCells`
 * `BoundaryVectorCells` (can be egocentric or allocentric)
 * `ObjectVectorCells` (can be used as visual cues, i.e. only fire when `Agent` is looking towards them)
 * `HeadDirectionCells`
 * `VelocityCells`
 * `SpeedCells`
 * `FeedForwardLayer` - calculates activated weighted sum of inputs from a provide list of input `Neurons` layers.
 * `FieldOfViewNeurons` - Egocentric encoding of what the `Agent` can see 
+* `SuccessorFeatures` - Learns the successor features for a set of features under teh current motion policy
 
-This last class, `FeedForwardLayer` deserves special mention. Instead of its firing rate being determined explicitly by the state of the `Agent` it summates synaptic inputs from a provided list of input layers (which can be any `Neurons` subclass). This layer is the building block for how more complex networks can be studied using `RatInABox`. 
+`FeedForwardLayer` deserves special mention. Instead of its firing rate being determined explicitly by the state of the `Agent` it summates synaptic inputs from a provided list of input layers (which can be any `Neurons` subclass). This layer is the building block for how more complex networks can be studied using `RatInABox`. 
 
 
-#### Noise 
+#### **Noise** 
 Use the `Neurons.noise_std` and `Neurons.noise_coherence_time` parameters to control the amount of noise (Hz) and autocorrelation timescale of the noise (seconds). For example (work with all `Neurons` classes, not just `PlaceCells`): 
 
 ```python
 PCs = PlaceCells(Ag,params={
     'noise_std':0.1, #defaults to 0 i.e. no noise
     'noise_coherence_time':0.5, #autocorrelation timescale of additive noise vector 
 })
@@ -253,27 +283,27 @@
 ```
 Neurons.plot_ratemap(spikes=True)
 ```
 
 <img src=".images/readme/spikes.png" width="1000">
 
 
-#### Rate maps 
+#### **Rate maps**
 `PlaceCells`, `GridCells` and allocentric `BoundaryVectorCells` (among others) have firing rates which depend exclusively on the position of the agent. These rate maps can be displayed by querying their firing rate at an array of positions spanning the environment, then plotting. This process is done for you using the function `Neurons.plot_rate_map()`. 
 
 More generally, however, cells firing is not only determined by position but potentially other factors (e.g. velocity, or historical effects if the layer is part of a recurrent network). In these cases the above method of plotting rate maps will necessarily fail. A more robust way to display the receptive field is to plot a heatmap of the positions of the Agent has visited where each positions contribution to a bin is weighted by the firing rate observed at that position. Over time, as coverage become complete, the firing fields become visible.
 ```
 Neurons.plot_rate_map() #attempts to plot "ground truth" rate map 
 Neurons.plot_rate_map(method="history") #plots rate map by firing-rate-weighted position heatmap
 ``` 
 
 <img src=".images/readme/rate_map.png" width=600>
 
 
-#### Place cell models
+#### **Place cell models**
 
 Place cells come in multiple types (given by `params['description']`), or it would be easy to write your own:
 * `"gaussian"`: normal gaussian place cell 
 * `"gaussian_threshold"`: gaussian thresholded at 1 sigma
 * `"diff_of_gaussians"`: gaussian(sigma) - gaussian(1.5 sigma)
 * `"top_hat"`: circular receptive field, max firing rate within, min firing rate otherwise
 * `"one_hot"`: the closest palce cell to any given location is established. This and only this cell fires. 
@@ -283,21 +313,21 @@
 <img src=".images/readme/placecellmodels.png" width=800>
 
 These place cells (with the exception of `"one_hot"`s) can all be made to phase precess by instead initialising them with the `PhasePrecessingPlaceCells()` class currently residing in the `contribs` folder. This figure shows example output data. 
 
 <img src=".images/readme/phaseprecession.png" width=500>
 
 
-#### Geometry of `PlaceCells` 
+#### **Geometry of `PlaceCells`** 
 Choose how you want `PlaceCells` to interact with walls in the `Environment`. We provide three types of geometries.  
 
 <img src=".images/readme/wall_geometry.png" width=900>
 
 
-#### Egocentric encodings
+#### **Egocentric encodings**
 Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric. `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. With an adequately defined field of view these can make, for example, "whisker cells". 
 
 ```python
 FoV_BVCs = FieldOfViewNeurons(Ag)
 FoV_OVCs = FieldOfViewNeurons(Ag,params={
     'cell_type':'OVC',
     })
@@ -305,37 +335,43 @@
     "FoV_angles":[75,105],
     "FoV_distance":[0.1,0.2],
     "spatial_resolution":0.02,})
 ```
 
 <img src=".images/readme/field_of_view.gif" width=600>
 
+#### **Successor Features and Reinforcement Learning**
+A dedicated `Neurons` class called `SuccessorFeatures` learns the successor features for a given feature set under teh current policy. See [this demo](./demos/successor_features_example.ipynb) for more info. 
+<img src=".images/demos/SF_development.gif" width=600>
+
+`SuccessorFeatures` are a specific instance of a more general class of neurons called `ValueNeuron`s which learn value function for any reward density under the `Agent`s motion policy. This can be used to do reinforcement learning tasks such as finding rewards hidden behind walls etc as shown in [this demo](./demos/reinforcement_learning_example.ipynb). 
 
+Finally, we are working on making an OpenAI `Gym` environment wrapper for `RatInABox`. This should be available soon, keep an eye on [this issue](https://github.com/TomGeorge1234/RatInABox/issues/30). 
 
-#### More complex Neuron types and networks of Neurons
-We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here](./demos/path_integration_example.ipynb) and [here](./demos/reinforcement_learning_example.ipynb). 
+#### **More complex Neuron types and networks of Neurons**
+We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here (path integration)](./demos/path_integration_example.ipynb), [here (reinforcement learning)](./demos/reinforcement_learning_example.ipynb) and [here (successor features)](./demos/successor_features_example.ipynb). 
 
 
 
 ### (iv) Figures and animations 
 `RatInABox` is built to be highly visual. It is easy to plot or animate data and save these plots/animations. Here are some tips
 
-#### Saving
+#### **Saving**
 * `ratinabox.figure_directory` a global variable specifying the directory into which figures/animations will be saved 
 * `ratinabox.utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within the figure directory  as both `".svg"` and `".png"` (`".mp4"` or `".gif"`). The current time will be appended to the `fig_name` so you won't ever overwrite. 
 
 
-#### Saving (but automatically)
+#### **Saving (but automatically)**
 * Setting `ratinabox.autosave_plots = True` means RatInABox figure will be automatically saved in the figure directory without having to indvidually call the `utils` function above. 
 
-#### Styling
+#### **Styling**
 * `ratinabox.stylize_plots()` this call sets some global matplotlib rcParams to make plots look pretty/exactly like they do in this repo
 
 
-#### Most important plotting functions
+#### **Most important plotting functions**
 The most important plotting functions are (see source code for the available arguments/kwargs):
 
 ```python
 Environment.plot_environment() #visualises current environment with walls and objects
 Agent.plot_trajectory() #plots trajectory
 Agent.animate_trajectory() #animate trajectory
 Neurons.plot_rate_map() # plots the rate map of the neurons at all positions
@@ -369,14 +405,15 @@
 ```
 * [extensive_example.ipynb](./demos/extensive_example.ipynb): a more involved tutorial. More complex enivornment, more complex cell types and more complex plots are used. 
 * [list_of_plotting_functions.md](./demos/list_of_plotting_fuctions.md): All the types of plots available for are listed and explained. 
 * [readme_figures.ipynb](./demos/readme_figures.ipynb): (Almost) all plots/animations shown in the root readme are produced from this script (plus some minor formatting done afterwards in powerpoint).
 * [paper_figures.ipynb](./demos/paper_figures.ipynb): (Almost) all plots/animations shown in the paper are produced from this script (plus some major formatting done afterwards in powerpoint).
 * [decoding_position_example.ipynb](./demos/decoding_position_example.ipynb): Postion is decoded from neural data generated with RatInABox. Place cells, grid cell and boundary vector cells are compared. 
 * [reinforcement_learning_example.ipynb](./demos/reinforcement_learning_example.ipynb): RatInABox is use to construct, train and visualise a small two-layer network capable of model free reinforcement learning in order to find a reward hidden behind a wall. 
+* [successor_features_example.ipynb](./successor_features_example.ipynb): RatInABox is use to learn and visualise successor features under random and biased motion policies.
 * [path_integration_example.ipynb](./demos/path_integration_example.ipynb): RatInABox is use to construct, train and visualise a large multi-layer network capable of learning a "ring attractor" capable of path integrating a position estimate using only velocity inputs.
 
 ## Contribute 
 `RatInABox` is an open source project, and we actively encourage community contributions, for example bug fixes, new cells types, new features, new plotting functions, new motion datasets, documentation, citations of relevant work, or additional experiment notebooks. Typically the best way to go about this is by opening an issue or feel free to make a pull request. 
 
 We have a dedicated [contribs](./ratinabox/contribs/) directory where you can safely add awesome scripts and new `Neurons` classes etc.
 
@@ -399,8 +436,8 @@
 }
 ```
 
 Formatted:
 ```
 Tom M George, William de Cothi, Claudia Clopath, Kimberly Stachenfeld, Caswell Barry. "RatInABox: A toolkit for modelling locomotion and neuronal activity in continuous environments" (2022).
 ``` 
-The research paper corresponding to the above citation can be found [here](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3).
+The research paper corresponding to the above citation can be found [here](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3).
```

### Comparing `ratinabox-1.5.1/ratinabox/Agent.py` & `ratinabox-1.6.0/ratinabox/Agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,17 @@
         """Initialise Agent, takes as input a parameter dictionary.
         Any values not provided by the params dictionary are taken from a default dictionary below.
 
         Args:
             params (dict, optional). Defaults to {}.
         """
         self.Environment = Environment
+        self.Environment.Agents.append(self)
 
-        self.params = copy.deepcopy(__class__.default_params)        
+        self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         utils.update_class_params(self, self.params, get_all_defaults=True)
         utils.check_params(self, params.keys())
 
         # initialise history dataframes
         self.history = {}
@@ -564,138 +565,149 @@
     def plot_trajectory(
         self,
         t_start=0,
         t_end=None,
         framerate=10,
         fig=None,
         ax=None,
+        plot_all_agents=False,
         point_size=15,
         decay_point_size=False,
         decay_point_timescale=10,
         plot_agent=True,
-        color="#7b699a",
+        color=None,
         alpha=0.7,
         xlim=None,
         background_color=None,
         axis_labels=True,
         autosave=None,
         **kwargs,
     ):
         """Plots the trajectory between t_start (seconds) and t_end (defaulting to the last time available)
         Args:
             • t_start: start time in seconds
             • t_end: end time in seconds (default = self.history["t"][-1])
             • framerate: how many scatter points / per second of motion to display
             • fig, ax: the fig, ax to plot on top of, optional, if not provided used self.Environment.plot_Environment().
               This can be used to plot trajectory on top of receptive fields etc.
+            • plot_all_agents: if True, this will plot the trajectory of all agents in the list Environment.Agents
             • point_size: size of scatter points
             • decay_point_size: decay trajectory point size over time (recent times = largest)
             • decay_point_timescale: if decay_point_size is True, this is the timescale over which sizes decay
             • plot_agent: dedicated point show agent current position
             • color: plot point color, if color == 'changing' will smoothly change trajectory color from start to finish
             • alpha: plot point opaqness
             • xlim: In 1D, forces the xlim to be a certain time (minutes) (useful if animating this function)
             • background_color: color of the background if not matplotlib default, only for 1D (probably white)
             • axis_labels: whether to show axes labels
             • autosave: if True, will try to save the figure to the figure directory `ratinabox.figure_directory`. Defaults to None in which case looks for global constant ratinabox.autosave_plots
 
         Returns:
             fig, ax
         """
-
-        dt = self.dt
-        t, pos = np.array(self.history["t"]), np.array(self.history["pos"])
-        if t_end == None:
-            t_end = t[-1]
-        startid = np.nanargmin(np.abs(t - (t_start)))
-        endid = np.nanargmin(np.abs(t - (t_end)))
-        if self.Environment.dimensionality == "2D":
-            skiprate = max(1, int((1 / framerate) / dt))
-            trajectory = pos[startid:endid, :][::skiprate]
-        if self.Environment.dimensionality == "1D":
-            skiprate = max(1, int((1 / framerate) / dt))
-            trajectory = pos[startid:endid][::skiprate]
-        time = t[startid:endid][::skiprate]
-        if color is None:
-            color = ["C0"] * len(time)
-        elif color == "changing":
-            trajectory_cmap = matplotlib.colormaps["viridis_r"]
-            color = [trajectory_cmap(t / len(time)) for t in range(len(time))]
-            decay_point_size = (
-                False  # if changing colour, may as well show WHOLE trajectory
-            )
+        # loop over all agents in the Environment if plot_all_agents is True
+        if plot_all_agents == False:
+            agent_list = [self]
+            if color is None:
+                color = "#7b699a"
         else:
-            color = [color] * len(time)
-
-        if self.Environment.dimensionality == "2D":
-            fig, ax = self.Environment.plot_environment(fig=fig, ax=ax, autosave=False)
-            s = point_size * np.ones_like(time)
-            if decay_point_size == True:
-                s = point_size * np.exp((time - time[-1]) / decay_point_timescale)
-                s[(time[-1] - time) > (1.5 * decay_point_timescale)] *= 0
-
-            if plot_agent == True:
-                s[-1] = 40
-                color[-1] = "r"
-
-            ax.scatter(
-                trajectory[:, 0],
-                trajectory[:, 1],
-                s=s,
-                alpha=alpha,
-                zorder=1.1,
-                c=color,
-                linewidth=0,
-            )
-            # #plot the rat? TODO haha probably never gonna do this
-            # ratpath = os.path.join(
-            #     os.path.abspath(os.path.join(ratinabox.__file__, os.pardir)),
-            #         "data/rat.png",
-            #     )
-            # rat = plt.imread(ratpath)
-            # rect = 0.5, 0.4, 0.4, 0.4 # What should these values be?
-            # newax = fig.add_axes(rect, anchor='NE', zorder=1)
-            # newax.axis('off')
-            # newax.imshow(rat)
+            agent_list = self.Environment.Agents
+        replot_env = True
+        for i, self_ in enumerate(agent_list):
+            dt = self_.dt
+            t, pos = np.array(self_.history["t"]), np.array(self_.history["pos"])
+            if t_end == None:
+                t_end = t[-1]
+            startid = np.nanargmin(np.abs(t - (t_start)))
+            endid = np.nanargmin(np.abs(t - (t_end)))
+            if self_.Environment.dimensionality == "2D":
+                skiprate = max(1, int((1 / framerate) / dt))
+                trajectory = pos[startid:endid, :][::skiprate]
+            if self_.Environment.dimensionality == "1D":
+                skiprate = max(1, int((1 / framerate) / dt))
+                trajectory = pos[startid:endid][::skiprate]
+            time = t[startid:endid][::skiprate]
+            if color is None:
+                color_list = [f"C{i}"] * len(time)
+            elif color == "changing":
+                trajectory_cmap = matplotlib.colormaps["viridis_r"]
+                color_list = [trajectory_cmap(t / len(time)) for t in range(len(time))]
+                decay_point_size = (
+                    False  # if changing colour, may as well show WHOLE trajectory
+                )
+            else:
+                color_list = [color] * len(time)
 
-        if self.Environment.dimensionality == "1D":
-            if fig is None and ax is None:
-                fig, ax = plt.subplots(figsize=(3, 1.5))
-            ax.scatter(time / 60, trajectory, alpha=alpha, linewidth=0, c=color, s=5)
-            ax.spines["left"].set_position(("data", t_start / 60))
-            if axis_labels == True:
-                ax.set_xlabel("Time / min")
-                ax.set_ylabel("Position / m")
-            ax.set_xlim([t_start / 60, t_end / 60])
-            if xlim is not None:
-                ax.set_xlim(right=xlim)
-
-            ax.set_ylim(bottom=0, top=self.Environment.extent[1])
-            ax.spines["right"].set_color(None)
-            ax.spines["top"].set_color(None)
-            ax.set_xticks([t_start / 60, t_end / 60])
-            ex = self.Environment.extent
-            ax.set_yticks([ex[1]])
-            if background_color is not None:
-                ax.set_facecolor(background_color)
-                fig.patch.set_facecolor(background_color)
+            if self_.Environment.dimensionality == "2D":
+                if replot_env == True:
+                    fig, ax = self_.Environment.plot_environment(
+                        fig=fig, ax=ax, autosave=False
+                    )
+                replot_env = False
+                s = point_size * np.ones_like(time)
+                if decay_point_size == True:
+                    s = point_size * np.exp((time - time[-1]) / decay_point_timescale)
+                    s[(time[-1] - time) > (1.5 * decay_point_timescale)] *= 0
+
+                if plot_agent == True:
+                    s[-1] = 40
+                    color_list[-1] = "r"
+
+                ax.scatter(
+                    trajectory[:, 0],
+                    trajectory[:, 1],
+                    s=s,
+                    alpha=alpha,
+                    zorder=1.1,
+                    c=color_list,
+                    linewidth=0,
+                )
+                # #plot the rat? TODO haha probably never gonna do this
+                # ratpath = os.path.join(
+                #     os.path.abspath(os.path.join(ratinabox.__file__, os.pardir)),
+                #         "data/rat.png",
+                #     )
+                # rat = plt.imread(ratpath)
+                # rect = 0.5, 0.4, 0.4, 0.4 # What should these values be?
+                # newax = fig.add_axes(rect, anchor='NE', zorder=1)
+                # newax.axis('off')
+                # newax.imshow(rat)
+
+            if self_.Environment.dimensionality == "1D":
+                if fig is None and ax is None:
+                    fig, ax = plt.subplots(figsize=(3, 1.5))
+                ax.scatter(
+                    time / 60, trajectory, alpha=alpha, linewidth=0, c=color_list, s=5
+                )
+                ax.spines["left"].set_position(("data", t_start / 60))
+                if axis_labels == True:
+                    ax.set_xlabel("Time / min")
+                    ax.set_ylabel("Position / m")
+                ax.set_xlim([t_start / 60, t_end / 60])
+                if xlim is not None:
+                    ax.set_xlim(right=xlim)
+
+                ax.set_ylim(bottom=0, top=self_.Environment.extent[1])
+                ax.spines["right"].set_color(None)
+                ax.spines["top"].set_color(None)
+                ax.set_xticks([t_start / 60, t_end / 60])
+                ex = self_.Environment.extent
+                ax.set_yticks([ex[1]])
+                if background_color is not None:
+                    ax.set_facecolor(background_color)
+                    fig.patch.set_facecolor(background_color)
 
         ratinabox.utils.save_figure(fig, "trajectory", save=autosave)
 
         return fig, ax
 
     def animate_trajectory(
         self, t_start=None, t_end=None, fps=15, speed_up=1, autosave=None, **kwargs
     ):
         """Returns an animation (anim) of the trajectory, 25fps.
-        Should be saved using command like
-            >>> anim.save("./where_to_save/animations.gif",dpi=300)
-        To display in jupyter notebook, call it:
-            >>> anim
-
         Args:
             t_start: Agent time at which to start animation
             t_end (_type_, optional): _description_. Defaults to None.
             fps: frames per second of end video
             speed_up: #times real speed animation should come out at
             autosave (bool): whether to automatical try and save this. Defaults to None in which case looks for global constant ratinabox.autosave_plots
             kwargs: passed to trajectory plotting function (chuck anything you wish in here). A particularly useful kwarg is 'additional_plot_func': any function which takes a fig, ax and t as input. The animation wll be passed through this each time after plotting the trajectory, use it to modify your animations however you like
```

### Comparing `ratinabox-1.5.1/ratinabox/Environment.py` & `ratinabox-1.6.0/ratinabox/Environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
             self.objects = {
                 "objects": np.empty((0, 2)),
                 "object_types": np.empty(0, int),
             }
             self.n_object_types = 0
             self.object_colormap = "rainbow"
             self.plot_objects = True
+            self.Agents = [] #each new Agent will append itself to this list
 
             # make some other attributes
             left = min([c[0] for c in b])
             right = max([c[0] for c in b])
             bottom = min([c[1] for c in b])
             top = max([c[1] for c in b])
             self.centre = np.array([(left + right) / 2, (top + bottom) / 2])
```

### Comparing `ratinabox-1.5.1/ratinabox/Neurons.py` & `ratinabox-1.6.0/ratinabox/Neurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ratinabox
 
 import copy
+import warnings
 import pprint
 import numpy as np
 import matplotlib
 from matplotlib import pyplot as plt
 import scipy
 from scipy import stats as stats
 
@@ -355,15 +356,21 @@
             from mpl_toolkits.axes_grid1 import ImageGrid
 
             if fig is None and ax is None:
                 if shape is None:
                     Nx, Ny = 1, len(chosen_neurons)
                 else:
                     Nx, Ny = shape[0], shape[1]
-                fig = plt.figure(figsize=(2 * Ny, 2 * Nx))
+                env_fig, env_ax = self.Agent.Environment.plot_environment(
+                    autosave=False
+                )
+                width, height = env_fig.get_size_inches()
+                plt.close(env_fig)
+                plt.show
+                fig = plt.figure(figsize=(height * Ny, width * Nx))
                 if colorbar == True and (method in ["groundtruth", "history"]):
                     cbar_mode = "single"
                 else:
                     cbar_mode = None
                 axes = ImageGrid(
                     fig,
                     # (0, 0, 3, 3),
@@ -811,14 +818,22 @@
             s=15,
             zorder=2,
         )
         ratinabox.utils.save_figure(fig, "place_cell_locations", save=autosave)
 
         return fig, ax
 
+    def remap(self):
+        """Resets the place cell centres to a new random distribution. These will be uniformly randomly distributed in the environment (i.e. they will still approximately span the space)"""
+        self.place_cell_centres = self.Agent.Environment.sample_positions(
+            n=self.n, method="uniform_jitter"
+        )
+        np.random.shuffle(self.place_cell_centres)
+        return
+
 
 class GridCells(Neurons):
     """The GridCells class defines a population of GridCells. This class is a subclass of Neurons() and inherits it properties/plotting functions.
 
     Must be initialised with an Agent and a 'params' dictionary.
 
     GridCells defines a set of 'n' grid cells with random orientations, grid scales and offsets (these can be set non-randomly of coursse). Grids are modelled as the rectified sum of three cosine waves at 60 degrees to each other.
@@ -1722,14 +1737,22 @@
         self.Agent = Agent
 
         self.params = copy.deepcopy(__class__.default_params)
         self.params.update(params)
 
         super().__init__(Agent, self.params)
 
+        assert isinstance(
+            self.input_layers, list
+        ), "param['input_layers'] must be a list."
+        if len(self.input_layers) == 0:
+            warnings.warn(
+                "No input layers have been provided. Either hand them in in the params dictionary params['input_layers']=[list,of,inputs] or use self.add_input_layer() to add them manually."
+            )
+
         self.inputs = {}
         for input_layer in self.input_layers:
             self.add_input(input_layer)
 
         if self.biases is None:
             self.biases = np.zeros(self.n)
 
@@ -1760,21 +1783,22 @@
             w = np.random.normal(
                 loc=0, scale=w_init_scale / np.sqrt(n), size=(self.n, n)
             )
         I = np.zeros(n)
         if name in self.inputs.keys():
             if ratinabox.verbose is True:
                 print(
-                    f"There already exists a layer called {name}. Overwriting it now."
+                    f"There already exists a layer called {name}. This may be because you have two input players with the same attribute `InputLayer.name`. Overwriting it now."
                 )
         self.inputs[name] = {}
         self.inputs[name]["layer"] = input_layer
         self.inputs[name]["w"] = w
         self.inputs[name]["w_init"] = w.copy()
         self.inputs[name]["I"] = I
+        self.inputs[name]["n"] = input_layer.n  # a copy for convenience
         for key, value in kwargs.items():
             self.inputs[name][key] = value
         if ratinabox.verbose is True:
             print(
                 f'An input layer called {name} was added. The weights can be accessed with "self.inputs[{name}]["w"]"'
             )
```

### Comparing `ratinabox-1.5.1/ratinabox/README.md` & `ratinabox-1.6.0/ratinabox/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/__init__.py` & `ratinabox-1.6.0/ratinabox/__init__.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/FieldOfViewNeurons.py` & `ratinabox-1.6.0/ratinabox/contribs/FieldOfViewNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/PhasePrecessingPlaceCells.py` & `ratinabox-1.6.0/ratinabox/contribs/PhasePrecessingPlaceCells.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/PlaneWaveNeurons.py` & `ratinabox-1.6.0/ratinabox/contribs/PlaneWaveNeurons.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/README.md` & `ratinabox-1.6.0/ratinabox/contribs/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/STDPFeedForwardLayer.py` & `ratinabox-1.6.0/ratinabox/contribs/STDPFeedForwardLayer.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/ThetaSequenceAgent.py` & `ratinabox-1.6.0/ratinabox/contribs/ThetaSequenceAgent.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/contribs/ValueNeuron.py` & `ratinabox-1.6.0/ratinabox/contribs/ValueNeuron.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,103 +11,105 @@
     """
     Contributer: Tom George tomgeorge1@btinternet.com
 
     The ValueNeuron class defines neuron(s) which learns the "value" of a policy using TD learning. For n > 1 the reward function is assumed to be multidimensional and n value functions (one neuron for each reward function) will be learned under the current policy.  
 
     The true value function, V, is approximated, \hat{V}, as a non-linearly activated (default relu) linear sum of input features (i.e. one layer neural network, in later classes we may generalise this):
 
-    V_i(x) = \int_{t}^{\infty}e^{-\frac{t^{\prime}-t}{\tau}}R_(x(t^{\prime}))) dt^{\prime} | x(t) = x    \\
-    \hat{V}_i(x) \approx \psi_{nonlinearity} ( \w_{ij} \cdot \phi_j(x) )
+    V_i(x) = \int_{t}^{\infty}e^{-\frac{t^{\prime}-t}{\tau}}R_i(x(t^{\prime}))) dt^{\prime} | x(t) = x    \\
+    \hat{V}_i(x) \approx \sigma_{nonlinearity} ( \w_{ij} \cdot \phi_j(x) )
 
     For this we calculate the (temporally continuous) temporal difference error and apply it to the weights:
     
     td_error(t) = R(t) + dV(t)/dt - V(t) 
     d w_i = \eta td_error(t) \z_i(t) \psi_prime(t)
 
     where z is the eligibility trace of the i^th feature (psi_prime accounts for the non-linearrity in the learning rule and is caluclated by the parent class. 
 
-    Input features can be any RatInABox Neurons class here (a set of PlaceCells, BoundaryVectorCells, GridCells etc...or more complex things). It linearly sums these inputs to calculate its firing rate (this summation is all handled by the FeedForwardLayer class). Weights are trained using TD learning, self.update_weights() should be called at each update step and passed the current reward density or reward density vector. For more infor see ratinabox/example_scripts/reinforcement_learning_example/
+    Input features can be any list of RatInABox Neurons class here (a set of PlaceCells, BoundaryVectorCells, GridCells etc...or more complex things). It linearly sums these inputs to calculate its firing rate (this summation is all handled by the FeedForwardLayer class). Weights are trained using TD learning, self.update_weights() should be called at each update step and passed the current reward density or reward density vector. For more infor see ratinabox/example_scripts/reinforcement_learning_example/
 
     Since this is a Neurons subclass, after (or even during) learning you can plot the value function just by querying the ValueNeurons rate map (ValueNeuron.plot_rate_map()), or check the estimate of value at a postion using ValueNeuron.get_state(evaluate_at=None, pos=np.array([[x,y]]))
 
     To see the weights try ValueNeuron.inputs['name_of_input_layer']['w']
     """
 
     default_params = {
-        "input_layer": None,  # the features it is using as inputs
         "tau": 2,  # discount time horizon (equivalent to gamma in discrete RL)
         "tau_e": None,  # eligibility trace timescale, must be <= tau (defaults to tau/2)
         "eta": 0.001,  # learning rate
         "L2": 0.001,  # L2 regularisation
         "activation_params": {"activation": "relu"},  # non-linearity for
         "n": 1,  # how many rewards there will be and thus how many Values function (each represented by one ValueNeuron) there are
     }
 
     def __init__(self, Agent, params={}):
 
         self.params = copy.deepcopy(__class__.default_params)        
         self.params.update(params)
 
-        self.params["input_layers"] = [self.params["input_layer"]]
-        super().__init__(Agent, self.params)  # initialise parent class
+        super().__init__(Agent, self.params)  # initialise parent classes
 
         if self.tau_e == None:
-            self.tau_e = self.tau / 2
-        self.et = np.zeros(self.n)  # initialise eligibility trace
+            self.tau_e = self.tau / 4
+        for input_layer in self.inputs.values():
+            input_layer['eligibility_trace'] = np.zeros(input_layer['n'])  # initialise eligibility trace for each input
         self.firingrate = np.zeros(self.n)  # initialise firing rate
-        self.firingrate_deriv = np.zeros(self.n)  # initialise firing rate derivative
+        self.firingrate_deriv = np.zeros(self.n)  # initialise firing rate temporal derivative
         self.td_error = np.zeros(self.n)  # initialise td error
 
     def update(self):
         """Updates firing rate as weighted linear sum of feature inputs"""
         firingrate_last = self.firingrate
         # update the firing rate
         super().update()  # FeedForwardLayer builtin function. This sums the inputs from the input features over the weight matrix and saves the firingrate.
 
         # calculate temporal derivative of the firing rate
         self.firingrate_deriv = (self.firingrate - firingrate_last) / self.Agent.dt
         # update eligibility trace
-        if self.tau_e == 0:
-            self.et = self.input_layer.firingrate
-        else:
-            self.et = (
-                self.Agent.dt * self.input_layer.firingrate
-                + (1 - self.Agent.dt / self.tau_e) * self.et
+        for input_layer in self.inputs.values():
+            layer = input_layer['layer']
+            if self.tau_e == 0:
+                input_layer['eligibility_trace'] = input_layer.firingrate
+            else:
+                input_layer['eligibility_trace'] = (
+                self.Agent.dt * layer.firingrate
+                + (1 - self.Agent.dt / self.tau_e) * input_layer['eligibility_trace']
             )
         return
 
     def update_weights(self, reward):
         """Trains the weights by implementing the TD learning rule,
         reward is the vector of reward densities"""
         reward = np.array(reward).reshape(-1)
         assert len(reward) == self.n, print(
             f"Must send same number of reward signals as value neurons (n={self.n}), you sent {len(reward)}"
         )
-        w = self.inputs[self.input_layer.name]["w"]  # weights
         V = self.firingrate  # current value estimate
         dVdt = self.firingrate_deriv  # currrent value derivative estimate
         self.td_error = (
             reward + dVdt - V / self.tau
         )  # this is the continuous analog of the TD error
-        dw = (
-            self.Agent.dt
-            * self.eta
-            * (np.outer(self.td_error * self.firingrate_prime, self.et))
-            - self.eta * self.Agent.dt * self.L2 * w
-        )  # note L2 regularisation
-        if np.linalg.norm(dw) > 10:
-            print(np.linalg.norm(dw))
-        self.inputs[self.input_layer.name]["w"] += dw
+        for input_layer in self.inputs.values():
+            w = input_layer["w"] # weights
+            et = input_layer['eligibility_trace']
+            dw = (
+                self.Agent.dt
+                * self.eta
+                * (np.outer(self.td_error * self.firingrate_prime, et))
+                - self.eta * self.Agent.dt * self.L2 * w
+            )  # note L2 regularisation
+            input_layer['w'] += dw
         return
 
     def reset(
         self,
     ):
         """Resets the value neuron by wiping the current eligibility trace and firing rate"""
-        self.et = np.zeros(self.n)  # reinitialise eligibility trace
+        for input_layer in self.inputs.values():
+            input_layer["eligibility_trace"] = np.zeros(input_layer['n'])  # reinitialise eligibility trace
         self.firingrate = np.zeros(self.n)  # reinitialise firing rate
         self.firingrate_deriv = np.zeros(self.n)  # reinitialise firing rate derivative
         self.td_error = np.zeros(self.n)  # reinitialise td error
 
         return
 
 
@@ -135,15 +137,15 @@
             "place_cell_centres": np.array([[0.5, 0.5]]),
             "description": "gaussian_threshold",
         },
     )
     VN = ValueNeuron(
         Ag,
         params={
-            "input_layer": PCs,
+            "input_layers": [PCs],
             "tau": 1,
         },
     )
 
     fig, ax = plt.subplots(1, 4, figsize=(16, 4))
     Reward.plot_place_cell_locations(fig=fig, ax=ax[0])
     VN.plot_rate_map(fig=fig, ax=ax[1])
```

### Comparing `ratinabox-1.5.1/ratinabox/data/README.md` & `ratinabox-1.6.0/ratinabox/data/README.md`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/data/rat.png` & `ratinabox-1.6.0/ratinabox/data/rat.png`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/data/sargolini.npz` & `ratinabox-1.6.0/ratinabox/data/sargolini.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/data/tanni.npz` & `ratinabox-1.6.0/ratinabox/data/tanni.npz`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox/utils.py` & `ratinabox-1.6.0/ratinabox/utils.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/ratinabox.egg-info/PKG-INFO` & `ratinabox-1.6.0/ratinabox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratinabox
-Version: 1.5.1
+Version: 1.6.0
 Summary: RatInABox: A package for simulating motion and ephys data in continuous environments
 Author: Tom George
 Author-email: tomgeorge1@btinternet.com
 License: MIT
 Project-URL: Documentation, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Source, https://github.com/TomGeorge1234/RatInABox
 Project-URL: Tracker, https://github.com/TomGeorge1234/RatInABox/issues
@@ -41,14 +41,15 @@
     * `GridCells`
     * `BoundaryVectorCells` (egocentric or allocentric)
     * `ObjectVectorCells`
     * `VelocityCells`
     * `SpeedCells`
     * `HeadDirectionCells`
     * `FeedForwardLayer` (a generic class analagous to a feedforward layer in a deep neural network)
+    * `SuccessorFeatures` 
     * ...
 
 The top animation shows an example use case: an `Agent` randomly explores a 2D `Environment` with a wall. Three populations of `Neurons` (`PlaceCells`, `GridCells`, `BoundaryVectorCells`) fire according to the receptive fields shown. All data is saved into the history for downstream use. `RatInABox` is fully continuous is space; this means that position and neuronal firing rates are calculated rapidly online with float precision rather than pre-calculated over a discretised mesh. `RatInABox` is flexibly discretised in time; `dt` can be set by the user (defaulting to 10 ms) depending on requirements.
 
 
 ## Key features
 * **Non-specific**: Trajectories can be randomly generated, imported, or adaptively controlled making `RatInABox` a powerful engine for many tasks involving continuous motion (e.g. control theory or [reinforcement learning](#policy-control)). 
@@ -97,44 +98,46 @@
 * [1- or 2-dimensions](#1--or-2-dimensions) 
 
 (ii) the [`Agent`](#ii-agent-features)
 * [Random motion](#random-motion-model)
 * [Importing trajectories](#importing-trajectories)
 * [Policy control](#policy-control)
 * [Wall repelling](#wall-repelling)
+* [Multiple Agents](#multiple-agents)
 * [Advanced `Agent` classes](#advanced-agent-classes)
 
 (iii) the [`Neurons`](#iii-neurons-features).
 * [Cell types](#multiple-cell-types) 
 * [Noise](#noise)
 * [Spikes vs rates](#spiking)
 * [Plotting rate maps](#rate-maps)
 * [Place cell models](#place-cell-models) 
 * [Place cell geometry](#geometry-of-placecells)
 * [Egocentric encodings](#egocentric-encodings)
+* [Successor features and reinforcement learning](#successor-features-and-reinforcement-learning)
 * [Deep neural networks](#more-complex-neuron-types-and-networks-of-neurons)
 
 (iv) [Figures and animations plotting](#iv-figures-and-animations)
 
 Specific details can be found in the [paper](https://www.biorxiv.org/content/10.1101/2022.08.10.503541v3). 
 
 
 
 ### (i) `Environment` features
-#### Walls 
+#### **Walls**
 Arbitrarily add walls to the environment to produce arbitrarily complex mazes:
 ```python 
 Environment.add_wall([[x0,y0],[x1,y1]])
 ```
 Here are some easy to make examples.
 
 <img src=".images/readme/walls.png" width=1000>
 
 
-#### Complex `Environment`s: Polygons, curves, and holes
+#### **Complex `Environment`s: Polygons, curves, and holes**
 By default, `Environments` in RatInABox are square (or rectangular if `aspect != 1`). It is possible to create arbitrary environment shapes using the `"boundary"` parameter at initialisation. 
 
 One can all add holes to the `Environment` using the `"holes"` parameter at initialisation. Positions sampled from the Environment (e.g. at initialisation) won't be inside holes.
 
 Any curved environments can be made by creating a boundary of many small walls (uyse sparingly, walls may slow down computations)
 
 ```python 
@@ -157,39 +160,39 @@
 ```
 
 
 <img src=".images/readme/complex_envs.png" width=1000>
 
 
 
-#### Boundary conditions 
+#### **Boundary conditions**
 Boundary conditions (for default square/rectangular environments) can be "periodic" or "solid". Place cells and the motion of the Agent will respect these boundaries accordingly. 
 ```python
 Env = Environment(
     params = {'boundary_conditions':'periodic'} #or 'solid' (default)
 ) 
 ```
 
 <img src=".images/readme/boundary_conditions.png" width=500>
 
-#### 1- or 2-dimensions 
+#### **1- or 2-dimensions**
 `RatInABox` supports 1- or 2-dimensional `Environment`s. Almost all applicable features and plotting functions work in both. The following figure shows 1 minute of exploration of an `Agent` in a 1D environment with periodic boundary conditions spanned by 10 place cells. 
 ```python 
 Env = Environment(
     params = {'dimensionality':'1D'} #or '2D' (default)
 ) 
 ```
 
 <img src=".images/readme/one_dimension.png" width=500>
 
 
 
 ### (ii) `Agent` features
 
-#### Random motion model
+#### **Random motion model**
 By defaut the `Agent` follows a random motion policy.  Random motion is stochastic but smooth. The speed (and rotational speed, if in 2D) of an Agent take constrained random walks governed by Ornstein-Uhlenbeck processes. You can change the means, variance and coherence times of these processes to control the shape of the trajectory. Default parameters are fit to real rat locomotion data from Sargolini et al. (2006): 
 
 <img src=".images/readme/riab_vs_sargolini.gif" width=500>
 
 The default parameters can be changed to obtain different style trajectories. The following set of trajectories were generated by modifying the rotational speed parameter `Agent.rotational_velocity_std`:
 
 ```python
@@ -198,68 +201,76 @@
 Agent.rotation_velocity_std = 120 * np.pi/180 #radians 
 Agent.rotational_velocity_coherence_time = 0.08
 ```
 
 <img src=".images/readme/motion_model.png" width=800>
 
 
-#### Importing trajectories
+#### **Importing trajectories**
 `RatInABox` supports importing external trajectory data (rather than using the in built random motion policy). Imported data can be of low temporal resolution. It will be smoothly upsampled using a cubic splines interpolation technique. We provide a 10 minute trajectory from the open-source data set of Sargolini et al. (2006) ready to import. In the following figure blue shows (low resolution) trajectory data imported into an `Agent` and purple shows the smoothly upsampled trajectory taken by the `Agent` during exploration. 
 ```python
 Agent.import_trajectory(dataset='sargolini')
 #or 
 Agent.import_trajectory(times=array_of_times,
                         positions=array_of_positions)
 
 ```
 
 <img src=".images/readme/imported_trajectory.png" width=200>
 
-#### Policy control 
+#### **Policy control**
 By default the movement policy is an random and uncontrolled (e.g. displayed above). It is possible, however, to manually pass a "drift_velocity" to the Agent on each `Agent.update()` step. This 'closes the loop' allowing, for example, Actor-Critic systems to control the Agent policy. As a demonstration that this method can be used to control the agent's movement we set a radial drift velocity to encourage circular motion. We also use RatInABox to perform a simple model-free RL task and find a reward hidden behind a wall (the full script is given as an example script [here](./demos/reinforcement_learning_example.ipynb))
 ```python
 Agent.update(drift_velocity=drift_velocity)
 ```
 
 <img src=".images/readme/motion.gif" width=600>
 
-#### Wall repelling 
+#### **Wall repelling**
 Under the random motion policy, walls in the environment mildly "repel" the `Agent`. Coupled with the finite turning speed this replicates an effect (known as thigmotaxis, sometimes linked to anxiety) where the `Agent` is biased to over-explore near walls and corners (as shown in these heatmaps) matching real rodent behaviour. It can be turned up or down with the `thigmotaxis` parameter.
 ```python 
 Αgent.thigmotaxis = 0.8 #1 = high thigmotaxis (left plot), 0 = low (right)
 ```
 
 <img src=".images/readme/wall_repel.png" width=900>
 
+#### **Multiple `Agent`s**
+There is nothing to stop multiple `Agent`s being added to the same `Environment`. When plotting/animating trajectories set the kwarg `plot_all_agents=True` to visualise all `Agent`s simultaneously. 
 
-#### Advanced `Agent` classes
+The following animation shows three `Agent`s in an `Environment`. Drift velocities are set so that `Agent`s weally locally attract one another creating "interactive" behaviour.
+
+<img src=".images/readme/multi_agents.gif" width=350>
+
+
+#### **Advanced `Agent` classes**
 One can make more advanced Agent classes, for example `ThetaSequenceAgent()` where the position "sweeps" (blue) over the position of an underlying true (regular) `Agent()` (purple), highly reminiscent of theta sequences observed when one decodes position from the hippocampal populaton code on sub-theta (10 Hz) timescales. This class can be found in the [`contribs`](./ratinabox/contribs/) directory. 
 
 <img src=".images/readme/theta_sequences.gif" width=350>
 
 
 ### (iii) `Neurons` features 
 
-#### Multiple cell types: 
-We provide a list of premade `Neurons` subclasses. These include: 
+#### **Multiple cell types:**
+We provide a list of premade `Neurons` subclasses. These include (but are not limited to): 
 
 * `PlaceCells` 
 * `GridCells`
 * `BoundaryVectorCells` (can be egocentric or allocentric)
 * `ObjectVectorCells` (can be used as visual cues, i.e. only fire when `Agent` is looking towards them)
 * `HeadDirectionCells`
 * `VelocityCells`
 * `SpeedCells`
 * `FeedForwardLayer` - calculates activated weighted sum of inputs from a provide list of input `Neurons` layers.
 * `FieldOfViewNeurons` - Egocentric encoding of what the `Agent` can see 
+* `SuccessorFeatures` - Learns the successor features for a set of features under teh current motion policy
 
-This last class, `FeedForwardLayer` deserves special mention. Instead of its firing rate being determined explicitly by the state of the `Agent` it summates synaptic inputs from a provided list of input layers (which can be any `Neurons` subclass). This layer is the building block for how more complex networks can be studied using `RatInABox`. 
+`FeedForwardLayer` deserves special mention. Instead of its firing rate being determined explicitly by the state of the `Agent` it summates synaptic inputs from a provided list of input layers (which can be any `Neurons` subclass). This layer is the building block for how more complex networks can be studied using `RatInABox`. 
 
 
-#### Noise 
+#### **Noise** 
 Use the `Neurons.noise_std` and `Neurons.noise_coherence_time` parameters to control the amount of noise (Hz) and autocorrelation timescale of the noise (seconds). For example (work with all `Neurons` classes, not just `PlaceCells`): 
 
 ```python
 PCs = PlaceCells(Ag,params={
     'noise_std':0.1, #defaults to 0 i.e. no noise
     'noise_coherence_time':0.5, #autocorrelation timescale of additive noise vector 
 })
@@ -272,27 +283,27 @@
 ```
 Neurons.plot_ratemap(spikes=True)
 ```
 
 <img src=".images/readme/spikes.png" width="1000">
 
 
-#### Rate maps 
+#### **Rate maps**
 `PlaceCells`, `GridCells` and allocentric `BoundaryVectorCells` (among others) have firing rates which depend exclusively on the position of the agent. These rate maps can be displayed by querying their firing rate at an array of positions spanning the environment, then plotting. This process is done for you using the function `Neurons.plot_rate_map()`. 
 
 More generally, however, cells firing is not only determined by position but potentially other factors (e.g. velocity, or historical effects if the layer is part of a recurrent network). In these cases the above method of plotting rate maps will necessarily fail. A more robust way to display the receptive field is to plot a heatmap of the positions of the Agent has visited where each positions contribution to a bin is weighted by the firing rate observed at that position. Over time, as coverage become complete, the firing fields become visible.
 ```
 Neurons.plot_rate_map() #attempts to plot "ground truth" rate map 
 Neurons.plot_rate_map(method="history") #plots rate map by firing-rate-weighted position heatmap
 ``` 
 
 <img src=".images/readme/rate_map.png" width=600>
 
 
-#### Place cell models
+#### **Place cell models**
 
 Place cells come in multiple types (given by `params['description']`), or it would be easy to write your own:
 * `"gaussian"`: normal gaussian place cell 
 * `"gaussian_threshold"`: gaussian thresholded at 1 sigma
 * `"diff_of_gaussians"`: gaussian(sigma) - gaussian(1.5 sigma)
 * `"top_hat"`: circular receptive field, max firing rate within, min firing rate otherwise
 * `"one_hot"`: the closest palce cell to any given location is established. This and only this cell fires. 
@@ -302,21 +313,21 @@
 <img src=".images/readme/placecellmodels.png" width=800>
 
 These place cells (with the exception of `"one_hot"`s) can all be made to phase precess by instead initialising them with the `PhasePrecessingPlaceCells()` class currently residing in the `contribs` folder. This figure shows example output data. 
 
 <img src=".images/readme/phaseprecession.png" width=500>
 
 
-#### Geometry of `PlaceCells` 
+#### **Geometry of `PlaceCells`** 
 Choose how you want `PlaceCells` to interact with walls in the `Environment`. We provide three types of geometries.  
 
 <img src=".images/readme/wall_geometry.png" width=900>
 
 
-#### Egocentric encodings
+#### **Egocentric encodings**
 Most `RatInABox` cell classes are allocentric (e.g. `PlaceCells`, `GridCells` etc. do not depend on the agents point of view) not egocentric. `BoundaryVectorCells` (BVCs) and `ObjectVectorCells` (OVCs) can be either. `FieldOfViewNeurons` exploit this by arranging sets of egocentric BVC or OVCs to tile to agents local field of view creating a comprehensive egocentric encoding of what boundaries or objects the agent can 'see' from it's current point of view. A custom plotting function displays the tiling and the firing rates as shown below. With an adequately defined field of view these can make, for example, "whisker cells". 
 
 ```python
 FoV_BVCs = FieldOfViewNeurons(Ag)
 FoV_OVCs = FieldOfViewNeurons(Ag,params={
     'cell_type':'OVC',
     })
@@ -324,37 +335,43 @@
     "FoV_angles":[75,105],
     "FoV_distance":[0.1,0.2],
     "spatial_resolution":0.02,})
 ```
 
 <img src=".images/readme/field_of_view.gif" width=600>
 
+#### **Successor Features and Reinforcement Learning**
+A dedicated `Neurons` class called `SuccessorFeatures` learns the successor features for a given feature set under teh current policy. See [this demo](./demos/successor_features_example.ipynb) for more info. 
+<img src=".images/demos/SF_development.gif" width=600>
+
+`SuccessorFeatures` are a specific instance of a more general class of neurons called `ValueNeuron`s which learn value function for any reward density under the `Agent`s motion policy. This can be used to do reinforcement learning tasks such as finding rewards hidden behind walls etc as shown in [this demo](./demos/reinforcement_learning_example.ipynb). 
 
+Finally, we are working on making an OpenAI `Gym` environment wrapper for `RatInABox`. This should be available soon, keep an eye on [this issue](https://github.com/TomGeorge1234/RatInABox/issues/30). 
 
-#### More complex Neuron types and networks of Neurons
-We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here](./demos/path_integration_example.ipynb) and [here](./demos/reinforcement_learning_example.ipynb). 
+#### **More complex Neuron types and networks of Neurons**
+We encourage users to create their own subclasses of `Neurons`. This is easy to do, see comments in the `Neurons` class within the [code](./ratinabox/Neurons.py) for explanation. By forming these classes from the parent `Neurons` class, the plotting and analysis features described above remain available to these bespoke Neuron types. Additionally we provide a `Neurons` subclass called `FeedForwardLayer`. This neuron sums inputs from any provied list of other `Neurons` classes and can be used as the building block for constructing complex multilayer networks of `Neurons`, as we do [here (path integration)](./demos/path_integration_example.ipynb), [here (reinforcement learning)](./demos/reinforcement_learning_example.ipynb) and [here (successor features)](./demos/successor_features_example.ipynb). 
 
 
 
 ### (iv) Figures and animations 
 `RatInABox` is built to be highly visual. It is easy to plot or animate data and save these plots/animations. Here are some tips
 
-#### Saving
+#### **Saving**
 * `ratinabox.figure_directory` a global variable specifying the directory into which figures/animations will be saved 
 * `ratinabox.utils.save_figure(fig,fig_name)` saves a figure (or animation) into a dated folder within the figure directory  as both `".svg"` and `".png"` (`".mp4"` or `".gif"`). The current time will be appended to the `fig_name` so you won't ever overwrite. 
 
 
-#### Saving (but automatically)
+#### **Saving (but automatically)**
 * Setting `ratinabox.autosave_plots = True` means RatInABox figure will be automatically saved in the figure directory without having to indvidually call the `utils` function above. 
 
-#### Styling
+#### **Styling**
 * `ratinabox.stylize_plots()` this call sets some global matplotlib rcParams to make plots look pretty/exactly like they do in this repo
 
 
-#### Most important plotting functions
+#### **Most important plotting functions**
 The most important plotting functions are (see source code for the available arguments/kwargs):
 
 ```python
 Environment.plot_environment() #visualises current environment with walls and objects
 Agent.plot_trajectory() #plots trajectory
 Agent.animate_trajectory() #animate trajectory
 Neurons.plot_rate_map() # plots the rate map of the neurons at all positions
@@ -388,14 +405,15 @@
 ```
 * [extensive_example.ipynb](./demos/extensive_example.ipynb): a more involved tutorial. More complex enivornment, more complex cell types and more complex plots are used. 
 * [list_of_plotting_functions.md](./demos/list_of_plotting_fuctions.md): All the types of plots available for are listed and explained. 
 * [readme_figures.ipynb](./demos/readme_figures.ipynb): (Almost) all plots/animations shown in the root readme are produced from this script (plus some minor formatting done afterwards in powerpoint).
 * [paper_figures.ipynb](./demos/paper_figures.ipynb): (Almost) all plots/animations shown in the paper are produced from this script (plus some major formatting done afterwards in powerpoint).
 * [decoding_position_example.ipynb](./demos/decoding_position_example.ipynb): Postion is decoded from neural data generated with RatInABox. Place cells, grid cell and boundary vector cells are compared. 
 * [reinforcement_learning_example.ipynb](./demos/reinforcement_learning_example.ipynb): RatInABox is use to construct, train and visualise a small two-layer network capable of model free reinforcement learning in order to find a reward hidden behind a wall. 
+* [successor_features_example.ipynb](./successor_features_example.ipynb): RatInABox is use to learn and visualise successor features under random and biased motion policies.
 * [path_integration_example.ipynb](./demos/path_integration_example.ipynb): RatInABox is use to construct, train and visualise a large multi-layer network capable of learning a "ring attractor" capable of path integrating a position estimate using only velocity inputs.
 
 ## Contribute 
 `RatInABox` is an open source project, and we actively encourage community contributions, for example bug fixes, new cells types, new features, new plotting functions, new motion datasets, documentation, citations of relevant work, or additional experiment notebooks. Typically the best way to go about this is by opening an issue or feel free to make a pull request. 
 
 We have a dedicated [contribs](./ratinabox/contribs/) directory where you can safely add awesome scripts and new `Neurons` classes etc.
```

### Comparing `ratinabox-1.5.1/ratinabox.egg-info/SOURCES.txt` & `ratinabox-1.6.0/ratinabox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/setup.cfg` & `ratinabox-1.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratinabox
-version = 1.5.1
+version = 1.6.0
 author = Tom George
 author_email = tomgeorge1@btinternet.com
 project_urls = 
 	Documentation = https://github.com/TomGeorge1234/RatInABox
 	Source = https://github.com/TomGeorge1234/RatInABox
 	Tracker = https://github.com/TomGeorge1234/RatInABox/issues
 description = RatInABox: A package for simulating motion and ephys data in continuous environments
```

### Comparing `ratinabox-1.5.1/tests/test_advanced.py` & `ratinabox-1.6.0/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `ratinabox-1.5.1/tests/test_environment.py` & `ratinabox-1.6.0/tests/test_environment.py`

 * *Files identical despite different names*

