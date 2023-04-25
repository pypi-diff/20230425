# Comparing `tmp/gym-trading-env-0.2.2.tar.gz` & `tmp/gym-trading-env-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.2.2.tar", last modified: Tue Apr 25 12:32:25 2023, max compression
+gzip compressed data, was "gym-trading-env-0.2.3.tar", last modified: Tue Apr 25 12:46:34 2023, max compression
```

## Comparing `gym-trading-env-0.2.2.tar` & `gym-trading-env-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 12:32:25.695796 gym-trading-env-0.2.2/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0       44 2023-04-23 18:13:37.000000 gym-trading-env-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1860 2023-04-25 12:32:25.694798 gym-trading-env-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2985 2023-04-25 12:31:39.000000 gym-trading-env-0.2.2/README.rst
--rw-rw-rw-   0        0        0      870 2023-04-25 12:31:45.000000 gym-trading-env-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 12:32:25.696793 gym-trading-env-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 12:32:25.593556 gym-trading-env-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 12:32:25.630969 gym-trading-env-0.2.2/src/gym_trading_env/
--rw-rw-rw-   0        0        0      333 2023-04-15 09:28:44.000000 gym-trading-env-0.2.2/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     4164 2023-04-13 12:51:04.000000 gym-trading-env-0.2.2/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0    14459 2023-04-25 09:39:29.000000 gym-trading-env-0.2.2/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2504 2023-04-24 23:59:53.000000 gym-trading-env-0.2.2/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:32:25.674852 gym-trading-env-0.2.2/src/gym_trading_env/templates/
--rw-rw-rw-   0        0        0     3878 2023-04-25 08:50:20.000000 gym-trading-env-0.2.2/src/gym_trading_env/templates/index.html
-drwxrwxrwx   0        0        0        0 2023-04-25 12:32:25.692803 gym-trading-env-0.2.2/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.2.2/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.2.2/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.2.2/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.2.2/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-25 12:32:25.668868 gym-trading-env-0.2.2/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0     1860 2023-04-25 12:32:25.000000 gym-trading-env-0.2.2/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-04-25 12:32:25.000000 gym-trading-env-0.2.2/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:32:25.000000 gym-trading-env-0.2.2/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-25 12:32:25.000000 gym-trading-env-0.2.2/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-25 12:32:25.000000 gym-trading-env-0.2.2/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.488030 gym-trading-env-0.2.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       44 2023-04-23 18:13:37.000000 gym-trading-env-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4431 2023-04-25 12:46:34.486034 gym-trading-env-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2569 2023-04-25 12:45:18.000000 gym-trading-env-0.2.3/README.md
+-rw-rw-rw-   0        0        0      870 2023-04-25 12:45:19.000000 gym-trading-env-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 12:46:34.489028 gym-trading-env-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.382312 gym-trading-env-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.420211 gym-trading-env-0.2.3/src/gym_trading_env/
+-rw-rw-rw-   0        0        0      333 2023-04-15 09:28:44.000000 gym-trading-env-0.2.3/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     4164 2023-04-13 12:51:04.000000 gym-trading-env-0.2.3/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0    14459 2023-04-25 09:39:29.000000 gym-trading-env-0.2.3/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2504 2023-04-24 23:59:53.000000 gym-trading-env-0.2.3/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.465091 gym-trading-env-0.2.3/src/gym_trading_env/templates/
+-rw-rw-rw-   0        0        0     3878 2023-04-25 08:50:20.000000 gym-trading-env-0.2.3/src/gym_trading_env/templates/index.html
+drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.481048 gym-trading-env-0.2.3/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.2.3/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:46:34.463097 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0     4431 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-25 12:46:34.000000 gym-trading-env-0.2.3/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.2.2/LICENSE.txt` & `gym-trading-env-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/README.rst` & `gym-trading-env-0.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,63 @@
-|Crypto Trading Environment|
-================================
 
-.. |Crypto Trading Environment| raw:: html
-
-   <h1 align='center'>
-      <img src = 'https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/images/logo_light-bg.png' width='500'>
-   </h1>
-
- 
-.. raw:: html
-
-   <section class="shields" align="center">
-      <a href="https://www.python.org/">
-         <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"
-            alt="python">
-      </a>
-      <a href="https://pypi.org/project/gym-trading-env/">
-         <img src="https://img.shields.io/badge/pypi-v1.1.3-brightgreen.svg"
-            alt="PyPI">
-      </a>
-      <a href="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/LICENSE.txt">
-      <img src="https://img.shields.io/badge/license-MIT%202.0%20Clause-green"
-            alt="Apache 2.0 with Commons Clause">
-      </a>
-      <a href='https://gym-trading-env.readthedocs.io/en/latest/?badge=latest'>
-          <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
-      </a>
-      
-      <br>
-      <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
-         <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
-      </a>
-   </section>
+<h1 align='center'>
+   <img src = 'https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/images/logo_light-bg.png' width='500'>
+</h1>
+
+<section class="shields" align="center">
+   <a href="https://www.python.org/">
+      <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"
+         alt="python">
+   </a>
+   <a href="https://pypi.org/project/gym-trading-env/">
+      <img src="https://img.shields.io/badge/pypi-v1.1.3-brightgreen.svg"
+         alt="PyPI">
+   </a>
+   <a href="https://github.com/ClementPerroud/Gym-Trading-Env/blob/main/LICENSE.txt">
+   <img src="https://img.shields.io/badge/license-MIT%202.0%20Clause-green"
+         alt="Apache 2.0 with Commons Clause">
+   </a>
+   <a href='https://gym-trading-env.readthedocs.io/en/latest/?badge=latest'>
+         <img src='https://readthedocs.org/projects/gym-trading-env/badge/?version=latest' alt='Documentation Status' />
+   </a>
+   <a href="https://github.com/ClementPerroud/Gym-Trading-Env">
+      <img src="https://img.shields.io/github/stars/ClementPerroud/gym-trading-env?style=social" alt="Github stars">
+   </a>
+</section>
   
 Cryto Trading Env is an OpenAI Gym environment for simulating stocks and train Reinforcement Learning (RL) trading agents.
 It was designed to be fast and customizable for easy RL trading algorythms implementation.
 
-+---------------------------------------------------------------------------------+
-| `Documentation <https://gym-trading-env.readthedocs.io/en/latest/index.html>`_  |
-+---------------------------------------------------------------------------------+
+
+| [Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
+
 
 Key features
 ---------------
 
 This package aims to greatly simplify the research phase by offering :
 
 * Easy and quick download technical data on several exchanges
 * A simple and fast environment for the user and the AI, but which allows complex operations (Short, Margin trading).
 * A high performance rendering (can display several hundred thousand candles simultaneously), customizable to visualize the actions of its agent and its results.
 * (Coming soon) An easy way to backtest any RL-Agents or any king 
 
-.. image:: https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif
+![Render animated image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif)
 
 Installation
 ---------------
 
 Crypto Trading Env supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
 
-.. code-block:: console
-
-   >>> pip install gym-trading-env
+```bash
+pip install gym-trading-env
+```
 
 Or using git :
 
-.. code-block:: console
-   
-   >>> git clone https://github.com/ClementPerroud/Gym-Trading-Env
+```bash
+git clone https://github.com/ClementPerroud/Gym-Trading-Env
+```
 
 
-`Documentation available here <https://gym-trading-env.readthedocs.io/en/latest/index.html>`_
+[Documentation available here](https://gym-trading-env.readthedocs.io/en/latest/index.html)
 -----------------------------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -1,27 +1,21 @@
-|Crypto Trading Environment| ================================ .. |Crypto
-Trading Environment| raw:: html
 ****** [https://github.com/ClementPerroud/Gym-Trading-Env/raw/main/docs/source/
                        images/logo_light-bg.png] ******
-.. raw:: html  [python] [PyPI] [Apache_2.0_with_Commons_Clause] [Documentation
-Status]
+ [python] [PyPI] [Apache_2.0_with_Commons_Clause] [Documentation_Status]
 [Github_stars]  Cryto Trading Env is an OpenAI Gym environment for simulating
 stocks and train Reinforcement Learning (RL) trading agents. It was designed to
-be fast and customizable for easy RL trading algorythms implementation. +------
----------------------------------------------------------------------------+ |
-`Documentation
-gym-trading-env.readthedocs.io/en/latest/index.html>`_ | +---------------------
-------------------------------------------------------------+ Key features ----
------------ This package aims to greatly simplify the research phase by
-offering : * Easy and quick download technical data on several exchanges * A
-simple and fast environment for the user and the AI, but which allows complex
-operations (Short, Margin trading). * A high performance rendering (can display
-several hundred thousand candles simultaneously), customizable to visualize the
-actions of its agent and its results. * (Coming soon) An easy way to backtest
-any RL-Agents or any king .. image:: https://raw.githubusercontent.com/
-ClementPerroud/Gym-Trading-Env/main/docs/source/images/render.gif Installation
---------------- Crypto Trading Env supports Python 3.9+ on Windows, Mac, and
-Linux. You can install it using pip: .. code-block:: console >>> pip install
-gym-trading-env Or using git : .. code-block:: console >>> git clone https://
-github.com/ClementPerroud/Gym-Trading-Env `Documentation available here
-gym-trading-env.readthedocs.io/en/latest/index.html>`_ ------------------------
------------------------------------------------------------------------
+be fast and customizable for easy RL trading algorythms implementation. |
+[Documentation](https://gym-trading-env.readthedocs.io/en/latest/index.html) |
+Key features --------------- This package aims to greatly simplify the research
+phase by offering : * Easy and quick download technical data on several
+exchanges * A simple and fast environment for the user and the AI, but which
+allows complex operations (Short, Margin trading). * A high performance
+rendering (can display several hundred thousand candles simultaneously),
+customizable to visualize the actions of its agent and its results. * (Coming
+soon) An easy way to backtest any RL-Agents or any king ![Render animated
+image](https://raw.githubusercontent.com/ClementPerroud/Gym-Trading-Env/main/
+docs/source/images/render.gif) Installation --------------- Crypto Trading Env
+supports Python 3.9+ on Windows, Mac, and Linux. You can install it using pip:
+```bash pip install gym-trading-env ``` Or using git : ```bash git clone https:
+//github.com/ClementPerroud/Gym-Trading-Env ``` [Documentation available here]
+(https://gym-trading-env.readthedocs.io/en/latest/index.html) -----------------
+------------------------------------------------------------------------------
```

### Comparing `gym-trading-env-0.2.2/pyproject.toml` & `gym-trading-env-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.2.2"
+version = "0.2.3"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/downloader.py` & `gym-trading-env-0.2.3/src/gym_trading_env/downloader.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/environments.py` & `gym-trading-env-0.2.3/src/gym_trading_env/environments.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/renderer.py` & `gym-trading-env-0.2.3/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/templates/index.html` & `gym-trading-env-0.2.3/src/gym_trading_env/templates/index.html`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.2.3/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.2.3/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.2.3/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.2.2/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.2.3/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE.txt
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 src/gym_trading_env/__init__.py
 src/gym_trading_env/downloader.py
 src/gym_trading_env/environments.py
 src/gym_trading_env/renderer.py
 src/gym_trading_env.egg-info/PKG-INFO
 src/gym_trading_env.egg-info/SOURCES.txt
```

