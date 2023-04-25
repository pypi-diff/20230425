# Comparing `tmp/scippnexus-23.4.0.tar.gz` & `tmp/scippnexus-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippnexus-23.4.0.tar", last modified: Thu Apr 20 09:02:14 2023, max compression
+gzip compressed data, was "scippnexus-23.4.1.tar", last modified: Tue Apr 25 05:46:29 2023, max compression
```

## Comparing `scippnexus-23.4.0.tar` & `scippnexus-23.4.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3554 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-20 09:02:00.000000 scippnexus-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-20 09:02:00.000000 scippnexus-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-20 09:02:00.000000 scippnexus-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-20 09:02:14.796720 scippnexus-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-20 09:02:00.000000 scippnexus-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-20 09:02:00.000000 scippnexus-23.4.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_static/logo-2022.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6546 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/about/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/getting-started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/getting-started/quick-start-guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/application-definitions.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/functions.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/user-guide/nexus-classes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-04-20 09:02:00.000000 scippnexus-23.4.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-20 09:02:00.000000 scippnexus-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-20 09:02:00.000000 scippnexus-23.4.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.788720 scippnexus-23.4.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-04-20 09:02:00.000000 scippnexus-23.4.0/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-20 09:02:14.796720 scippnexus-23.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/_hdf5_nexus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/data/
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/definitions/
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/definitions/nxcansas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/file.py
--rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/leaf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxdetector.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxdisk_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxfermi_chopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxlog.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxmonitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxsource.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/nxtransformations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/src/scippnexus/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.784720 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4970 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/attrs.py
--rw-r--r--   0 runner    (1001) docker     (122)    18014 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/file.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nexus_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxcylindrical_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     6001 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxevent_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxoff_geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxsample.py
--rw-r--r--   0 runner    (1001) docker     (122)     8552 2023-04-20 09:02:00.000000 scippnexus-23.4.0/src/scippnexus/v2/nxtransformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.792720 scippnexus-23.4.0/src/scippnexus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2805 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-20 09:02:14.000000 scippnexus-23.4.0/src/scippnexus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 09:02:14.796720 scippnexus-23.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/application_definition_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/externalfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/load_files_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    23629 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxcylindrical_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    26815 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxdata_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    25349 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxdetector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxevent_data_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxmonitor_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxoff_geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxsample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18218 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tests/nxtransformations_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-20 09:02:00.000000 scippnexus-23.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.400649 scippnexus-23.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-25 05:46:13.000000 scippnexus-23.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-25 05:46:13.000000 scippnexus-23.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-25 05:46:13.000000 scippnexus-23.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 05:46:29.400649 scippnexus-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-04-25 05:46:13.000000 scippnexus-23.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-25 05:46:13.000000 scippnexus-23.4.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    17823 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_static/logo-2022.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6546 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/about/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8453 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/getting-started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10348 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/getting-started/quick-start-guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.388649 scippnexus-23.4.1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     9320 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/application-definitions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/user-guide/nexus-classes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-04-25 05:46:13.000000 scippnexus-23.4.1/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-25 05:46:13.000000 scippnexus-23.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.392649 scippnexus-23.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4747 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-25 05:46:13.000000 scippnexus-23.4.1/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.392649 scippnexus-23.4.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-04-25 05:46:13.000000 scippnexus-23.4.1/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-04-25 05:46:29.400649 scippnexus-23.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.384649 scippnexus-23.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/_hdf5_nexus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/definitions/
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/definitions/nxcansas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7424 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11291 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9912 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxdetector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxdisk_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5064 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxfermi_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxlog.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24870 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxsource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/nxtransformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.384649 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4970 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18014 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8974 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nexus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxcylindrical_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6001 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxevent_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxoff_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxsample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8552 2023-04-25 05:46:13.000000 scippnexus-23.4.1/src/scippnexus/v2/nxtransformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.396649 scippnexus-23.4.1/src/scippnexus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2805 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-25 05:46:29.000000 scippnexus-23.4.1/src/scippnexus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 05:46:29.400649 scippnexus-23.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3863 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/application_definition_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/externalfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/load_files_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23629 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxcylindrical_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26815 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxdata_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27234 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxdetector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxevent_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxmonitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxoff_geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxsample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18218 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tests/nxtransformations_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-25 05:46:13.000000 scippnexus-23.4.1/tox.ini
```

### Comparing `scippnexus-23.4.0/.github/workflows/ci.yml` & `scippnexus-23.4.1/.github/workflows/ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -41,7 +41,11 @@
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e ${{ matrix.tox }}
 
   docs:
     needs: tests
     uses: ./.github/workflows/docs.yml
+    with:
+      publish: false
+      version: ${{ github.ref_name }}
+      branch: ${{ github.head_ref == '' && github.ref_name || github.head_ref }}
```

### Comparing `scippnexus-23.4.0/.github/workflows/docs.yml` & `scippnexus-23.4.1/.github/workflows/docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -6,36 +6,46 @@
       publish:
         default: false
         type: boolean
       version:
         default: ''
         required: false
         type: string
+      branch:
+        description: 'Branch/tag with documentation source. If not set, the current branch will be used.'
+        default: ''
+        required: false
+        type: string
   workflow_call:
     inputs:
       publish:
         default: false
         type: boolean
       version:
         default: ''
         required: false
         type: string
+      branch:
+        description: 'Branch/tag with documentation source. If not set, the current branch will be used.'
+        default: ''
+        required: false
+        type: string
 
 env:
   VERSION: ${{ inputs.version }}
 
 jobs:
   docs:
     name: Build documentation
     runs-on: ubuntu-20.04
     steps:
       - run: sudo apt install --yes graphviz pandoc
       - uses: actions/checkout@v3
         with:
-          ref: ${{ inputs.version }}
+          ref: ${{ inputs.branch == '' && github.ref_name || inputs.branch }}
           fetch-depth: 0  # history required so cmake can determine version
       - uses: actions/setup-python@v3
         with:
           python-version: 3.8
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: |
```

### Comparing `scippnexus-23.4.0/.github/workflows/release.yml` & `scippnexus-23.4.1/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     name: Manage Versions
     runs-on: ubuntu-20.04
     outputs:
       version-new: ${{ steps.version.outputs.new }}
       version-replaced: ${{ steps.version.outputs.replaced }}
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0  # history required so cmake can determine version
       - uses: actions/setup-python@v3
         with:
           python-version: 3.8
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - name: Set outputs
         id: version
```

### Comparing `scippnexus-23.4.0/.pre-commit-config.yaml` & `scippnexus-23.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/LICENSE` & `scippnexus-23.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/PKG-INFO` & `scippnexus-23.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.4.0
+Version: 23.4.1
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.4.0/README.md` & `scippnexus-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/conda/meta.yaml` & `scippnexus-23.4.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/_static/favicon.ico` & `scippnexus-23.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/_static/logo-2022.svg` & `scippnexus-23.4.1/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/_templates/scipp-class-template.rst` & `scippnexus-23.4.1/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/_templates/scipp-module-template.rst` & `scippnexus-23.4.1/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/_templates/sections/header-article.html` & `scippnexus-23.4.1/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/about/about.rst` & `scippnexus-23.4.1/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/about/release-notes.rst` & `scippnexus-23.4.1/docs/about/release-notes.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/conf.py` & `scippnexus-23.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/getting-started/installation.rst` & `scippnexus-23.4.1/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/getting-started/quick-start-guide.ipynb` & `scippnexus-23.4.1/docs/getting-started/quick-start-guide.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/index.rst` & `scippnexus-23.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/user-guide/application-definitions.ipynb` & `scippnexus-23.4.1/docs/user-guide/application-definitions.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/user-guide/classes.rst` & `scippnexus-23.4.1/docs/user-guide/classes.rst`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/user-guide/nexus-classes.ipynb` & `scippnexus-23.4.1/docs/user-guide/nexus-classes.ipynb`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/docs/version.py` & `scippnexus-23.4.1/docs/version.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/pyproject.toml` & `scippnexus-23.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/requirements/ci.txt` & `scippnexus-23.4.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/requirements/docs.txt` & `scippnexus-23.4.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/requirements/static.txt` & `scippnexus-23.4.1/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/resources/logo-2022.svg` & `scippnexus-23.4.1/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/setup.cfg` & `scippnexus-23.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/__init__.py` & `scippnexus-23.4.1/src/scippnexus/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/_common.py` & `scippnexus-23.4.1/src/scippnexus/_common.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/_hdf5_nexus.py` & `scippnexus-23.4.1/src/scippnexus/_hdf5_nexus.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/data/__init__.py` & `scippnexus-23.4.1/src/scippnexus/data/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/definition.py` & `scippnexus-23.4.1/src/scippnexus/definition.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/definitions/nxcansas.py` & `scippnexus-23.4.1/src/scippnexus/definitions/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md` & `scippnexus-23.4.1/src/scippnexus/docs/our-interpretation-of-the-nexus-format.md`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/leaf.py` & `scippnexus-23.4.1/src/scippnexus/leaf.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nexus_classes.py` & `scippnexus-23.4.1/src/scippnexus/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxcylindrical_geometry.py` & `scippnexus-23.4.1/src/scippnexus/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxdata.py` & `scippnexus-23.4.1/src/scippnexus/nxdata.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxdetector.py` & `scippnexus-23.4.1/src/scippnexus/nxdetector.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxevent_data.py` & `scippnexus-23.4.1/src/scippnexus/nxevent_data.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxlog.py` & `scippnexus-23.4.1/src/scippnexus/nxlog.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxmonitor.py` & `scippnexus-23.4.1/src/scippnexus/nxmonitor.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxobject.py` & `scippnexus-23.4.1/src/scippnexus/nxobject.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxoff_geometry.py` & `scippnexus-23.4.1/src/scippnexus/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxsample.py` & `scippnexus-23.4.1/src/scippnexus/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/nxtransformations.py` & `scippnexus-23.4.1/src/scippnexus/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/typing.py` & `scippnexus-23.4.1/src/scippnexus/typing.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/__init__.py` & `scippnexus-23.4.1/src/scippnexus/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py` & `scippnexus-23.4.1/src/scippnexus/v2/application_definitions/nxcansas/nxcansas.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/attrs.py` & `scippnexus-23.4.1/src/scippnexus/v2/attrs.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/base.py` & `scippnexus-23.4.1/src/scippnexus/v2/base.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/field.py` & `scippnexus-23.4.1/src/scippnexus/v2/field.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/file.py` & `scippnexus-23.4.1/src/scippnexus/v2/file.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nexus_classes.py` & `scippnexus-23.4.1/src/scippnexus/v2/nexus_classes.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nxcylindrical_geometry.py` & `scippnexus-23.4.1/src/scippnexus/v2/nxcylindrical_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nxdata.py` & `scippnexus-23.4.1/src/scippnexus/v2/nxdata.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nxevent_data.py` & `scippnexus-23.4.1/src/scippnexus/v2/nxevent_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         # conversion to int64. This is a hack to get around this.
         event_index[event_index < 0] = num_event
 
         if len(event_index) > 0:
             event_select = slice(event_index[0],
                                  event_index[-1] if last_loaded else num_event)
         else:
-            event_select = slice(None)
+            event_select = slice(0, 0)
 
         event_time_offset = children['event_time_offset'][event_select]
 
         event_index = sc.array(dims=[_pulse_dimension],
                                values=event_index[:-1] if last_loaded else event_index,
                                dtype=sc.DType.int64,
                                unit=None)
```

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nxoff_geometry.py` & `scippnexus-23.4.1/src/scippnexus/v2/nxoff_geometry.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nxsample.py` & `scippnexus-23.4.1/src/scippnexus/v2/nxsample.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus/v2/nxtransformations.py` & `scippnexus-23.4.1/src/scippnexus/v2/nxtransformations.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/src/scippnexus.egg-info/PKG-INFO` & `scippnexus-23.4.1/src/scippnexus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippnexus
-Version: 23.4.0
+Version: 23.4.1
 Summary: h5py-like utility for NeXus files based with seamless scipp integration
 Home-page: https://scipp.github.io/scippnexus
 Author: Scipp contributors (https://github.com/scipp)
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/scippnexus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `scippnexus-23.4.0/src/scippnexus.egg-info/SOURCES.txt` & `scippnexus-23.4.1/src/scippnexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/application_definition_test.py` & `scippnexus-23.4.1/tests/application_definition_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/conftest.py` & `scippnexus-23.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/externalfile.py` & `scippnexus-23.4.1/tests/externalfile.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/load_files_test.py` & `scippnexus-23.4.1/tests/load_files_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nexus_test.py` & `scippnexus-23.4.1/tests/nexus_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxcylindrical_geometry_test.py` & `scippnexus-23.4.1/tests/nxcylindrical_geometry_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxdata_test.py` & `scippnexus-23.4.1/tests/nxdata_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxdetector_test.py` & `scippnexus-23.4.1/tests/nxdetector_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -322,22 +322,24 @@
     detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
     detector = nxroot.create_class('detector0', NXdetector)
     detector.create_field('detector_number', detector_numbers)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
     assert detector['detector_number'].dims == ('detector_number', )
 
 
-def test_nxevent_data_selection_yields_correct_pulses(nxroot):
+def test_nxevent_data_without_detector_number_selection_yields_correct_pulses(nxroot):
     detector = nxroot.create_class('detector0', NXdetector)
     create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
 
     class Load:
 
         def __getitem__(self, select=...):
-            da = detector['events'][select]
+            da = detector[select]
+            assert da.bins.size().sum(
+            ).value == da.bins.constituents['data'].sizes['event']
             return da.bins.size().values
 
     assert np.array_equal(Load()[...], [3, 0, 2, 1])
     assert np.array_equal(Load()['event_time_zero', 0], 3)
     assert np.array_equal(Load()['event_time_zero', 1], 0)
     assert np.array_equal(Load()['event_time_zero', 3], 1)
     assert np.array_equal(Load()['event_time_zero', -1], 1)
@@ -351,14 +353,46 @@
     assert np.array_equal(Load()['event_time_zero', 0:-3], [3])
     assert np.array_equal(Load()['event_time_zero', -1:], [1])
     assert np.array_equal(Load()['event_time_zero', -2:-1], [2])
     assert np.array_equal(Load()['event_time_zero', -2:], [2, 1])
     assert np.array_equal(Load()['event_time_zero', :-2], [3, 0])
 
 
+def test_nxevent_data_selection_yields_correct_pulses(nxroot):
+    detector_numbers = sc.array(dims=[''], unit=None, values=np.array([1, 2, 3, 4]))
+    detector = nxroot.create_class('detector0', NXdetector)
+    detector.create_field('detector_number', detector_numbers)
+    create_event_data_ids_1234(detector.create_class('events', snx.NXevent_data))
+
+    class Load:
+
+        def __getitem__(self, select=...):
+            da = detector[select]
+            return da.bins.size().values
+
+    assert np.array_equal(Load()[...], [2, 3, 0, 1])
+    assert np.array_equal(Load()['event_time_zero', 0], [1, 1, 0, 1])
+    assert np.array_equal(Load()['event_time_zero', 1], [0, 0, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 2], [1, 1, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 3], [0, 1, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', -1], [0, 1, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', -2], [1, 1, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 0:0], [0, 0, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 1:1], [0, 0, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 1:-3], [0, 0, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 3:3], [0, 0, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', -1:-1], [0, 0, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', 0:1], [1, 1, 0, 1])
+    assert np.array_equal(Load()['event_time_zero', 0:-3], [1, 1, 0, 1])
+    assert np.array_equal(Load()['event_time_zero', -1:], [0, 1, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', -2:-1], [1, 1, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', -2:], [1, 2, 0, 0])
+    assert np.array_equal(Load()['event_time_zero', :-2], [1, 1, 0, 1])
+
+
 def create_off_geometry_detector_numbers_1234(group: snx.Group,
                                               name: str,
                                               detector_faces: bool = True
                                               ) -> sc.DataGroup:
     dg = sc.DataGroup()
     off = group.create_class(name, NXoff_geometry)
     # square with point in center
```

### Comparing `scippnexus-23.4.0/tests/nxevent_data_test.py` & `scippnexus-23.4.1/tests/nxevent_data_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxmonitor_test.py` & `scippnexus-23.4.1/tests/nxmonitor_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxoff_geometry_test.py` & `scippnexus-23.4.1/tests/nxoff_geometry_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxsample_test.py` & `scippnexus-23.4.1/tests/nxsample_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tests/nxtransformations_test.py` & `scippnexus-23.4.1/tests/nxtransformations_test.py`

 * *Files identical despite different names*

### Comparing `scippnexus-23.4.0/tox.ini` & `scippnexus-23.4.1/tox.ini`

 * *Files identical despite different names*

