# Comparing `tmp/sos_ansible-1.0.3.tar.gz` & `tmp/sos_ansible-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sos_ansible-1.0.3.tar", last modified: Mon Apr 10 07:59:41 2023, max compression
+gzip compressed data, was "sos_ansible-1.0.4.tar", last modified: Tue Apr 25 13:18:37 2023, max compression
```

## Comparing `sos_ansible-1.0.3.tar` & `sos_ansible-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.428466 sos_ansible-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/DockerfileDebug
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/controller.json
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/hub-rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/rules/tower.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/sos_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/sos_ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/file_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.436466 sos_ansible-1.0.3/sos_ansible/modules/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/helpers/write_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/locating_sos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-10 07:59:28.000000 sos_ansible-1.0.3/sos_ansible/modules/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 07:59:41.432466 sos_ansible-1.0.3/sos_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 07:59:41.000000 sos_ansible-1.0.3/sos_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.127536 sos_ansible-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.127536 sos_ansible-1.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21187 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/DockerfileDebug
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/rules/controller.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/rules/hub-rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/rules/rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/rules/tower.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:18:37.135536 sos_ansible-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/sos_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/sos_ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/file_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/sos_ansible/modules/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/helpers/rule_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/helpers/rule_writer_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/helpers/write_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/locating_sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/sos_ansible/modules/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/sos_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-25 13:18:37.000000 sos_ansible-1.0.4/sos_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-25 13:18:37.000000 sos_ansible-1.0.4/sos_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:18:37.000000 sos_ansible-1.0.4/sos_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 13:18:37.000000 sos_ansible-1.0.4/sos_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 13:18:37.000000 sos_ansible-1.0.4/sos_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 13:18:37.000000 sos_ansible-1.0.4/sos_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:37.131536 sos_ansible-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/tests/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/tests/test_locating_sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-25 13:18:19.000000 sos_ansible-1.0.4/tests/test_parser.py
```

### Comparing `sos_ansible-1.0.3/.github/workflows/pylint.yml` & `sos_ansible-1.0.4/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/.github/workflows/python-publish.yml` & `sos_ansible-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/.gitignore` & `sos_ansible-1.0.4/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
+.benchmarks
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `sos_ansible-1.0.3/.pylintrc` & `sos_ansible-1.0.4/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -274,27 +274,27 @@
 exclude-too-few-public-methods=
 
 # List of qualified class names to ignore when counting class parents (see
 # R0901)
 ignored-parents=
 
 # Maximum number of arguments for function / method.
-max-args=5
+max-args=10
 
 # Maximum number of attributes for a class (see R0902).
 max-attributes=7
 
 # Maximum number of boolean expressions in an if statement (see R0916).
 max-bool-expr=5
 
 # Maximum number of branch for function / method body.
 max-branches=12
 
 # Maximum number of locals for function / method body.
-max-locals=15
+max-locals=20
 
 # Maximum number of parents for a class (see R0901).
 max-parents=7
 
 # Maximum number of public methods for a class (see R0904).
 max-public-methods=20
```

### Comparing `sos_ansible-1.0.3/LICENSE` & `sos_ansible-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/Makefile` & `sos_ansible-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/PKG-INFO` & `sos_ansible-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,8 @@
-Metadata-Version: 2.1
-Name: sos_ansible
-Version: 1.0.3
-Summary: A sosreport parser for ansible
-Author-email: Lucas Benedito <lbenedit@redhat.com>
-License: GPL-3.0 license
-Project-URL: Homepage, https://github.com/lucas-benedito/sos-ansible
-Project-URL: Bug Tracker, https://github.com/lucas-benedito/sos-ansible/issues
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-[![GPL-3.0 license](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg)](https://github.com/lucas-benedito/sos-ansible/blob/devel/LICENSE)[![PyPI version](https://img.shields.io/pypi/v/sos_ansible.svg)](https://pypi.org/project/sos-ansible/)[![PR - Pylint Status](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml)[![Python Builds](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml)
+[![GPL-3.0 license](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg)](https://github.com/lucas-benedito/sos-ansible/blob/devel/LICENSE)[![PyPI version](https://img.shields.io/pypi/v/sos_ansible.svg)](https://pypi.org/project/sos-ansible/)[![PR - Pylint Status](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml)[![Python Builds](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml)[![PR - Pytest](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pytest.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pytest.yml)
 
 # sos-ansible
 
 This tool has the purpose of achieving easy sosreport reviewing based on custom rules.
 
 ---
```

### Comparing `sos_ansible-1.0.3/README.md` & `sos_ansible-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-[![GPL-3.0 license](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg)](https://github.com/lucas-benedito/sos-ansible/blob/devel/LICENSE)[![PyPI version](https://img.shields.io/pypi/v/sos_ansible.svg)](https://pypi.org/project/sos-ansible/)[![PR - Pylint Status](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml)[![Python Builds](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml)
+Metadata-Version: 2.1
+Name: sos_ansible
+Version: 1.0.4
+Summary: A sosreport parser for ansible
+Author-email: Lucas Benedito <lbenedit@redhat.com>
+License: GPL-3.0 license
+Project-URL: Homepage, https://github.com/lucas-benedito/sos-ansible
+Project-URL: Bug Tracker, https://github.com/lucas-benedito/sos-ansible/issues
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+[![GPL-3.0 license](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg)](https://github.com/lucas-benedito/sos-ansible/blob/devel/LICENSE)[![PyPI version](https://img.shields.io/pypi/v/sos_ansible.svg)](https://pypi.org/project/sos-ansible/)[![PR - Pylint Status](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml)[![Python Builds](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml)[![PR - Pytest](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pytest.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pytest.yml)
 
 # sos-ansible
 
 This tool has the purpose of achieving easy sosreport reviewing based on custom rules.
 
 ---
```

### Comparing `sos_ansible-1.0.3/pyproject.toml` & `sos_ansible-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sos_ansible"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name = "Lucas Benedito", email = "lbenedit@redhat.com"},
 ]
 description = "A sosreport parser for ansible"
 requires-python = ">=3.9"
 license = {text = "GPL-3.0 license"}
 dependencies = [
```

### Comparing `sos_ansible-1.0.3/rules/controller.json` & `sos_ansible-1.0.4/rules/controller.json`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/rules/hub-rules.json` & `sos_ansible-1.0.4/rules/hub-rules.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'Antivirus'": "{'query': 'falcon, crowd, mcafee'}",*

 * * "'Nginx'": "{'files': {insert: [(2, 'automationhub.access.log'), (3, "*

 * *            "'automationhub.error.log')]}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "Antivirus": {
         "files": [
             "installed-rpms"
         ],
         "path": "",
-        "query": "falcon, crowd"
+        "query": "falcon, crowd, mcafee"
     },
     "Filesystem": {
         "files": [
             "df"
         ],
         "path": "",
         "query": "100%"
@@ -33,15 +33,17 @@
         ],
         "path": "var/log",
         "query": "error, Traceback, cryptography"
     },
     "Nginx": {
         "files": [
             "error.log",
-            "access.log"
+            "access.log",
+            "automationhub.access.log",
+            "automationhub.error.log"
         ],
         "path": "var/log/nginx",
         "query": "error, 504, denied"
     },
     "OOM": {
         "files": [
             "dmesg"
```

### Comparing `sos_ansible-1.0.3/rules/rules.json` & `sos_ansible-1.0.4/rules/rules.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950980392156862%*

 * *Differences: {"'Antivirus'": "{'query': 'falcon, crowd, mcafee'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "Antivirus": {
         "files": [
             "installed-rpms"
         ],
         "path": "",
-        "query": "falcon, crowd"
+        "query": "falcon, crowd, mcafee"
     },
     "Controller Info": {
         "files": [
             "awx-manage_--version",
             "awx-manage_check_license_--data",
             "awx-manage_run_wsbroadcast_--status",
             "supervisorctl_status"
```

### Comparing `sos_ansible-1.0.3/rules/tower.json` & `sos_ansible-1.0.4/rules/tower.json`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/sos_ansible/__main__.py` & `sos_ansible-1.0.4/sos_ansible/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,21 @@
 config.setup()
 
 # Setting up Logger
 logger = getLogger("root")
 
 
 # Processing user input for directory choice
-def get_user_input(sos_directory):
-    """Select work directory"""
+def get_user_input(sos_directory: os.path) -> str:
+    """
+    Select work directory
+
+    :params os.path sos_directory: Directory containing the sosreports
+    :return str
+    """
     choice = os.listdir(sos_directory)
     try:
         questions = [
             inquirer.List("case", message="Choose the sos directory", choices=choice),
         ]
     except TypeError:
         logger.critical("Cancelled by user.")
@@ -37,28 +42,31 @@
     return inquirer.prompt(questions)["case"]
 
 
 def main():
     """
     Main function from sos_ansible. This will process all steps for sosreports reading
     """
+    tgt_dir = os.path.join(
+        os.path.expanduser(config.config_handler.get("files", "target"))
+    )
 
     params = Parser.get_args()
     if params.directory:
         sos_directory = os.path.abspath(params.directory)
     else:
         sos_directory = os.path.abspath(
             os.path.expanduser(config.config_handler.get("files", "source"))
         )
     if params.rules:
         rules_file = os.path.expanduser(params.rules)
     else:
         rules_file = os.path.expanduser(config.config_handler.get("files", "rules"))
     if params.tarball:
-        expand_sosreport(params.tarball, params.case)
+        expand_sosreport(params.tarball, params.case, sos_directory)
     # In order to allow both container and standard command line usage must check for env
     try:
         if os.environ["IS_CONTAINER"]:
             if not params.case:
                 logger.error("A case number must be used if running from a container")
                 sys.exit("A case number must be used if running from a container")
     except KeyError:
@@ -82,17 +90,17 @@
         logger.critical(
             "No sosreports found, please review the directory %s", sos_directory
         )
         sys.exit(0)
     logger.debug("Node data: %s", node_data)
     logger.debug("Current policy: %s", curr_policy)
 
-    validate_out_dir(user_choice)
+    validate_out_dir(user_choice, tgt_dir)
 
-    rules_processing(node_data, curr_policy, user_choice, params.debug)
+    rules_processing(node_data, curr_policy, user_choice, params.debug, tgt_dir)
 
     logger.critical(
         "Read the matches at %s/%s",
         config.config_handler.get("files", "target"),
         user_choice,
     )
     logger.critical("SOS_ANSIBLE - END")
```

### Comparing `sos_ansible-1.0.3/sos_ansible/modules/config_manager.py` & `sos_ansible-1.0.4/sos_ansible/modules/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 # from shutil import rmtree
 
 
 class ConfigParser:
     """config_parser class for initialization and validation"""
 
     def __init__(self, home_dir=os.path.expanduser("~"), tgt_file=".sos_ansible.ini"):
-        """Initializing required values"""
+        """
+        Initializing required values
+
+        :param os.path home_dir: Directory where to save config file
+        :param str tgt_file: config file name
+        """
         self.home_dir = home_dir
         self.tgt_file = tgt_file
         self.config_file = os.path.join(self.home_dir, self.tgt_file)
         self.config_handler = configparser.ConfigParser()
 
     def setup(self):
         """Setting up config files"""
         if os.path.isfile(self.config_file):
             with open(self.config_file, "r", encoding="utf-8") as file:
                 self.config_handler.read_file(file)
         else:
-            try:
-                self.set_files_config()
-            except Exception as err:  # pylint: disable=broad-except
-                print(err)
+            self.set_files_config()
         self.set_logger_config()
 
     def set_files_config(self):
         """Load config for local files"""
         if "files" not in self.config_handler:
             self.config_handler.add_section("files")
             self.config_handler.set("files", "source", "/tmp/sosreports")
```

### Comparing `sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer.py` & `sos_ansible-1.0.4/sos_ansible/modules/helpers/rule_writer.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/sos_ansible/modules/helpers/rule_writer_input.py` & `sos_ansible-1.0.4/sos_ansible/modules/helpers/rule_writer_input.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/sos_ansible/modules/helpers/write_json.py` & `sos_ansible-1.0.4/sos_ansible/modules/helpers/write_json.py`

 * *Files identical despite different names*

### Comparing `sos_ansible-1.0.3/sos_ansible/modules/locating_sos.py` & `sos_ansible-1.0.4/sos_ansible/modules/locating_sos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Class based on the lookup plugin created by Chris Meyers.
 https://github.com/chrismeyersfsu/sosreport-elk
 """
 
 import glob
 import os
+from typing import Union
 import re
 from logging import getLogger
 
 from sos_ansible.modules.config_manager import ConfigParser
 
 config = ConfigParser()
 config.setup()
@@ -17,16 +18,22 @@
 
 
 class LocateReports:
     """
     Validate the sosreport directory existance and provide the hostname and path for reference
     """
 
-    def get_tower_hostname(self, pathname):
-        """Return the hostname"""
+    def get_tower_hostname(self, pathname: os.path) -> Union[str, str]:
+        """
+        Return the hostname
+
+        :param os.path pathname: Directory containing sosreports
+        :return hostname, controller
+        :rtype: Union[str, str] | str
+        """
         path = os.path.join(pathname, "etc", "tower", "conf.d", "cluster_host_id.py")
         try:
             with open(path, encoding="utf-8") as file:
                 data = file.read()
             cl_id = re.search("CLUSTER_HOST_ID = '(.*?)'", data)
             if cl_id.group(1):
                 hostname = cl_id.group(1)
@@ -42,16 +49,21 @@
                 hostname = file.read().rstrip("\n")
                 controller = False
             return hostname, controller
         except FileNotFoundError:
             pass
         return "NOTFOUND"
 
-    def run(self, terms, user_choice):
-        """Return the hostname, path keypair"""
+    def run(self, terms: list, user_choice: str):
+        """
+        :param list terms: list of directories to search
+        :param str user_choice: case number
+
+        Return the hostname, path keypair
+        """
         entry = {
             "hostname": "",
             "path": "",
         }
 
         # lookups in general are expected to both take a list as input and output a list
         # this is done so they work with the looping construct 'with_'.
@@ -59,22 +71,18 @@
         if not isinstance(terms, list):
             dirs_handler = []
             dirs_handler.append(terms)
         for sos_directory in dirs_handler:
             sos_dir = os.path.abspath(sos_directory)
             search_dir = os.path.join(sos_dir, user_choice, "sosreport-*")
             logger.error(sos_dir)
-            try:
-                for directory in glob.glob(search_dir, recursive=False):
-                    if not os.path.isdir(directory):
-                        continue
+            for directory in glob.glob(search_dir, recursive=False):
+                if os.path.isdir(directory):
                     hostname, controller = self.get_tower_hostname(directory)
                     entry = {
                         "hostname": hostname,
                         "path": directory.replace(directory + "/", ""),
                         "controller": controller,
                     }
                     ret.append(entry)
-            except Exception:  # pylint: disable=broad-except
-                pass
 
         return ret
```

### Comparing `sos_ansible-1.0.3/sos_ansible/modules/parsing.py` & `sos_ansible-1.0.4/sos_ansible/modules/parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Custom parser to evaluate conditions"""
 import argparse
 
 
-class CheckDependsAction(argparse.Action): # pylint: disable=too-few-public-methods
+class CheckDependsAction(argparse.Action):  # pylint: disable=too-few-public-methods
     """custom action to evaluate dependency on case number"""
 
     def __call__(self, parser, namespace, values, option_string=None):
         if namespace.case:
             namespace.tarball = [value.strip() for value in values.split(",")]
         else:
             parser.error("Missing case number")
```

### Comparing `sos_ansible-1.0.3/sos_ansible.egg-info/PKG-INFO` & `sos_ansible-1.0.4/sos_ansible.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sos-ansible
-Version: 1.0.3
+Version: 1.0.4
 Summary: A sosreport parser for ansible
 Author-email: Lucas Benedito <lbenedit@redhat.com>
 License: GPL-3.0 license
 Project-URL: Homepage, https://github.com/lucas-benedito/sos-ansible
 Project-URL: Bug Tracker, https://github.com/lucas-benedito/sos-ansible/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-[![GPL-3.0 license](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg)](https://github.com/lucas-benedito/sos-ansible/blob/devel/LICENSE)[![PyPI version](https://img.shields.io/pypi/v/sos_ansible.svg)](https://pypi.org/project/sos-ansible/)[![PR - Pylint Status](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml)[![Python Builds](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml)
+[![GPL-3.0 license](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg)](https://github.com/lucas-benedito/sos-ansible/blob/devel/LICENSE)[![PyPI version](https://img.shields.io/pypi/v/sos_ansible.svg)](https://pypi.org/project/sos-ansible/)[![PR - Pylint Status](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pylint.yml)[![Python Builds](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/python-publish.yml)[![PR - Pytest](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pytest.yml/badge.svg)](https://github.com/lucas-benedito/sos-ansible/actions/workflows/pytest.yml)
 
 # sos-ansible
 
 This tool has the purpose of achieving easy sosreport reviewing based on custom rules.
 
 ---
```

