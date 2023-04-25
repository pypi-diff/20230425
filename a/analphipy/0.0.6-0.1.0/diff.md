# Comparing `tmp/analphipy-0.0.6.tar.gz` & `tmp/analphipy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analphipy-0.0.6.tar", last modified: Wed Mar 22 18:05:49 2023, max compression
+gzip compressed data, was "analphipy-0.1.0.tar", last modified: Tue Apr 25 03:08:15 2023, max compression
```

## Comparing `analphipy-0.0.6.tar` & `analphipy-0.1.0.tar`

### file list

```diff
@@ -1,147 +1,142 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.339197 analphipy-0.0.6/
--rw-r--r--   0 wpk      (42033)    36681     1407 2023-03-22 17:48:12.000000 analphipy-0.0.6/.cruft.json
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.288020 analphipy-0.0.6/.github/
--rw-r--r--   0 wpk      (42033)    36681      320 2023-03-22 17:48:12.000000 analphipy-0.0.6/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1310 2023-03-22 17:48:12.000000 analphipy-0.0.6/.gitignore
--rw-r--r--   0 wpk      (42033)    36681     2848 2023-03-22 17:48:12.000000 analphipy-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681      131 2023-03-22 17:48:12.000000 analphipy-0.0.6/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681     6738 2023-03-22 17:48:12.000000 analphipy-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681       59 2023-03-22 17:48:12.000000 analphipy-0.0.6/HISTORY.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2022-09-26 16:03:57.000000 analphipy-0.0.6/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      313 2023-03-22 17:48:12.000000 analphipy-0.0.6/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681     8348 2023-03-22 17:48:12.000000 analphipy-0.0.6/Makefile
--rw-r--r--   0 wpk      (42033)    36681     5693 2023-03-22 18:05:49.339395 analphipy-0.0.6/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     3072 2023-03-22 17:48:12.000000 analphipy-0.0.6/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.296303 analphipy-0.0.6/docs/
--rw-r--r--   0 wpk      (42033)    36681      610 2022-09-26 16:03:57.000000 analphipy-0.0.6/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.277696 analphipy-0.0.6/docs/_build/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.277016 analphipy-0.0.6/docs/_build/html/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.299276 analphipy-0.0.6/docs/_build/html/_images/
--rw-r--r--   0 wpk      (42033)    36681    17184 2023-03-22 18:02:41.000000 analphipy-0.0.6/docs/_build/html/_images/2665049d231f1552592a9b4ebfe544e7fc2249641db2cd515b09893598cab06e.png
--rw-r--r--   0 wpk      (42033)    36681    14809 2023-03-22 18:02:42.000000 analphipy-0.0.6/docs/_build/html/_images/85d4d3c0746fc4dde40187d4ed004db4bb5c1b2173aa1cc4e9e1c0aad9baacab.png
--rw-r--r--   0 wpk      (42033)    36681    16319 2023-03-22 18:02:41.000000 analphipy-0.0.6/docs/_build/html/_images/a7daef54af051750721878d0fe1674dbdf739ddcbce632e4830ac315e17debb6.png
--rw-r--r--   0 wpk      (42033)    36681    18722 2023-03-22 18:02:41.000000 analphipy-0.0.6/docs/_build/html/_images/e70d17a92a249f8fb79a136340bdb51930448700e0b7c787eb8579198d275ed7.png
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.276675 analphipy-0.0.6/docs/_build/html/_sources/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.302606 analphipy-0.0.6/docs/_build/html/_sources/generated/
--rw-r--r--   0 wpk      (42033)    36681      212 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/_build/html/_sources/generated/analphipy.base_potential.rst
--rw-r--r--   0 wpk      (42033)    36681      183 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/_build/html/_sources/generated/analphipy.measures.rst
--rw-r--r--   0 wpk      (42033)    36681      186 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/_build/html/_sources/generated/analphipy.norofrenkel.rst
--rw-r--r--   0 wpk      (42033)    36681      184 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/_build/html/_sources/generated/analphipy.potential.rst
--rw-r--r--   0 wpk      (42033)    36681      180 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/_build/html/_sources/generated/analphipy.utils.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.304367 analphipy-0.0.6/docs/_build/html/_static/
--rw-r--r--   0 wpk      (42033)    36681      286 2023-03-22 16:59:08.000000 analphipy-0.0.6/docs/_build/html/_static/file.png
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.304814 analphipy-0.0.6/docs/_build/html/_static/images/
--rw-r--r--   0 wpk      (42033)    36681     7601 2023-03-22 16:59:09.000000 analphipy-0.0.6/docs/_build/html/_static/images/logo_colab.png
--rw-r--r--   0 wpk      (42033)    36681       90 2023-03-22 16:59:08.000000 analphipy-0.0.6/docs/_build/html/_static/minus.png
--rw-r--r--   0 wpk      (42033)    36681       90 2023-03-22 16:59:08.000000 analphipy-0.0.6/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.306651 analphipy-0.0.6/docs/_build/jupyter_execute/
--rw-r--r--   0 wpk      (42033)    36681    17184 2023-03-22 18:02:41.000000 analphipy-0.0.6/docs/_build/jupyter_execute/2665049d231f1552592a9b4ebfe544e7fc2249641db2cd515b09893598cab06e.png
--rw-r--r--   0 wpk      (42033)    36681    14809 2023-03-22 18:02:42.000000 analphipy-0.0.6/docs/_build/jupyter_execute/85d4d3c0746fc4dde40187d4ed004db4bb5c1b2173aa1cc4e9e1c0aad9baacab.png
--rw-r--r--   0 wpk      (42033)    36681    16319 2023-03-22 18:02:41.000000 analphipy-0.0.6/docs/_build/jupyter_execute/a7daef54af051750721878d0fe1674dbdf739ddcbce632e4830ac315e17debb6.png
--rw-r--r--   0 wpk      (42033)    36681    18722 2023-03-22 18:02:41.000000 analphipy-0.0.6/docs/_build/jupyter_execute/e70d17a92a249f8fb79a136340bdb51930448700e0b7c787eb8579198d275ed7.png
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.278584 analphipy-0.0.6/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.307125 analphipy-0.0.6/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2777 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.307973 analphipy-0.0.6/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      703 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      624 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.310895 analphipy-0.0.6/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.313494 analphipy-0.0.6/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.314772 analphipy-0.0.6/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/module-template.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.315211 analphipy-0.0.6/docs/_templates/test/
--rw-r--r--   0 wpk      (42033)    36681     1166 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/_templates/test/class-1.rst
--rw-r--r--   0 wpk      (42033)    36681     3147 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/api.md
--rw-r--r--   0 wpk      (42033)    36681       31 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681    14396 2023-03-22 18:01:13.000000 analphipy-0.0.6/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       36 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/contributing.md
--rw-r--r--   0 wpk      (42033)    36681      850 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/environment-docs-extras.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.317357 analphipy-0.0.6/docs/generated/
--rw-r--r--   0 wpk      (42033)    36681      212 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/generated/analphipy.base_potential.rst
--rw-r--r--   0 wpk      (42033)    36681      183 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/generated/analphipy.measures.rst
--rw-r--r--   0 wpk      (42033)    36681      186 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/generated/analphipy.norofrenkel.rst
--rw-r--r--   0 wpk      (42033)    36681      184 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/generated/analphipy.potential.rst
--rw-r--r--   0 wpk      (42033)    36681      180 2023-03-22 18:02:38.000000 analphipy-0.0.6/docs/generated/analphipy.utils.rst
--rw-r--r--   0 wpk      (42033)    36681       31 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/history.md
--rw-r--r--   0 wpk      (42033)    36681      261 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681     1123 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       39 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/make.bat
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.317777 analphipy-0.0.6/docs/notebooks/
--rw-r--r--   0 wpk      (42033)    36681   113133 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/notebooks/usage.ipynb
--rw-r--r--   0 wpk      (42033)    36681       37 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/requirements-conda.txt
--rw-r--r--   0 wpk      (42033)    36681      536 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/requirements.txt
--rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 17:48:12.000000 analphipy-0.0.6/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.322294 analphipy-0.0.6/environment/
--rw-r--r--   0 wpk      (42033)    36681     1059 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      120 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681      109 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      674 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      366 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       39 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/example-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      153 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/example.yaml
--rw-r--r--   0 wpk      (42033)    36681      140 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      162 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      384 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment/tox_conda_tmp_gl80gok.yaml
--rw-r--r--   0 wpk      (42033)    36681      186 2023-03-22 17:48:12.000000 analphipy-0.0.6/environment.yaml
--rw-r--r--   0 wpk      (42033)    36681     4187 2023-03-22 17:48:12.000000 analphipy-0.0.6/pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681      147 2023-03-22 18:05:49.340033 analphipy-0.0.6/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.281079 analphipy-0.0.6/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.327177 analphipy-0.0.6/src/analphipy/
--rw-r--r--   0 wpk      (42033)    36681     1100 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     1072 2022-09-27 20:23:36.000000 analphipy-0.0.6/src/analphipy/_attrs_utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.328110 analphipy-0.0.6/src/analphipy/_docfiller/
--rw-r--r--   0 wpk      (42033)    36681    19502 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/_docfiller/__init__.py
--rw-r--r--   0 wpk      (42033)    36681    23552 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/_docfiller/docscrape.py
--rw-r--r--   0 wpk      (42033)    36681     2526 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/_docstrings.py
--rw-r--r--   0 wpk      (42033)    36681      478 2022-09-27 20:23:36.000000 analphipy-0.0.6/src/analphipy/_typing.py
--rw-r--r--   0 wpk      (42033)    36681    12712 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/base_potential.py
--rw-r--r--   0 wpk      (42033)    36681     6287 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/cached_decorators.py
--rw-r--r--   0 wpk      (42033)    36681    12932 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/measures.py
--rw-r--r--   0 wpk      (42033)    36681    15054 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/norofrenkel.py
--rw-r--r--   0 wpk      (42033)    36681    14184 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/potential.py
--rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/py.typed
--rw-r--r--   0 wpk      (42033)    36681     9883 2023-03-22 17:48:12.000000 analphipy-0.0.6/src/analphipy/utils.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.338938 analphipy-0.0.6/src/analphipy.egg-info/
--rw-r--r--   0 wpk      (42033)    36681     3910 2023-03-22 18:05:49.000000 analphipy-0.0.6/src/analphipy.egg-info/SOURCES.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.331615 analphipy-0.0.6/tests/
--rw-r--r--   0 wpk      (42033)    36681       39 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     6651 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/conftest.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-03-22 18:05:49.338537 analphipy-0.0.6/tests/data/
--rw-r--r--   0 wpk      (42033)    36681     1175 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/crit_eff_lj_.csv
--rw-r--r--   0 wpk      (42033)    36681      671 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/crit_eff_lj_nm_.csv
--rw-r--r--   0 wpk      (42033)    36681     1273 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/crit_eff_sw_.csv
--rw-r--r--   0 wpk      (42033)    36681      862 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/crit_eff_yukawa_.csv
--rw-r--r--   0 wpk      (42033)    36681      110 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/eff_hs_.csv
--rw-r--r--   0 wpk      (42033)    36681    15874 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/eff_lj_.csv
--rw-r--r--   0 wpk      (42033)    36681     5137 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/eff_lj_nm_.csv
--rw-r--r--   0 wpk      (42033)    36681     2479 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/eff_stockmayer_.csv
--rw-r--r--   0 wpk      (42033)    36681    14148 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/eff_sw_.csv
--rw-r--r--   0 wpk      (42033)    36681     5317 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/eff_yukawa_.csv
--rw-r--r--   0 wpk      (42033)    36681    18038 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/vir_hs_.csv
--rw-r--r--   0 wpk      (42033)    36681    21577 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/vir_lj_.csv
--rw-r--r--   0 wpk      (42033)    36681     7033 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/vir_lj_nm_.csv
--rw-r--r--   0 wpk      (42033)    36681     3284 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/vir_stockmayer_.csv
--rw-r--r--   0 wpk      (42033)    36681     9423 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/vir_sw_.csv
--rw-r--r--   0 wpk      (42033)    36681     4247 2022-09-26 16:03:57.000000 analphipy-0.0.6/tests/data/vir_yukawa_.csv
--rw-r--r--   0 wpk      (42033)    36681     2145 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/test_generic.py
--rw-r--r--   0 wpk      (42033)    36681      737 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/test_js.py
--rw-r--r--   0 wpk      (42033)    36681     1738 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/test_nf_derivs.py
--rw-r--r--   0 wpk      (42033)    36681     3037 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/test_norofrenkel.py
--rw-r--r--   0 wpk      (42033)    36681     2027 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/test_potentials.py
--rw-r--r--   0 wpk      (42033)    36681     3355 2023-03-22 17:48:12.000000 analphipy-0.0.6/tests/test_secondvirial.py
--rw-r--r--   0 wpk      (42033)    36681     4162 2023-03-22 17:48:12.000000 analphipy-0.0.6/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.086929 analphipy-0.1.0/
+-rw-r--r--   0 wpk      (42033)    36681     1502 2023-04-25 03:05:00.000000 analphipy-0.1.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      513 2023-04-25 03:05:00.000000 analphipy-0.1.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.941852 analphipy-0.1.0/.github/
+-rw-r--r--   0 wpk      (42033)    36681      361 2023-04-25 03:05:00.000000 analphipy-0.1.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1313 2023-04-25 03:05:00.000000 analphipy-0.1.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-04-25 03:05:00.000000 analphipy-0.1.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3549 2023-04-25 03:05:00.000000 analphipy-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-04-25 03:05:00.000000 analphipy-0.1.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      131 2023-04-19 04:41:12.000000 analphipy-0.1.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681      967 2023-04-25 03:05:00.000000 analphipy-0.1.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9146 2023-04-25 03:05:00.000000 analphipy-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2022-09-26 16:03:57.000000 analphipy-0.1.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-04-25 03:05:00.000000 analphipy-0.1.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    10568 2023-04-25 03:05:00.000000 analphipy-0.1.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     6596 2023-04-25 03:08:15.087669 analphipy-0.1.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2966 2023-04-25 03:05:00.000000 analphipy-0.1.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.942689 analphipy-0.1.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.943590 analphipy-0.1.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.945373 analphipy-0.1.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-04-25 03:05:00.000000 analphipy-0.1.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.957554 analphipy-0.1.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1201 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.916256 analphipy-0.1.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.958915 analphipy-0.1.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.961143 analphipy-0.1.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      837 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.975721 analphipy-0.1.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.982266 analphipy-0.1.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.986764 analphipy-0.1.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-14 18:58:52.000000 analphipy-0.1.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.988405 analphipy-0.1.0/docs/_templates/test/
+-rw-r--r--   0 wpk      (42033)    36681     1166 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/_templates/test/class-1.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14667 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.991160 analphipy-0.1.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681      887 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/examples/create-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681       58 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.992727 analphipy-0.1.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681   113096 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/examples/usage/usage.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      224 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      768 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      170 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.994331 analphipy-0.1.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      324 2023-04-25 03:05:00.000000 analphipy-0.1.0/docs/reference/index.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 17:48:12.000000 analphipy-0.1.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.009710 analphipy-0.1.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      929 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      381 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      552 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      430 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       50 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      208 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681      124 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      182 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      168 2023-04-25 03:05:00.000000 analphipy-0.1.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.011342 analphipy-0.1.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-04-25 03:05:00.000000 analphipy-0.1.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.012467 analphipy-0.1.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681   113096 2023-04-25 03:05:00.000000 analphipy-0.1.0/examples/usage/usage.ipynb
+-rw-r--r--   0 wpk      (42033)    36681     5428 2023-04-25 03:05:00.000000 analphipy-0.1.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.015821 analphipy-0.1.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-25 03:05:00.000000 analphipy-0.1.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-04-25 03:05:00.000000 analphipy-0.1.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681      290 2023-04-25 03:08:15.089612 analphipy-0.1.0/setup.cfg
+-rw-r--r--   0 wpk      (42033)    36681      323 2023-04-25 03:05:00.000000 analphipy-0.1.0/setup.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:14.924342 analphipy-0.1.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.035095 analphipy-0.1.0/src/analphipy/
+-rw-r--r--   0 wpk      (42033)    36681     1074 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     1031 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/_attrs_utils.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.048091 analphipy-0.1.0/src/analphipy/_docfiller/
+-rw-r--r--   0 wpk      (42033)    36681    19472 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/_docfiller/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    23552 2023-03-22 17:48:12.000000 analphipy-0.1.0/src/analphipy/_docfiller/docscrape.py
+-rw-r--r--   0 wpk      (42033)    36681     2526 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/_docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681      478 2022-09-27 20:23:36.000000 analphipy-0.1.0/src/analphipy/_typing.py
+-rw-r--r--   0 wpk      (42033)    36681    12807 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/base_potential.py
+-rw-r--r--   0 wpk      (42033)    36681     6297 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/cached_decorators.py
+-rw-r--r--   0 wpk      (42033)    36681    12925 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/measures.py
+-rw-r--r--   0 wpk      (42033)    36681    15134 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/norofrenkel.py
+-rw-r--r--   0 wpk      (42033)    36681    14197 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/potential.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 17:48:12.000000 analphipy-0.1.0/src/analphipy/py.typed
+-rw-r--r--   0 wpk      (42033)    36681     9878 2023-04-25 03:05:00.000000 analphipy-0.1.0/src/analphipy/utils.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.045326 analphipy-0.1.0/src/analphipy.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     6596 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     3074 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-04-07 19:52:25.000000 analphipy-0.1.0/src/analphipy.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033)    36681       73 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       10 2023-04-25 03:08:14.000000 analphipy-0.1.0/src/analphipy.egg-info/top_level.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.060512 analphipy-0.1.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681       39 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     6600 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-04-25 03:08:15.085562 analphipy-0.1.0/tests/data/
+-rw-r--r--   0 wpk      (42033)    36681     1175 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_lj_.csv
+-rw-r--r--   0 wpk      (42033)    36681      671 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_lj_nm_.csv
+-rw-r--r--   0 wpk      (42033)    36681     1273 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_sw_.csv
+-rw-r--r--   0 wpk      (42033)    36681      862 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/crit_eff_yukawa_.csv
+-rw-r--r--   0 wpk      (42033)    36681      110 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_hs_.csv
+-rw-r--r--   0 wpk      (42033)    36681    15874 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_lj_.csv
+-rw-r--r--   0 wpk      (42033)    36681     5137 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_lj_nm_.csv
+-rw-r--r--   0 wpk      (42033)    36681     2479 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_stockmayer_.csv
+-rw-r--r--   0 wpk      (42033)    36681    14148 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_sw_.csv
+-rw-r--r--   0 wpk      (42033)    36681     5317 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/eff_yukawa_.csv
+-rw-r--r--   0 wpk      (42033)    36681    18038 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_hs_.csv
+-rw-r--r--   0 wpk      (42033)    36681    21577 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_lj_.csv
+-rw-r--r--   0 wpk      (42033)    36681     7033 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_lj_nm_.csv
+-rw-r--r--   0 wpk      (42033)    36681     3284 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_stockmayer_.csv
+-rw-r--r--   0 wpk      (42033)    36681     9423 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_sw_.csv
+-rw-r--r--   0 wpk      (42033)    36681     4247 2022-09-26 16:03:57.000000 analphipy-0.1.0/tests/data/vir_yukawa_.csv
+-rw-r--r--   0 wpk      (42033)    36681     2145 2023-03-22 17:48:12.000000 analphipy-0.1.0/tests/test_generic.py
+-rw-r--r--   0 wpk      (42033)    36681      735 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/test_js.py
+-rw-r--r--   0 wpk      (42033)    36681     1738 2023-03-22 17:48:12.000000 analphipy-0.1.0/tests/test_nf_derivs.py
+-rw-r--r--   0 wpk      (42033)    36681     3035 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/test_norofrenkel.py
+-rw-r--r--   0 wpk      (42033)    36681     2027 2023-03-22 17:48:12.000000 analphipy-0.1.0/tests/test_potentials.py
+-rw-r--r--   0 wpk      (42033)    36681     3353 2023-04-25 03:05:00.000000 analphipy-0.1.0/tests/test_secondvirial.py
+-rw-r--r--   0 wpk      (42033)    36681     4569 2023-04-25 03:05:00.000000 analphipy-0.1.0/tox.ini
```

### Comparing `analphipy-0.0.6/.cruft.json` & `analphipy-0.1.0/.cruft.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8390582827260459%*

 * *Differences: {"'commit'": "'f7522615a7ab432e28a39c485f4110b86b9e37af'",*

 * * "'context'": "{'cookiecutter': {'_copy_without_render': {insert: [(3, "*

 * *              "'docs/_templates/autodocsumm/*.rst'), (4, 'docs/_static/css/*'), (5, "*

 * *              "'docs/_static/js/*'), (6, 'changelog.d/templates/*'), (7, "*

 * *              "'changelog.d/templates/auto-changlog/*')]}}}",*

 * * "'skip'": "{insert: [(1, 'docs/examples/usage/demo.ipynb'), (2, 'examples/usage/demo.ipynb'), (3, "*

 * *           "'docs/examples/example-usage.md')], delete:  […]*

```diff
@@ -1,16 +1,21 @@
 {
     "checkout": "feature/markdown",
-    "commit": "d3593d03bd05ad4e3c61b1d2afcdd2ad65ce669d",
+    "commit": "f7522615a7ab432e28a39c485f4110b86b9e37af",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
-                "docs/_templates/autosummary/*.rst"
+                "docs/_templates/autosummary/*.rst",
+                "docs/_templates/autodocsumm/*.rst",
+                "docs/_static/css/*",
+                "docs/_static/js/*",
+                "changelog.d/templates/*",
+                "changelog.d/templates/auto-changlog/*"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
             "conda_channel": "wpk-nist",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
@@ -27,19 +32,13 @@
             "use_pytest": "y",
             "version": "0.0.1"
         }
     },
     "directory": null,
     "skip": [
         "src/analphipy/__init__.py",
-        "README.md",
-        "HISTORY.md",
-        "AUTHORS.md",
-        "environment.yaml",
-        "environment/",
-        "docs/api.md",
-        "docs/index.md",
-        "docs/spelling_wordlist.txt",
-        "tests/test_analphipy.py"
+        "docs/examples/usage/demo.ipynb",
+        "examples/usage/demo.ipynb",
+        "docs/examples/example-usage.md"
     ],
     "template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git"
 }
```

### Comparing `analphipy-0.0.6/.gitignore` & `analphipy-0.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -103,10 +103,10 @@
 .mypy_cache/
 
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
-/docs/generated/
+/docs/**/generated/
 /monkeytype.sqlite3
 /dist-conda/
```

### Comparing `analphipy-0.0.6/.pre-commit-config.yaml` & `analphipy-0.1.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,88 +1,132 @@
 ---
-# pre-commit install
+# pre-commt install
 # pre-commit run --all-files
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
+default_install_hook_types:
+  - pre-commit
+  - commit-msg
+
+# default_stages: [commit]
+
 repos:
+  #* Top level
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-added-large-files
       - id: check-yaml
-        #     args: [--unsafe]
-  # Ruff
+      - id: check-json
+      - id: check-merge-conflict
+      - id: check-symlinks
+      - id: check-toml
+  - repo: https://github.com/pre-commit/pre-commit
+    rev: v3.2.2
+    hooks:
+      - id: validate_manifest
+  #* Formatting
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: "v3.0.0-alpha.6" # Use the sha / tag you want to point at
+    hooks:
+      - id: prettier
+        stages: [commit]
+        additional_dependencies:
+          - prettier-plugin-toml
+  #** markdown
+  - repo: https://github.com/DavidAnson/markdownlint-cli2
+    rev: v0.6.0
+    hooks:
+      - id: markdownlint-cli2
+        args: ["--style prettier"]
+  #* Linting
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.254'
+    rev: "v0.0.261"
     hooks:
       - id: ruff
-        args: ["--fix"]
-  # isort should run before black as black sometimes tweaks the isort output
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        stages: [manual]
-  # https://github.com/python/black#version-control-integration
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
+      # - id: black-jupyter
+      # Move to just black.  use nbqa for notebook formatting
       - id: black
+  # blacken-docs
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: "1.13.0"  # replace with latest tag on GitHub
+    rev: "1.13.0" # replace with latest tag on GitHub
     hooks:
       - id: blacken-docs
         additional_dependencies:
-          - black==23.1.0
+          - black==23.3.0
         exclude: ^README.md
-  - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.8
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: blackdoc
-        additional_dependencies: ["black==23.1.0"]
-      - id: blackdoc-autoupdate-black
-  - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+      - id: nbqa-ruff
+        additional_dependencies: [ruff]
+      - id: nbqa-black
+        additional_dependencies: [black]
+
+  #* Commit message
+  - repo: https://github.com/commitizen-tools/commitizen
+    rev: v3.0.1
+    hooks:
+      - id: commitizen
+        stages: [commit-msg]
+
+  #* Manual Linting
+  - repo: local
     hooks:
-      - id: codespell
-        types_or: [python, rst, markdown, cython, c]
-        additional_dependencies: [tomli]
-        args: [-I, docs/spelling_wordlist.txt]
+      - id: mypy
+        name: mypy
+        entry: tox
+        args: ["-e", "lint-mypy"]
+        language: system
+        pass_filenames: false
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
+        stages: [manual]
+  # isort, pyupgrade, flake8 defer to ruff
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
         stages: [manual]
-  # this should be run before flake8 to
-  # this should be run externally
-  # messes up too many things
-  # - repo: https://github.com/PyCQA/docformatter
-  #   rev: v1.5.0
-  #   hooks:
-  #     - id: docformatter
-  #       args: [--in-place]
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
+    hooks:
+      - id: pyupgrade
+        stages: [manual]
+        args: [--py38-plus]
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         stages: [manual]
-        additional_dependencies: [flake8-docstrings]
-        exclude: ^src/cmomy/tests/|^docs/conf.py|^setup.py
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+        additional_dependencies:
+          - flake8-docstrings
+          - Flake8-pyproject
+          # - pep8-naming
+          # - flake8-rst-docstrings
+        exclude: ^tests/|^src/analphipy/tests/|^docs/conf.py|^setup.py
+  - repo: https://github.com/nbQA-dev/nbQA
+    rev: 1.7.0
     hooks:
-      - id: mypy
-        # `properies` & `asv_bench` are copied from setup.cfg.
-        # `_typed_ops.py` is added since otherwise mypy will complain (but notably only in pre-commit)
-        exclude: properties|asv_bench|_typed_ops.py|conf.py
-        # This is slow and so we take it out of the fast-path; requires passing
-        # `--hook-stage manual` to pre-commit
+      - id: nbqa-pyupgrade
+        additional_dependencies: [pyupgrade]
         stages: [manual]
-        additional_dependencies: [types-pkg_resources, typing-extensions==3.10.0.0, numpy]
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+        args: [--py38-plus]
+      - id: nbqa-isort
+        additional_dependencies: [isort]
+        stages: [manual]
+  #** spelling
+  - repo: https://github.com/codespell-project/codespell
+    rev: v2.2.4
     hooks:
-      - id: pyupgrade
+      - id: codespell
+        types_or: [python, rst, markdown, cython, c]
+        additional_dependencies: [tomli]
+        args: [-I, docs/spelling_wordlist.txt]
         stages: [manual]
-        args:
-          - --py38-plus
-          # remove on f-strings in Py3.7
-          - --keep-percent-format
```

### Comparing `analphipy-0.0.6/LICENSE` & `analphipy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/PKG-INFO` & `analphipy-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,181 @@
 Metadata-Version: 2.1
 Name: analphipy
-Version: 0.0.6
+Version: 0.1.0
 Summary: Utilities to perform stat mech analysis of pair potentials
+Home-page: https://github.com/usnistgov/analphipy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/usnistgov/analphipy
 Project-URL: documentation, https://pages.nist.gov/analphipy/
 Keywords: analphipy
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+<!-- markdownlint-disable MD041 -->
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!-- For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/analphipy
+-->
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/analphipy
-<!-- [pypi-badge]: https://badge.fury.io/py/analphipy -->
 [pypi-link]: https://pypi.org/project/analphipy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/analphipy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/analphipy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/analphipy
 [conda-link]: https://anaconda.org/wpk-nist/analphipy
-<!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/analphipy/blob/master/LICENSE
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
+[license-link]: https://github.com/usnistgov/analphipy/blob/main/LICENSE
 
-[numpy]: https://numpy.org
-[Numba]: https://numba.pydata.org/
-[xarray]: https://docs.xarray.dev/en/stable/
-[jensen-shannon]: https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence
-[noro-frenkel]: https://en.wikipedia.org/wiki/Noro%E2%80%93Frenkel_law_of_corresponding_states
+<!-- other links -->
 
-# `analphipy`
+[jensen-shannon]:
+  https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence
+[noro-frenkel]:
+  https://en.wikipedia.org/wiki/Noro%E2%80%93Frenkel_law_of_corresponding_states
 
-Utilities to perform metric analysis on fluid pair potentials.  The main features of `analphipy` as follows:
+# `analphipy`
 
+Utilities to perform metric analysis on fluid pair potentials. The main features
+of `analphipy` as follows:
 
 ## Overview
 
-`analphipy` is a python package to calculate metrics for classical models for pair potentials.  It provides a simple and extendable api for pair potentials creation.  Several routines to calculate metrics are included in the package.
+`analphipy` is a python package to calculate metrics for classical models for
+pair potentials. It provides a simple and extendable api for pair potentials
+creation. Several routines to calculate metrics are included in the package.
 
 ## Features
 
 - Pre-defined spherically symmetric potentials
 - Simple interface to extended to user defined pair potentials
 - Routines to calculate [Noro-Frenkel] effective parameters.
 - Routines to calculate [Jensen-Shannon] divergence
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 Use one of the following to install `analphipy`
 
-``` bash
+```bash
 pip install analphipy
 ```
 
 or
 
-``` bash
+```bash
 conda install -c wpk-nist analphipy
 ```
 
 ## Example usage
 
 ```python
 import analphipy
 
 ```
 
-
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `analphipy` in action.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Contact
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
-This package was created with [Cookiecutter] and the [wpk-nist-gov/cookiecutter-pypackage] Project template forked from [audreyr/cookiecutter-pypackage].
+This package was created with [Cookiecutter] and the
+[wpk-nist-gov/cookiecutter-pypackage] Project template forked from
+[audreyr/cookiecutter-pypackage].
 
-[audreyr/cookiecutter-pypackage]: https://github.com/audreyr/cookiecutter-pypackage
+[audreyr/cookiecutter-pypackage]:
+  https://github.com/audreyr/cookiecutter-pypackage
 [cookiecutter]: https://github.com/audreyr/cookiecutter
-[wpk-nist-gov/cookiecutter-pypackage]: https://github.com/wpk-nist-gov/cookiecutter-pypackage
+[wpk-nist-gov/cookiecutter-pypackage]:
+  https://github.com/wpk-nist-gov/cookiecutter-pypackage
+
+# Changelog
+
+Changelog for `analphipy`
+
+## Unreleased
+
+See the fragment files in [changelog.d](https://github.com/usnistgov/analphipy)
+
+<!-- scriv-insert-here -->
+
+## v0.1.0 — 2023-04-24
+
+### Changed
+
+- Update package layout
+- New linters via pre-commit
+- Development env now handled by tox
+
+## v0.0.6 - 2023-03-22
+
+Full set of changes:
+[`v0.0.5...v0.0.6`](https://github.com/usnistgov/analphipy/compare/v0.0.5...v0.0.6)
+
+## v0.0.5 - 2023-03-22
+
+Full set of changes:
+[`v0.0.4...v0.0.5`](https://github.com/usnistgov/analphipy/compare/v0.0.4...v0.0.5)
+
+## v0.0.4 - 2022-09-27
+
+Full set of changes:
+[`v0.0.3...v0.0.4`](https://github.com/usnistgov/analphipy/compare/v0.0.3...v0.0.4)
+
+## v0.0.3 - 2022-09-26
+
+Full set of changes:
+[`v0.0.2...v0.0.3`](https://github.com/usnistgov/analphipy/compare/v0.0.2...v0.0.3)
 
-# History
+## v0.0.2 - 2022-09-26
 
-## 0.0.1 (2021-12-09)
+Full set of changes:
+[`v0.0.1...v0.0.2`](https://github.com/usnistgov/analphipy/compare/v0.0.1...v0.0.2)
 
-- First release on PyPI.
+## v0.0.1 - 2022-09-26
 
 This software was developed by employees of the National Institute of Standards
 and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
 United States Code Section 105, works of NIST employees are not subject to
 copyright protection in the United States and are considered to be in the public
 domain. Permission to freely use, copy, modify, and distribute this software and
 its documentation without fee is hereby granted, provided that this notice and
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `analphipy-0.0.6/README.md` & `analphipy-0.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,103 @@
-[![Repo][repo-badge]][repo-link]
-[![Docs][docs-badge]][docs-link]
+<!-- markdownlint-disable MD041 -->
+
+[![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!-- For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/analphipy
+-->
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/analphipy
-<!-- [pypi-badge]: https://badge.fury.io/py/analphipy -->
 [pypi-link]: https://pypi.org/project/analphipy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/analphipy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/analphipy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/analphipy
 [conda-link]: https://anaconda.org/wpk-nist/analphipy
-<!-- Use total link so works from anywhere -->
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/analphipy/blob/master/LICENSE
-<!-- For more badges, see https://shields.io/category/other and https://naereen.github.io/badges/ -->
+[license-link]: https://github.com/usnistgov/analphipy/blob/main/LICENSE
 
-[numpy]: https://numpy.org
-[Numba]: https://numba.pydata.org/
-[xarray]: https://docs.xarray.dev/en/stable/
-[jensen-shannon]: https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence
-[noro-frenkel]: https://en.wikipedia.org/wiki/Noro%E2%80%93Frenkel_law_of_corresponding_states
+<!-- other links -->
 
-# `analphipy`
+[jensen-shannon]:
+  https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence
+[noro-frenkel]:
+  https://en.wikipedia.org/wiki/Noro%E2%80%93Frenkel_law_of_corresponding_states
 
-Utilities to perform metric analysis on fluid pair potentials.  The main features of `analphipy` as follows:
+# `analphipy`
 
+Utilities to perform metric analysis on fluid pair potentials. The main features
+of `analphipy` as follows:
 
 ## Overview
 
-`analphipy` is a python package to calculate metrics for classical models for pair potentials.  It provides a simple and extendable api for pair potentials creation.  Several routines to calculate metrics are included in the package.
+`analphipy` is a python package to calculate metrics for classical models for
+pair potentials. It provides a simple and extendable api for pair potentials
+creation. Several routines to calculate metrics are included in the package.
 
 ## Features
 
 - Pre-defined spherically symmetric potentials
 - Simple interface to extended to user defined pair potentials
 - Routines to calculate [Noro-Frenkel] effective parameters.
 - Routines to calculate [Jensen-Shannon] divergence
 
 ## Status
 
-This package is actively used by the author.  Please feel free to create a pull request for wanted features and suggestions!
+This package is actively used by the author. Please feel free to create a pull
+request for wanted features and suggestions!
 
 ## Quick start
 
 Use one of the following to install `analphipy`
 
-``` bash
+```bash
 pip install analphipy
 ```
 
 or
 
-``` bash
+```bash
 conda install -c wpk-nist analphipy
 ```
 
 ## Example usage
 
 ```python
 import analphipy
 
 ```
 
-
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `analphipy` in action.
 
 ## License
 
-This is free software.  See [LICENSE][license-link].
+This is free software. See [LICENSE][license-link].
 
 ## Contact
 
 The author can be reached at wpk@nist.gov.
 
 ## Credits
 
-This package was created with [Cookiecutter] and the [wpk-nist-gov/cookiecutter-pypackage] Project template forked from [audreyr/cookiecutter-pypackage].
+This package was created with [Cookiecutter] and the
+[wpk-nist-gov/cookiecutter-pypackage] Project template forked from
+[audreyr/cookiecutter-pypackage].
 
-[audreyr/cookiecutter-pypackage]: https://github.com/audreyr/cookiecutter-pypackage
+[audreyr/cookiecutter-pypackage]:
+  https://github.com/audreyr/cookiecutter-pypackage
 [cookiecutter]: https://github.com/audreyr/cookiecutter
-[wpk-nist-gov/cookiecutter-pypackage]: https://github.com/wpk-nist-gov/cookiecutter-pypackage
+[wpk-nist-gov/cookiecutter-pypackage]:
+  https://github.com/wpk-nist-gov/cookiecutter-pypackage
```

### Comparing `analphipy-0.0.6/docs/_static/css/nist-combined.css` & `analphipy-0.1.0/docs/_static/css/nist-combined.css`

 * *Files 13% similar despite different names*

```diff
@@ -2,168 +2,168 @@
  * @file
  * Header and Footer styles
  *
  */
 
 /* Header Styles */
 .nist-header {
-  background: #000;
-  font-family: Helvetica, Arial, sans-serif;
-  padding: 10px 16px 0;
-  font-size: 16px;
+    background: #000;
+    font-family: Helvetica, Arial, sans-serif;
+    padding: 10px 16px 0;
+    font-size: 16px;
 }
 
 .nist-header__logo-link {
-  display: inline-block;
-  height: 35px;
+    display: inline-block;
+    height: 35px;
 }
 
 /* For Bootstrap Users - Updated the vertical align property since it interfered with NIST SVG icon. */
 .nist-header__logo-link svg {
-  vertical-align: inherit;
+    vertical-align: inherit;
 }
 
 .nist-header__logo-icon {
-  fill: #fff;
-  display: inline-block;
-  height: 16px;
-  position: relative;
-  top: -2px;
-  margin-right: 2px;
+    fill: #fff;
+    display: inline-block;
+    height: 16px;
+    position: relative;
+    top: -2px;
+    margin-right: 2px;
 }
 
 .nist-header__logo-image {
-  fill: #fff;
-  display: inline-block;
-  height: 24px;
-  width: 90px;
+    fill: #fff;
+    display: inline-block;
+    height: 24px;
+    width: 90px;
 }
 
 /* Limit main content area width */
 .nist-main {
-  margin-left: auto;
-  margin-right: auto;
-  max-width: 1200px;
-  padding: 0 16px;
-  box-sizing: border-box;
+    margin-left: auto;
+    margin-right: auto;
+    max-width: 1200px;
+    padding: 0 16px;
+    box-sizing: border-box;
 }
 
 /* Make sure body has no margin or padding when using only this header component */
 body {
-  padding: 0;
-  margin: 0;
+    padding: 0;
+    margin: 0;
 }
 
 /* Footer styles */
 
 .nist-footer {
-  background: #333333;
-  position: relative;
-  z-index: 200;
-  font-family: Helvetica, Arial, sans-serif;
-  font-size: 16px;
-  box-sizing: border-box;
+    background: #333333;
+    position: relative;
+    z-index: 200;
+    font-family: Helvetica, Arial, sans-serif;
+    font-size: 16px;
+    box-sizing: border-box;
 }
 
 .nist-footer__inner {
-  margin-left: auto;
-  margin-right: auto;
-  max-width: 1200px;
-  padding: 0 16px;
+    margin-left: auto;
+    margin-right: auto;
+    max-width: 1200px;
+    padding: 0 16px;
 }
 
 .nist-footer__inner:after {
-  content: "";
-  display: table;
-  clear: both;
+    content: "";
+    display: table;
+    clear: both;
 }
 
 .nist-footer {
-  background: #333333;
-  color: white;
-  padding: 40px 0px;
-  position: relative;
+    background: #333333;
+    color: white;
+    padding: 40px 0px;
+    position: relative;
 }
 
 .nist-footer a {
-  color: white;
-  text-decoration: none;
+    color: white;
+    text-decoration: none;
 }
 
 .nist-footer .nist-footer__logo img {
-  width: 340px;
-  display: block;
-  margin-left: auto;
-  margin-right: auto;
-  margin-top: 30px;
+    width: 340px;
+    display: block;
+    margin-left: auto;
+    margin-right: auto;
+    margin-top: 30px;
 }
 
 .nist-footer__logo {
-  display: flex;
-  justify-content: center;
-  align-items: center;
+    display: flex;
+    justify-content: center;
+    align-items: center;
 }
 
 .nist-footer__menu {
-  clear: both;
-  margin-bottom: 10px;
+    clear: both;
+    margin-bottom: 10px;
 }
 
 .nist-footer__menu.first {
-  padding-top: 20px;
+    padding-top: 20px;
 }
 
 .nist-footer__menu ul {
-  margin: 0;
-  padding: 0;
-  list-style: none;
-  text-align: center;
+    margin: 0;
+    padding: 0;
+    list-style: none;
+    text-align: center;
 }
 
 .nist-footer__menu-item {
-  display: inline-block;
-  font-size: 14px;
-  padding: 0;
-  margin-left: 0;
+    display: inline-block;
+    font-size: 14px;
+    padding: 0;
+    margin-left: 0;
 }
 
 .nist-footer__menu-item:after {
-  content: '|';
-  margin-right: 1.6px;
-  display: inherit;
-  position: static;
-  font: inherit;
-  line-height: inherit;
-  color: inherit;
+    content: "|";
+    margin-right: 1.6px;
+    display: inherit;
+    position: static;
+    font: inherit;
+    line-height: inherit;
+    color: inherit;
 }
 
 .nist-footer__menu-item:last-child:after {
-  content: none;
+    content: none;
 }
 
 .nist-footer__menu-item a {
-  font-weight: normal;
-  margin-right: 6px;
-  white-space: nowrap;
-  padding: 0.5em 0;
-  display: inline-block;
+    font-weight: normal;
+    margin-right: 6px;
+    white-space: nowrap;
+    padding: 0.5em 0;
+    display: inline-block;
 }
 
 /**
  * Stick footer to bottom of page
  * Source: https://css-tricks.com/couple-takes-sticky-footer/
  */
 
 html.nist-footer-bottom,
 html.nist-footer-bottom body {
-  height: 100%;
+    height: 100%;
 }
 html.nist-footer-bottom body {
-  display: flex;
-  flex-direction: column;
+    display: flex;
+    flex-direction: column;
 }
 html.nist-footer-bottom #main {
-  flex: 1 0 auto;
+    flex: 1 0 auto;
 }
 html.nist-footer-bottom .nist-footer {
-  flex-shrink: 0;
+    flex-shrink: 0;
 }
```

### Comparing `analphipy-0.0.6/docs/_static/js/nist-header-footer.js` & `analphipy-0.1.0/docs/_static/js/nist-header-footer.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,27 @@
 /**
  * @file
  * Header and footer scripts
  *
  */
 
 $(document).ready(function() {
-
     $("body").prepend('<div id="nistheadergoeshere"></div>');
     $.ajax({
         url: "https://pages.nist.gov/nist-header-footer/boilerplate-header.html",
         cache: false,
         dataType: "html",
         success: function(data) {
-            $('#nistheadergoeshere').append(data);
+            $("#nistheadergoeshere").append(data);
         },
     });
 
     $("body").append('<div id="nistfootergoeshere"></div>');
     $.ajax({
         url: "https://pages.nist.gov/nist-header-footer/boilerplate-footer.html",
         cache: false,
         dataType: "html",
         success: function(data) {
-            $('#nistfootergoeshere').append(data);
+            $("#nistfootergoeshere").append(data);
         },
     });
-
 });
```

### Comparing `analphipy-0.0.6/docs/_templates/autosummary/class.rst` & `analphipy-0.1.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/autosummary/module.rst` & `analphipy-0.1.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/class-individual-pages.rst` & `analphipy-0.1.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/class-single-page.rst` & `analphipy-0.1.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/custom-module-template.rst` & `analphipy-0.1.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/module-custom-imported.rst` & `analphipy-0.1.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/module-custom.rst` & `analphipy-0.1.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/module-single.rst` & `analphipy-0.1.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/module-template.rst` & `analphipy-0.1.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/_templates/test/class-1.rst` & `analphipy-0.1.0/docs/_templates/test/class-1.rst`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/conf.py` & `analphipy-0.1.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
+"""Build docs."""
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath(".."))
 
 import analphipy
 
@@ -35,14 +36,15 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "autodocsumm",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
+    "sphinx.ext.autosectionlabel",
     "IPython.sphinxext.ipython_directive",
     "IPython.sphinxext.ipython_console_highlighting",
     # "nbsphinx",
     ## easier external links
     # "sphinx.ext.extlinks",
     ## view source code on created page
     # "sphinx.ext.viewcode",
@@ -55,14 +57,15 @@
     ## pretty things up?
     # "sphinx_design"
     ## myst stuff
     "myst_nb",
 ]
 
 nitpicky = True
+autosectionlabel_prefix_document = True
 
 # -- myst stuff ---------------------------------------------------------
 myst_enable_extensions = [
     "dollarmath",
     "amsmath",
     "deflist",
     "fieldlist",
@@ -136,20 +139,20 @@
     "members",
     "inherited-members",
     "private-members",
     "show-inheritance",
 ]
 autodoc_typehints = "none"
 
-# -- napolean ------------------------------------------------------------------
+# -- napoleon ------------------------------------------------------------------
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 
 napoleon_use_param = False
-napoleon_use_rtype = True
+napoleon_use_rtype = False
 napoleon_preprocess_types = True
 napoleon_type_aliases = {
     # general terms
     "sequence": ":term:`sequence`",
     "iterable": ":term:`iterable`",
     "callable": ":py:func:`callable`",
     "dict_like": ":term:`dict-like <mapping>`",
@@ -273,23 +276,23 @@
 #
 
 html_theme = "sphinx_book_theme"
 
 html_theme_options = dict(
     # analytics_id=''  this is configured in rtfd.io
     # canonical_url="",
-    repository_url="https://github.com/usnistgov/cmomy",
+    repository_url=f"https://github.com/{github_username}/analphipy",
     repository_branch=html_context["github_version"],
     path_to_docs=html_context["doc_path"],
     # use_edit_page_button=True,
     use_repository_button=True,
     use_issues_button=True,
     home_page_in_toc=True,
-    show_toc_level=6,
-    show_navbar_depth=2,
+    show_toc_level=2,
+    show_navbar_depth=0,
 )
 # handle nist css/js from here.
 html_css_files = [
     # "css/nist-combined.css",
     "https://pages.nist.gov/nist-header-footer/css/nist-combined.css",
     "https://pages.nist.gov/leaveNotice/css/jquery.leaveNotice.css",
 ]
@@ -411,38 +414,41 @@
     "matplotlib": ("https://matplotlib.org/stable/", None),
     "dask": ("https://docs.dask.org/en/latest", None),
     "cftime": ("https://unidata.github.io/cftime", None),
     "sparse": ("https://sparse.pydata.org/en/latest/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
 }
 
+linkcheck_ignore = ["https://doi.org/"]
+
 
 # based on numpy doc/source/conf.py
 def linkcode_resolve(domain, info):
-    """
-    Determine the URL corresponding to Python object
-    """
+    """Determine the URL corresponding to Python object"""
     import inspect
+    from operator import attrgetter
 
     if domain != "py":
         return None
 
-    modname = info["module"]
-    fullname = info["fullname"]
+    parent_name, *sub_parts = info["module"].split(".")
+    parent_mod = sys.modules.get(parent_name)
 
-    submod = sys.modules.get(modname)
-    if submod is None:
-        return None
+    try:
+        if len(sub_parts) > 0:
+            sub_name = ".".join(sub_parts)
+            obj = attrgetter(sub_name)(parent_mod)
+        else:
+            obj = parent_mod
 
-    obj = submod
-    for part in fullname.split("."):
-        try:
-            obj = getattr(obj, part)
-        except AttributeError:
-            return None
+        # get fullname
+        obj = attrgetter(info["fullname"])(obj)
+
+    except AttributeError:
+        return None
 
     try:
         fn = inspect.getsourcefile(inspect.unwrap(obj))
     except TypeError:
         fn = None
     if not fn:
         return None
```

### Comparing `analphipy-0.0.6/docs/make.bat` & `analphipy-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/docs/notebooks/usage.ipynb` & `analphipy-0.1.0/docs/examples/usage/usage.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9790146010350465%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(4, \'* [M.G. Noro and D. Frenkel (2000), "Extended '*

 * *            'corresponding-states behavior for particles with variable range attractions". Journal '*

 * *            "of Chemical Physics, 113, 2941.](https://doi.org/10.1063/1.1288684)\\n'), (6, '* "*

 * *            '[J.D. Weeks, D. Chandler and H.C. Andersen (1971), "Role of Repulsive Forces in '*

 * *            'Determining the Equilibrium Structure of Simple Liquids", Journal of Chemical Physics '*

 * *            "54, 5237-524 […]*

```diff
@@ -21,17 +21,17 @@
             "id": "16d3dad0",
             "metadata": {},
             "source": [
                 "## Useful references\n",
                 "\n",
                 "Please see the following for a primer on the type of analysis provided in `analphipy`.\n",
                 "\n",
-                "* [M.G. Noro and D. Frenkel (2000), \"Extended corresponding-states behavior for particles with variable range attractions\". Journal of Chemical Physics, 113, 2941.](https://aip.scitation.org/doi/10.1063/1.1288684)\n",
+                "* [M.G. Noro and D. Frenkel (2000), \"Extended corresponding-states behavior for particles with variable range attractions\". Journal of Chemical Physics, 113, 2941.](https://doi.org/10.1063/1.1288684)\n",
                 "* [J.A. Barker and D. Henderson (1976), \"What Is Liquid? Understanding the States of Matter\". Reviews of Modern Physics, 48, 587-671.](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.48.587)\n",
-                "* [J.D. Weeks, D. Chandler and H.C. Andersen (1971), \"Role of Repulsive Forces in Determining the Equilibrium Structure of Simple Liquids\", Journal of Chemical Physics 54, 5237-5247](https://aip.scitation.org/doi/abs/10.1063/1.1674820)\n",
+                "* [J.D. Weeks, D. Chandler and H.C. Andersen (1971), \"Role of Repulsive Forces in Determining the Equilibrium Structure of Simple Liquids\", Journal of Chemical Physics 54, 5237-5247](https://doi.org/10.1063/1.1674820)\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d652eba9",
             "metadata": {},
@@ -39,57 +39,65 @@
                 "# A simple example\n",
                 "\n",
                 "Let's take a look at the properties of a [Lennard-Jones](https://en.wikipedia.org/wiki/Lennard-Jones_potential) (LJ), which has a length scale $\\sigma$ and energy scale $\\epsilon$.  It is typical to consider units of length in terms of $\\sigma$ and energy in terms of $\\epsilon$, which is the same as setting $\\sigma=1$ and $\\epsilon=1$.  We create a LJ potential object using the following:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "8e7e61ab",
             "metadata": {},
             "outputs": [],
             "source": [
+                "# the passed function should only be a function of r, so use partial\n",
+                "from functools import partial\n",
+                "\n",
+                "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
+                "import pandas as pd\n",
+                "\n",
                 "import analphipy\n",
-                "p = analphipy.potential.LennardJones(sig=1., eps=1.)"
+                "\n",
+                "p = analphipy.potential.LennardJones(sig=1.0, eps=1.0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "ff1da7cd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "1.122462048309373"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p.r_min"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "6941c582",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<analphipy.measures.Measures at 0x110fb4cd0>"
+                            "<analphipy.measures.Measures at 0x109de5fd0>"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p.to_measures()"
             ]
@@ -106,14 +114,24 @@
                 "This defines an LJ potential.  This contains things like the potential energy function {meth}`LennardJones.phi`, the derivative function {meth}`LennardJones.dphidr`, the location of the minimum in the potential {attr}`Analytic.r_min`, and the value at the minimum {attr}`Analytic.phi_min`. \n",
                 "For example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
+            "id": "77d2bdbe",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%matplotlib inline"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
             "id": "b6408369",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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b3/725owYYKefvrpFp/7fD5dcskl6t27tzZu3KiysjJdf/31Mk1TTzzxhCSpoqJCF110kSZPnqzNmzdrx44duuGGG5Samqof//jHkSy/y3zKma8AACDCIhrqFi5cKEl65plnWv189erV2rZtm4qKitS3b19J0qOPPqobbrhBDz30kDIyMrR06VLV1dXpmWeekdvt1siRI7Vjxw499thjmjdvngzDiOQQTpvfb2o7twcDAAARZukxdZs2bdLIkSPDgU6Spk+fLo/Ho61bt4b7TJo0SW63u1mfAwcOaO/eva2u1+PxqKKiotnDKsXHGm8PNpjbgwEAgAixNNSVlJQoNze3WVvPnj2VmJiokpKSNvuE3of6nGjRokXKzMwMPwoKCiJQffuErk83JDdNLm4PBgAAIqTDKeOBBx6QYRgnfWzZsqXd62tt96lpms3aT+wTOkmirV2vCxYsUHl5efhRVFTU7nq6WujMV3a9AgCASOrwMXVz5szRd77znZP2GThwYLvW1adPH7333nvN2o4dO6aGhobwbFyfPn1azMgdPnxYklrM4IW43e5mu2utRKgDAADR0OFQl52drezs7C758gkTJuihhx7SwYMHlZeXJylw8oTb7dZZZ50V7vOzn/1M9fX1SkxMDPfp27dvu8OjlUIXHh7ehzNfAQBA5ET0IK/9+/frgw8+0P79++Xz+fTBBx/ogw8+UFVVlSRp2rRpGjFihK699loVFhbqjTfe0N13361bbrlFGRmBma2rr75abrdbN9xwgz7++GOtXLlSv/rVr+LizNcqbg8GAACiJKKXNLnvvvv017/+Nfz+zDPPlCStXbtWF1xwgZxOp1555RXddtttmjhxopKTk3X11Vfrt7/9bXiZzMxMrVmzRrfffrvGjRunnj17at68eZo3b14kS+8S27k9GAAAiBLDjKdbM3RSRUWFMjMzVV5eHp4BjIbn3t+v+S9+pPOH9tbfvj8+at8LAADso705hmtsRNDe4K5Xrk8HAAAijVAXQfvKqiVJA7JSLK4EAADYHaEugkIzdYQ6AAAQaYS6CDFNU/vDM3XsfgUAAJFFqIuQ0qp6Vdf75DCk/J7JVpcDAABsjlAXIaHj6fIyk+V2OS2uBgAA2B2hLkJCFx0emM3xdAAAIPIIdRGyj+PpAABAFBHqIiR85msvZuoAAEDkEeoiZN/R0OVM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",
                         "text/plain": [
@@ -121,31 +139,26 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "%matplotlib inline\n",
-                "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "\n",
                 "r = np.linspace(0.9, 2.5, 100)\n",
                 "fig, axes = plt.subplots(2)\n",
-                "axes[0].set_title('phi')\n",
+                "axes[0].set_title(\"phi\")\n",
                 "axes[0].plot(r, p.phi(r))\n",
                 "\n",
-                "axes[0].plot(p.r_min, p.phi_min, marker='o')\n",
+                "axes[0].plot(p.r_min, p.phi_min, marker=\"o\")\n",
                 "\n",
-                "axes[1].set_title('dphidr')\n",
+                "axes[1].set_title(\"dphidr\")\n",
                 "axes[1].plot(r, p.dphidr(r))\n",
-                "axes[1].plot(p.r_min, p.dphidr(p.r_min), marker='o')\n",
+                "axes[1].plot(p.r_min, p.dphidr(p.r_min), marker=\"o\")\n",
                 "\n",
-                "fig.tight_layout()\n",
-                "\n"
+                "fig.tight_layout()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6002f2ba",
             "metadata": {},
             "source": [
@@ -158,15 +171,15 @@
                 "3. Determine an effective square-well attractive range.\n",
                 "\n",
                 "Please look at the above references for further information. To perform the analysis on our LJ potential, we first need to create a {class}`analphipy.norofrenkel.NoroFrenkelPair` object.  This is conveniently done with the following method."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 6,
             "id": "f6401305",
             "metadata": {},
             "outputs": [],
             "source": [
                 "nf = p.to_nf()"
             ]
         },
@@ -176,46 +189,46 @@
             "metadata": {},
             "source": [
                 "Now, the object `nf` can be used to calculate effective metrics.  For example, to calculate the effective hard-sphere diameter at an inverse temperature $\\beta = 1/(k_{\\rm B} T)$, where $k_{\\rm B}$ is Boltzmann's constant, use the following:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 7,
             "id": "e02fe163",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "1.0156054202252172"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "nf.sig(beta=1.0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "id": "f559659f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[<matplotlib.lines.Line2D at 0x1a1b98310>]"
+                            "[<matplotlib.lines.Line2D at 0x10af53890>]"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
                         "image/png": "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denSRUuWLGnsbtRabfp91113XbDfXbt2tbdxln2+Zs0ajR07VhEREbJYLFq6dOll37N69WolJibKx8dH7du315tvvlmtjaPv89r225WO89r23ZWO89r23VWO9RkzZqhfv37y8/NTmzZtNH78eO3fv/+y7zP7WCewXMbChQs1efJk/e1vf9O2bds0bNgwjR49WhkZGRdsv2bNGl177bVavny5tmzZouHDh2vs2LHatm1blXb+/v7Kysqq8vDx8WmKLtVYbft+3v79+6v0q2PHjvbXkpOTNWHCBE2cOFE7duzQxIkTdcstt2jjxo2N3Z0aq22///Wvf1Xpb2ZmpoKCgvSb3/ymSjtn2OfFxcXq2bOnZs6cWaP2aWlpuv766zVs2DBt27ZNjz76qB566CEtWrTI3sYZ9nlt++1Kx3lt+36esx/nUu377irH+urVq/XAAw/o+++/18qVK1VRUaGkpCQVFxdf9D0OcawbuKT+/fsbkyZNqrKtc+fOxrRp02r8GV26dDGefPJJ+/P33nvPCAgIaKgSG01t+/7dd98ZkozTp09f9DNvueUW47rrrquybdSoUcatt95a73obSn33+ZIlSwyLxWKkp6fbtznLPv85ScaSJUsu2eavf/2r0blz5yrb/vCHPxgDBw60P3eGff5zNen3hTjrcf5zNem7qxznv1SX/e4qx3pOTo4hyVi9evVF2zjCsc4ZlksoKyvTli1blJSUVGV7UlKSNmzYUKPPsNlsKiwsVFBQUJXtRUVFateunaKionTDDTdU+z8zs9Wn771791Z4eLhGjBih7777rsprycnJ1T5z1KhRNf73bGwNsc9nz56tkSNHql27dlW2O/o+r4uL7c/NmzervLz8km0cZZ83BGc9zuvDmY/zhuIqx3p+fr4kVfv9/TlHONYJLJeQm5srq9WqsLCwKtvDwsKUnZ1do8946aWXVFxcrFtuucW+rXPnzpo7d66WLVum+fPny8fHR0OGDNGBAwcatP76qEvfw8PD9fbbb2vRokVavHix4uPjNWLECK1Zs8beJjs7u17/no2tvvs8KytLX375pe69994q251hn9fFxfZnRUWFcnNzL9nGUfZ5Q3DW47wuXOE4bwiucqwbhqGpU6dq6NCh6tat20XbOcKx7jKrNTcmi8VS5blhGNW2Xcj8+fP1xBNP6NNPP1WbNm3s2wcOHKiBAwfanw8ZMkR9+vTRv//9b7322msNV3gDqE3f4+PjFR8fb38+aNAgZWZm6sUXX9SVV15Zp880S11rnDt3rlq3bq3x48dX2e5M+7y2LvRv9cvtzrDP68oVjvPacKXjvD5c5Vh/8MEH9eOPP2rdunWXbWv2sc4ZlksICQmRu7t7tXSYk5NTLUX+0sKFC3XPPffo448/1siRIy/Z1s3NTf369XOoBF6fvv/cwIEDq/Srbdu29f7MxlSffhuGoTlz5mjixIny8vK6ZFtH3Od1cbH96eHhoeDg4Eu2cZR9Xh/Ofpw3FGc7zuvLVY71P/3pT1q2bJm+++47RUVFXbKtIxzrBJZL8PLyUmJiolauXFll+8qVKzV48OCLvm/+/Pm666679NFHH2nMmDGX/TmGYWj79u0KDw+vd80Npa59/6Vt27ZV6degQYOqfeaKFStq9ZmNqT79Xr16tVJTU3XPPfdc9uc44j6vi4vtz759+8rT0/OSbRxln9eVKxznDcXZjvP6cvZj3TAMPfjgg1q8eLG+/fZbxcXFXfY9DnGsN8ituy5swYIFhqenpzF79mxjz549xuTJk42WLVva7wqfNm2aMXHiRHv7jz76yPDw8DBef/11Iysry/7Iy8uzt3niiSeM//73v8bBgweNbdu2GXfffbfh4eFhbNy4scn7dym17fsrr7xiLFmyxEhJSTF27dplTJs2zZBkLFq0yN5m/fr1hru7u/GPf/zD2Lt3r/GPf/zD8PDwML7//vsm79/F1Lbf5/3ud78zBgwYcMHPdJZ9XlhYaGzbts3Ytm2bIcl4+eWXjW3bthmHDx82DKN63w8dOmS0aNHCmDJlirFnzx5j9uzZhqenp/HJJ5/Y2zjDPq9tv13pOK9t313lODeM2vf9PGc/1u+//34jICDAWLVqVZXf35KSEnsbRzzWCSw18Prrrxvt2rUzvLy8jD59+lQZ+nXnnXcaV111lf35VVddZUiq9rjzzjvtbSZPnmzExMQYXl5eRmhoqJGUlGRs2LChCXtUc7Xp+z//+U+jQ4cOho+PjxEYGGgMHTrU+OKLL6p95n/+8x8jPj7e8PT0NDp37lzlD52jqE2/DcMw8vLyDF9fX+Ptt9++4Oc5yz4/P2T1Yr+/F+r7qlWrjN69exteXl5GbGys8cYbb1T7XEff57Xttysd57Xtuysd53X5fXeFY/1CfZZkvPfee/Y2jnisW84VDwAA4LC4hwUAADg8AgsAAHB4BBYAAODwCCwAAMDhEVgAAIDDI7AAAACHR2ABAAAOj8ACAAAcHoEFAAA4PAILAABweAQWAADg8AgsAADA4f1/PBPc+FRiDbAAAAAASUVORK5CYII=",
                         "text/plain": [
@@ -238,25 +251,25 @@
             "metadata": {},
             "source": [
                 "Likewise, the effective attractive range `lambda` can be found using"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "id": "bf9027e4",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[<matplotlib.lines.Line2D at 0x1a1c4ad50>]"
+                            "[<matplotlib.lines.Line2D at 0x10d841a50>]"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
@@ -277,15 +290,15 @@
             "metadata": {},
             "source": [
                 "Since it is common want to calculate such metrics over a spectrum of values of $\\beta$, there is a utility method {meth}`~analphipy.norofrenkel.NoroFrenkelPair.table`.  This creates a dictionary of results, which can be easily converted to a pandas DataFrame"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "id": "cdcae496",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'beta': array([0.2, 0.8, 1.4, 2. ]),\n",
@@ -296,29 +309,29 @@
                             " 'eps': [-1.0, -1.0, -1.0, -1.0],\n",
                             " 'lam': [1.6162246932413373,\n",
                             "  1.4699861479698415,\n",
                             "  1.3923506242906025,\n",
                             "  1.333901317192492]}"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# create a dictionary of values\n",
-                "betas = np.linspace(0.2, 2., 4)\n",
-                "table = nf.table(betas=betas, props=['sig','eps','lam'])\n",
+                "betas = np.linspace(0.2, 2.0, 4)\n",
+                "table = nf.table(betas=betas, props=[\"sig\", \"eps\", \"lam\"])\n",
                 "table"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "id": "364a4f37",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -382,21 +395,20 @@
                             "   beta       sig  eps       lam\n",
                             "0   0.2  0.946847 -1.0  1.616225\n",
                             "1   0.8  1.007239 -1.0  1.469986\n",
                             "2   1.4  1.027454 -1.0  1.392351\n",
                             "3   2.0  1.038996 -1.0  1.333901"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "import pandas as pd\n",
                 "pd.DataFrame(table)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "cbce0b36",
             "metadata": {},
@@ -430,37 +442,33 @@
             "execution_count": 12,
             "id": "28e63848",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "Generic(r_min=None, phi_min=None, segments=None, phi_func=functools.partial(<function my_lj_func at 0x1a3ac0f40>, sig=1.0, eps=1.0), dphidr_func=None)"
+                            "Generic(r_min=None, phi_min=None, segments=None, phi_func=functools.partial(<function my_lj_func at 0x19b71a520>, sig=1.0, eps=1.0), dphidr_func=None)"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "def my_lj_func(r, sig, eps):\n",
                 "    # function should always return an array\n",
                 "    r = np.asarray(r)\n",
-                "    x = (sig / r)\n",
-                "    \n",
-                "    return 4. * eps * (x ** 12 - x ** 6)\n",
-                "    \n",
-                "    \n",
-                "    \n",
-                "# the passed function should only be a function of r, so use partial\n",
-                "from functools import partial\n",
+                "    x = sig / r\n",
                 "\n",
-                "g = analphipy.potential.Generic(phi_func=partial(my_lj_func, sig=1., eps=1.))\n",
-                "g    "
+                "    return 4.0 * eps * (x**12 - x**6)\n",
+                "\n",
+                "\n",
+                "g = analphipy.potential.Generic(phi_func=partial(my_lj_func, sig=1.0, eps=1.0))\n",
+                "g"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "d0e515ad",
             "metadata": {},
@@ -490,49 +498,50 @@
             "source": [
                 "Note that additional info is not required, but you can explicitly pass it if so desired.  For example, include a \n",
                 "form for $d\\phi(r)/dr$"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "id": "40dab97a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def my_lj_deriv_func(r, sig, eps):\n",
                 "    r = np.asarray(r)\n",
-                "    x = (sig / r)\n",
-                "    \n",
+                "    x = sig / r\n",
+                "\n",
                 "    return -48 * eps * (x**12 - 0.5 * x**6) / r\n",
                 "\n",
-                "sig = 1.\n",
-                "eps = 1.\n",
+                "\n",
+                "sig = 1.0\n",
+                "eps = 1.0\n",
                 "g = analphipy.potential.Generic(\n",
-                "    phi_func=partial(my_lj_func, sig=sig, eps=eps), \n",
-                "    dphidr_func=partial(my_lj_deriv_func, sig=1., eps=1.),\n",
+                "    phi_func=partial(my_lj_func, sig=sig, eps=eps),\n",
+                "    dphidr_func=partial(my_lj_deriv_func, sig=1.0, eps=1.0),\n",
                 "    # infinte integration bounds\n",
-                "    segments=[0.0, np.inf]\n",
+                "    segments=[0.0, np.inf],\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 15,
             "id": "e1063d7d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([ 0.00000000e+00,  0.00000000e+00, -2.22044605e-16,  0.00000000e+00,\n",
                             "        0.00000000e+00])"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g.dphidr(r) - p.dphidr(r)"
             ]
@@ -543,84 +552,84 @@
             "metadata": {},
             "source": [
                 "Note that to investigate the Noro-Frenkel metrics, the values of `r_min` and `segments` must be set.  The latter is the integration bounds including any discontinuities.  This was done analytically in {class}`analphipy.potential.LennardJones`, but is not set in {class}`analphipy.potential.Generic`.  You can pass a value directly during the creation, or set the value numerically.  For example, we could use:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 16,
             "id": "0d31650c",
             "metadata": {},
             "outputs": [
                 {
                     "ename": "ValueError",
                     "evalue": "must set `self.r_min` to use NoroFrenkel",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[0;31mValueError\u001b[0m                                Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[17], line 2\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[38;5;66;03m# this will raise an error because we don't have a minimum\u001b[39;00m\n\u001b[0;32m----> 2\u001b[0m \u001b[43mg\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mto_nf\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
-                        "File \u001b[0;32m~/Documents/python/projects/analphipy/src/analphipy/base_potential.py:286\u001b[0m, in \u001b[0;36m_PhiBase.to_nf\u001b[0;34m(self, **kws)\u001b[0m\n\u001b[1;32m    271\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"\u001b[39;00m\n\u001b[1;32m    272\u001b[0m \u001b[38;5;124;03mCreate a :class:`analphipy.NoroFrenkelPair` object.\u001b[39;00m\n\u001b[1;32m    273\u001b[0m \n\u001b[0;32m   (...)\u001b[0m\n\u001b[1;32m    283\u001b[0m \n\u001b[1;32m    284\u001b[0m \u001b[38;5;124;03m\"\"\"\u001b[39;00m\n\u001b[1;32m    285\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mr_min \u001b[38;5;129;01mis\u001b[39;00m \u001b[38;5;28;01mNone\u001b[39;00m:\n\u001b[0;32m--> 286\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m \u001b[38;5;167;01mValueError\u001b[39;00m(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mmust set `self.r_min` to use NoroFrenkel\u001b[39m\u001b[38;5;124m\"\u001b[39m)\n\u001b[1;32m    288\u001b[0m \u001b[38;5;28;01mfor\u001b[39;00m k \u001b[38;5;129;01min\u001b[39;00m [\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mphi\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124msegments\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mr_min\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mphi_min\u001b[39m\u001b[38;5;124m\"\u001b[39m]:\n\u001b[1;32m    289\u001b[0m     \u001b[38;5;28;01mif\u001b[39;00m k \u001b[38;5;129;01mnot\u001b[39;00m \u001b[38;5;129;01min\u001b[39;00m kws:\n",
+                        "Cell \u001b[0;32mIn[16], line 2\u001b[0m\n\u001b[1;32m      1\u001b[0m \u001b[38;5;66;03m# this will raise an error because we don't have a minimum\u001b[39;00m\n\u001b[0;32m----> 2\u001b[0m \u001b[43mg\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mto_nf\u001b[49m\u001b[43m(\u001b[49m\u001b[43m)\u001b[49m\n",
+                        "File \u001b[0;32m~/Documents/python/projects/analphipy/src/analphipy/base_potential.py:290\u001b[0m, in \u001b[0;36mPhiAbstract.to_nf\u001b[0;34m(self, **kws)\u001b[0m\n\u001b[1;32m    275\u001b[0m \u001b[38;5;250m\u001b[39m\u001b[38;5;124;03m\"\"\"\u001b[39;00m\n\u001b[1;32m    276\u001b[0m \u001b[38;5;124;03mCreate a :class:`analphipy.norofrenkel.NoroFrenkelPair` object.\u001b[39;00m\n\u001b[1;32m    277\u001b[0m \n\u001b[0;32m   (...)\u001b[0m\n\u001b[1;32m    287\u001b[0m \n\u001b[1;32m    288\u001b[0m \u001b[38;5;124;03m\"\"\"\u001b[39;00m\n\u001b[1;32m    289\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mr_min \u001b[38;5;129;01mis\u001b[39;00m \u001b[38;5;28;01mNone\u001b[39;00m:\n\u001b[0;32m--> 290\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m \u001b[38;5;167;01mValueError\u001b[39;00m(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mmust set `self.r_min` to use NoroFrenkel\u001b[39m\u001b[38;5;124m\"\u001b[39m)\n\u001b[1;32m    292\u001b[0m \u001b[38;5;28;01mfor\u001b[39;00m k \u001b[38;5;129;01min\u001b[39;00m [\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mphi\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124msegments\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mr_min\u001b[39m\u001b[38;5;124m\"\u001b[39m, \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mphi_min\u001b[39m\u001b[38;5;124m\"\u001b[39m]:\n\u001b[1;32m    293\u001b[0m     \u001b[38;5;28;01mif\u001b[39;00m k \u001b[38;5;129;01mnot\u001b[39;00m \u001b[38;5;129;01min\u001b[39;00m kws:\n",
                         "\u001b[0;31mValueError\u001b[0m: must set `self.r_min` to use NoroFrenkel"
                     ]
                 }
             ],
             "source": [
                 "# this will raise an error because we don't have a minimum\n",
                 "g.to_nf()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 17,
             "id": "05b49312",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# instead set the minimum numerically with the following\n",
                 "g_with_min = g.assign_min_numeric(\n",
-                "    r0=1.0, # guess for location of minimum\n",
-                "    bounds = [0.5, 1.5], # bounds for search\n",
+                "    r0=1.0,  # guess for location of minimum\n",
+                "    bounds=[0.5, 1.5],  # bounds for search\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 18,
             "id": "2abfa2a8",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "1.3815918477142934"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g_with_min.to_nf().lam(beta=1.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 19,
             "id": "ae4bd1d3",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "1.3815918477142932"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p.to_nf().lam(beta=1.5)"
             ]
@@ -639,77 +648,77 @@
             "metadata": {},
             "source": [
                 "The classes {mod}`analphipy.potential` module provides a simple means to 'cut' the potential.  To perform a simple cut, use the method {meth}`analphipy.base_potential.PhiBase.cut`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 20,
             "id": "b8d5d48c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "p_cut = p.cut(2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 21,
             "id": "d60f722a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(0.)"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p_cut.phi(2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 22,
             "id": "98e09804",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "-0.016316891136000003"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p.phi(2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 23,
             "id": "05750d8e",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[<matplotlib.lines.Line2D at 0x1a3b8f950>]"
+                            "[<matplotlib.lines.Line2D at 0x19bc30810>]"
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
@@ -732,98 +741,98 @@
             "metadata": {},
             "source": [
                 "To perform a cut with linear force shift, use the method {meth}`analphipy.base_potential.PhiBase.lfs`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 24,
             "id": "aecaee9f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "p_lfs = p.lfs(rcut=2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 25,
             "id": "2a69e096",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(0.)"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 25,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p_lfs.phi(2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 26,
             "id": "8b890552",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(0.)"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p_lfs.dphidr(2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 27,
             "id": "3ab93509",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array(0.03899948)"
                         ]
                     },
-                    "execution_count": 28,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p_cut.dphidr(2.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 28,
             "id": "d165d42d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.03899947745280001"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 28,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "p.dphidr(2.5)"
             ]
@@ -839,41 +848,33 @@
         {
             "cell_type": "markdown",
             "id": "82b1e33d",
             "metadata": {},
             "source": [
                 "Please take a look at the api documentation for more information!"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "1b017920",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python [conda env:analphipy-env]",
+            "display_name": "analphipy-dev [conda env:dev]",
             "language": "python",
-            "name": "conda-env-analphipy-env-py"
+            "name": "conda-env-dev-py"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.0"
+            "version": "3.10.10"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `analphipy-0.0.6/environment/dev-extras.yaml` & `analphipy-0.1.0/environment/dev-extras.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 dependencies:
-    # numerics/tests
-    - matplotlib
-    - pandas
-    # development
-    # - isort
-    # - black
-    # - blackdoc
-    # - flake8
-    # testing
-    - pytest
-    - pytest-cov
-    - pytest-xdist
-    # - tox-conda
-    # specials
-    # - pre-commit
-    # repl
-    - ipython
-    - ipykernel
-    # build
-    - setuptools-scm
-    # - setuptools
-    # - twine
-    # - setuptools_scm_git_archive
-    # - build
-    # conda specific
-    # - conda-build
-    # - anaconda-client
-    # - greyskull
-    # doc stuff
-    # - sphinx
-    # - sphinx_rtd_theme
-    # - recommonmark # if want markdown
-    # - nbsphinx # if want notebooks
-    # - sphinxcontrib-spelling
-    # - sphinx-toolbox
-    # lsp stuff
-    # - autoflake
-    # - pyls-mypy
-    # - pyls-black
-    # - pyls-isort
-    # mypy
-    - mypy
-    - pytest-mypy
-    # Monkeytype: autocreate type hints
-    - MonkeyType
-    - pip
-    - pip:
-            - mypy-extensions
-            - pytest-monkeytype
-            # - flake8-mypy
-            # - attr-utils
-            # spelling?
-            # - pyenchant
+  # numerics/tests
+  - matplotlib
+  - pandas
+  # development
+  # - isort
+  # - black
+  # - blackdoc
+  # - flake8
+  # testing
+  - pytest
+  - pytest-cov
+  - pytest-xdist
+  # - tox-conda
+  # specials
+  # - pre-commit
+  # repl
+  - ipython
+  - ipykernel
+  # build
+  - setuptools-scm
+  # - setuptools
+  # - twine
+  # - setuptools_scm_git_archive
+  # - build
+  # conda specific
+  # - conda-build
+  # - anaconda-client
+  # - greyskull
+  # doc stuff
+  # - sphinx
+  # - sphinx_rtd_theme
+  # - recommonmark # if want markdown
+  # - nbsphinx # if want notebooks
+  # - sphinxcontrib-spelling
+  # - sphinx-toolbox
+  # lsp stuff
+  # - autoflake
+  # - pyls-mypy
+  # - pyls-black
+  # - pyls-isort
+  # mypy
+  - mypy
+  - pytest-mypy
+  # Monkeytype: autocreate type hints
+  - MonkeyType
+  - pip
+  - pip:
+      - mypy-extensions
+      - pytest-monkeytype
+      # - flake8-mypy
+      # - attr-utils
+      # spelling?
+      # - pyenchant
```

### Comparing `analphipy-0.0.6/environment/docs-extras.yaml` & `analphipy-0.1.0/environment/docs-extras.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 channels:
-    - conda-forge
+  - conda-forge
 dependencies:
-    - setuptools-scm
-    - ipython
-    - matplotlib
-    - pandas
-    - pip
-    - pip:
-            - pyenchant
-            # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
-            - ghp-import
-            - sphinx
-            ## themes
-            - sphinx-book-theme
-            ## optionals
-            # sphinx-design
-            - sphinx-copybutton
-            - sphinxcontrib-spelling
-            # sphinxext-rediraffe
-            ## autobuild
-            - sphinx-autobuild
-            ## myst
-            # myst-parser
-            - myst-nb
-            ## others
-            - autodocsumm
+  - setuptools-scm
+  - ipython
+  - matplotlib
+  - pandas
+  - pip
+  - pip:
+      - pyenchant
+      # TODO: something goes wonky with sphinx-book-theme and higher versions of sphinx
+      - ghp-import
+      - sphinx
+      ## themes
+      - sphinx-book-theme
+      ## optionals
+      # sphinx-design
+      - sphinx-copybutton
+      - sphinxcontrib-spelling
+      # sphinxext-rediraffe
+      ## autobuild
+      - sphinx-autobuild
+      ## myst
+      # myst-parser
+      - myst-nb
+      ## others
+      - autodocsumm
```

### Comparing `analphipy-0.0.6/pyproject.toml` & `analphipy-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,74 @@
 [build-system]
-requires = [
-    "setuptools>=61.2",
-    "setuptools_scm[toml]>=3.4",
-    "setuptools_scm_git_archive",
-]
+requires = ["setuptools>=61.2", "setuptools_scm[toml]>=7.0"]
 build-backend = "setuptools.build_meta"
 
-
 [project]
 name = "analphipy"
-authors = [{name = "William P. Krekelberg", email = "wpk@nist.gov"}]
-license = {text = "NIST license"}
+authors = [{ name = "William P. Krekelberg", email = "wpk@nist.gov" }]
+license = { text = "NIST license" }
 description = "Utilities to perform stat mech analysis of pair potentials"
 # if using markdown
 # long_description_content_type = text/markdown
 keywords = ["analphipy"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: Public Domain",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["readme", "version"]
 requires-python = ">=3.8"
 dependencies = [
     # additional packages
     "attrs",
     "typing-extensions",
     "numpy",
     "scipy",
     "custom-inherit",
 ]
 
-
 [project.urls]
 homepage = "https://github.com/usnistgov/analphipy"
 documentation = "https://pages.nist.gov/analphipy/"
 
 [project.optional-dependencies]
 test = [
     "pandas",
     "pytest",
     # "pytest-mypy",
     # "mypy",
-]
-# dev = []
-# docs = []
-
 
-[tool.setuptools]
-package-dir = {"" = "src"}
-zip-safe = true # if using mypy, must be False
-include-package-data = true
-license-files = ["LICENSE"]
-
-[tool.setuptools.packages.find]
-where = ["src"]
-namespaces = false
-
-[tool.setuptools.package-data]
-analphipy = [
-    "py.typed"
 ]
 
+## Defer this to setup.cfg
+## Will transition when everything works (grayskull in particular)
+## and will remove setup.py
+# [tool.setuptools]
+# zip-safe = true # if using mypy, must be False
+# include-package-data = true
+# license-files = ["LICENSE"]
+# [tool.setuptools.packages.find]
+# namespaces = true
+# where = ["src"]
+## include = []
+## exclude = []
 [tool.setuptools.dynamic]
-readme = {file = ["README.md", "HISTORY.md", "LICENSE"], content-type = "text/markdown"}
+readme = { file = [
+    "README.md",
+    "CHANGELOG.md",
+    "LICENSE"
+], content-type = "text/markdown" }
 
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
@@ -83,53 +77,51 @@
 testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["analphipy"]
 
-
 [tool.ruff]
+fix = true
 line-length = 88
 update-check = false
 target-version = "py38"
-
 select = [
-  # pyflakes
-  "F",
-  # pycodestyle
-  "E",
-  "W",
-  # isort
-  "I",
-  # pyupgrade
-  "UP",
-  # # flake8-2020
-  # "YTT",
-  # # flake8-bugbear
-  # "B",
-  # # flake8-quotes
-  # "Q",
-  # # pylint
-  # "PLE", "PLR", "PLW",
-  # # misc lints
-  # "PIE",
-  # # tidy imports
-  # "TID",
-  # # implicit string concatenation
-  # "ISC",
-  # # type-checking imports
-  # "TCH",
+    # pyflakes
+    "F",
+    # pycodestyle
+    "E",
+    "W",
+    # isort
+    "I",
+    # pyupgrade
+    "UP",
+    # pydocstyle
+    "D",
+    # # flake8-2020
+    "YTT",
+    # flake8-bugbear
+    "B",
+    # flake8-quotes
+    "Q",
+    # # pylint
+    # "PLE", "PLR", "PLW",
+    # misc lints
+    "PIE",
+    # # tidy imports
+    "TID",
+    # # implicit string concatenation
+    # "ISC",
+    # type-checking imports
+    "TCH",
 ]
-
-
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 # fixable = ["A", "B", "C", "D", "E", "F", "..."]
-unfixable = []
-
+unfixable = ["TID"]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
@@ -144,18 +136,17 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "tests/",
     "src/analphipy/tests",
 ]
-
-
 ignore = [
     # # whitespace before ':' - doesn't work well with black
     # "E203",
     # module level import not at top of file
     "E402",
     # line too long - let black worry about that
     "E501",
@@ -163,54 +154,99 @@
     "E731",
     # # line break before binary operator
     # "W503",
     # allow black line after docstring
     "D202",
     "D105",
     "D205",
+    # this leads to errors with placing titles in module
+    # docstrings
     "D400",
     "D401",
+    "D415",
+    "D102",
+    "D103",
+    # these are useful, but too many errors
+    # due to use of docfiller
+    "D417",
+    "D107",
+    "D203",
+    "D212",
+    # Allow relative imports
+    "TID252",
 ]
-
-per-file-ignores = {}
-
+per-file-ignores = {  }
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.isort]
 known-first-party = ["analphipy"]
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
-[tool.cruft]
+[tool.nbqa.addopts]
+ruff = ["--fix", "--extend-ignore=D100,B018"]
 
+[tool.flake8]
+docstring-convention = "numpy"
+ignore = [
+    # # whitespace before ':' - doesn't work well with black
+    "E203",
+    # module level import not at top of file
+    "E402",
+    # line too long - let black worry about that
+    "E501",
+    # do not assign a lambda expression, use a def
+    "E731",
+    # # line break before binary operator
+    "W503",
+    # allow black line after docstring
+    "D202",
+    "D105",
+    "D205",
+    # this leads to errors with placing titles in module
+    # docstrings
+    "D400",
+    "D401",
+    "D415",
+    "D102",
+    "D103",
+    # these are useful, but too many errors
+    # due to use of docfiller
+    "D417",
+    "D107",
+    "D203",
+    "D212",
+]
+
+[tool.scriv]
+format = "md"
+md_header_level = "2"
+new_fragment_template = "file: changelog.d/templates/new_fragment.md.j2"
+
+[tool.commitizen]
+use_shortcuts = true
+
+[tool.cruft]
 
 [tool.mypy]
-files = ["src/analphipy"]
+files = ["src/analphipy", "tests"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
-exclude = [
-    ".eggs",
-    "doc",
-    "docs",
-]
+exclude = [".eggs", ".tox", "doc", "docs"]
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
-       "numpy.*",
-       "pandas.*",
-       "pytest.*",
-       "scipy.*",
-       "setuptools",
+    "custom_inherit",
+    "scipy.integrate.*",
+    "scipy.optimize.*",
+    "scipy.misc.*"
 ]
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = []
-
-# version spanning code is hard to type annotate (and most of this module will
-# be going away soon anyways)
```

### Comparing `analphipy-0.0.6/src/analphipy/__init__.py` & `analphipy-0.1.0/src/analphipy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # from .potentials_base import PhiAnalytic, PhiBase, PhiCut, PhiGeneric, PhiLFS
 
 # updated versioning scheme
 try:
     from importlib.metadata import version as _version
 except ImportError:
     # if the fallback library is missing, we are doomed.
-    from importlib_metadata import version as _version  # type: ignore[no-redef]
+    from importlib_metadata import version as _version
 
 try:
     __version__ = _version("analphipy")
 except Exception:
     # Local copy or not installed with setuptools.
     # Disable minimum version checks on downstream libraries.
     __version__ = "999"
```

### Comparing `analphipy-0.0.6/src/analphipy/_attrs_utils.py` & `analphipy-0.1.0/src/analphipy/_attrs_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from __future__ import annotations
 
 import attrs
 import numpy as np
 
 
 def attrs_clear_cache(self, attribute, value):
-    """
-    clear out _cache if setting value
-    """
-    setattr(self, "_cache", {})
+    """Clear out _cache if setting value"""
+    self._cache = {}
     return value
 
 
 def optional_converter(converter):
-    """
-    Create a converter which can pass through None
-    """
+    """Create a converter which can pass through None"""
 
     def wrapped(value):
         if value is None or attrs.NOTHING:
             return value
         else:
             return converter(value)
 
@@ -44,11 +40,9 @@
         with np.printoptions(threshold=threshold, **kws):
             return str(value)
 
     return wrapped
 
 
 def private_field(init=False, repr=False, **kws):
-    """
-    Create a private attrs field.
-    """
+    """Create a private attrs field."""
     return attrs.field(init=init, repr=repr, **kws)
```

### Comparing `analphipy-0.0.6/src/analphipy/_docfiller/__init__.py` & `analphipy-0.1.0/src/analphipy/_docfiller/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         out = join_string.join(out)
 
     return out
 
 
 class AttributeDict(Mapping):
     """
-    Dictionary with recusive attribute like access.
+    Dictionary with recursive attribute like access.
 
     To be used in str.format calls, so can expand on fields like
     `{name.property}` in a nested manner.
 
     Parameters
     ----------
     entries : dict
@@ -288,14 +288,15 @@
 
 
 def _build_param_docstring(name, ptype, desc):
     """
     Create multiline documentation of single name, type, desc.
 
     Parameters
+    ----------
     ==========
     name : str
         Parameter Name
     ptype : str
         Parameter type
     desc : list of str
         Parameter description
@@ -450,17 +451,15 @@
                 "Examples",
             ]
         }
     return parsed
 
 
 def dedent_recursive(data):
-    """
-    Dedent nested mapping of strings.
-    """
+    """Dedent nested mapping of strings."""
     out = type(data)()
     for k in data:
         v = data[k]
         if isinstance(v, str):
             v = dedent(v).strip()
         else:
             v = dedent_recursive(v)
@@ -513,17 +512,15 @@
         return type(self)(dedent_recursive(self.data))
 
     @gcached(prop=False)
     def keys(self):
         return _recursive_keys(self.data)
 
     def assign_combined_key(self, new_key, keys):
-        """
-        combine multiple keys into single key
-        """
+        """Combine multiple keys into single key"""
 
         data = self.data.copy()
 
         data[new_key] = "\n".join([self.data[k] for k in keys])
         return type(self)(data)
 
     @classmethod
@@ -563,17 +560,15 @@
             if isinstance(v, cls):
                 kwargs[k] = v.data
 
         _update_data(kwargs)
         return cls(data)
 
     def append(self, *args, **kwargs):
-        """
-        Calls ``concat`` method with ``self`` as first argument.
-        """
+        """Calls ``concat`` method with ``self`` as first argument."""
 
         return type(self).concat(self, *args, **kwargs)
 
     @gcached()
     def params(self):
         return AttributeDict.from_dict(self.data, max_level=1)
 
@@ -696,15 +691,15 @@
         namespace=None,
         combine_keys=None,
         key_char="|",
         keep_keys=True,
         key_map=None,
     ):
         """
-        create a Docfiller instance from a function or docstring.
+        Create a Docfiller instance from a function or docstring.
 
         Parameters
         ----------
         func_or_doc
         """
         params = parse_docstring(
             func_or_doc=func_or_doc, key_char=key_char, expand=True
```

### Comparing `analphipy-0.0.6/src/analphipy/_docfiller/docscrape.py` & `analphipy-0.1.0/src/analphipy/_docfiller/docscrape.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/src/analphipy/_docstrings.py` & `analphipy-0.1.0/src/analphipy/_docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ._docfiller import DocFiller
 
 _docstrings_shared = """
 Parameters
 ----------
 segments : sequence of int
-    Integration limits. For ``n = len(segmetns)`` integration will be performed over ranges
+    Integration limits. For ``n = len(segments)`` integration will be performed over ranges
     ``(segments[0], segments[1]), (segments[1], segments[2]), ..., (segments[n-2], segments[n-]])``
 phi_rep : callable
     Repulsive part of pair potential.
 beta : float
     Inverse temperature.
 phi : callable
     Potential function.
```

### Comparing `analphipy-0.0.6/src/analphipy/base_potential.py` & `analphipy-0.1.0/src/analphipy/base_potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # type: ignore
 """
 Base classes (:mod:`analphipy.base_potential`)
 ==============================================
 """
 from __future__ import annotations
 
-from typing import Literal, Sequence, cast
+from typing import TYPE_CHECKING, Literal, Sequence, cast
 
 import attrs
 import numpy as np
 from attrs import field
 from custom_inherit import DocInheritMeta
 
 from ._attrs_utils import field_formatter, optional_converter, private_field
 from ._docstrings import docfiller_shared
-from ._typing import Float_or_ArrayLike
+
+if TYPE_CHECKING:
+    from ._typing import Float_or_ArrayLike
 from .measures import Measures
 from .norofrenkel import NoroFrenkelPair
 from .utils import minimize_phi
 
 
 # * attrs utilities
 @optional_converter
@@ -65,15 +67,16 @@
     )
 
     def asdict(self) -> dict:
         """Convert object to dictionary"""
         return attrs.asdict(self, filter=self._get_smart_filter())
 
     def new_like(self, **kws):
-        """Create a new object with optional parameters
+        """
+        Create a new object with optional parameters
 
         Parameters
         ----------
         **kws
             `attribute`, `value` pairs.
         """
         return attrs.evolve(self, **kws)
@@ -112,30 +115,30 @@
         for key, value in kws.items():
             object.__setattr__(self, key, value)
 
     def _get_smart_filter(
         self, include=None, exclude=None, exclude_private=True, exclude_no_init=True
     ):
         """
-        create a filter to include exclude names
+        Create a filter to include exclude names
 
         Parameters
         ----------
         include : sequence of str
             Names to include
         exclude : sequence of str
             names to exclude
         exclude_private : bool, default=True
             If True, exclude any names starting with '_'
         exclude_no_init : bool, default=True
             If True, exclude any fields defined with ``field(init=False)``.
 
         Notes
         -----
-        Precidence is in order
+        Precedence is in order
         `include, exclude, exclude_private exclude_no_init`.
         That is, if a name is in include and exclude and is private/no_init,
         it will be included
         """
         fields = attrs.fields(type(self))
 
         if include is None:
@@ -206,15 +209,16 @@
 
     def minimize(
         self,
         r0: float | Literal["mean"],
         bounds: tuple[float, float] | Literal["segments"] | None = None,
         **kws,
     ):
-        """Determine position `r` where ``phi`` is minimized.
+        """
+        Determine position `r` where ``phi`` is minimized.
 
         Parameters
         ----------
         r0 : float
             Guess for position of minimum.
             If value is `'mean'`, then use ``r0 = mean(bounds)``.
 
@@ -268,15 +272,15 @@
         return self.new_like(r_min=r_min, phi_min=phi_min)
 
     def to_nf(self, **kws):
         """
         Create a :class:`analphipy.norofrenkel.NoroFrenkelPair` object.
 
         Parameters
-        ---------
+        ----------
         **kws :
             Extra arguments to :class:`analphipy.norofrenkel.NoroFrenkelPair` constructor.
             parameters `phi`, `semgnets`, `r_min', `phi_min` default to values from `self`.
 
         Returns
         -------
         nf : :class:`analphipy.norofrenkel.NoroFrenkelPair`
@@ -458,14 +462,16 @@
     def _dvdrcorrect(self, r: np.ndarray) -> np.ndarray:
         out = -self._dvdrcut
         return cast(np.ndarray, out)
 
 
 @attrs.frozen
 class PhiBase(PhiAbstract):
+    """Base class for potentials."""
+
     def cut(self, rcut):
         """Create a :class:`PhiCut` potential."""
         return PhiCut(phi_base=self, rcut=rcut)
 
     def lfs(self, rcut):
         """Create a :class:`PhiLFS` potential."""
         return PhiLFS(phi_base=self, rcut=rcut)
```

### Comparing `analphipy-0.0.6/src/analphipy/cached_decorators.py` & `analphipy-0.1.0/src/analphipy/cached_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-routines to define a cached class without needing to subclass Cached class
-"""
+"""routines to define a cached class without needing to subclass Cached class"""
 
 from functools import wraps
 from inspect import signature
 
 __all__ = ["cached", "cached_func", "cached_clear", "gcached"]
 
 
@@ -17,30 +15,31 @@
         return wrapped
 
     return wrapper
 
 
 def gcached_use_cache(key=None, prop=True):
     """
-    same as gcached, but only cache func/prop if
+    Same as gcached, but only cache func/prop if
     has attribute self._use_cache and self._use_cache is True
     """
 
     def wrapper(func):
         if prop:
             wrapped = property(cached(key, check_use_cache=True)(func))
         else:
             wrapped = cached_func(key, check_use_cache=True)(func)
         return wrapped
 
     return wrapper
 
 
 def cached(key=None, check_use_cache=False):
-    """Decorator to cache a property within a class
+    """
+    Decorator to cache a property within a class
 
     Requires the Class to have a cache dict called ``_cache``.
 
     Notes
     -----
     Usage::
 
@@ -53,15 +52,15 @@
            @cached('keyname')
            def size(self):
                # This code gets ran only if the lookup of keyname fails
                # After this code has been ran once, the result is stored in
                # _cache with the key: 'keyname'
                size = 10.0
 
-            #no aguments implies give cache function name
+            #no arguments implies give cache function name
             @property
             @cached()
             def myprop(self):
                 #results in _cache['myprop']
 
     See Also
     --------
@@ -92,15 +91,16 @@
 
         return wrapper
 
     return cached_lookup
 
 
 def cached_func(key=None, check_use_cache=False):
-    """Decorator to cache a function within a class
+    """
+    Decorator to cache a function within a class
 
     Requires the Class to have a cache dict called ``_cache``.
 
     Notes
     -----
     Usage::
 
@@ -113,22 +113,22 @@
                # This code gets ran only if the lookup of keyname fails
                # After this code has been ran once, the result is stored in
                # _cache with the key: 'keyname'
                # a long calculation...
                return long_calc(self,val)
                # if already executed result in _cache[('keyname',) + args]
 
-            #no aguments implies give cache function name
+            #no arguments implies give cache function name
             @property
             @cached()
             def myprop(self):
                 #results in _cache['myprop']
 
 
-    See also
+    See Also
     --------
     cached_clear : corresponding decorator to remove cache
 
     cached : decorator for properties
 
     """
```

### Comparing `analphipy-0.0.6/src/analphipy/measures.py` & `analphipy-0.1.0/src/analphipy/measures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 """
 Routines to calculate measures of pair potentials (:mod:`analphipy.measures`)
 =============================================================================
 """
 
 from __future__ import annotations
 
-from typing import Callable, Mapping, Sequence, Union, cast
+from typing import TYPE_CHECKING, Callable, Mapping, Sequence, Union, cast
 
 import numpy as np
 from custom_inherit import doc_inherit
 
 from analphipy.cached_decorators import gcached
 
 from ._docstrings import docfiller_shared  # type: ignore
-from ._typing import ArrayLike, Float_or_ArrayLike, Phi_Signature
+
+if TYPE_CHECKING:
+    from ._typing import ArrayLike, Float_or_ArrayLike, Phi_Signature
 from .utils import TWO_PI, add_quad_kws, combine_segmets, quad_segments
 
 __all__ = [
     "Measures",
     "secondvirial",
     "secondvirial_dbeta",
     "secondvirial_sw",
     "diverg_kl_cont",
     "diverg_js_cont",
 ]
 
 
-def other():
-    """A function"""
-    pass
-
-
 @docfiller_shared
 def secondvirial(
     phi: Phi_Signature,
     beta: float,
     segments: ArrayLike,
     err: bool = False,
     full_output: bool = False,
@@ -196,16 +193,16 @@
 @docfiller_shared
 def diverg_kl_disc(
     P: Float_or_ArrayLike, Q: Float_or_ArrayLike, axis: int | None = None
 ) -> float | np.ndarray:
     """
     Calculate discrete Kullback–Leibler divergence
 
-    Parameteres
-    -----------
+    Parameters
+    ----------
     P, Q : array-like
         Probabilities to consider
     Returns
     -------
     result : float or ndarray
         value of KB divergence
 
@@ -509,15 +506,15 @@
         {volume_int_func}
 
         See Also
         --------
         ~analphipy.measures.diverg_js_cont
 
         References
-        --------
+        ----------
         `See here for more info <https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence#Symmetrised_divergence>`
         """
 
         if beta_other is None:
             beta_other = beta
 
         p = lambda x: np.exp(-beta * self.phi(x))
```

### Comparing `analphipy-0.0.6/src/analphipy/norofrenkel.py` & `analphipy-0.1.0/src/analphipy/norofrenkel.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 
 from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
 
 import numpy as np
 from custom_inherit import doc_inherit
 
 from ._docstrings import DOCFILLER_SHARED, docfiller_shared  # type: ignore
-from ._typing import ArrayLike, Float_or_Array, Float_or_ArrayLike, Phi_Signature
 from .cached_decorators import gcached
 from .measures import secondvirial, secondvirial_dbeta, secondvirial_sw
 from .utils import TWO_PI, add_quad_kws, minimize_phi, quad_segments
 
 if TYPE_CHECKING:
+    from ._typing import ArrayLike, Float_or_Array, Float_or_ArrayLike, Phi_Signature
     from .base_potential import PhiBase  # type: ignore
-
 # Hack to document module level docstring
 __doc__ = __doc__.format(**DOCFILLER_SHARED.data)
 
 __all__ = [
     "sig_nf",
     "sig_nf_dbeta",
     "lam_nf",
@@ -46,15 +45,16 @@
     phi_rep: Phi_Signature,
     beta: float,
     segments: ArrayLike,
     err: bool = False,
     full_output: bool = False,
     **kws,
 ):
-    r"""Noro-Frenkel/Barker-Henderson effective hard sphere diameter.
+    r"""
+    Noro-Frenkel/Barker-Henderson effective hard sphere diameter.
 
     This is calculated using the formula [1]_ [2]_
 
     .. math::
 
         \sigma_{{\rm BH}}(\beta) = \int_0^{{\infty}} dr \left( 1 - \exp[-\beta \phi_{{\rm rep}}(r)]\right)
 
@@ -419,49 +419,53 @@
                 quad_kws=quad_kws,
                 **kws,
             )
 
     @gcached(prop=False)
     @add_quad_kws
     def secondvirial(self, beta: float, **kws):
-        """Second virial coefficient.
+        """
+        Second virial coefficient.
 
         See Also
         --------
         ~analphipy.measures.secondvirial
         """
         return secondvirial(phi=self.phi, beta=beta, segments=self.segments, **kws)
 
     @gcached()
     def _segments_rep(self) -> list:
         return [x for x in self.segments if x < self.r_min] + [self.r_min]
 
     @gcached(prop=False)
     @add_quad_kws
     def sig(self, beta: float, **kws):
-        """Effective hard sphere diameter.
+        """
+        Effective hard sphere diameter.
 
         See Also
         --------
         ~analphipy.norofrenkel.sig_nf
 
         """
         return sig_nf(self.phi_rep, beta=beta, segments=self._segments_rep, **kws)
 
     def eps(self, beta: float, **kws) -> float:
-        """Effective square well epsilon.
+        """
+        Effective square well epsilon.
 
         This is equal to the minimum in ``phi``.
         """
         return cast(float, self.phi_min)
 
     @gcached(prop=False)
     @add_quad_kws
     def lam(self, beta: float, **kws):
-        """Effective square well lambda.
+        """
+        Effective square well lambda.
 
         See Also
         --------
         ~analphipy.norofrenkel.lam_nf
         """
         return lam_nf(
             beta=beta,
@@ -478,39 +482,42 @@
         eps = self.eps(beta, **kws)
         lam = lam_nf(beta=beta, sig=sig, eps=eps, B2=self.secondvirial(beta, **kws))
         return {"sig": sig, "eps": eps, "lam": lam}
 
     @gcached(prop=False)
     @add_quad_kws
     def secondvirial_dbeta(self, beta: float, **kws):
-        """Derivative of ``secondvirial`` with respect to ``beta``
+        """
+        Derivative of ``secondvirial`` with respect to ``beta``
 
         See Also
         --------
         ~analphipy.measures.secondvirial_dbeta
         """
         return secondvirial_dbeta(
             phi=self.phi, beta=beta, segments=self.segments, **kws
         )
 
     @gcached(prop=False)
     @add_quad_kws
     def sig_dbeta(self, beta: float, **kws):
-        """Derivative of effective hard-sphere diameter with respect to ``beta``
+        """
+        Derivative of effective hard-sphere diameter with respect to ``beta``
 
         See Also
         --------
         ~analphipy.norofrenkel.sig_nf_dbeta
 
         """
         return sig_nf_dbeta(self.phi_rep, beta=beta, segments=self.segments, **kws)
 
     @gcached(prop=False)
     def lam_dbeta(self, beta: float, **kws):
-        """Derivative of effective lambda parameter with respect to ``beta``.
+        """
+        Derivative of effective lambda parameter with respect to ``beta``.
 
         See Also
         --------
         ~analphipy.norofrenkel.lam_nf_dbeta
         """
         return lam_nf_dbeta(
             beta=beta,
@@ -520,15 +527,16 @@
             B2=self.secondvirial(beta, **kws),
             B2_dbeta=self.secondvirial_dbeta(beta, **kws),
             sig_dbeta=self.sig_dbeta(beta, **kws),
         )
 
     @gcached(prop=False)
     def secondvirial_sw(self, beta: float, **kws):
-        """Second virial coefficient of effective square well fluid.
+        """
+        Second virial coefficient of effective square well fluid.
 
         For testing.  This should be the same of value from :meth:`secondvirial`
         """
         return secondvirial_sw(
             beta=beta,
             sig=self.sig(beta, **kws),
             eps=self.eps(beta, **kws),
```

### Comparing `analphipy-0.0.6/src/analphipy/potential.py` & `analphipy-0.1.0/src/analphipy/potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # type: ignore
 """
 Classes/routines for pair potentials (:mod:`analphipy.potential`)
 =================================================================
 """
 from __future__ import annotations
 
-from typing import Literal, Sequence, cast
+from typing import TYPE_CHECKING, Literal, Sequence, cast
 
 import attrs
 import numpy as np
 from attrs import field
 
 from ._attrs_utils import field_array_formatter, field_formatter, private_field
-from ._typing import Float_or_ArrayLike, Phi_Signature
+
+if TYPE_CHECKING:
+    from ._typing import Float_or_ArrayLike, Phi_Signature
+
 from .base_potential import PhiBase
 
 
 @attrs.frozen
 class Generic(PhiBase):
     """
     Class to define potential using callables.
@@ -65,15 +68,16 @@
     phi_min: float = field(init=False, repr=False)
     #: Integration limits.
     segments: float = field(init=False)
 
 
 @attrs.frozen
 class LennardJones(Analytic):
-    r"""Lennard-Jones potential.
+    r"""
+    Lennard-Jones potential.
 
     .. math::
 
         \phi(r) = 4 \epsilon \left[ \left(\frac{{\sigma}}{{r}}\right)^{{12}} - \left(\frac{{\sigma}}{{r}}\right)^6\right]
 
     Parameters
     ----------
@@ -106,15 +110,15 @@
     def phi(self, r: Float_or_ArrayLike) -> np.ndarray:
         r = np.array(r)
         x2 = self._sigsq / (r * r)
         x6 = x2**3
         return cast(np.ndarray, self._four_eps * x6 * (x6 - 1.0))
 
     def dphidr(self, r: Float_or_ArrayLike) -> np.ndarray:
-        """calculate phi and dphi (=-1/r dphi/dr) at particular r"""
+        """Calculate phi and dphi (=-1/r dphi/dr) at particular r"""
         r = np.array(r)
         rinvsq = 1.0 / (r * r)
 
         x2 = self._sigsq * rinvsq
         x6 = x2 * x2 * x2
         return cast(np.ndarray, -12.0 * self._four_eps * x6 * (x6 - 0.5) / r)
 
@@ -373,15 +377,15 @@
 
         if self.segments is None:
             self._immutable_setattrs(segments=tuple(np.sqrt(x) for x in self.bounds))
 
     @classmethod
     def from_phi(cls, phi: Phi_Signature, rmin: float, rmax: float, ds: float, **kws):
         """
-        Create object from callable pair potential funciton.
+        Create object from callable pair potential function.
 
         This will evaluate ``phi`` at even spacing in ``s = r**2`` space.
 
 
         Parameters
         ----------
         phi : callable
@@ -430,17 +434,15 @@
 
     @property
     def smax(self) -> float:
         """Maximum value of `s = r**2`"""
         return self.bounds[1]
 
     def phidphi(self, r: Float_or_ArrayLike) -> tuple[np.ndarray, np.ndarray]:
-        """
-        Values of `phi` and `dphi` at `r`
-        """
+        """Values of `phi` and `dphi` at `r`"""
         r = np.asarray(r)
 
         v = np.empty_like(r)
         dv = np.empty_like(r)
 
         s = r * r
         left = s <= self.smin
@@ -473,37 +475,36 @@
 
     def dphidr(self, r: Float_or_ArrayLike) -> np.ndarray:
         r = np.asarray(r)
         return cast(np.ndarray, -r * self.phidphi(r)[1])
 
     @property
     def rsq_table(self):
-        """value of ``r**2`` where potential is defined."""
+        """Value of ``r**2`` where potential is defined."""
 
         return self.smin + np.arange(self.size + 1) * self._ds
 
     @property
     def r_table(self):
-        """
-        Values of ``r`` where potential is defined
-        """
+        """Values of ``r`` where potential is defined"""
         return np.sqrt(self.rsq_table)
 
 
 _PHI_NAMES = Literal["lj", "nm", "sw", "hs", "yk", "LJ", "NM", "SW", "HS", "YK"]
 
 
 def factory(
     potential_name: _PHI_NAMES,
     rcut: float | None = None,
     lfs: bool = False,
     cut: bool = False,
     **kws,
 ) -> PhiBase:
-    """Factory function to construct Phi object by name
+    """
+    Factory function to construct Phi object by name
 
     Parameters
     ----------
     potential_name : {lj, nm, sw, hs, yk}
         Name of potential.
     rcut : float, optional
         if passed, Construct either and 'lfs' or 'cut' version of the potential.
```

### Comparing `analphipy-0.0.6/src/analphipy/utils.py` & `analphipy-0.1.0/src/analphipy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 Utilities module (:mod:`analphipy.utils`)
 =========================================
 """
 
 from __future__ import annotations
 
 from functools import wraps
-from typing import Any, Callable, Mapping
+from typing import TYPE_CHECKING, Any, Callable, Mapping
 
 import numpy as np
 from scipy.integrate import quad
 from scipy.optimize import minimize
 
 from ._docstrings import docfiller_shared  # type: ignore
-from ._typing import ArrayLike, Float_or_ArrayLike
+
+if TYPE_CHECKING:
+    from ._typing import ArrayLike, Float_or_ArrayLike
 
 # from typing_extensions import Protocol
 
 # ArrayLike = Union[Sequence[float], NDArray[np.float_]]
 # Float_or_ArrayLike = Union[float, ArrayLike]
 # Float_or_Array = Union[float, NDArray[np.float_]]
 
@@ -31,15 +33,16 @@
 # Vector = list[float]
 
 # def scale(scalar: float, vector: Vector) -> Vector:
 #     return [scalar * num for num in vector]
 
 
 def combine_segmets(a: ArrayLike, b: ArrayLike) -> list[float]:
-    """Combine two lists of segments.
+    """
+    Combine two lists of segments.
 
     Parameters
     ----------
     a, b : array-like
         list of segments.
 
     Returns
@@ -209,17 +212,15 @@
 def partial_phi(phi, **params):
     from functools import partial
 
     return partial(phi, **params)
 
 
 def segments_to_segments_cut(segments, rcut):
-    """
-    Update segments for 'cut' potential
-    """
+    """Update segments for 'cut' potential"""
     return [x for x in segments if x < rcut] + [rcut]
 
 
 def phi_to_phi_cut(
     rcut: float,
     phi: Callable,
     dphidr: Callable | None = None,
@@ -227,15 +228,15 @@
 ):
     r"""
     Create callable ``phi`` and ``dphidr`` cut potentials.
 
     Parameters
     ----------
     rcut : float
-        Postition of cut.
+        Position of cut.
     phi : callable
         input callable function.
     dphidr : callable, optional
     input callable for :math:`d\phi/dr`
 
     Returns
     -------
@@ -293,15 +294,15 @@
 ):
     r"""
     Create callable ``phi`` and ``dphidr`` cut potentials.
 
     Parameters
     ----------
     rcut : float
-        Postition of cut.
+        Position of cut.
     phi : callable
         input callable function.
     dphidr : callable, optional
     input callable for :math:`d\phi/dr`
 
     Returns
     -------
@@ -345,17 +346,15 @@
         meta["style"] = meta.get("style", ()) + ("lfs",)
 
     return phi_cut, dphidr_cut, meta
 
 
 def wca_decomp_rep(phi, dphidr, r_min, phi_min, meta):
     def phi_rep(r: Float_or_ArrayLike) -> np.ndarray:
-        """
-        WCA repulsive potential
-        """
+        """WCA repulsive potential"""
         r = np.array(r)
         v = np.empty_like(r)
 
         left = r <= r_min
         right = ~left
 
         v[left] = phi(r[left]) - phi_min
@@ -384,17 +383,15 @@
         meta["style"] = meta.get("style", ()) + ("wca_rep",)
 
     return phi_rep, dphidr_rep, meta
 
 
 def wca_decomp_att(phi, dphidr, r_min, phi_min, meta):
     def phi_att(r: Float_or_ArrayLike) -> np.ndarray:
-        """
-        WCA repulsive potential
-        """
+        """WCA repulsive potential"""
         r = np.array(r)
         v = np.empty_like(r)
 
         left = r <= r_min
         right = ~left
 
         v[left] = phi_min
```

### Comparing `analphipy-0.0.6/tests/conftest.py` & `analphipy-0.1.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from dataclasses import asdict, dataclass
 
 import numpy as np
 import pytest
 
-# from analphipy.cached_decorators import gcached
-
 
 def phidphi_lj(r, sig=1.0, eps=1.0):
     """
     lennard jones potential and radial force
 
     Returns
     -------
```

### Comparing `analphipy-0.0.6/tests/data/crit_eff_lj_.csv` & `analphipy-0.1.0/tests/data/crit_eff_lj_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/crit_eff_lj_nm_.csv` & `analphipy-0.1.0/tests/data/crit_eff_lj_nm_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/crit_eff_sw_.csv` & `analphipy-0.1.0/tests/data/crit_eff_sw_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/crit_eff_yukawa_.csv` & `analphipy-0.1.0/tests/data/crit_eff_yukawa_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/eff_lj_.csv` & `analphipy-0.1.0/tests/data/eff_lj_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/eff_lj_nm_.csv` & `analphipy-0.1.0/tests/data/eff_lj_nm_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/eff_stockmayer_.csv` & `analphipy-0.1.0/tests/data/eff_stockmayer_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/eff_sw_.csv` & `analphipy-0.1.0/tests/data/eff_sw_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/eff_yukawa_.csv` & `analphipy-0.1.0/tests/data/eff_yukawa_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/vir_hs_.csv` & `analphipy-0.1.0/tests/data/vir_hs_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/vir_lj_.csv` & `analphipy-0.1.0/tests/data/vir_lj_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/vir_lj_nm_.csv` & `analphipy-0.1.0/tests/data/vir_lj_nm_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/vir_stockmayer_.csv` & `analphipy-0.1.0/tests/data/vir_stockmayer_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/vir_sw_.csv` & `analphipy-0.1.0/tests/data/vir_sw_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/data/vir_yukawa_.csv` & `analphipy-0.1.0/tests/data/vir_yukawa_.csv`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/test_generic.py` & `analphipy-0.1.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/test_js.py` & `analphipy-0.1.0/tests/test_js.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Simple tests for js divergence...
-"""
+"""Simple tests for js divergence..."""
 import numpy as np
 import pytest
 
 import analphipy
 from analphipy.measures import diverg_js_cont
```

### Comparing `analphipy-0.0.6/tests/test_nf_derivs.py` & `analphipy-0.1.0/tests/test_nf_derivs.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/test_norofrenkel.py` & `analphipy-0.1.0/tests/test_norofrenkel.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         .drop_duplicates()
     )
 
     if len(df) > nsamp:
         df = df.sample(nsamp)
     sig = eps = 1.0
 
-    for (z_yukawa), g in df.groupby(["z_yukawa"]):
+    for (z_yukawa), g in df.groupby("z_yukawa"):
         p = pots.Yukawa(z=z_yukawa, sig=sig, eps=eps)
 
         a = NoroFrenkelPair(phi=p.phi, segments=p.segments, r_min=sig, phi_min=-1.0)
 
         out = a.table(g["beta"], cols)
 
         for col in cols:
```

### Comparing `analphipy-0.0.6/tests/test_potentials.py` & `analphipy-0.1.0/tests/test_potentials.py`

 * *Files identical despite different names*

### Comparing `analphipy-0.0.6/tests/test_secondvirial.py` & `analphipy-0.1.0/tests/test_secondvirial.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         .drop_duplicates()
     )
 
     if len(df) > nsamp:
         df = df.sample(nsamp)
     sig = eps = 1.0
 
-    for (z_yukawa), g in df.groupby(["z_yukawa"]):
+    for (z_yukawa), g in df.groupby("z_yukawa"):
         p = pots.Yukawa(z=z_yukawa, sig=sig, eps=eps)
 
         a = NoroFrenkelPair(phi=p.phi, segments=p.segments, r_min=sig, phi_min=-1.0)
 
         out = a.table(g["beta"], ["B2", "B2_dbeta"])
 
         np.testing.assert_allclose(g["Bn_2"], out["B2"], rtol=1e-6)
```

### Comparing `analphipy-0.0.6/tox.ini` & `analphipy-0.1.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 [tox]
-skipsdist=True
+isolated_build = True
 requires = tox-conda
 envlist =
         # test
-        py3{8, 9, 10}-tests
-
+        py3{8, 9, 10, 11}-tests
 
 [base]
 package_name = analphipy
 import_name  = analphipy
 build_python = python3.10
 conda_env            = {toxinidir}/environment.yaml
 conda_env_dev        = {toxinidir}/environment/dev.yaml
 conda_env_test       = {toxinidir}/environment/test.yaml
 conda_env_docs       = {toxinidir}/environment/docs.yaml
 conda_env_dist_pypi  = {toxinidir}/environment/dist-pypi.yaml
 conda_env_dist_conda = {toxinidir}/environment/dist-conda.yaml
+conda_env_lint       = {toxinidir}/environment/lint.yaml
 conda_channels =
     wpk-nist
     conda-forge
 conda_deps_test =
 allowlist_externals =
     bash
+    zsh
     open
     cat
     rm
     echo
     mkdir
     make
+    conda
 commands_test_check =
     python --version
     python -c 'import {[base]import_name}; print( {[base]import_name}.__version__)'
     bash -ec 'echo $PWD'
     echo {posargs:{toxinidir}}
 
-
 [testenv]
+passenv = SETUPTOOLS_SCM_PRETEND_VERSION
 usedevelop =
     tests: True
 conda_env =
     tests: {[base]conda_env_test}
 allowlist_externals =
     {[base]allowlist_externals}
 commands =
     {[base]commands_test_check}
     pytest {posargs}
 
+[testenv:dev]
+description =
+    Create development environment.
+usedevelop = True
+basepython = {[base]build_python}
+conda_env = {[base]conda_env_dev}
+envdir = {toxworkdir}/dev
+commands =
+    {posargs:bash -ec 'conda list'}
 
-# Build documentation
-[testenv:docs-{build, release, clean, command, spelling, live, open}]
+[testenv:docs-{build, release, clean, command, spelling, live, open, make}]
 description =
     build: build documentation.
     release: create documentation branch.
     clean: clean build.
     spelling: run spell checking on documentation and docstrings.
     command: run arbitrary command
     live: use sphinx-autobuild
+    make: run arbitrary make command from docs/Makefile.  Passes in posargs
 usedevelop = True
 envdir     = {toxworkdir}/docs
 basepython = {[base]build_python}
 conda_env  = {[base]conda_env_docs}
 changedir  = {toxinidir}/docs
 commands =
     build: bash -c "echo $PWD"
     build: make {posargs:html}
-    # build: bash -c 'rm -rf {toxworkdir}/docs-dist/*'
-    # build: sphinx-build  --color -b html -d "{toxinidir}/docs/_build/doctrees" "{toxinidir}/docs"  "{toxworkdir}/docs/_build/html"
     open: open {toxinidir}/docs/_build/html/index.html
-    release: ghp-import -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
-    clean: rm -rf generated
-    clean: make clean
-    spelling: sphinx-build -b spelling . _build
+    release: ghp-import -o -n {posargs:-m 'update docs'} -b nist-pages {toxinidir}/docs/_build/html
+    clean: make allclean
+    spelling: make spelling
     command: {posargs}
-    live: sphinx-autobuild {toxinidir}/docs {toxinidir}/docs/_build/html
-
+    live: make livehtml
+    make: make {posargs}
 
-# create pypi dist
 [testenv:dist-pypi-{build, testrelease, release}]
 description  =
     build: build distribution.
     testrelease: upload to testpypi
     release: upload to pypi
 skip_install = True
 envdir       = {toxworkdir}/dist-pypi
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_pypi}
 changedir    = {toxinidir}
 commands     =
     build: rm -rf {toxinidir}/dist
     build: python -m build --outdir "{toxinidir}/dist/"
-
     testrelease: twine upload --repository testpypi {toxinidir}/dist/*
     release: twine upload {toxinidir}/dist/*
 
-
-# create conda dist
 [testenv:dist-conda-{recipe, build, command}]
 description  =
-    recipe: build conda recipe using grayskull
+    recipe: build conda recipe using grayskull (can optionally pass a local sdist)
     build: build conda distribution
     command: run arbitrary command
 skip_install = True
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
 changedir    = {toxinidir}/dist-conda
 commands     =
     recipe: rm -rf {toxinidir}/dist-conda/{[base]package_name}
-    recipe: grayskull pypi {[base]package_name}
+    recipe: grayskull pypi {posargs:{[base]package_name}}
     recipe: cat {[base]package_name}/meta.yaml
-
     build: rm -rf build
     build: mkdir -p build
     build: conda mambabuild --output-folder=build --no-anaconda-upload .
     command: {posargs:python}
 
-
-# test pypi/conda install from local/remote
 [testenv:test-dist-{pypi, conda}-{local,remote}-py3{8,9,10}]
 conda_channels =
     {[base]conda_channels}
 description  =
     Test install from
     pypi: pypi
     conda: conda
@@ -133,15 +134,24 @@
 conda_deps =
     conda-remote: {[base]package_name}
     conda-local: {posargs}
 deps =
     pypi-remote: {[base]package_name}
     pypi-local: {posargs}
 
-
-# Test pip installed dependencies
 [testenv:test-pip-py3{8,9,10}]
 description  =
     Test package against pip installed packages
 usedevelop   = True
 extras = test
 conda_env    = {toxinidir}/environment/test-extras.yaml
+
+[testenv:lint-{mypy,command}]
+description =
+    Run mypy on code. (run with tox -e lint -- --no-incremental to rebuild cache).
+conda_env = {[base]conda_env_lint}
+usedevelop = True
+envdir     = {toxworkdir}/lint
+basepython = {[base]build_python}
+commands =
+         mypy: mypy --color-output {posargs}
+         command: {posargs}
```

