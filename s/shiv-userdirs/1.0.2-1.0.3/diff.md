# Comparing `tmp/shiv-userdirs-1.0.2.tar.gz` & `tmp/shiv-userdirs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiv-userdirs-1.0.2.tar", last modified: Thu May 19 12:07:41 2022, max compression
+gzip compressed data, was "shiv-userdirs-1.0.3.tar", last modified: Tue Apr 25 09:55:54 2023, max compression
```

## Comparing `shiv-userdirs-1.0.2.tar` & `shiv-userdirs-1.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1326 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/LICENSE
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      155 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/MANIFEST.in
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      174 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/NOTICE
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     4573 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/PKG-INFO
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     3852 2022-05-19 11:06:39.000000 shiv-userdirs-1.0.2/README.md
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/docs/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      731 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/docs/api.rst
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1192 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/docs/cli-reference.rst
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     2008 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/docs/django.rst
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     3014 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/docs/history.rst
--rw-rw-r--   0 manfred   (1000) manfred   (1000)    10913 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/docs/index.rst
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      117 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/pyproject.toml
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1550 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/setup.cfg
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.414505 shiv-userdirs-1.0.2/src/
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/src/shiv/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)        0 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/__init__.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      139 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/__main__.py
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/src/shiv/bootstrap/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     9402 2022-05-19 11:40:13.000000 shiv-userdirs-1.0.2/src/shiv/bootstrap/__init__.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     2878 2022-05-19 11:06:19.000000 shiv-userdirs-1.0.2/src/shiv/bootstrap/environment.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     2063 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/bootstrap/filelock.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1762 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/bootstrap/interpreter.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     6032 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/builder.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     9518 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/cli.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1586 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/constants.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1010 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/info.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1983 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/src/shiv/pip.py
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     4573 2022-05-19 12:07:41.000000 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/PKG-INFO
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      847 2022-05-19 12:07:41.000000 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/SOURCES.txt
--rw-rw-r--   0 manfred   (1000) manfred   (1000)        1 2022-05-19 12:07:41.000000 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/dependency_links.txt
--rw-rw-r--   0 manfred   (1000) manfred   (1000)       66 2022-05-19 12:07:41.000000 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/entry_points.txt
--rw-rw-r--   0 manfred   (1000) manfred   (1000)       86 2022-05-19 12:07:41.000000 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/requires.txt
--rw-rw-r--   0 manfred   (1000) manfred   (1000)        5 2022-05-19 12:07:41.000000 shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/top_level.txt
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/test/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      917 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/conftest.py
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/test/package/
-drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2022-05-19 12:07:41.418505 shiv-userdirs-1.0.2/test/package/hello/
--rw-rw-r--   0 manfred   (1000) manfred   (1000)       37 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/package/hello/__init__.py
--rwxrwxr-x   0 manfred   (1000) manfred   (1000)       28 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/package/hello/script.sh
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      200 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/package/setup.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      342 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/test.zip
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     6765 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/test_bootstrap.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)     1934 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/test_builder.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)    14303 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/test_cli.py
--rw-rw-r--   0 manfred   (1000) manfred   (1000)      379 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.2/test/test_pip.py
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1326 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/LICENSE
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      155 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/MANIFEST.in
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      174 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/NOTICE
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     4764 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/PKG-INFO
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     3911 2023-04-25 09:47:29.000000 shiv-userdirs-1.0.3/README.md
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.482508 shiv-userdirs-1.0.3/docs/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      731 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/docs/api.rst
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1192 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/docs/cli-reference.rst
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     2008 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/docs/django.rst
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     3015 2023-04-25 09:47:29.000000 shiv-userdirs-1.0.3/docs/history.rst
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)    10914 2023-04-25 09:47:29.000000 shiv-userdirs-1.0.3/docs/index.rst
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      117 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/pyproject.toml
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1671 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/setup.cfg
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.478507 shiv-userdirs-1.0.3/src/
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.482508 shiv-userdirs-1.0.3/src/shiv/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)        0 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/__init__.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      139 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/__main__.py
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.482508 shiv-userdirs-1.0.3/src/shiv/bootstrap/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     9570 2023-04-25 09:49:34.000000 shiv-userdirs-1.0.3/src/shiv/bootstrap/__init__.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     2878 2022-05-19 11:06:19.000000 shiv-userdirs-1.0.3/src/shiv/bootstrap/environment.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     2063 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/bootstrap/filelock.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1762 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/bootstrap/interpreter.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     6226 2023-04-25 09:49:34.000000 shiv-userdirs-1.0.3/src/shiv/builder.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     9518 2023-04-25 09:49:34.000000 shiv-userdirs-1.0.3/src/shiv/cli.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1586 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/constants.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1010 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/info.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1983 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/src/shiv/pip.py
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     4764 2023-04-25 09:55:54.000000 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/PKG-INFO
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      847 2023-04-25 09:55:54.000000 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/SOURCES.txt
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)        1 2023-04-25 09:55:54.000000 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/dependency_links.txt
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)       66 2023-04-25 09:55:54.000000 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/entry_points.txt
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)       86 2023-04-25 09:55:54.000000 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/requires.txt
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)        5 2023-04-25 09:55:54.000000 shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/top_level.txt
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/test/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      917 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/conftest.py
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/test/package/
+drwxrwxr-x   0 manfred   (1000) manfred   (1000)        0 2023-04-25 09:55:54.486508 shiv-userdirs-1.0.3/test/package/hello/
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)       37 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/package/hello/__init__.py
+-rwxrwxr-x   0 manfred   (1000) manfred   (1000)       28 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/package/hello/script.sh
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      200 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/package/setup.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      342 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/test.zip
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     6765 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/test_bootstrap.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)     1934 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/test_builder.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)    14303 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/test_cli.py
+-rw-rw-r--   0 manfred   (1000) manfred   (1000)      379 2022-05-19 06:22:03.000000 shiv-userdirs-1.0.3/test/test_pip.py
```

### Comparing `shiv-userdirs-1.0.2/LICENSE` & `shiv-userdirs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/PKG-INFO` & `shiv-userdirs-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: shiv-userdirs
-Version: 1.0.2
-Summary: Python SHIV-version, which creates user owned directires if SHIV_ROOT is used.
+Version: 1.0.3
+Summary: Python SHIV-version, which creates user owned directires if SHIV_ROOT is used. SHIV is a command line utility for building fully self contained Python zipapps.
 Home-page: https://github.com/manfred-kaiser/shiv
 Author: Manfred Kaiser
 Author-email: manfred.kaiser@ssh-mitm.at
 License: BSD License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pypi](https://img.shields.io/pypi/v/shiv.svg)](https://pypi.python.org/pypi/shiv)
 [![ci](https://github.com/linkedin/shiv/workflows/ci/badge.svg)](https://github.com/linkedin/shiv/actions?query=workflow%3Aci)
 [![codecov](https://codecov.io/gh/linkedin/shiv/branch/master/graph/badge.svg)](https://codecov.io/gh/linkedin/shiv)
@@ -96,15 +97,17 @@
 We'd love contributions! Getting bootstrapped to develop is easy:
 
 ```sh
 git clone git@github.com:linkedin/shiv.git
 cd shiv
 python3 -m venv venv
 source ./venv/bin/activate
-python3 setup.py develop
+python3 -m pip install --upgrade build
+python3 -m build
+python3 -m pip install -e .
 ```
 
 Don't forget to run and write tests:
 
 ```sh
 python3 -m pip install tox
 tox
```

### Comparing `shiv-userdirs-1.0.2/README.md` & `shiv-userdirs-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -77,15 +77,17 @@
 We'd love contributions! Getting bootstrapped to develop is easy:
 
 ```sh
 git clone git@github.com:linkedin/shiv.git
 cd shiv
 python3 -m venv venv
 source ./venv/bin/activate
-python3 setup.py develop
+python3 -m pip install --upgrade build
+python3 -m build
+python3 -m pip install -e .
 ```
 
 Don't forget to run and write tests:
 
 ```sh
 python3 -m pip install tox
 tox
```

### Comparing `shiv-userdirs-1.0.2/docs/api.rst` & `shiv-userdirs-1.0.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/docs/cli-reference.rst` & `shiv-userdirs-1.0.3/docs/cli-reference.rst`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/docs/django.rst` & `shiv-userdirs-1.0.3/docs/django.rst`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/docs/history.rst` & `shiv-userdirs-1.0.3/docs/history.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Motivation & Comparisons
 ========================
 
 Why?
 ----
 
 At LinkedIn we ship hundreds of command line utilities to every machine in our data-centers and all
-of our employees workstations. The vast majority of these utilties are written in Python. In
+of our employees workstations. The vast majority of these utilities are written in Python. In
 addition to these utilities we also have many internal libraries that are uprev'd daily.
 
 Because of differences in iteration rate and the inherent problems present when dealing with such a
 huge dependency graph, we need to package the executables discretely. Initially we took advantage
 of the great open source tool `PEX <https://github.com/pantsbuild/pex>`_. PEX elegantly solved the
 isolated packaging requirement we had by including all of a tool's dependencies inside of a single
 binary file that we could then distribute!
```

### Comparing `shiv-userdirs-1.0.2/docs/index.rst` & `shiv-userdirs-1.0.3/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 For such a use case, ``shiv`` provides a ``--preamble`` flag.
 Any executable script passed to that flag will be packed into the zipapp and invoked during bootstrapping (*after* extracting dependencies but *before* invoking an entry point / console script).
 
 If the preamble file is written in Python (e.g. ends in ``.py``) then shiv will inject three variables into the runtime that may be useful to preamble authors:
 
 * ``archive``: (a string) path to the current PYZ file
 * ``env``: an instance of the `Environment <api:bootstrap.environment.Environment>`_ object.
-* ``site_packages``: a :py:class:`pathlib.Path` of the directory where the current PYZ's site_packages were extracted to during bootsrap.
+* ``site_packages``: a :py:class:`pathlib.Path` of the directory where the current PYZ's site_packages were extracted to during bootstrap.
 
 For an example, a preamble file that cleans up prior extracted ``~/.shiv`` directories might look like:
 
 .. code-block:: py
 
     #!/usr/bin/env python3
```

### Comparing `shiv-userdirs-1.0.2/setup.cfg` & `shiv-userdirs-1.0.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 include_trailing_comma = true
 use_parentheses = true
 not_skip = __init__.py
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [metadata]
 name = shiv-userdirs
-version = 1.0.2
-description = Python SHIV-version, which creates user owned directires if SHIV_ROOT is used.
+version = 1.0.3
+description = Python SHIV-version, which creates user owned directires if SHIV_ROOT is used. SHIV is a command line utility for building fully self contained Python zipapps.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/manfred-kaiser/shiv
 author = Manfred Kaiser
 author_email = manfred.kaiser@ssh-mitm.at
 license = BSD License
 license_file = LICENSE
@@ -37,14 +37,15 @@
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	click>=6.7,!=7.0
```

### Comparing `shiv-userdirs-1.0.2/src/shiv/bootstrap/__init__.py` & `shiv-userdirs-1.0.3/src/shiv/bootstrap/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,28 +218,34 @@
 
     # get sys.path's length
     length = len(sys.path)
 
     # Find the first instance of an existing site-packages on sys.path
     index = get_first_sitedir_index() or length
 
+    # copy sys.path to determine diff
+    sys_path_before = sys.path.copy()
+
     # append site-packages using the stdlib blessed way of extending path
     # so as to handle .pth files correctly
     site.addsitedir(site_packages)
 
     # reorder to place our site-packages before any others found
     sys.path = sys.path[:index] + sys.path[length:] + sys.path[index:length]
 
+    # determine newly added paths
+    new_paths = [p for p in sys.path if p not in sys_path_before]
+
     # check if source files have been modified, if required
     if env.no_modify:
         ensure_no_modify(site_packages, env.hashes)
 
-    # add our site-packages to the environment, if requested
+    # add any new paths to the environment, if requested
     if env.extend_pythonpath:
-        extend_python_path(os.environ, sys.path.copy())
+        extend_python_path(os.environ, new_paths)
 
     # if a preamble script was provided, run it
     if env.preamble:
 
         # path to the preamble
         preamble_bin = site_packages / "bin" / env.preamble
```

### Comparing `shiv-userdirs-1.0.2/src/shiv/bootstrap/environment.py` & `shiv-userdirs-1.0.3/src/shiv/bootstrap/environment.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/src/shiv/bootstrap/filelock.py` & `shiv-userdirs-1.0.3/src/shiv/bootstrap/filelock.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/src/shiv/bootstrap/interpreter.py` & `shiv-userdirs-1.0.3/src/shiv/bootstrap/interpreter.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/src/shiv/builder.py` & `shiv-userdirs-1.0.3/src/shiv/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,16 @@
                     if path.suffix == ".pyc" or path.is_dir():
                         continue
 
                     data = path.read_bytes()
 
                     # update the contents hash
                     contents_hash.update(data)
+                    # take filenames into account as well - build_id should change if a file is moved or renamed
+                    contents_hash.update(str(path.relative_to(source)).encode())
 
                     arcname = str(site_packages / path.relative_to(source))
 
                     write_to_zipapp(archive, arcname, data, zipinfo_datetime, compression, stat=path.stat())
 
             if env.build_id is None:
                 # Now that we have a hash of all the source files, use it as our build id if the user did not
@@ -149,15 +151,15 @@
                             compression,
                             stat=path.stat(),
                         )
 
             # Write environment info in json file.
             #
             # The environment file contains build_id which is a SHA-256 checksum of all **site-packages** contents.
-            # the bootstarp code, environment.json and __main__.py are not used to calculate the checksum, is it's
+            # the bootstrap code, environment.json and __main__.py are not used to calculate the checksum, is it's
             # only used for local caching of site-packages and these files are always read from archive.
             write_to_zipapp(archive, "environment.json", env.to_json().encode("utf-8"), zipinfo_datetime, compression)
 
             # write __main__
             write_to_zipapp(archive, "__main__.py", main_py.encode("utf-8"), zipinfo_datetime, compression)
 
     # Make pyz executable (on windows this is no-op).
```

### Comparing `shiv-userdirs-1.0.2/src/shiv/cli.py` & `shiv-userdirs-1.0.3/src/shiv/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     NO_ENTRY_POINT,
     NO_OUTFILE,
     NO_PIP_ARGS_OR_SITE_PACKAGES,
     SOURCE_DATE_EPOCH_DEFAULT,
     SOURCE_DATE_EPOCH_ENV,
 )
 
-__version__ = "1.0.1"
+__version__ = "1.0.3"
 
 
 def find_entry_point(site_packages_dirs: List[Path], console_script: str) -> str:
     """Find a console_script in a site-packages directory.
 
     Console script metadata is stored in entry_points.txt per setuptools
     convention. This function searches all entry_points.txt files and
```

### Comparing `shiv-userdirs-1.0.2/src/shiv/constants.py` & `shiv-userdirs-1.0.3/src/shiv/constants.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/src/shiv/info.py` & `shiv-userdirs-1.0.3/src/shiv/info.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/src/shiv/pip.py` & `shiv-userdirs-1.0.3/src/shiv/pip.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/PKG-INFO` & `shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: shiv-userdirs
-Version: 1.0.2
-Summary: Python SHIV-version, which creates user owned directires if SHIV_ROOT is used.
+Version: 1.0.3
+Summary: Python SHIV-version, which creates user owned directires if SHIV_ROOT is used. SHIV is a command line utility for building fully self contained Python zipapps.
 Home-page: https://github.com/manfred-kaiser/shiv
 Author: Manfred Kaiser
 Author-email: manfred.kaiser@ssh-mitm.at
 License: BSD License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pypi](https://img.shields.io/pypi/v/shiv.svg)](https://pypi.python.org/pypi/shiv)
 [![ci](https://github.com/linkedin/shiv/workflows/ci/badge.svg)](https://github.com/linkedin/shiv/actions?query=workflow%3Aci)
 [![codecov](https://codecov.io/gh/linkedin/shiv/branch/master/graph/badge.svg)](https://codecov.io/gh/linkedin/shiv)
@@ -96,15 +97,17 @@
 We'd love contributions! Getting bootstrapped to develop is easy:
 
 ```sh
 git clone git@github.com:linkedin/shiv.git
 cd shiv
 python3 -m venv venv
 source ./venv/bin/activate
-python3 setup.py develop
+python3 -m pip install --upgrade build
+python3 -m build
+python3 -m pip install -e .
 ```
 
 Don't forget to run and write tests:
 
 ```sh
 python3 -m pip install tox
 tox
```

### Comparing `shiv-userdirs-1.0.2/src/shiv_userdirs.egg-info/SOURCES.txt` & `shiv-userdirs-1.0.3/src/shiv_userdirs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/test/conftest.py` & `shiv-userdirs-1.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/test/test_bootstrap.py` & `shiv-userdirs-1.0.3/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/test/test_builder.py` & `shiv-userdirs-1.0.3/test/test_builder.py`

 * *Files identical despite different names*

### Comparing `shiv-userdirs-1.0.2/test/test_cli.py` & `shiv-userdirs-1.0.3/test/test_cli.py`

 * *Files identical despite different names*

