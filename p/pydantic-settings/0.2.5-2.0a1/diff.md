# Comparing `tmp/pydantic-settings-0.2.5.tar.gz` & `tmp/pydantic_settings-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-settings-0.2.5.tar", last modified: Wed Jun  3 19:46:03 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pydantic-settings-0.2.5.tar` & `pydantic_settings-2.0a1.tar`

### file list

```diff
@@ -1,16 +1,22 @@
--rw-r--r--   0        0        0     4604 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/README.rst
--rw-r--r--   0        0        0      295 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     1521 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/attrs_docs.py
--rw-r--r--   0        0        0     3942 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/base.py
--rw-r--r--   0        0        0     2367 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/decoder/__init__.py
--rw-r--r--   0        0        0     2165 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/decoder/common.py
--rw-r--r--   0        0        0     9608 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/decoder/json.py
--rw-r--r--   0        0        0     2913 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/decoder/yaml.py
--rw-r--r--   0        0        0     8667 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/errors.py
--rw-r--r--   0        0        0     6010 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/load.py
--rw-r--r--   0        0        0     9020 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/restorer.py
--rw-r--r--   0        0        0     2060 2020-05-25 07:49:20.666370 pydantic-settings-0.2.5/pydantic_settings/types.py
--rw-r--r--   0        0        0     1231 2020-05-22 15:57:18.217325 pydantic-settings-0.2.5/pydantic_settings/utils.py
--rw-r--r--   0        0        0     1383 2020-06-03 19:38:41.452001 pydantic-settings-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5670 2020-06-03 19:46:03.315518 pydantic-settings-0.2.5/setup.py
--rw-r--r--   0        0        0     5810 2020-06-03 19:46:03.316002 pydantic-settings-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/Makefile
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/__init__.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/main.py
+-rw-r--r--   0        0        0    15054 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/sources.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/utils.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pydantic_settings/version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/all.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/linting.in
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/linting.txt
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/pyproject.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/testing.in
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/requirements/testing.txt
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/tests/conftest.py
+-rw-r--r--   0        0        0    40327 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/tests/test_settings.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/LICENSE
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/README.md
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pydantic_settings-2.0a1/PKG-INFO
```

