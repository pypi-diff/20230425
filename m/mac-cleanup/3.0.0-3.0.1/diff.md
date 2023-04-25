# Comparing `tmp/mac_cleanup-3.0.0.tar.gz` & `tmp/mac_cleanup-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mac_cleanup-3.0.0.tar", max compression
+gzip compressed data, was "mac_cleanup-3.0.1.tar", max compression
```

## Comparing `mac_cleanup-3.0.0.tar` & `mac_cleanup-3.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2022-08-09 13:15:49.497915 mac_cleanup-3.0.0/LICENSE
--rw-r--r--   0        0        0     3795 2023-04-13 13:54:59.884936 mac_cleanup-3.0.0/README.md
--rw-r--r--   0        0        0      425 2023-04-10 17:33:48.121290 mac_cleanup-3.0.0/mac_cleanup/__init__.py
--rw-r--r--   0        0        0      181 2023-03-26 22:15:29.161722 mac_cleanup-3.0.0/mac_cleanup/__version__.py
--rw-r--r--   0        0        0     8333 2023-04-13 22:09:29.474991 mac_cleanup-3.0.0/mac_cleanup/config.py
--rw-r--r--   0        0        0      653 2023-04-10 18:13:35.057667 mac_cleanup-3.0.0/mac_cleanup/console.py
--rw-r--r--   0        0        0     7730 2023-04-13 22:09:29.475076 mac_cleanup-3.0.0/mac_cleanup/core.py
--rw-r--r--   0        0        0     4257 2023-04-13 13:45:07.200604 mac_cleanup-3.0.0/mac_cleanup/core_modules.py
--rw-r--r--   0        0        0    14351 2023-04-10 17:33:48.122468 mac_cleanup-3.0.0/mac_cleanup/default_modules.py
--rw-r--r--   0        0        0     3791 2023-04-10 17:33:48.298687 mac_cleanup-3.0.0/mac_cleanup/error_handling.py
--rw-r--r--   0        0        0     2918 2023-04-11 04:55:56.810107 mac_cleanup-3.0.0/mac_cleanup/main.py
--rw-r--r--   0        0        0     1181 2023-04-10 17:33:48.299151 mac_cleanup-3.0.0/mac_cleanup/parser.py
--rw-r--r--   0        0        0     3380 2023-04-13 13:40:37.272889 mac_cleanup-3.0.0/mac_cleanup/progress.py
--rwxr-xr-x   0        0        0     3181 2023-04-10 17:33:48.299577 mac_cleanup-3.0.0/mac_cleanup/utils.py
--rw-r--r--   0        0        0     3217 2023-04-13 22:01:45.095001 mac_cleanup-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 mac_cleanup-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-09 13:15:49.497915 mac_cleanup-3.0.1/LICENSE
+-rw-r--r--   0        0        0     3795 2023-04-25 11:33:45.460404 mac_cleanup-3.0.1/README.md
+-rw-r--r--   0        0        0      425 2023-04-14 12:16:23.955827 mac_cleanup-3.0.1/mac_cleanup/__init__.py
+-rw-r--r--   0        0        0      181 2023-03-26 22:15:29.161722 mac_cleanup-3.0.1/mac_cleanup/__version__.py
+-rw-r--r--   0        0        0     8333 2023-04-14 12:16:23.956897 mac_cleanup-3.0.1/mac_cleanup/config.py
+-rw-r--r--   0        0        0      653 2023-04-14 12:16:23.957364 mac_cleanup-3.0.1/mac_cleanup/console.py
+-rw-r--r--   0        0        0     7743 2023-04-25 11:33:45.272323 mac_cleanup-3.0.1/mac_cleanup/core.py
+-rw-r--r--   0        0        0     4257 2023-04-14 12:16:23.958176 mac_cleanup-3.0.1/mac_cleanup/core_modules.py
+-rw-r--r--   0        0        0    14351 2023-04-14 12:16:23.958627 mac_cleanup-3.0.1/mac_cleanup/default_modules.py
+-rw-r--r--   0        0        0     3791 2023-04-14 12:16:23.958905 mac_cleanup-3.0.1/mac_cleanup/error_handling.py
+-rw-r--r--   0        0        0     2918 2023-04-14 12:16:23.959175 mac_cleanup-3.0.1/mac_cleanup/main.py
+-rw-r--r--   0        0        0     1181 2023-04-14 12:16:23.959495 mac_cleanup-3.0.1/mac_cleanup/parser.py
+-rw-r--r--   0        0        0     3380 2023-04-14 12:16:23.960159 mac_cleanup-3.0.1/mac_cleanup/progress.py
+-rwxr-xr-x   0        0        0     3181 2023-04-14 12:16:23.960392 mac_cleanup-3.0.1/mac_cleanup/utils.py
+-rw-r--r--   0        0        0     2959 2023-04-25 11:33:45.461381 mac_cleanup-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 mac_cleanup-3.0.1/PKG-INFO
```

### Comparing `mac_cleanup-3.0.0/LICENSE` & `mac_cleanup-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/README.md` & `mac_cleanup-3.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.0
+    3.0.1
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
```

### Comparing `mac_cleanup-3.0.0/mac_cleanup/config.py` & `mac_cleanup-3.0.1/mac_cleanup/config.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/console.py` & `mac_cleanup-3.0.1/mac_cleanup/console.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/core.py` & `mac_cleanup-3.0.1/mac_cleanup/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         """
 
         from concurrent.futures import ThreadPoolExecutor, as_completed
 
         from mac_cleanup.progress import ProgressBar
 
         # Extract all modules
-        all_modules = list(chain(*[unit.modules for unit in self._execute_list]))
+        all_modules = list(chain.from_iterable([unit.modules for unit in self._execute_list]))
 
         # Filter modules based on Path
         path_modules: list[Path] = list(filter(partial(self.__filter_modules, filter_type=Path), all_modules))
 
         # Extracts paths from path_modules list
         path_list: list[Path_] = [path.get_path for path in path_modules]
```

### Comparing `mac_cleanup-3.0.0/mac_cleanup/core_modules.py` & `mac_cleanup-3.0.1/mac_cleanup/core_modules.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/default_modules.py` & `mac_cleanup-3.0.1/mac_cleanup/default_modules.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/error_handling.py` & `mac_cleanup-3.0.1/mac_cleanup/error_handling.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/main.py` & `mac_cleanup-3.0.1/mac_cleanup/main.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/parser.py` & `mac_cleanup-3.0.1/mac_cleanup/parser.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/progress.py` & `mac_cleanup-3.0.1/mac_cleanup/progress.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/mac_cleanup/utils.py` & `mac_cleanup-3.0.1/mac_cleanup/utils.py`

 * *Files identical despite different names*

### Comparing `mac_cleanup-3.0.0/pyproject.toml` & `mac_cleanup-3.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mac_cleanup"
-version = "3.0.0"
+version = "3.0.1"
 description = "Python cleanup script for macOS"
 license = "Apache-2.0"
 authors = [ "Drugsosos" ]
 readme = "README.md"
 homepage = "https://github.com/mac-cleanup/mac-cleanup-py"
 repository = "https://github.com/mac-cleanup/mac-cleanup-py"
 keywords = [
@@ -27,46 +27,37 @@
 "Documentation" = "https://github.com/mac-cleanup/mac-cleanup-py#install-automatically"
 "Issue Tracker" = "https://github.com/mac-cleanup/mac-cleanup-py/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 rich = "^13.3.4"
-attrs = "^22.2.0"
+attrs = "^23.1.0"
 inquirer = "^3.1.3"
 toml = "^0.10.2"
 beartype = "^0.13.1"
 
 [tool.poetry.scripts]
 mac-cleanup = "mac_cleanup:main"
 
 [tool.poetry.group.test.dependencies]
-tox = "^4.4.11"
-pytest = "^7.3.0"
+tox = "^4.5.0"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-pyright = "^1.1.302"
-ruff = "^0.0.261"
-flake8-bugbear = "^23.3.23"
-flake8-comprehensions = "^3.12.0"
-flake8-print = "^5.0.0"
-flake8-quotes = "^3.3.2"
-flake8-builtins = "^2.1.0"
-flake8-pytest-style = "^1.7.2"
-flake8-blind-except = "^0.2.1"
-flake8-no-pep420 = "^2.3.0"
-flake8-simplify = "^0.20.0"
+pyright = "^1.1.304"
+ruff = "^0.0.263"
 
 [tool.poetry.group.dev.dependencies]
-commitizen = "^2.42.1"
+commitizen = "^3.0.1"
 pre-commit = "^3.2.2"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
-docformatter = "1.5.1"
+docformatter = "^1.6.3"
 
 [build-system]
 requires = [ "poetry-core>=1.0.0" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -131,16 +122,15 @@
     "Q",  # quotes
     "A",  # builtins
     "PT",  # pytest-style
     "INP",  # pep420
     "SIM",  # simplify
 ]
 
-
 [tool.ruff.flake8-quotes]
 inline-quotes = "double"
 multiline-quotes = "double"
 
 [tool.pytest.ini_options]
-minversion = "7.2.2"
+minversion = "7.3.1"
 addopts = "--cov=mac_cleanup"
 testpaths = [ "tests" ]
```

### Comparing `mac_cleanup-3.0.0/PKG-INFO` & `mac_cleanup-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mac-cleanup
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python cleanup script for macOS
 Home-page: https://github.com/mac-cleanup/mac-cleanup-py
 License: Apache-2.0
 Keywords: macos,script,cleanup,cleaner
 Author: Drugsosos
 Requires-Python: >=3.10,<3.12
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: beartype (>=0.13.1,<0.14.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://github.com/mac-cleanup/mac-cleanup-py#install-automatically
 Project-URL: Issue Tracker, https://github.com/mac-cleanup/mac-cleanup-py/issues
 Project-URL: Repository, https://github.com/mac-cleanup/mac-cleanup-py
@@ -129,15 +129,15 @@
 
 ```
 $ mac-cleanup -h
 
 usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    3.0.0
+    3.0.1
     https://github.com/mac-cleanup/mac-cleanup-py    
 
 options:
   -h, --help         show this help message and exit
   -n, --dry-run      Dry run without deleting stuff
   -u, --update       Update HomeBrew on cleanup
   -c, --configure    Configure default and custom modules
```

