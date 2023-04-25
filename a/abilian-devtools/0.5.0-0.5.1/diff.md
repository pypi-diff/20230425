# Comparing `tmp/abilian_devtools-0.5.0.tar.gz` & `tmp/abilian_devtools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abilian_devtools-0.5.0.tar", max compression
+gzip compressed data, was "abilian_devtools-0.5.1.tar", max compression
```

## Comparing `abilian_devtools-0.5.0.tar` & `abilian_devtools-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0        0        0        0 2023-01-05 08:13:44.808895 abilian_devtools-0.5.0/LICENSES/
--rw-r--r--   0        0        0     3410 2023-03-30 06:46:33.989878 abilian_devtools-0.5.0/README.md
--rw-r--r--   0        0        0     3512 2023-04-25 11:27:16.910745 abilian_devtools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      109 2023-01-05 08:19:38.548365 abilian_devtools-0.5.0/src/abilian_devtools/__init__.py
--rw-r--r--   0        0        0      789 2023-04-25 11:18:44.030393 abilian_devtools-0.5.0/src/abilian_devtools/cli.py
--rw-r--r--   0        0        0        0 2023-04-17 19:33:43.016062 abilian_devtools-0.5.0/src/abilian_devtools/commands/__init__.py
--rw-r--r--   0        0        0      321 2023-04-18 10:19:01.175151 abilian_devtools-0.5.0/src/abilian_devtools/commands/_util.py
--rw-r--r--   0        0        0      445 2023-04-18 10:21:00.387107 abilian_devtools-0.5.0/src/abilian_devtools/commands/all.py
--rw-r--r--   0        0        0      544 2023-04-18 10:21:00.406348 abilian_devtools-0.5.0/src/abilian_devtools/commands/audit.py
--rw-r--r--   0        0        0     1839 2023-04-25 11:24:43.696109 abilian_devtools-0.5.0/src/abilian_devtools/commands/bump.py
--rw-r--r--   0        0        0      956 2023-04-25 11:21:33.062708 abilian_devtools-0.5.0/src/abilian_devtools/commands/check.py
--rw-r--r--   0        0        0      794 2023-04-18 10:17:57.973688 abilian_devtools-0.5.0/src/abilian_devtools/commands/clean.py
--rw-r--r--   0        0        0      764 2023-04-25 11:21:33.063995 abilian_devtools-0.5.0/src/abilian_devtools/commands/format.py
--rw-r--r--   0        0        0     1424 2023-04-18 10:30:55.666246 abilian_devtools-0.5.0/src/abilian_devtools/commands/help.py
--rw-r--r--   0        0        0      687 2023-04-25 11:21:33.065600 abilian_devtools-0.5.0/src/abilian_devtools/commands/test.py
--rw-r--r--   0        0        0      718 2023-04-25 11:23:18.045129 abilian_devtools-0.5.0/src/abilian_devtools/invoke/__init__.py
--rw-r--r--   0        0        0      307 2023-04-18 10:31:18.457907 abilian_devtools-0.5.0/src/abilian_devtools/invoke/help.py
--rw-r--r--   0        0        0      470 2023-04-18 10:30:32.605718 abilian_devtools-0.5.0/src/abilian_devtools/invoke/subrepos.py
--rw-r--r--   0        0        0      795 2023-04-18 10:31:22.407446 abilian_devtools-0.5.0/src/abilian_devtools/invoke/versions.py
--rw-r--r--   0        0        0      479 2023-04-17 19:32:18.135821 abilian_devtools-0.5.0/src/abilian_devtools/shell.py
--rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 abilian_devtools-0.5.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-01-05 08:13:44.808895 abilian_devtools-0.5.1/LICENSES/
+-rw-r--r--   0        0        0     3410 2023-03-30 06:46:33.989878 abilian_devtools-0.5.1/README.md
+-rw-r--r--   0        0        0     3523 2023-04-25 11:54:35.057513 abilian_devtools-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-01-05 08:19:38.548365 abilian_devtools-0.5.1/src/abilian_devtools/__init__.py
+-rw-r--r--   0        0        0      824 2023-04-25 11:48:17.306722 abilian_devtools-0.5.1/src/abilian_devtools/cli.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:33:43.016062 abilian_devtools-0.5.1/src/abilian_devtools/commands/__init__.py
+-rw-r--r--   0        0        0      321 2023-04-18 10:19:01.175151 abilian_devtools-0.5.1/src/abilian_devtools/commands/_util.py
+-rw-r--r--   0        0        0      445 2023-04-18 10:21:00.387107 abilian_devtools-0.5.1/src/abilian_devtools/commands/all.py
+-rw-r--r--   0        0        0      544 2023-04-18 10:21:00.406348 abilian_devtools-0.5.1/src/abilian_devtools/commands/audit.py
+-rw-r--r--   0        0        0     1839 2023-04-25 11:24:43.696109 abilian_devtools-0.5.1/src/abilian_devtools/commands/bump.py
+-rw-r--r--   0        0        0      956 2023-04-25 11:21:33.062708 abilian_devtools-0.5.1/src/abilian_devtools/commands/check.py
+-rw-r--r--   0        0        0      794 2023-04-18 10:17:57.973688 abilian_devtools-0.5.1/src/abilian_devtools/commands/clean.py
+-rw-r--r--   0        0        0      764 2023-04-25 11:21:33.063995 abilian_devtools-0.5.1/src/abilian_devtools/commands/format.py
+-rw-r--r--   0        0        0     1424 2023-04-18 10:30:55.666246 abilian_devtools-0.5.1/src/abilian_devtools/commands/help.py
+-rw-r--r--   0        0        0      687 2023-04-25 11:21:33.065600 abilian_devtools-0.5.1/src/abilian_devtools/commands/test.py
+-rw-r--r--   0        0        0      718 2023-04-25 11:23:18.045129 abilian_devtools-0.5.1/src/abilian_devtools/invoke/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-18 10:31:18.457907 abilian_devtools-0.5.1/src/abilian_devtools/invoke/help.py
+-rw-r--r--   0        0        0      470 2023-04-18 10:30:32.605718 abilian_devtools-0.5.1/src/abilian_devtools/invoke/subrepos.py
+-rw-r--r--   0        0        0      795 2023-04-18 10:31:22.407446 abilian_devtools-0.5.1/src/abilian_devtools/invoke/versions.py
+-rw-r--r--   0        0        0      479 2023-04-17 19:32:18.135821 abilian_devtools-0.5.1/src/abilian_devtools/shell.py
+-rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 abilian_devtools-0.5.1/PKG-INFO
```

### Comparing `abilian_devtools-0.5.0/README.md` & `abilian_devtools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/pyproject.toml` & `abilian_devtools-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abilian-devtools"
-version = "0.5.0"
+version = "0.5.1"
 description = "A curated set of dependencies for quality software development"
 authors = ["Stefane Fermigier <sf@abilian.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "abilian_devtools", from = "src" }]
 repository = "https://github.com/abilian/abilian-devtools"
 keywords = [
@@ -18,85 +18,94 @@
 
 [tool.poetry.scripts]
 adt = "abilian_devtools.cli:main"
 
 [tool.poetry.dependencies]
 # python = ">=3.8.1,<4.0"
 python = "^3.9"
+cleez = "^0.1.8"
+
 # Git integration
 pre-commit = "*"
+
 # Testing
 pytest = "^7"
 pytest-cov = "^4"
 profilehooks = "*"
 pytest-xdist = "*"
 pytest-random-order = "*"
 # pytest-testmon = "^1.2.0"
 nox = "*"
+
 # Linting
+ruff = "*"
 flake8 = "^6"
-# Plugins: see https://github.com/DmytroLitvinov/awesome-flake8-extensions
+# + Plugins: see https://github.com/DmytroLitvinov/awesome-flake8-extensions
 flake8-bandit = "*"
 flake8-breakpoint = "*"
 flake8-cognitive-complexity = "*"
 flake8-datetimez = "*"
 flake8-functions = "*"
 flake8-if-expr = "*"
 flake8-isort = "*"
 flake8-logging-format = "*"
 flake8-mutable = "*"
 flake8-super = "*"
 flake8-super-call = "*"
 flake8-tidy-imports = "*"
 flake8-tuple = "*"
+
 # Removing these as they are made redundant by Ruf
 # (See: https://notes.crmarsh.com/ruff-the-first-200-releases)
 # flake8-bugbear = "*"
 # flake8-comprehensions = "*"
 # flake8-simplify = "*"
 # pep8-naming = "*"
+
 # Typing
 flake8-pep3101 = "*"
 flake8-no-pep420 = "*"
 flake8-pep585 = "*"
 flake8-pep604 = "*"
+
 # Testing
 flake8-assertive = "*"
 flake8-pytest = "*"
 flake8-pytest-style = "*"
 # Useful but later:
 # flake8-requirements = "*"
 # flake8-return = "*"
 # flake8-expression-complexity = "*"
 # flake8-print = "*"
 # flake8-use-pathlib = "*"
 # tryceratops = "^0.6"
 # flake8-pie = "*"
 # dlint = "*" <- not compatible w/ flake8 6+
 # hacking = "*" <- not compatible w/ flake8 6+
-ruff = "*"
+
 # Formatting
 isort = "*"
 black = "*"
 docformatter = "*"
 # Later:
 # Typechecking
 mypy = "*"
 pyright = "*"
+
 # Dependencies & supply chain
 deptry = "*"
 pip = "*"
 pip-audit = "*"
 reuse = "*"
 safety = "*"
 vulture = "*"
+
 # Invoke
 invoke = "^2.0.0"
 tomlkit = "^0.11.6"
-cleez = "^0.1.7"
 
 [tool.poetry.group.dev.dependencies]
 scriv = "^1.2.0"
 types-invoke = "^2.0.0.1"
 snoop = "^0.4.3"
 
 [build-system]
```

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/cli.py` & `abilian_devtools-0.5.1/src/abilian_devtools/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import importlib.metadata
 
 from cleez import CLI
+from cleez.actions import VERSION
 
 
 def main():
     cli = get_cli()
     cli.run()
 
 
 def get_cli():
     version = importlib.metadata.version("abilian-devtools")
     cli = CLI(name="adt", version=version)
     cli.add_option(
         "-V",
         "--version",
-        default=False,
-        action="store_true",
+        action=VERSION,
+        version=cli.version,
         help="Show version and exit",
     )
     cli.add_option(
         "-d", "--debug", default=False, action="store_true", help="Enable debug mode"
     )
     cli.add_option(
         "-v", "--verbose", default=False, action="store_true", help="Increase verbosity"
```

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/audit.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/audit.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/bump.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/bump.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/check.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/check.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/clean.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/clean.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/format.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/format.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/help.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/help.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/commands/test.py` & `abilian_devtools-0.5.1/src/abilian_devtools/commands/test.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/invoke/__init__.py` & `abilian_devtools-0.5.1/src/abilian_devtools/invoke/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/src/abilian_devtools/invoke/versions.py` & `abilian_devtools-0.5.1/src/abilian_devtools/invoke/versions.py`

 * *Files identical despite different names*

### Comparing `abilian_devtools-0.5.0/PKG-INFO` & `abilian_devtools-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: abilian-devtools
-Version: 0.5.0
+Version: 0.5.1
 Summary: A curated set of dependencies for quality software development
 Home-page: https://github.com/abilian/abilian-devtools
 License: MIT
 Keywords: qa,testing,linting,typechecking,security,supply chain
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black
-Requires-Dist: cleez (>=0.1.7,<0.2.0)
+Requires-Dist: cleez (>=0.1.8,<0.2.0)
 Requires-Dist: deptry
 Requires-Dist: docformatter
 Requires-Dist: flake8 (>=6,<7)
 Requires-Dist: flake8-assertive
 Requires-Dist: flake8-bandit
 Requires-Dist: flake8-breakpoint
 Requires-Dist: flake8-cognitive-complexity
```

