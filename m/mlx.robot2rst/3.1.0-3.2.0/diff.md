# Comparing `tmp/mlx.robot2rst-3.1.0.tar.gz` & `tmp/mlx.robot2rst-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlx.robot2rst-3.1.0.tar", last modified: Fri Sep 16 08:02:21 2022, max compression
+gzip compressed data, was "dist/mlx.robot2rst-3.2.0.tar", last modified: Tue Apr 25 09:42:07 2023, max compression
```

## Comparing `mlx.robot2rst-3.1.0.tar` & `mlx.robot2rst-3.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/source/example.rst
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/source/requirements.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/doc/source/robot/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/doc/source/robot/example.robot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/mlx/robot2rst.mako
--rw-r--r--   0 runner    (1001) docker     (121)     5902 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/mlx/robot2rst.py
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/mlx/robot_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-09-16 08:02:21.000000 mlx.robot2rst-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-09-16 08:02:05.000000 mlx.robot2rst-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/requirements.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/doc/source/robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/doc/source/robot/example.robot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/mlx/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/robot2rst.mako
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/robot2rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/mlx/robot_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 09:42:06.000000 mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-25 09:42:07.000000 mlx.robot2rst-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-25 09:41:47.000000 mlx.robot2rst-3.2.0/tox.ini
```

### Comparing `mlx.robot2rst-3.1.0/.github/workflows/codeql-analysis.yml` & `mlx.robot2rst-3.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.1.0/.github/workflows/python-package.yml` & `mlx.robot2rst-3.2.0/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,60 +5,60 @@
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox tox-gh-actions
     - name: Build documentation with Sphinx 2.1
-      run: tox -e sphinx-latest
+      run: tox -e sphinx2.1
     - name: Build documentation with latest Sphinx versions
       run: tox -e sphinx-latest
     - name: Static checks
       if: matrix.python-version == 3.9
       run: tox -e check
     - name: Upload HTML documentation
       if: matrix.python-version == 3.9
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: html-doc
         path: doc/_build/html
 
   deploy:
 
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     needs: test
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Download HTML documentation from job 'test'
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: html-doc
         path: doc/_build/html
     - name: Disable jekyll
       run: touch doc/_build/html/.nojekyll
     - name: Deploy documentation
-      uses: JamesIves/github-pages-deploy-action@4.1.3
+      uses: JamesIves/github-pages-deploy-action@v4
       with:
         branch: gh-pages
         folder: doc/_build/html
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.7'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
     - name: Build and publish
```

### Comparing `mlx.robot2rst-3.1.0/.gitignore` & `mlx.robot2rst-3.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -101,8 +101,8 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
 # generated files
-doc/source/example_usage.rst
+doc/source/*_qtp.rst
```

### Comparing `mlx.robot2rst-3.1.0/LICENSE` & `mlx.robot2rst-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.1.0/PKG-INFO` & `mlx.robot2rst-3.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.robot2rst
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python script for converting a Robot Framework file to a reStructuredText (.rst) file
 Home-page: https://github.com/melexis/robot2rst
 Author: Jasper Craeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml/badge.svg?branch=master
             :target: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml
@@ -38,46 +38,51 @@
         
         -----
         Usage
         -----
         
         .. code-block:: console
         
-            robot2rst -i example.robot -o test_plan.rst --prefix ITEST_MY_LIB- --tags SWRQT- SYSRQT- --relationships validates ext_toolname
+            robot2rst -i example.robot -o test_plan.rst --prefix ITEST_MY_LIB- \
+                --tags SWRQT- SYSRQT- --relationships validates ext_toolname --coverage 100 66.66
         
             $ robot2rst --help
         
             usage: robot2rst [-h] -i ROBOT_FILE -o RST_FILE [--only EXPRESSION] [-p PREFIX]
                              [-r [RELATIONSHIPS [RELATIONSHIPS ...]]] [-t [TAGS [TAGS ...]]]
                              [--type TYPE] [--trim-suffix]
         
             Convert robot test cases to reStructuredText with traceable items.
         
-            optional arguments:
+            options:
               -h, --help            show this help message and exit
               -i ROBOT_FILE, --robot ROBOT_FILE
                                     Input robot file
               -o RST_FILE, --rst RST_FILE
-                                    Output RST file
+                                    Output RST file, e.g. my_component_qtp.rst
               --only EXPRESSION     Expression of tags for Sphinx' `only` directive that surrounds all RST
                                     content. By default, no `only` directive is generated.
               -p PREFIX, --prefix PREFIX
                                     Overrides the default 'QTEST-' prefix.
-              -r [RELATIONSHIPS [RELATIONSHIPS ...]], --relationships [RELATIONSHIPS [RELATIONSHIPS ...]]
+              -r [RELATIONSHIPS ...], --relationships [RELATIONSHIPS ...]
                                     Name(s) of the relationship(s) used to link to items in Tags section.
                                     The default value is 'validates'.
-              -t [TAGS [TAGS ...]], --tags [TAGS [TAGS ...]]
-                                    Regex(es) for matching tags to add a relationship link for. All tags get
-                                    matched by default.
+              -t [TAGS ...], --tags [TAGS ...]
+                                    Regex(es) for matching tags to add a relationship link for. All tags
+                                    get matched by default.
+              -c [COVERAGE ...], --coverage [COVERAGE ...]
+                                    Minumum coverage percentages for the item-matrix(es); 1 value per tag
+                                    in -t, --tags.
               --type TYPE           Give value that starts with 'q' or 'i' (case-insensitive) to
-                                    explicitly define the type of test: qualification/integration test. The
-                                    default is 'qualification'.
+                                    explicitly define the type of test: qualification/integration test.
+                                    The default is 'qualification'.
               --trim-suffix         If the suffix of any prefix or --tags argument ends with '_-' it gets
                                     trimmed to '-'.
         
+        
         -------------
         Configuration
         -------------
         
         To include the script's output in your documentation you want to add the aforementioned extension to your
         ``extensions`` list in your *conf.py* like so:
         
@@ -96,23 +101,24 @@
         .. _`mlx.traceability`: https://pypi.org/project/mlx.traceability/
         .. _`documentation of mlx.traceability`: https://melexis.github.io/sphinx-traceability-extension/readme.html
         .. |sphinx_selective_exclude.eager_only| replace:: ``'sphinx_selective_exclude.eager_only'``
         .. _sphinx_selective_exclude.eager_only: https://pypi.org/project/sphinx-selective-exclude/
         
 Keywords: robot,robotframework,sphinx,traceability
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `mlx.robot2rst-3.1.0/README.rst` & `mlx.robot2rst-3.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -30,46 +30,51 @@
 
 -----
 Usage
 -----
 
 .. code-block:: console
 
-    robot2rst -i example.robot -o test_plan.rst --prefix ITEST_MY_LIB- --tags SWRQT- SYSRQT- --relationships validates ext_toolname
+    robot2rst -i example.robot -o test_plan.rst --prefix ITEST_MY_LIB- \
+        --tags SWRQT- SYSRQT- --relationships validates ext_toolname --coverage 100 66.66
 
     $ robot2rst --help
 
     usage: robot2rst [-h] -i ROBOT_FILE -o RST_FILE [--only EXPRESSION] [-p PREFIX]
                      [-r [RELATIONSHIPS [RELATIONSHIPS ...]]] [-t [TAGS [TAGS ...]]]
                      [--type TYPE] [--trim-suffix]
 
     Convert robot test cases to reStructuredText with traceable items.
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -i ROBOT_FILE, --robot ROBOT_FILE
                             Input robot file
       -o RST_FILE, --rst RST_FILE
-                            Output RST file
+                            Output RST file, e.g. my_component_qtp.rst
       --only EXPRESSION     Expression of tags for Sphinx' `only` directive that surrounds all RST
                             content. By default, no `only` directive is generated.
       -p PREFIX, --prefix PREFIX
                             Overrides the default 'QTEST-' prefix.
-      -r [RELATIONSHIPS [RELATIONSHIPS ...]], --relationships [RELATIONSHIPS [RELATIONSHIPS ...]]
+      -r [RELATIONSHIPS ...], --relationships [RELATIONSHIPS ...]
                             Name(s) of the relationship(s) used to link to items in Tags section.
                             The default value is 'validates'.
-      -t [TAGS [TAGS ...]], --tags [TAGS [TAGS ...]]
-                            Regex(es) for matching tags to add a relationship link for. All tags get
-                            matched by default.
+      -t [TAGS ...], --tags [TAGS ...]
+                            Regex(es) for matching tags to add a relationship link for. All tags
+                            get matched by default.
+      -c [COVERAGE ...], --coverage [COVERAGE ...]
+                            Minumum coverage percentages for the item-matrix(es); 1 value per tag
+                            in -t, --tags.
       --type TYPE           Give value that starts with 'q' or 'i' (case-insensitive) to
-                            explicitly define the type of test: qualification/integration test. The
-                            default is 'qualification'.
+                            explicitly define the type of test: qualification/integration test.
+                            The default is 'qualification'.
       --trim-suffix         If the suffix of any prefix or --tags argument ends with '_-' it gets
                             trimmed to '-'.
 
+
 -------------
 Configuration
 -------------
 
 To include the script's output in your documentation you want to add the aforementioned extension to your
 ``extensions`` list in your *conf.py* like so:
```

### Comparing `mlx.robot2rst-3.1.0/doc/Makefile` & `mlx.robot2rst-3.2.0/doc/Makefile`

 * *Files 25% similar despite different names*

```diff
@@ -4,19 +4,28 @@
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = source
 BUILDDIR      = _build
 ROBOT2RST	  = robot2rst
+ROBOT2RST_OPTS += -i $(SOURCEDIR)/robot/example.robot
+ROBOT2RST_OPTS += -o $(SOURCEDIR)/example_usage_qtp.rst
+ROBOT2RST_OPTS += -t ^SWRQT- ^SYSRQT-
+ROBOT2RST_OPTS += -c 100 50.0
+ROBOT2RST_OPTS += -r validates ext_toolname
+ROBOT2RST_OPTS += --only FLASH
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
-.PHONY: help Makefile
+clean:
+	@rm -rf $(BUILDDIR) $(SOURCEDIR)/*_qtp.rst
+
+.PHONY: help Makefile clean
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(ROBOT2RST) -i $(SOURCEDIR)/robot/example.robot -o $(SOURCEDIR)/example_usage.rst -t ^SWRQT- ^SYSRQT- -r validates ext_toolname --only FLASH
+%: Makefile clean
+	@$(ROBOT2RST) $(ROBOT2RST_OPTS)
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `mlx.robot2rst-3.1.0/doc/source/conf.py` & `mlx.robot2rst-3.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.1.0/doc/source/robot/example.robot` & `mlx.robot2rst-3.2.0/doc/source/robot/example.robot`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 *** Settings ***
 Documentation    Example using the space separated plain text format.
 Library          OperatingSystem
 
 *** Variables ***
-${MESSAGE}       Hello, world!
+${NAD}    ${0x63}
+${MESSAGE}       Hello,
+...    world!
 
 *** Test Cases ***
 First Test
-    [Documentation]     Thorough and relatively lengthy documentation for the first example
-    ...  test case.
+    [Documentation]     Thorough and relatively lengthy documentation for the example test case that
+    ...  logs ${MESSAGE} and ${NAD}.
     [Tags]              SWRQT-SOME_RQT  ANOTHER-TAG  SWRQT-OTHER_RQT  SYSRQT-SOME_SYSTEM_RQT
                         Log    ${MESSAGE}
+                        Log    ${NAD}
                         My Keyword    /tmp
 
 Undocumented Test
                         Should Be Equal     ${MESSAGE}    Hello, world!
 
 Test with documentation in RST syntax
     [Documentation]     An example docstring for which it's important its line endings get preserved.
```

### Comparing `mlx.robot2rst-3.1.0/mlx/robot2rst.mako` & `mlx.robot2rst-3.2.0/mlx/robot2rst.mako`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 <%
 import re
 
+title = suite
+match = re.match(r"(.+)_[qi]tp", suite)
+if match:
+    title = f"{test_type.capitalize()} Test Plan for {match.group(1)}"
+
 def to_traceable_item(name, prefix=''):
     '''
     Converts a name, to the name of a traceabile item
 
     Args:
         name (str): The string to convert
 
@@ -32,39 +37,42 @@
 
     Returns:
         str: Body of the item, which is the input string with an added indent of four spaces
     '''
     indent = ' ' * 4
     newline = '\n'
     line_separator = newline + indent
+    for variable, value in parser.variables.items():
+        if variable in input_string:
+            input_string = input_string.replace(variable, value)
     input_string = input_string.replace(r'\r', '').strip()
     lines = input_string.split(newline)
     intermediate_output = indent
     for line in lines:
         if line:
             intermediate_output += line.rstrip()
         else:
             intermediate_output =  intermediate_output.rstrip(' ')
         intermediate_output += line_separator
     return intermediate_output.rstrip()
 %>\
 .. _${suite.replace(' ', '_')}:
 
-${'='*len(suite)}
-${suite}
-${'='*len(suite)}
+${'='*len(title)}
+${title}
+${'='*len(title)}
 
 .. contents:: `Contents`
     :depth: 2
     :local:
 
 
-% for test in tests:
+% for test in parser.tests:
 .. item:: ${to_traceable_item(test.name, prefix)} ${test.name}
-% for relationship, tag_regex in relationship_to_tag_mapping.items():
+% for relationship, tag_regex, _ in relationship_config:
 <%
 filtered_tags = [tag for tag in test.tags if re.search(tag_regex, tag)]
 %>\
     % if filtered_tags:
     :${relationship}: ${' '.join(filtered_tags)}
     % endif
 % endfor
@@ -75,22 +83,25 @@
 %endif
 % endfor
 
 % if gen_matrix:
 Traceability Matrix
 ===================
 
-% for relationship, tag_regex in relationship_to_tag_mapping.items():
+% for relationship, tag_regex, coverage in relationship_config:
 The below table traces the ${test_type} test cases to the ${relationship} requirements.
 
 .. item-matrix:: Linking these ${test_type} test cases to the ${relationship} requirements
     :source: ${prefix}
     :target: ${tag_regex}
     :sourcetitle: ${test_type.capitalize()} test case
     :targettitle: ${relationship} requirement
     :type: ${relationship}
     :stats:
     :group: top
     :nocaptions:
+    % if coverage:
+    :coverage: >= ${coverage}
+    % endif
 
 % endfor
 % endif
```

### Comparing `mlx.robot2rst-3.1.0/mlx/robot2rst.py` & `mlx.robot2rst-3.2.0/mlx/robot2rst.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 ''' Script to convert a robot test file to a reStructuredText file with traceable items '''
 import argparse
 import logging
+import sys
 from textwrap import indent
 from pathlib import Path
 
 from mako.exceptions import RichTraceback
 from mako.template import Template
 
-from .robot_parser import extract_tests
+from .robot_parser import ParserApplication
 
 TEMPLATE_FILE = Path(__file__).parent.joinpath('robot2rst.mako')
 LOGGER = logging.getLogger(__name__)
 
 
 def render_template(destination, only="", **kwargs):
     """
@@ -25,42 +26,44 @@
     Raises:
         CRITICAL: Error was raised by Mako template.
     """
     destination.parent.mkdir(parents=True, exist_ok=True)
     template = Template(filename=str(TEMPLATE_FILE))
     try:
         rst_content = template.render(**kwargs)
-    except Exception:
+    except Exception as err:
         traceback = RichTraceback()
-        for entry in traceback.traceback[-2:]:
-            LOGGER.critical("File %s, line %s, in %s: %r", *entry)
+        LOGGER.critical("File %s, line %s, in %s: %r", *traceback.traceback[-1])
+        LOGGER.critical(repr(err))
+        return 1
     else:
         if only:
             rst_content = f".. only:: {only}\n\n{indent(rst_content, ' ' * 4)}"
         with open(str(destination), 'w', encoding='utf-8', newline='\n') as rst_file:
             rst_file.write(rst_content)
+    return 0
 
 
-def generate_robot_2_rst(robot_file, rst_file, prefix, relationship_to_tag_mapping, gen_matrix, **kwargs):
+def generate_robot_2_rst(parser, rst_file, prefix, relationship_config, gen_matrix, **kwargs):
     """
     Calls mako template function and passes all needed parameters.
 
     Args:
-        robot_file (Path): Path to the input file (.robot).
+        parser (ParserApplication): Parser with data extracted from the .robot file
         rst_file (Path): Path to the output file (.rst).
         prefix (str): Prefix of generated item IDs.
-        relationship_to_tag_mapping (dict): Dictionary that maps each relationship to the corresponding tag regex.
+        relationship_config (list): List of tuples that contain a relationship, tag_regex and coverage percentage
         gen_matrix (bool): True if traceability matrices are to be generated, False if not.
     """
-    render_template(
+    return render_template(
         rst_file,
-        tests=extract_tests(str(robot_file.resolve(strict=True))),
+        parser=parser,
         suite=rst_file.stem,
         prefix=prefix,
-        relationship_to_tag_mapping=relationship_to_tag_mapping,
+        relationship_config=relationship_config,
         gen_matrix=gen_matrix,
         **kwargs,
     )
 
 
 def _tweak_prefix(prefix):
     """ If a prefix or regex ends with '_-', change it to end with '-' instead.
@@ -75,64 +78,74 @@
         prefix = prefix.rstrip('_-') + '-'
     return prefix
 
 
 def main():
     '''Main entry point for script: parse arguments and execute'''
     parser = argparse.ArgumentParser(description='Convert robot test cases to reStructuredText with traceable items.')
-    parser.add_argument("-i", "--robot", dest='robot_file', help='Input robot file', required=True,
-                        action='store')
-    parser.add_argument("-o", "--rst", dest='rst_file', help='Output RST file', required=True,
-                        action='store')
+    parser.add_argument("-i", "--robot", dest='robot_file', required=True,
+                        help='Input robot file')
+    parser.add_argument("-o", "--rst", dest='rst_file', required=True,
+                        help='Output RST file, e.g. my_component_qtp.rst')
     parser.add_argument("--only", dest="expression", default="",
                         help="Expression of tags for Sphinx' `only` directive that surrounds all RST content. "
                         "By default, no `only` directive is generated.")
-    parser.add_argument("-p", "--prefix", action='store', default='QTEST-',
+    parser.add_argument("-p", "--prefix", default='QTEST-',
                         help="Overrides the default 'QTEST-' prefix.")
     parser.add_argument("-r", "--relationships", nargs='*',
                         help="Name(s) of the relationship(s) used to link to items in Tags section. The default value "
                              "is 'validates'.")
     parser.add_argument("-t", "--tags", nargs='*',
                         help="Regex(es) for matching tags to add a relationship link for. All tags get matched by "
                              "default.")
+    parser.add_argument("-c", "--coverage", nargs='*',
+                        help="Minumum coverage percentages for the item-matrix(es); 1 value per tag in -t, --tags.")
     parser.add_argument("--type", default='q',
                         help="Give value that starts with 'q' or 'i' (case-insensitive) to explicitly define "
                              "the type of test: qualification/integration test. The default is 'qualification'.")
     parser.add_argument("--trim-suffix", action='store_true',
                         help="If the suffix of any prefix or --tags argument ends with '_-' it gets trimmed to '-'.")
 
     logging.basicConfig(level=logging.INFO)
     args = parser.parse_args()
-    gen_matrix = True
-    if not args.tags:
-        args.tags = ['.*']
-        gen_matrix = False
-        LOGGER.warning("No traceability matrix will be generated because of the use of default tag regex %r.",
-                       args.tags[0])
-    if not args.relationships:
-        args.relationships = ['validates']
 
     type_map = {
         'i': 'integration',
         'q': 'qualification',
     }
     if args.type and args.type.lower()[0] in type_map:
         test_type = type_map[args.type.lower()[0]]
     else:
         raise ValueError(f"The --type argument is invalid: expected a value that starts with {' or '.join(type_map)}; "
                          f"got {args.type.lower()!r}.")
 
+    relationships = args.relationships if args.relationships else ['validates']
+    coverages = args.coverage if args.coverage else [0] * len(relationships)
     prefix = _tweak_prefix(args.prefix) if args.trim_suffix else args.prefix
+    gen_matrix = True
+    if not args.tags:
+        args.tags = ['.*']  # only one relationship shall be used
+        gen_matrix = False
+        LOGGER.warning("No traceability matrix will be generated because of the use of default tag regex %r.",
+                       args.tags[0])
     tag_regexes = [_tweak_prefix(regex) if args.trim_suffix else regex for regex in args.tags]
-    relationships = args.relationships
 
     if len(relationships) != len(tag_regexes):
         raise ValueError(f"Number of relationships ({len(relationships)}) is not equal to number of tag regexes "
-                         f"({len(tag_regexes)}) given.")
-    relationship_to_tag_mapping = dict(zip(relationships, tag_regexes))
+                         f"({len(tag_regexes)}).")
+    if len(relationships) != len(coverages):
+        raise ValueError(f"Number of relationships ({len(relationships)}) is not equal to number of coverage "
+                         f"percentages ({len(coverages)}).")
+    relationship_config = [(relationships[i], tag_regexes[i], coverages[i]) for i in range(len(relationships))]
+
+    parser = ParserApplication(Path(args.robot_file))
+    parser.run()
+    return generate_robot_2_rst(parser, Path(args.rst_file), prefix, relationship_config,
+                                gen_matrix, test_type=test_type, only=args.expression, coverages=coverages)
+
 
-    generate_robot_2_rst(Path(args.robot_file), Path(args.rst_file), prefix, relationship_to_tag_mapping, gen_matrix,
-                         test_type=test_type, only=args.expression)
+def entrypoint():
+    sys.exit(main())
 
 
 if __name__ == "__main__":
-    main()
+    entrypoint()
```

### Comparing `mlx.robot2rst-3.1.0/mlx/robot_parser.py` & `mlx.robot2rst-3.2.0/mlx/robot_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-from ast import NodeVisitor
+import re
 from collections import namedtuple
 
 from robot.api import get_model, Token
+from robot.parsing import ModelVisitor
 
 
-def extract_tests(robot_file):
-    """ Extracts all useful information from the tests in the .robot file.
+class ParserApplication(ModelVisitor):
+    """ Class used to extract all useful info from the .robot file.
 
-    Args:
-        robot_file (str): Path to the .robot file.
+    See https://robot-framework.readthedocs.io/en/v6.0.2/autodoc/robot.api.html#inspecting-model
 
-    Returns:
-        list: List of objects with attributes name (str), doc (str) and tags (list).
-    """
-    model = get_model(robot_file)
-    parser = TestCaseParser()
-    parser.visit(model)
-    return parser.tests
-
-
-class TestCaseParser(NodeVisitor):
-    """ Class used to extract all useful info from test cases.
-
-    See https://robot-framework.readthedocs.io/en/latest/autodoc/robot.parsing.html#parsing-data-to-model
+    Attributes:
+        tests (list): List of objects with attributes name (str), doc (str) and tags (list).
+        variables (dict): Dictionary mapping variables, e.g. '${MESSAGE}', to their values
     """
     TestAttributes = namedtuple('TestAttributes', 'name doc tags')
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, robot_file, *args, **kwargs):
+        """ Constructor
+
+        Args:
+            robot_file (Path): Path to the .robot file.
+        """
         super().__init__(*args, **kwargs)
+        self.robot_file = str(robot_file.resolve(strict=True))
+        self.model = get_model(self.robot_file)
         self.tests = []
+        self.variables = {}
+
+    def run(self):
+        self.visit(self.model)
+
+    def visit_VariableSection(self, node):
+        for element in node.body:
+            if getattr(element, 'type') == Token.VARIABLE:
+                name = element.get_value(Token.VARIABLE)
+                value = ' '.join(element.get_values(Token.ARGUMENT))
+                match = re.fullmatch(r"\${(.+)}", value)
+                if match:
+                    value = match.group(1)
+                self.variables[name] = value
 
     def visit_TestCase(self, node):
         doc = ''
         tags = []
         for element in node.body:
-            if not hasattr(element, 'type'):
-                continue
-            if element.type == Token.DOCUMENTATION:
+            if getattr(element, 'type') == Token.DOCUMENTATION:
                 in_docstring = False
                 previous_token = None
                 for token in element.tokens:
                     if in_docstring and token.type in (Token.ARGUMENT, Token.EOL, Token.SEPARATOR):
                         if previous_token is None or previous_token.type != Token.CONTINUATION:
                             doc += token.value
                         elif len(token.value) > 2:
```

### Comparing `mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/PKG-INFO` & `mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx.robot2rst
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python script for converting a Robot Framework file to a reStructuredText (.rst) file
 Home-page: https://github.com/melexis/robot2rst
 Author: Jasper Craeghs
 Author-email: jce@melexis.com
 License: Apache License Version 2.0
 Description: .. image:: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml/badge.svg?branch=master
             :target: https://github.com/melexis/robot2rst/actions/workflows/python-package.yml
@@ -38,46 +38,51 @@
         
         -----
         Usage
         -----
         
         .. code-block:: console
         
-            robot2rst -i example.robot -o test_plan.rst --prefix ITEST_MY_LIB- --tags SWRQT- SYSRQT- --relationships validates ext_toolname
+            robot2rst -i example.robot -o test_plan.rst --prefix ITEST_MY_LIB- \
+                --tags SWRQT- SYSRQT- --relationships validates ext_toolname --coverage 100 66.66
         
             $ robot2rst --help
         
             usage: robot2rst [-h] -i ROBOT_FILE -o RST_FILE [--only EXPRESSION] [-p PREFIX]
                              [-r [RELATIONSHIPS [RELATIONSHIPS ...]]] [-t [TAGS [TAGS ...]]]
                              [--type TYPE] [--trim-suffix]
         
             Convert robot test cases to reStructuredText with traceable items.
         
-            optional arguments:
+            options:
               -h, --help            show this help message and exit
               -i ROBOT_FILE, --robot ROBOT_FILE
                                     Input robot file
               -o RST_FILE, --rst RST_FILE
-                                    Output RST file
+                                    Output RST file, e.g. my_component_qtp.rst
               --only EXPRESSION     Expression of tags for Sphinx' `only` directive that surrounds all RST
                                     content. By default, no `only` directive is generated.
               -p PREFIX, --prefix PREFIX
                                     Overrides the default 'QTEST-' prefix.
-              -r [RELATIONSHIPS [RELATIONSHIPS ...]], --relationships [RELATIONSHIPS [RELATIONSHIPS ...]]
+              -r [RELATIONSHIPS ...], --relationships [RELATIONSHIPS ...]
                                     Name(s) of the relationship(s) used to link to items in Tags section.
                                     The default value is 'validates'.
-              -t [TAGS [TAGS ...]], --tags [TAGS [TAGS ...]]
-                                    Regex(es) for matching tags to add a relationship link for. All tags get
-                                    matched by default.
+              -t [TAGS ...], --tags [TAGS ...]
+                                    Regex(es) for matching tags to add a relationship link for. All tags
+                                    get matched by default.
+              -c [COVERAGE ...], --coverage [COVERAGE ...]
+                                    Minumum coverage percentages for the item-matrix(es); 1 value per tag
+                                    in -t, --tags.
               --type TYPE           Give value that starts with 'q' or 'i' (case-insensitive) to
-                                    explicitly define the type of test: qualification/integration test. The
-                                    default is 'qualification'.
+                                    explicitly define the type of test: qualification/integration test.
+                                    The default is 'qualification'.
               --trim-suffix         If the suffix of any prefix or --tags argument ends with '_-' it gets
                                     trimmed to '-'.
         
+        
         -------------
         Configuration
         -------------
         
         To include the script's output in your documentation you want to add the aforementioned extension to your
         ``extensions`` list in your *conf.py* like so:
         
@@ -96,23 +101,24 @@
         .. _`mlx.traceability`: https://pypi.org/project/mlx.traceability/
         .. _`documentation of mlx.traceability`: https://melexis.github.io/sphinx-traceability-extension/readme.html
         .. |sphinx_selective_exclude.eager_only| replace:: ``'sphinx_selective_exclude.eager_only'``
         .. _sphinx_selective_exclude.eager_only: https://pypi.org/project/sphinx-selective-exclude/
         
 Keywords: robot,robotframework,sphinx,traceability
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `mlx.robot2rst-3.1.0/mlx.robot2rst.egg-info/SOURCES.txt` & `mlx.robot2rst-3.2.0/mlx.robot2rst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlx.robot2rst-3.1.0/setup.py` & `mlx.robot2rst-3.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,37 +14,38 @@
     author_email='jce@melexis.com',
     license='Apache License Version 2.0',
     description='Python script for converting a Robot Framework file to a reStructuredText (.rst) file',
     long_description=open("README.rst").read(),
     long_description_content_type='text/x-rst',
     zip_safe=False,
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Documentation',
         'Topic :: Documentation :: Sphinx',
         'Topic :: Utilities',
     ],
     platforms='any',
     packages=find_packages(exclude=['tests', 'doc']),
     include_package_data=True,
     install_requires=requires,
     setup_requires=['setuptools_scm'],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     namespace_packages=['mlx'],
     keywords=['robot', 'robotframework', 'sphinx', 'traceability'],
     entry_points={
         'console_scripts': [
-            'mlx.robot2rst = mlx.robot2rst:main',
-            'robot2rst = mlx.robot2rst:main',
+            'mlx.robot2rst = mlx.robot2rst:entrypoint',
+            'robot2rst = mlx.robot2rst:entrypoint',
         ]
     },
 )
```

### Comparing `mlx.robot2rst-3.1.0/tox.ini` & `mlx.robot2rst-3.2.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tox]
 envlist =
     check,
-    py36, py37, py38, py39,
+    py37, py38, py39, py310, py311
     sphinx2.1,
     sphinx-latest,
 
 [gh-actions]
 python =
-    3.6: py36
     3.7: py37
     3.8: py38
     3.9: py39
-    {sphinx2.1,sphinx-latest},
+    3.10: py310
+    3.11: py311
 
 [testenv]
 basepython =
     py: python3
-    py36: {env:TOXPYTHON:python3.6}
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
     py39: {env:TOXPYTHON:python3.9}
+    py310: {env:TOXPYTHON:python3.10}
+    py311: {env:TOXPYTHON:python3.11}
     {check,sphinx2.1,sphinx-latest}: python3
 passenv =
     *
 usedevelop = true
 deps=
     mock
     mako
@@ -42,33 +43,30 @@
     twine check --strict dist/*
     check-manifest {toxinidir} -u
     flake8 mlx setup.py
 
 [testenv:sphinx2.1]
 deps=
     {[testenv]deps}
+    jinja2 == 2.11.3
+    markupsafe == 1.1.0
+    docutils == 0.17
     sphinx <= 2.1.9999
-    mlx.warnings >= 1.2.0
+    mlx.warnings >= 4.3.2
     sphinx_selective_exclude >= 1.0.3
 whitelist_externals =
-    bash
     make
-    tee
     mlx-warnings
 commands=
-    bash -c 'make -C doc html 2>&1 | tee .tox/doc_html.log'
-    mlx-warnings --sphinx --maxwarnings 0 --minwarnings 0 .tox/doc_html.log
+    mlx-warnings --sphinx --exact-warnings 1 --command make -C doc html
 
 [testenv:sphinx-latest]
 deps=
     {[testenv]deps}
     sphinx
-    mlx.warnings >= 1.2.0
+    mlx.warnings >= 4.3.2
     sphinx_selective_exclude >= 1.0.3
 whitelist_externals =
-    bash
     make
-    tee
     mlx-warnings
 commands=
-    bash -c 'make -C doc html 2>&1 | tee .tox/doc_html.log'
-    mlx-warnings --sphinx --maxwarnings 0 --minwarnings 0 .tox/doc_html.log
+    mlx-warnings --sphinx --exact-warnings 1 --command make -C doc html
```

