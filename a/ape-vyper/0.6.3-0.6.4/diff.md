# Comparing `tmp/ape-vyper-0.6.3.tar.gz` & `tmp/ape-vyper-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.3.tar", last modified: Thu Apr 13 22:01:54 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.4.tar", last modified: Tue Apr 25 12:31:34 2023, max compression
```

## Comparing `ape-vyper-0.6.3.tar` & `ape-vyper-0.6.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:01:53.000000 ape-vyper-0.6.3/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/contract_with_dev_messages.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19829 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 12:31:33.000000 ape-vyper-0.6.4/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.009209 ape-vyper-0.6.4/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.009209 ape-vyper-0.6.4/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/erc20.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:31:34.013209 ape-vyper-0.6.4/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/contracts/passing_contracts/use_iface2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-04-25 12:30:36.000000 ape-vyper-0.6.4/tests/test_compiler.py
```

### Comparing `ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.4/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/release-drafter.yml` & `ape-vyper-0.6.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/workflows/commitlint.yaml` & `ape-vyper-0.6.4/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.4/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/workflows/publish.yaml` & `ape-vyper-0.6.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.github/workflows/test.yaml` & `ape-vyper-0.6.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.gitignore` & `ape-vyper-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/.pre-commit-config.yaml` & `ape-vyper-0.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/CONTRIBUTING.md` & `ape-vyper-0.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/LICENSE` & `ape-vyper-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/PKG-INFO` & `ape-vyper-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.3
+Version: 0.6.4
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-vyper-0.6.3/README.md` & `ape-vyper-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/ape_vyper/compiler.py` & `ape-vyper-0.6.4/ape_vyper/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
                                                 break
 
                                     elif stmt.ast_type == "Subscript":
                                         dev = RuntimeErrorType.INDEX_OUT_OF_RANGE
 
                                     if dev:
                                         val = f"dev: {dev.value}"
-                                        if is_revert_jump:
+                                        if is_revert_jump and len(pc_map_list) >= 1:
                                             pc_map_list[-1][1]["dev"] = val
                                         else:
                                             item["dev"] = val
 
                                 pc_map_list.append((pc, item))
 
                     # Find content-specified dev messages.
```

### Comparing `ape-vyper-0.6.3/ape_vyper/exceptions.py` & `ape-vyper-0.6.4/ape_vyper/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Dict, Optional, Type
+from typing import Dict, Optional, Type, Union
 
 from ape.exceptions import CompilerError, ContractLogicError
 from vvm.exceptions import VyperError  # type: ignore
 
 
 class VyperCompilerPluginError(CompilerError):
     """
@@ -18,19 +18,24 @@
 
 
 class VyperCompileError(VyperCompilerPluginError):
     """
     A compiler-specific error in Vyper.
     """
 
-    def __init__(self, err: VyperError):
-        self.base_err = err  # For debugging purposes.
-        message = "\n\n".join(
-            f"{e['sourceLocation']['file']}\n{e['type']}:{e['message']}" for e in err.error_dict
-        )
+    def __init__(self, err: Union[VyperError, str]):
+        if isinstance(err, VyperError):
+            self.base_err = err
+            message = "\n\n".join(
+                f"{e['sourceLocation']['file']}\n{e['type']}:{e['message']}" for e in err.error_dict
+            )
+        else:
+            self.base_err = None
+            message = str(err)
+
         super().__init__(message)
 
 
 class RuntimeErrorType(Enum):
     NONPAYABLE_CHECK = "Cannot send ether to non-payable function"
     INDEX_OUT_OF_RANGE = "Index out of range"
     INTEGER_OVERFLOW = "Integer overflow"
```

### Comparing `ape-vyper-0.6.3/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.4/ape_vyper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.3
+Version: 0.6.4
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-vyper-0.6.3/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.4/ape_vyper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,13 +33,14 @@
 tests/test_compiler.py
 tests/ExampleDependency/contracts/Dependency.vy
 tests/contracts/failing_contracts/contract_undeclared_variable.vy
 tests/contracts/failing_contracts/contract_unknown_pragma.vy
 tests/contracts/passing_contracts/contract.vy
 tests/contracts/passing_contracts/contract_no_pragma.vy
 tests/contracts/passing_contracts/contract_with_dev_messages.vy
+tests/contracts/passing_contracts/erc20.vy
 tests/contracts/passing_contracts/older_version.vy
 tests/contracts/passing_contracts/use_iface.vy
 tests/contracts/passing_contracts/use_iface2.vy
 tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
 tests/contracts/passing_contracts/interfaces/IFace.vy
 tests/contracts/passing_contracts/interfaces/IFace2.vy
```

### Comparing `ape-vyper-0.6.3/ape_vyper.egg-info/requires.txt` & `ape-vyper-0.6.4/ape_vyper.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/pyproject.toml` & `ape-vyper-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/setup.py` & `ape-vyper-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/tests/conftest.py` & `ape-vyper-0.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/tests/contracts/passing_contracts/contract.vy` & `ape-vyper-0.6.4/tests/contracts/passing_contracts/contract.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.3/tests/test_compiler.py` & `ape-vyper-0.6.4/tests/test_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,22 +93,23 @@
             continue
 
         sources = ", ".join([p.name for p in actual[version]])
         fail_message = f"Unexpected version '{version}' with sources: {sources}"
         pytest.fail(fail_message)
 
     assert len(actual[OLDER_VERSION_FROM_PRAGMA]) == 1
-    assert len(actual[VERSION_FROM_PRAGMA]) == 5
+    assert len(actual[VERSION_FROM_PRAGMA]) == 6
     assert actual[OLDER_VERSION_FROM_PRAGMA] == {project.contracts_folder / "older_version.vy"}
     assert actual[VERSION_FROM_PRAGMA] == {
         project.contracts_folder / "contract.vy",
         project.contracts_folder / "contract_no_pragma.vy",
         project.contracts_folder / "contract_with_dev_messages.vy",
         project.contracts_folder / "use_iface.vy",
         project.contracts_folder / "use_iface2.vy",
+        project.contracts_folder / "erc20.vy",
     }
 
 
 def test_compiler_data_in_manifest(project):
     _ = project.contracts
     manifest = project.extract_manifest()
     assert len(manifest.compilers) == 2, manifest.compilers
@@ -117,15 +118,15 @@
     vyper_028 = [c for c in manifest.compilers if str(c.version) == str(OLDER_VERSION_FROM_PRAGMA)][
         0
     ]
 
     for compiler in (vyper_028, vyper_034):
         assert compiler.name == "vyper"
 
-    assert len(vyper_034.contractTypes) == 5
+    assert len(vyper_034.contractTypes) == 6
     assert len(vyper_028.contractTypes) == 1
     assert "contract" in vyper_034.contractTypes
     assert "older_version" in vyper_028.contractTypes
     for compiler in (vyper_034, vyper_028):
         assert compiler.settings["evmVersion"] == "constantinople"
         assert compiler.settings["optimize"] is True
```

