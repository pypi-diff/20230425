# Comparing `tmp/airbase-0.6.0.tar.gz` & `tmp/airbase-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbase-0.6.0.tar", last modified: Thu Oct 27 14:17:13 2022, max compression
+gzip compressed data, was "airbase-0.7.0.tar", last modified: Tue Apr 25 08:26:54 2023, max compression
```

## Comparing `airbase-0.6.0.tar` & `airbase-0.7.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.152813 airbase-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.100813 airbase-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.104813 airbase-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-10-27 14:16:59.000000 airbase-0.6.0/.github/workflows/cicd.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-10-27 14:16:59.000000 airbase-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-10-27 14:16:59.000000 airbase-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-10-27 14:16:59.000000 airbase-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-27 14:16:59.000000 airbase-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-27 14:16:59.000000 airbase-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2022-10-27 14:17:13.152813 airbase-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-10-27 14:16:59.000000 airbase-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.108813 airbase-0.6.0/airbase/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14586 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/airbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.112813 airbase-0.6.0/airbase/summary/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/summary/db.py
--rw-r--r--   0 runner    (1001) docker     (121)    90112 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/summary/summary.sqlite
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-10-27 14:16:59.000000 airbase-0.6.0/airbase/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.112813 airbase-0.6.0/airbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2022-10-27 14:17:12.000000 airbase-0.6.0/airbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-10-27 14:17:13.000000 airbase-0.6.0/airbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 14:17:12.000000 airbase-0.6.0/airbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-27 14:17:12.000000 airbase-0.6.0/airbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-27 14:17:12.000000 airbase-0.6.0/airbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-27 14:17:12.000000 airbase-0.6.0/airbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.112813 airbase-0.6.0/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 14:16:59.000000 airbase-0.6.0/data/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.112813 airbase-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-27 14:16:59.000000 airbase-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-27 14:16:59.000000 airbase-0.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.112813 airbase-0.6.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-10-27 14:16:59.000000 airbase-0.6.0/docs/source/airbase.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2022-10-27 14:16:59.000000 airbase-0.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-10-27 14:16:59.000000 airbase-0.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-10-27 14:16:59.000000 airbase-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.116813 airbase-0.6.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2648 2022-10-27 14:16:59.000000 airbase-0.6.0/scripts/check_broken_links.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1697 2022-10-27 14:16:59.000000 airbase-0.6.0/scripts/create_summary_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-10-27 14:17:13.152813 airbase-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.116813 airbase-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.120813 airbase-0.6.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/integration/test_airbase.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/integration/test_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:17:13.124813 airbase-0.6.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/resources/csv_links_response.txt
--rw-r--r--   0 runner    (1001) docker     (121)  3948287 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/resources/csv_response.csv
--rw-r--r--   0 runner    (1001) docker     (121) 22708960 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/resources/metadata.tsv
--rw-r--r--   0 runner    (1001) docker     (121)     5937 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/test_airbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-10-27 14:16:59.000000 airbase-0.6.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.649175 airbase-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.609174 airbase-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.613174 airbase-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-25 08:26:44.000000 airbase-0.7.0/.github/workflows/cicd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-25 08:26:44.000000 airbase-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-25 08:26:44.000000 airbase-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-25 08:26:44.000000 airbase-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 08:26:44.000000 airbase-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-25 08:26:44.000000 airbase-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-25 08:26:54.649175 airbase-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-25 08:26:44.000000 airbase-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.617174 airbase-0.7.0/airbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15755 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/airbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.617174 airbase-0.7.0/airbase/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/summary/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90112 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/summary/summary.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-25 08:26:44.000000 airbase-0.7.0/airbase/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.617174 airbase-0.7.0/airbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-25 08:26:54.000000 airbase-0.7.0/airbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-25 08:26:54.000000 airbase-0.7.0/airbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:26:54.000000 airbase-0.7.0/airbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 08:26:54.000000 airbase-0.7.0/airbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 08:26:54.000000 airbase-0.7.0/airbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 08:26:54.000000 airbase-0.7.0/airbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.617174 airbase-0.7.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:44.000000 airbase-0.7.0/data/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.621174 airbase-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-25 08:26:44.000000 airbase-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 08:26:44.000000 airbase-0.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.621174 airbase-0.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 08:26:44.000000 airbase-0.7.0/docs/source/airbase.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-25 08:26:44.000000 airbase-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-25 08:26:44.000000 airbase-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 08:26:44.000000 airbase-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.621174 airbase-0.7.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-25 08:26:44.000000 airbase-0.7.0/scripts/check_broken_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-04-25 08:26:44.000000 airbase-0.7.0/scripts/create_summary_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-25 08:26:54.653175 airbase-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.621174 airbase-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.621174 airbase-0.7.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/integration/test_airbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/integration/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:26:54.625175 airbase-0.7.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/resources/csv_links_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3948287 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/resources/csv_response.csv
+-rw-r--r--   0 runner    (1001) docker     (123) 22708960 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/resources/metadata.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/test_airbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-25 08:26:44.000000 airbase-0.7.0/tests/test_version.py
```

### Comparing `airbase-0.6.0/.github/workflows/cicd.yaml` & `airbase-0.7.0/.github/workflows/cicd.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,51 +8,51 @@
 jobs:
   unit-test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python: [3.7, 3.8, 3.9, '3.10', '3.11']
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - run: |
           pip install .[test]
       - run: |
           pytest -lk "not integration" --cov
 
   integration-test:
     needs: unit-test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - run: |
           pip install .[test]
       - run: |
           pytest -lvk "integration"
 
   lint:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
-      - uses: pre-commit/action@v2.0.3
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
+      - uses: pre-commit/action@v3.0.0
         with:
           extra_args: --all-files
 
   build-and-deploy:
     needs: [unit-test, integration-test, lint]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - run: |
           pip install build
       - run: |
           python -m build
       - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `airbase-0.6.0/.gitignore` & `airbase-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/LICENSE` & `airbase-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/PKG-INFO` & `airbase-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: airbase
-Version: 0.6.0
-Summary: An easy downloader for the AirBase air quality data.
-Home-page: https://github.com/johnpaton/airbase
-Author: John Paton
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/airbase.svg)](https://badge.fury.io/py/airbase)
 [![Downloads](https://pepy.tech/badge/airbase)](https://pepy.tech/project/airbase)
 [![CI/CD](https://github.com/JohnPaton/airbase/actions/workflows/cicd.yaml/badge.svg?branch=master)](https://github.com/JohnPaton/airbase/actions/workflows/cicd.yaml)
 [![Documentation Status](https://readthedocs.org/projects/airbase/badge/?version=latest)](https://airbase.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
@@ -110,12 +86,35 @@
 🌡 Don't forget to get the metadata about the measurement stations:
 
 ```pycon
 >>> client.download_metadata("data/metadata.tsv")
 Writing metadata to data/metadata.tsv...
 ```
 
+## 🚆 Command line interface
+
+``` console
+$ airbase download --help
+Usage: airbase download [OPTIONS]
+  Download all pollutants for all countries
+
+  The -c/--country and -p/--pollutant allow to specify which data to download, e.g.
+  - download only Norwegian, Danish and Finish sites
+    airbase download -c NO -c DK -c FI
+  - download only SO2, PM10 and PM2.5 observations
+    airbase download -p SO2 -p PM10 -p PM2.5
+
+Options:
+  -c, --country [AD|AL|AT|...]
+  -p, --pollutant [k|CO|NO|...]
+  --path PATH                     [default: data]
+  --year INTEGER                  [default: 2022]
+  -O, --overwrite                 Re-download existing files.
+  -q, --quiet                     No progress-bar.
+  --help                          Show this message and exit.
+```
+
 ## 🛣 Roadmap
 
 * ~~Parallel CSV downloads~~ Contributed by @avaldebe
 * ~~CLI to avoid using Python all together~~ Contributed by @avaldebe
 * Data wrangling module for AirBase output data
```

### Comparing `airbase-0.6.0/airbase/airbase.py` & `airbase-0.7.0/airbase/airbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import sys
+import warnings
 from datetime import datetime
 from pathlib import Path
 
-if sys.version_info >= (3, 8):
+if sys.version_info >= (3, 8):  # pragma: no cover
     from typing import TypedDict
-else:
+else:  # pragma: no cover
     from typing_extensions import TypedDict
 
 from .fetch import (
     fetch_text,
     fetch_to_directory,
     fetch_to_file,
     fetch_unique_lines,
@@ -39,28 +40,48 @@
             Generated 5164 CSV links ready for downloading
             Downloading CSVs to data/raw...
             100%|██████████| 5164/5164 [43:39<00:00,  1.95it/s]
             >>> r.download_metadata("data/metadata.tsv")
             Writing metadata to data/metadata.tsv...
         """
 
-        self.all_countries = DB.countries()
         """All countries available from AirBase"""
+        self.countries = DB.countries()
 
-        self.all_pollutants = DB.pollutants()
         """All pollutants available from AirBase"""
+        self._pollutants_ids = DB.pollutants()
 
-        self.pollutants_per_country: dict[str, list[PollutantDict]] = dict()
         """The pollutants available in each country from AirBase."""
+        self.pollutants_per_country: dict[str, list[PollutantDict]] = dict()
 
         for country, pollutants in DB.pollutants_per_country().items():
             self.pollutants_per_country[country] = [
                 dict(pl=pl, shortpl=id) for pl, id in pollutants.items()
             ]
 
+    @property
+    def all_countries(self) -> list[str]:  # pragma: no cover
+        warnings.warn(
+            f"{type(self).__qualname__}.all_countries has been deprecated and will be removed on v1. "
+            f"Use {type(self).__qualname__}.countries instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.countries
+
+    @property
+    def all_pollutants(self) -> dict[str, str]:  # pragma: no cover
+        warnings.warn(
+            f"{type(self).__qualname__}.all_pollutants has been deprecated and will be removed on v1. "
+            f"Use {type(self).__qualname__}._pollutants_ids instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._pollutants_ids
+
     def request(
         self,
         country: str | list[str] | None = None,
         pl: str | list[str] | None = None,
         shortpl: str | list[str] | None = None,
         year_from: str = "2013",
         year_to: str = CURRENT_YEAR,
@@ -91,14 +112,15 @@
             requested. See `self.all_countries`.
         :param pl: (optional) The pollutant(s) to request data
             for. Must be one of the pollutants in `self.all_pollutants`.
             Cannot be used in conjunction with `shortpl`.
         :param shortpl: (optional). The pollutant code(s) to
             request data for. Will be applied to each country requested.
             Cannot be used in conjunction with `pl`.
+            Deprecated, will be removed on v1.
         :param year_from: (optional) The first year of data. Can
             not be earlier than 2013. Default 2013.
         :param year_to: (optional) The last year of data. Can not be
             later than the current year. Default <current year>.
         :param source: (optional) One of "E1a", "E2a" or "All". E2a
             (UTD) data are only available for years where E1a data have
             not yet been delivered (this will normally be the most
@@ -125,27 +147,35 @@
             Downloading CSVs to data/raw...
             100%|██████████| 5164/5164 [43:39<00:00,  1.95it/s]
             >>> r.download_metadata("data/metadata.tsv")
             Writing metadata to data/metadata.tsv...
         """
         # validation
         if country is None:
-            country = self.all_countries
+            country = self.countries
         else:
             country = string_safe_list(country)
             self._validate_country(country)
 
+        if shortpl is not None:
+            warnings.warn(
+                f"the shortpl option has been deprecated and will be removed on v1. "
+                f"Use client.request([client._pollutants_ids[p] for p in shortpl], ...) instead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
         if pl is not None and shortpl is not None:
             raise ValueError("You cannot specify both 'pl' and 'shortpl'")
 
         # construct shortpl form pl if applicable
         if pl is not None:
             pl_list = string_safe_list(pl)
             try:
-                shortpl = [self.all_pollutants[p] for p in pl_list]
+                shortpl = [self._pollutants_ids[p] for p in pl_list]
             except KeyError as e:
                 raise ValueError(
                     f"'{e.args[0]}' is not a valid pollutant name"
                 ) from e
 
         return AirbaseRequest(
             country,
@@ -197,15 +227,15 @@
         Must first download the country list using `.connect()`. Raises
         value error if a country does not exist.
 
         :param country: The 2-letter country code to validate.
         """
         country_list = string_safe_list(country)
         for c in country_list:
-            if c not in self.all_countries:
+            if c not in self.countries:
                 raise ValueError(
                     f"'{c}' is not an available 2-letter country code."
                 )
 
 
 class AirbaseRequest:
     def __init__(
```

### Comparing `airbase-0.6.0/airbase/fetch.py` & `airbase-0.7.0/airbase/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     timeout: float | None = None,
     encoding: str | None = None,
 ) -> list[dict[str, str]]:
     """Request url and read response’s body as JSON
 
     :param url: requested url
     :param timeout: maximum time to complete request (seconds)
-    :param encoding: text encoding used for decodding the response's body
+    :param encoding: text encoding used for decoding the response's body
 
     :return: decoded text from response's body as JSON
     """
     text = fetch_text(url, timeout=timeout, encoding=encoding)
     payload: dict[str, str] | list[dict[str, str]]
     payload = json.loads(text)
     if isinstance(payload, dict):
@@ -96,20 +96,20 @@
     urls: list[str] | dict[str, Path],
     *,
     encoding: str | None = None,
     progress: bool = DEFAULT.progress,
     raise_for_status: bool = DEFAULT.raise_for_status,
     max_concurrent: int = DEFAULT.max_concurrent,
 ) -> AsyncIterator[str | Path]:
-    """Request multiple urls and write resquest text into individual paths
+    """Request multiple urls and write request text into individual paths
     it a `dict[url, path]` is provided, or return the decoded text from each request
     if only a `list[url]` is provided.
 
     :param urls: requested urls
-    :param encoding: text encoding used for decodding each response's body
+    :param encoding: text encoding used for decoding each response's body
     :param progress: show progress bar
     :param raise_for_status: Raise exceptions if download links
         return "bad" HTTP status codes. If False,
         a :py:func:`warnings.warn` will be issued instead.
     :param max_concurrent: maximum concurrent requests
 
     :return: url text or path to downloaded text, one by one as the requests are completed
@@ -156,15 +156,15 @@
     progress: bool = DEFAULT.progress,
     raise_for_status: bool = DEFAULT.raise_for_status,
     max_concurrent: int = DEFAULT.max_concurrent,
 ) -> set[str]:
     """Request a list of url and return only the unique lines among all the responses
 
     :param urls: requested urls
-    :param encoding: text encoding used for decodding each response's body
+    :param encoding: text encoding used for decoding each response's body
     :param progress: show progress bar
     :param raise_for_status: Raise exceptions if download links
         return "bad" HTTP status codes. If False,
         a :py:func:`warnings.warn` will be issued instead.
     :param max_concurrent: maximum concurrent requests
 
     :return: unique lines among from all the responses
@@ -194,15 +194,15 @@
     raise_for_status: bool = DEFAULT.raise_for_status,
     max_concurrent: int = DEFAULT.max_concurrent,
 ) -> None:
     """Request a list of url write out all responses into a single text file
 
     :param urls: requested urls
     :param path: text file for all combined responses
-    :param encoding: text encoding used for decodding each response's body
+    :param encoding: text encoding used for decoding each response's body
     :param progress: show progress bar
     :param raise_for_status: Raise exceptions if download links
         return "bad" HTTP status codes. If False,
         a :py:func:`warnings.warn` will be issued instead.
     :param max_concurrent: maximum concurrent requests
     """
 
@@ -241,15 +241,15 @@
 ) -> None:
     """Request a list of url write each response to different file
 
     :param urls: requested urls
     :param root: directory to write all responses
     :param bool skip_existing: Do not re-download url if the corresponding file
         is found in `root`
-    :param encoding: text encoding used for decodding each response's body
+    :param encoding: text encoding used for decoding each response's body
     :param progress: show progress bar
     :param raise_for_status: Raise exceptions if download links
         return "bad" HTTP status codes. If False,
         a :py:func:`warnings.warn` will be issued instead.
     :param max_concurrent: maximum concurrent requests
     """
```

### Comparing `airbase-0.6.0/airbase/resources.py` & `airbase-0.7.0/airbase/resources.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/airbase/summary/db.py` & `airbase-0.7.0/airbase/summary/db.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import sqlite3
 import sys
 from collections import defaultdict
 from contextlib import closing, contextmanager
 from pathlib import Path
 from typing import Iterator
 
-if sys.version_info >= (3, 11):
+if sys.version_info >= (3, 11):  # pragma: no cover
     from importlib import resources
-else:
+else:  # pragma: no cover
     import importlib_resources as resources
 
 
 def summary() -> Path:
     source = resources.files(__package__) / "summary.sqlite"
     path: Path
     with resources.as_file(source) as path:
```

### Comparing `airbase-0.6.0/airbase/summary/summary.sqlite` & `airbase-0.7.0/airbase/summary/summary.sqlite`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/airbase/util.py` & `airbase-0.7.0/airbase/util.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/airbase.egg-info/PKG-INFO` & `airbase-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbase
-Version: 0.6.0
+Version: 0.7.0
 Summary: An easy downloader for the AirBase air quality data.
 Home-page: https://github.com/johnpaton/airbase
 Author: John Paton
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -110,12 +110,35 @@
 🌡 Don't forget to get the metadata about the measurement stations:
 
 ```pycon
 >>> client.download_metadata("data/metadata.tsv")
 Writing metadata to data/metadata.tsv...
 ```
 
+## 🚆 Command line interface
+
+``` console
+$ airbase download --help
+Usage: airbase download [OPTIONS]
+  Download all pollutants for all countries
+
+  The -c/--country and -p/--pollutant allow to specify which data to download, e.g.
+  - download only Norwegian, Danish and Finish sites
+    airbase download -c NO -c DK -c FI
+  - download only SO2, PM10 and PM2.5 observations
+    airbase download -p SO2 -p PM10 -p PM2.5
+
+Options:
+  -c, --country [AD|AL|AT|...]
+  -p, --pollutant [k|CO|NO|...]
+  --path PATH                     [default: data]
+  --year INTEGER                  [default: 2022]
+  -O, --overwrite                 Re-download existing files.
+  -q, --quiet                     No progress-bar.
+  --help                          Show this message and exit.
+```
+
 ## 🛣 Roadmap
 
 * ~~Parallel CSV downloads~~ Contributed by @avaldebe
 * ~~CLI to avoid using Python all together~~ Contributed by @avaldebe
 * Data wrangling module for AirBase output data
```

### Comparing `airbase-0.6.0/airbase.egg-info/SOURCES.txt` & `airbase-0.7.0/airbase.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,20 @@
 docs/source/conf.py
 docs/source/index.rst
 scripts/check_broken_links.py
 scripts/create_summary_db.py
 tests/__init__.py
 tests/conftest.py
 tests/test_airbase.py
+tests/test_cli.py
 tests/test_fetch.py
 tests/test_summary.py
 tests/test_utils.py
 tests/test_version.py
 tests/integration/__init__.py
 tests/integration/test_airbase.py
+tests/integration/test_cli.py
 tests/integration/test_summary.py
 tests/resources/__init__.py
 tests/resources/csv_links_response.txt
 tests/resources/csv_response.csv
 tests/resources/metadata.tsv
```

### Comparing `airbase-0.6.0/docs/Makefile` & `airbase-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/docs/source/airbase.rst` & `airbase-0.7.0/docs/source/airbase.rst`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/docs/source/conf.py` & `airbase-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/docs/source/index.rst` & `airbase-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/pyproject.toml` & `airbase-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--showlocals"
 testpaths = ["tests"]
+filterwarnings = [
+    # DeprecationWarning are errors
+    "error::DeprecationWarning:(airbase|tests).*:",
+]
 
 [tool.coverage.run]
 source = ["airbase"]
 
 [tool.coverage.report]
 skip_covered = true
 skip_empty = true
```

### Comparing `airbase-0.6.0/scripts/check_broken_links.py` & `airbase-0.7.0/scripts/check_broken_links.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/scripts/create_summary_db.py` & `airbase-0.7.0/scripts/create_summary_db.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/setup.cfg` & `airbase-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 python_requires = >=3.7,<4
 install_requires = 
 	aiohttp
 	aiofiles
 	importlib_resources; python_version < "3.11"
 	tqdm
 	typing_extensions; python_version < "3.8"
-	typer
+	click
 packages = find:
 include_package_data = True
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `airbase-0.6.0/tests/conftest.py` & `airbase-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/integration/test_airbase.py` & `airbase-0.7.0/tests/integration/test_airbase.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/integration/test_summary.py` & `airbase-0.7.0/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/resources/csv_response.csv` & `airbase-0.7.0/tests/resources/csv_response.csv`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/resources/metadata.tsv` & `airbase-0.7.0/tests/resources/metadata.tsv`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/test_airbase.py` & `airbase-0.7.0/tests/test_airbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     """mock responses from relevant urls"""
     return
 
 
 class TestAirbaseClient:
     def test_init(self):
         client = airbase.AirbaseClient()
-        assert isinstance(client.all_countries, list)
-        assert isinstance(client.all_pollutants, dict)
+        assert isinstance(client.countries, list)
+        assert isinstance(client._pollutants_ids, dict)
         assert isinstance(client.pollutants_per_country, dict)
 
     def test_download_metadata(
         self, tmp_path: Path, capsys, client: airbase.AirbaseClient
     ):
         path = tmp_path / "meta.csv"
         client.download_metadata(path)
@@ -64,15 +64,15 @@
             r = client.request(pl=["NO", "NO3", "Not a pl"])
 
     def test_request_response_generated(self, client: airbase.AirbaseClient):
         r = client.request()
         assert isinstance(r, airbase.AirbaseRequest)
 
     def test_request_not_pl_and_shortpl(self, client: airbase.AirbaseClient):
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError), pytest.warns(DeprecationWarning):
             client.request(pl="O3", shortpl="123")
 
     def test_search_pl_exact(self, client: airbase.AirbaseClient):
         result = client.search_pollutant("NO3")
         assert result[0]["pl"] == "NO3"
 
     def test_search_pl_shortest_first(self, client: airbase.AirbaseClient):
```

### Comparing `airbase-0.6.0/tests/test_fetch.py` & `airbase-0.7.0/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/test_summary.py` & `airbase-0.7.0/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `airbase-0.6.0/tests/test_utils.py` & `airbase-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

