# Comparing `tmp/swh.dataset-1.3.1.tar.gz` & `tmp/swh.dataset-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.dataset-1.3.1.tar", last modified: Tue Apr 25 07:54:41 2023, max compression
+gzip compressed data, was "dist/swh.dataset-1.3.2.tar", last modified: Tue Apr 25 08:45:20 2023, max compression
```

## Comparing `swh.dataset-1.3.1.tar` & `swh.dataset-1.3.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)       99 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1182 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      244 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1215 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/bin/orc-merge
--rwxr-xr-x   0 jenkins    (115) docker     (999)      662 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/bin/orc-print-contents
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      244 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3427 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/export.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3452 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/generate_subdataset.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/docs/graph/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/docs/graph/_images/
--rw-r--r--   0 jenkins    (115) docker     (999)    54727 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/_images/athena_tables.png
--rw-r--r--   0 jenkins    (115) docker     (999)    14683 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/_images/dataset-schema.dot
--rw-r--r--   0 jenkins    (115) docker     (999)    44610 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/_images/dataset-schema.svg
--rw-r--r--   0 jenkins    (115) docker     (999)     3945 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/athena.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     2482 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/databricks.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     9180 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/dataset.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     2239 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     6269 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/graph/schema.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      462 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      602 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/requirements-luigi.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/requirements-swh-with-content.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2458 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh/dataset/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8522 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/athena.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9351 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2529 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/exporter.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh/dataset/exporters/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/exporters/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9311 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/exporters/edges.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14298 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/exporters/orc.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18692 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/journalprocessor.py
--rw-r--r--   0 jenkins    (115) docker     (999)    25239 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/luigi.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     3026 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/relational.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh/dataset/test/
--rw-r--r--   0 jenkins    (115) docker     (999)    19632 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/test/test_edges.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11486 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/test/test_orc.py
--rw-r--r--   0 jenkins    (115) docker     (999)      719 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/test/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4462 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/swh/dataset/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1182 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1365 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      206 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-25 07:54:41.000000 swh.dataset-1.3.1/swh.dataset.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1549 2023-04-25 07:54:39.000000 swh.dataset-1.3.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)       99 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1182 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      244 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1215 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/bin/orc-merge
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      662 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/bin/orc-print-contents
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      244 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3427 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/export.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3452 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/generate_subdataset.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/docs/graph/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/docs/graph/_images/
+-rw-r--r--   0 jenkins    (115) docker     (999)    54727 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/_images/athena_tables.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    14683 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/_images/dataset-schema.dot
+-rw-r--r--   0 jenkins    (115) docker     (999)    44610 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/_images/dataset-schema.svg
+-rw-r--r--   0 jenkins    (115) docker     (999)     3945 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/athena.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     2482 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/databricks.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     9180 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/dataset.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     2239 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     6269 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/graph/schema.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      462 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      602 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/requirements-luigi.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/requirements-swh-with-content.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2458 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh/dataset/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8522 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/athena.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9351 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2529 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/exporter.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh/dataset/exporters/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/exporters/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9311 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/exporters/edges.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14298 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/exporters/orc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18692 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/journalprocessor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    25736 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/luigi.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     3026 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/relational.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh/dataset/test/
+-rw-r--r--   0 jenkins    (115) docker     (999)    19632 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/test/test_edges.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11486 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/test/test_orc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      719 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/test/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4462 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/swh/dataset/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1182 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1365 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      206 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-25 08:45:20.000000 swh.dataset-1.3.2/swh.dataset.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1549 2023-04-25 08:45:19.000000 swh.dataset-1.3.2/tox.ini
```

### Comparing `swh.dataset-1.3.1/.pre-commit-config.yaml` & `swh.dataset-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/CODE_OF_CONDUCT.md` & `swh.dataset-1.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/LICENSE` & `swh.dataset-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/PKG-INFO` & `swh.dataset-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.dataset
-Version: 1.3.1
+Version: 1.3.2
 Summary: Software Heritage dataset tools
 Home-page: https://forge.softwareheritage.org/source/swh-dataset/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-dataset
```

### Comparing `swh.dataset-1.3.1/bin/orc-merge` & `swh.dataset-1.3.2/bin/orc-merge`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/bin/orc-print-contents` & `swh.dataset-1.3.2/bin/orc-print-contents`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/export.rst` & `swh.dataset-1.3.2/docs/export.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/generate_subdataset.rst` & `swh.dataset-1.3.2/docs/generate_subdataset.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/_images/athena_tables.png` & `swh.dataset-1.3.2/docs/graph/_images/athena_tables.png`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/_images/dataset-schema.dot` & `swh.dataset-1.3.2/docs/graph/_images/dataset-schema.dot`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/_images/dataset-schema.svg` & `swh.dataset-1.3.2/docs/graph/_images/dataset-schema.svg`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/athena.rst` & `swh.dataset-1.3.2/docs/graph/athena.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/databricks.rst` & `swh.dataset-1.3.2/docs/graph/databricks.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/dataset.rst` & `swh.dataset-1.3.2/docs/graph/dataset.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/index.rst` & `swh.dataset-1.3.2/docs/graph/index.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/docs/graph/schema.rst` & `swh.dataset-1.3.2/docs/graph/schema.rst`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/mypy.ini` & `swh.dataset-1.3.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/setup.py` & `swh.dataset-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/athena.py` & `swh.dataset-1.3.2/swh/dataset/athena.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/cli.py` & `swh.dataset-1.3.2/swh/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/exporter.py` & `swh.dataset-1.3.2/swh/dataset/exporter.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/exporters/edges.py` & `swh.dataset-1.3.2/swh/dataset/exporters/edges.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/exporters/orc.py` & `swh.dataset-1.3.2/swh/dataset/exporters/orc.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/journalprocessor.py` & `swh.dataset-1.3.2/swh/dataset/journalprocessor.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/luigi.py` & `swh.dataset-1.3.2/swh/dataset/luigi.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,14 +163,23 @@
         self,
         is_dir: bool = False,
         is_file: bool = False,
         exists: bool = False,
         create: bool = False,
         **kwargs,
     ):
+        """
+        :param is_dir: whether the path should be to a directory
+        :param is_file: whether the path should be to a directory
+        :param exists: whether the path should already exist
+        :param create: whether the path should be created if it does not exist
+
+        ``is_dir`` and ``is_file`` are mutually exclusive.
+        ``exists`` and ``create`` are mutually exclusive.
+        """
         if create and not is_dir:
             raise ValueError("`is_dir` must be True if `create` is True")
         if is_dir and is_file:
             raise ValueError("`is_dir` and `is_file` are mutually exclusive")
 
         super().__init__(**kwargs)
 
@@ -717,14 +726,15 @@
         enum=ObjectType, default=list(ObjectType), batch_method=merge_lists
     )
     s3_export_path = S3PathParameter()
     s3_athena_output_location = S3PathParameter()
     athena_db_name = luigi.Parameter()
 
     def requires(self) -> List[luigi.Task]:
+        """Returns instances of :cls:`CreateAthena` and :cls:`UploadExportToS3`."""
         # CreateAthena depends on UploadExportToS3(formats=[edges]), so we need to
         # explicitly depend on UploadExportToS3(formats=self.formats) here, to also
         # export the formats requested by the user.
         return [
             CreateAthena(
                 object_types=self.object_types,
                 s3_export_path=self.s3_export_path,
```

### Comparing `swh.dataset-1.3.1/swh/dataset/relational.py` & `swh.dataset-1.3.2/swh/dataset/relational.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/test/test_edges.py` & `swh.dataset-1.3.2/swh/dataset/test/test_edges.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/test/test_orc.py` & `swh.dataset-1.3.2/swh/dataset/test/test_orc.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/test/test_utils.py` & `swh.dataset-1.3.2/swh/dataset/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh/dataset/utils.py` & `swh.dataset-1.3.2/swh/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/swh.dataset.egg-info/PKG-INFO` & `swh.dataset-1.3.2/swh.dataset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.dataset
-Version: 1.3.1
+Version: 1.3.2
 Summary: Software Heritage dataset tools
 Home-page: https://forge.softwareheritage.org/source/swh-dataset/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-dataset
```

### Comparing `swh.dataset-1.3.1/swh.dataset.egg-info/SOURCES.txt` & `swh.dataset-1.3.2/swh.dataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.dataset-1.3.1/tox.ini` & `swh.dataset-1.3.2/tox.ini`

 * *Files identical despite different names*

