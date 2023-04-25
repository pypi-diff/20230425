# Comparing `tmp/financeager-flask-0.5.0.0.tar.gz` & `tmp/financeager-flask-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financeager-flask-0.5.0.0.tar", last modified: Sun May  8 18:33:30 2022, max compression
+gzip compressed data, was "financeager-flask-1.0.0.tar", last modified: Tue Apr 25 09:50:38 2023, max compression
```

## Comparing `financeager-flask-0.5.0.0.tar` & `financeager-flask-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/examples/fcgi.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/examples/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/financeager_flask/
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/flask.py
--rw-r--r--   0 runner    (1001) docker     (121)     4261 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/httprequests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2749 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/offline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/financeager_flask/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/financeager_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-05-08 18:33:29.000000 financeager-flask-0.5.0.0/financeager_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-05-08 18:33:30.000000 financeager-flask-0.5.0.0/financeager_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-08 18:33:29.000000 financeager-flask-0.5.0.0/financeager_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-05-08 18:33:30.000000 financeager-flask-0.5.0.0/financeager_flask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-05-08 18:33:30.000000 financeager-flask-0.5.0.0/financeager_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-08 18:33:30.000000 financeager-flask-0.5.0.0/financeager_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-05-08 18:33:30.395329 financeager-flask-0.5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 18:33:30.391329 financeager-flask-0.5.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12404 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/test_fflask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/test_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/test_offline.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-05-08 18:32:55.000000 financeager-flask-0.5.0.0/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.973162 financeager-flask-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.961162 financeager-flask-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.965162 financeager-flask-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-25 09:50:38.969162 financeager-flask-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.965162 financeager-flask-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/examples/fcgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/examples/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.965162 financeager-flask-1.0.0/financeager_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/financeager_flask/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.969162 financeager-flask-1.0.0/financeager_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 09:50:38.000000 financeager-flask-1.0.0/financeager_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 09:50:38.973162 financeager-flask-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:38.969162 financeager-flask-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_fflask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/test_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-25 09:50:16.000000 financeager-flask-1.0.0/test/utils.py
```

### Comparing `financeager-flask-0.5.0.0/.github/workflows/ci.yml` & `financeager-flask-1.0.0/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   # This workflow contains a single job called "build"
   build:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9, "3.10"]
+        python-version: [3.7, 3.8, 3.9, "3.10"]
 
     # Steps represent a sequence of tasks that will be executed as part of the job
     steps:
       # Checks-out your repository under $GITHUB_WORKSPACE, so your job can access it
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
@@ -41,15 +41,16 @@
           # Look to see if there is a cache hit for the corresponding setup file (better: requirements.txt)
           key: ${{ runner.os }}-pip-${{ hashFiles('setup.py') }}
           restore-keys: |
             ${{ runner.os }}-pip-
             ${{ runner.os }}-
       - name: Install dependencies
         run: |
-          python -m pip install -U -e .[develop]
+          pip install -U pip
+          pip install -U -e .[develop]
           pip install -U coveralls
       - name: Run style-checks
         uses: pre-commit/action@v2.0.0
       - name: Run test suite
         run: |
           coverage run -m unittest
       - name: Upload coverage result
```

### Comparing `financeager-flask-0.5.0.0/.github/workflows/release.yml` & `financeager-flask-1.0.0/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Upload Python Package
 
 on:
   push:
     tags:
-      - v*.*.*.*
+      - v*.*.*
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 jobs:
   publish:
 
     runs-on: ubuntu-latest
```

### Comparing `financeager-flask-0.5.0.0/.pre-commit-config.yaml` & `financeager-flask-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/Changelog.md` & `financeager-flask-1.0.0/Changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 
 ## [unreleased]
 ### Added
 ### Changed
 ### Removed
 ### Fixed
 
+## [v1.0.0] - 2023-04-25
+### Removed
+- Support for Python 3.6 is removed.
+### Changed
+- The upstream `financeager` dependency is required as lower than v1.3.0. (#34)
+- The `setup.py` and `setup.cfg` files are replaced by `pyproject.toml` entirely.
+
 ## [v0.5.0.0] - 2022-05-08
 ### Added
 - Rename `fflask` module to `flask`, adjust WSGI/FCGI scripts accordingly.
 ### Changed
 - The upstream `financeager` dependency is required as lower than v1.1.0.
 ### Deprecated
 - Python 3.6 support will be removed in v1.0.0.
```

### Comparing `financeager-flask-0.5.0.0/LICENSE` & `financeager-flask-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/Makefile` & `financeager-flask-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/PKG-INFO` & `financeager-flask-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: financeager-flask
-Version: 0.5.0.0
+Version: 1.0.0
 Summary: Plugin to use flask as backend for financeager
-Home-page: https://github.com/pylipp/financeager-flask
-Author: Philipp Metzner
-Author-email: beth.aleph@yahoo.de
+Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
-Keywords: commandline finances
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/pylipp/financeager-flask/issues
+Project-URL: Documentation, https://github.com/pylipp/financeager-flask
+Project-URL: Homepage, https://github.com/pylipp/financeager-flask
+Project-URL: Source Code, https://github.com/pylipp/financeager-flask
+Keywords: commandline,finances
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-Provides-Extra: packaging
 Provides-Extra: develop
+Provides-Extra: packaging
 License-File: LICENSE
 
 ![Build Status](https://github.com/pylipp/financeager-flask/workflows/CI/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/pylipp/financeager-flask/badge.svg?branch=master)](https://coveralls.io/github/pylipp/financeager-flask?branch=master)
 
 # financeager-flask
 
 Plugin that enables you to run [financeager](https://github.com/pylipp/financeager) as a Flask-powered webservice!
 
 ## Installation
 
-`financeager-flask` requires Python 3.6 or higher.
+`financeager-flask` requires Python 3.7 or higher.
 
     pip install financeager-flask
 
 Installation via [`pipx`](https://pipxproject.github.io/pipx/) is recommended:
 
     pipx install financeager
     pipx inject financeager financeager-flask
@@ -151,9 +151,7 @@
 
 If you added a non-cosmetic change (i.e. a change in functionality, e.g. a bug fix or a new feature), please update `Changelog.md` accordingly as well. Check this README whether the content is still up to date.
 
 ### Releasing
 
 1. Tag the latest commit on master by incrementing the current version accordingly (scheme `v0.major.minor.patch`).
 1. Run `make release`.
-
-
```

### Comparing `financeager-flask-0.5.0.0/README.md` & `financeager-flask-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # financeager-flask
 
 Plugin that enables you to run [financeager](https://github.com/pylipp/financeager) as a Flask-powered webservice!
 
 ## Installation
 
-`financeager-flask` requires Python 3.6 or higher.
+`financeager-flask` requires Python 3.7 or higher.
 
     pip install financeager-flask
 
 Installation via [`pipx`](https://pipxproject.github.io/pipx/) is recommended:
 
     pipx install financeager
     pipx inject financeager financeager-flask
```

### Comparing `financeager-flask-0.5.0.0/examples/fcgi.py` & `financeager-flask-1.0.0/examples/fcgi.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/examples/wsgi.py` & `financeager-flask-1.0.0/examples/wsgi.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/financeager_flask/flask.py` & `financeager-flask-1.0.0/financeager_flask/flask.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/financeager_flask/httprequests.py` & `financeager-flask-1.0.0/financeager_flask/httprequests.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/financeager_flask/main.py` & `financeager-flask-1.0.0/financeager_flask/main.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/financeager_flask/offline.py` & `financeager-flask-1.0.0/financeager_flask/offline.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/financeager_flask/resources.py` & `financeager-flask-1.0.0/financeager_flask/resources.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/financeager_flask.egg-info/PKG-INFO` & `financeager-flask-1.0.0/financeager_flask.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: financeager-flask
-Version: 0.5.0.0
+Version: 1.0.0
 Summary: Plugin to use flask as backend for financeager
-Home-page: https://github.com/pylipp/financeager-flask
-Author: Philipp Metzner
-Author-email: beth.aleph@yahoo.de
+Author-email: Philipp Metzner <beth.aleph@yahoo.de>
 License: GPLv3
-Keywords: commandline finances
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/pylipp/financeager-flask/issues
+Project-URL: Documentation, https://github.com/pylipp/financeager-flask
+Project-URL: Homepage, https://github.com/pylipp/financeager-flask
+Project-URL: Source Code, https://github.com/pylipp/financeager-flask
+Keywords: commandline,finances
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
-Provides-Extra: packaging
 Provides-Extra: develop
+Provides-Extra: packaging
 License-File: LICENSE
 
 ![Build Status](https://github.com/pylipp/financeager-flask/workflows/CI/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/pylipp/financeager-flask/badge.svg?branch=master)](https://coveralls.io/github/pylipp/financeager-flask?branch=master)
 
 # financeager-flask
 
 Plugin that enables you to run [financeager](https://github.com/pylipp/financeager) as a Flask-powered webservice!
 
 ## Installation
 
-`financeager-flask` requires Python 3.6 or higher.
+`financeager-flask` requires Python 3.7 or higher.
 
     pip install financeager-flask
 
 Installation via [`pipx`](https://pipxproject.github.io/pipx/) is recommended:
 
     pipx install financeager
     pipx inject financeager financeager-flask
@@ -151,9 +151,7 @@
 
 If you added a non-cosmetic change (i.e. a change in functionality, e.g. a bug fix or a new feature), please update `Changelog.md` accordingly as well. Check this README whether the content is still up to date.
 
 ### Releasing
 
 1. Tag the latest commit on master by incrementing the current version accordingly (scheme `v0.major.minor.patch`).
 1. Run `make release`.
-
-
```

### Comparing `financeager-flask-0.5.0.0/financeager_flask.egg-info/SOURCES.txt` & `financeager-flask-1.0.0/financeager_flask.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 Changelog.md
 LICENSE
 Makefile
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/release.yml
 examples/fcgi.py
 examples/wsgi.py
 financeager_flask/__init__.py
 financeager_flask/exceptions.py
```

### Comparing `financeager-flask-0.5.0.0/test/test_cli.py` & `financeager-flask-1.0.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/test/test_config.py` & `financeager-flask-1.0.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/test/test_fflask.py` & `financeager-flask-1.0.0/test/test_fflask.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/test/test_httprequests.py` & `financeager-flask-1.0.0/test/test_httprequests.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/test/test_offline.py` & `financeager-flask-1.0.0/test/test_offline.py`

 * *Files identical despite different names*

### Comparing `financeager-flask-0.5.0.0/test/utils.py` & `financeager-flask-1.0.0/test/utils.py`

 * *Files identical despite different names*

