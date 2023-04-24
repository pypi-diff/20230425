# Comparing `tmp/pydantic_settings-1.99.tar.gz` & `tmp/pydantic_settings-2.0a1.tar.gz`

## Comparing `pydantic_settings-1.99.tar` & `pydantic_settings-2.0a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-1.99/.pre-commit-config.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-1.99/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-1.99/.github/FUNDING.yml
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pydantic_settings-1.99/.github/workflows/ci.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-1.99/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pydantic_settings-1.99/pydantic_settings/main.py
--rw-r--r--   0        0        0    15054 2020-02-02 00:00:00.000000 pydantic_settings-1.99/pydantic_settings/sources.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-1.99/pydantic_settings/utils.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pydantic_settings-1.99/pydantic_settings/version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-1.99/requirements/all.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-1.99/requirements/linting.in
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-1.99/requirements/linting.txt
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-1.99/requirements/pyproject.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-1.99/requirements/testing.in
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-1.99/requirements/testing.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-1.99/tests/conftest.py
--rw-r--r--   0        0        0    40327 2020-02-02 00:00:00.000000 pydantic_settings-1.99/tests/test_settings.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-1.99/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-1.99/LICENSE
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pydantic_settings-1.99/README.md
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 pydantic_settings-1.99/pyproject.toml
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pydantic_settings-1.99/PKG-INFO
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

### Comparing `pydantic_settings-1.99/.pre-commit-config.yaml` & `pydantic_settings-2.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/Makefile` & `pydantic_settings-2.0a1/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/.github/workflows/ci.yml` & `pydantic_settings-2.0a1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/pydantic_settings/main.py` & `pydantic_settings-2.0a1/pydantic_settings/main.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/pydantic_settings/sources.py` & `pydantic_settings-2.0a1/pydantic_settings/sources.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/pydantic_settings/utils.py` & `pydantic_settings-2.0a1/pydantic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/requirements/linting.txt` & `pydantic_settings-2.0a1/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/requirements/testing.txt` & `pydantic_settings-2.0a1/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/tests/test_settings.py` & `pydantic_settings-2.0a1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/LICENSE` & `pydantic_settings-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/pyproject.toml` & `pydantic_settings-2.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-1.99/PKG-INFO` & `pydantic_settings-2.0a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-settings
-Version: 1.99
+Version: 2.0a1
 Summary: Settings management using Pydantic
 Project-URL: Homepage, https://github.com/pydantic/pydantic-settings
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic-settings
 Project-URL: Changelog, https://github.com/pydantic/pydantic-settings/releases
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>
 License: The MIT License (MIT)
@@ -55,14 +55,8 @@
 
 # pydantic-settings
 
 [![CI](https://github.com/pydantic/pydantic-settings/workflows/CI/badge.svg?event=push)](https://github.com/pydantic/pydantic-settings/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
 [![Coverage](https://codecov.io/gh/pydantic/pydantic-settings/branch/main/graph/badge.svg)](https://codecov.io/gh/pydantic/pydantic-settings)
 [![license](https://img.shields.io/github/license/pydantic/pydantic-settings.svg)](https://github.com/pydantic/pydantic-settings/blob/main/LICENSE)
 
-Settings management using Pydantic, this is the new official home of Pydantic's `BaseSettings`.
-
-**Currently a work in progress.**
-
-This package was kindly donated to the [Pydantic organisation]() by Daniel Daniels, see [pydantic/pydantic#4492](https://github.com/pydantic/pydantic/pull/4492) for discussion.
-
-For the old "Hipster-orgazmic tool to mange application settings" package, see [version 0.2.5](https://pypi.org/project/pydantic-settings/0.2.5/).
+Settings management using Pydantic. **Currently a work in progress.**
```

