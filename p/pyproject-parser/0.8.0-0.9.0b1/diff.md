# Comparing `tmp/pyproject-parser-0.8.0.tar.gz` & `tmp/pyproject-parser-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-parser-0.8.0.tar", last modified: Tue Apr 11 12:28:04 2023, max compression
+gzip compressed data, was "pyproject-parser-0.9.0b1.tar", last modified: Tue Apr 25 08:02:41 2023, max compression
```

## Comparing `pyproject-parser-0.8.0.tar` & `pyproject-parser-0.9.0b1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8391 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5472 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.391500 pyproject-parser-0.8.0/pyproject_parser/
--rw-r--r--   0 runner    (1001) docker     (122)    10900 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9377 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.391500 pyproject-parser-0.8.0/pyproject_parser/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     6437 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/cli/_json_encoders.py
--rw-r--r--   0 runner    (1001) docker     (122)    35674 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/type_hints.py
--rw-r--r--   0 runner    (1001) docker     (122)     5126 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/pyproject_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.391500 pyproject-parser-0.8.0/pyproject_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8391 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-11 12:28:04.000000 pyproject-parser-0.8.0/pyproject_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:28:04.395501 pyproject-parser-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_cli_module.py
--rw-r--r--   0 runner    (1001) docker     (122)    12980 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_dumping.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_pyproject_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-11 12:27:33.000000 pyproject-parser-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5474 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.650429 pyproject-parser-0.9.0b1/pyproject_parser/
+-rw-r--r--   0 runner    (1001) docker     (122)    10945 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9433 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.650429 pyproject-parser-0.9.0b1/pyproject_parser/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/cli/_json_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35674 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5500 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/pyproject_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.650429 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8395 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 08:02:41.000000 pyproject-parser-0.9.0b1/pyproject_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:02:41.654429 pyproject-parser-0.9.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    10428 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15102 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3793 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_cli_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12953 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5900 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_dumping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_pyproject_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-04-25 08:02:08.000000 pyproject-parser-0.9.0b1/tests/test_utils.py
```

### Comparing `pyproject-parser-0.8.0/LICENSE` & `pyproject-parser-0.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/PKG-INFO` & `pyproject-parser-0.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.8.0
+Version: 0.9.0b1
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -156,15 +156,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b1
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.8.0/README.rst` & `pyproject-parser-0.9.0b1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b1
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.8.0/pyproject.toml` & `pyproject-parser-0.9.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyproject-parser"
-version = "0.8.0"
+version = "0.9.0b1"
 description = "Parser for 'pyproject.toml'"
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "metadata", "packaging", "pep518", "pep621", "pyproject", "toml",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `pyproject-parser-0.8.0/pyproject_parser/__init__.py` & `pyproject-parser-0.9.0b1/pyproject_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,19 +50,20 @@
 from pyproject_parser.type_hints import (  # noqa: F401
 		Author,
 		BuildSystemDict,
 		ContentTypes,
 		ProjectDict,
 		_PyProjectAsTomlDict
 		)
+from pyproject_parser.utils import _load_toml
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.8.0"
+__version__: str = "0.9.0b1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PyProject", "PyProjectTomlEncoder", "_PP"]
 
 _PP = TypeVar("_PP", bound="PyProject")
 
 
@@ -169,15 +170,15 @@
 			the :meth:`parse() <dom_toml.parser.AbstractConfigParser.parse>` method on
 			:attr:`~.build_system_table_parser` and :attr:`~.project_table_parser`.
 		"""
 
 		filename = PathPlus(filename)
 
 		project_dir = filename.parent
-		config = dom_toml.load(filename)
+		config = _load_toml(filename)
 
 		keys = set(config.keys())
 
 		build_system_table: Optional[BuildSystemDict] = None
 		project_table: Optional[ProjectDict] = None
 		tool_table: Dict[str, Dict[str, Any]] = {}
```

### Comparing `pyproject-parser-0.8.0/pyproject_parser/__main__.py` & `pyproject-parser-0.9.0b1/pyproject_parser/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  __main__.py
 """
 CLI entry point.
 
 .. versionadded:: 0.2.0
 """
 #
-#  Copyright © 2021-2022 Dominic Davis-Foster <dominic@davis-foster.co.uk>
+#  Copyright © 2021-2023 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -49,14 +49,15 @@
 from pyproject_parser import License
 from pyproject_parser.cli import prettify_deprecation_warning
 
 if TYPE_CHECKING:
 	# 3rd party
 	from consolekit.terminal_colours import ColourTrilean
 	from domdf_python_tools.typing import PathLike
+	from toml import TomlEncoder
 
 __all__ = ["main", "reformat", "check"]
 
 
 @click_group()
 def main() -> None:  # pragma: no cover  # noqa: D103
 	pass
@@ -95,36 +96,36 @@
 		show_traceback: bool = False,
 		) -> None:
 	"""
 	Validate the given ``pyproject.toml`` file.
 	"""
 
 	# 3rd party
-	import dom_toml
 	from dom_toml.parser import BadConfigError
 	from domdf_python_tools.paths import PathPlus
 	from domdf_python_tools.words import Plural, word_join
 
 	# this package
 	from pyproject_parser import PyProject
 	from pyproject_parser.cli import ConfigTracebackHandler, resolve_class
 	from pyproject_parser.parsers import BuildSystemParser, PEP621Parser
+	from pyproject_parser.utils import _load_toml
 
 	if not show_traceback:
 		prettify_deprecation_warning()
 
 	pyproject_file = PathPlus(pyproject_file)
 
 	click.echo(f"Validating {str(pyproject_file)!r}")
 
 	with handle_tracebacks(show_traceback, ConfigTracebackHandler):
 		parser: Type[PyProject] = resolve_class(parser_class, "parser-class")
 		parser.load(filename=pyproject_file)
 
-		raw_config = dom_toml.load(pyproject_file)
+		raw_config = _load_toml(pyproject_file)
 
 		_keys = Plural("key", "keys")
 
 		def error_on_unknown(
 				keys: Iterable[str],
 				expected_keys: Iterable[str],
 				table_name: str,
@@ -194,23 +195,23 @@
 	"""
 
 	# stdlib
 	import os
 	import re
 
 	# 3rd party
-	import dom_toml
 	import sdjson  # nodep
 	from domdf_python_tools.paths import PathPlus, in_directory
 
 	# this package
 	from pyproject_parser import PyProject
 	from pyproject_parser.cli import _json_encoders  # noqa: F401
 	from pyproject_parser.cli import ConfigTracebackHandler, resolve_class
 	from pyproject_parser.type_hints import Readme
+	from pyproject_parser.utils import _load_toml
 
 	if not show_traceback:
 		prettify_deprecation_warning()
 
 	pyproject_file = PathPlus(pyproject_file)
 
 	with handle_tracebacks(show_traceback, ConfigTracebackHandler):
@@ -225,15 +226,15 @@
 
 			config = parser.load(filename=pyproject_file)
 
 			if resolve:
 				with in_directory(pyproject_file.parent):
 					config.resolve_files()
 
-			raw_config = dom_toml.load(pyproject_file)
+			raw_config = _load_toml(pyproject_file)
 
 			output: Any
 
 			if not field:
 				print(sdjson.dumps(config, indent=indent))
 				sys.exit(0)
 
@@ -290,30 +291,29 @@
 	Reformat the given ``pyproject.toml`` file.
 	"""
 
 	# 3rd party
 	from consolekit.terminal_colours import resolve_color_default  # nodep
 	from consolekit.utils import coloured_diff  # nodep
 	from domdf_python_tools.paths import PathPlus
-	from toml import TomlEncoder
 
 	# this package
 	from pyproject_parser import PyProject, _NormalisedName
 	from pyproject_parser.cli import ConfigTracebackHandler, resolve_class
 
 	if not show_traceback:
 		prettify_deprecation_warning()
 
 	pyproject_file = PathPlus(pyproject_file)
 
 	click.echo(f"Reformatting {str(pyproject_file)!r}")
 
 	with handle_tracebacks(show_traceback, ConfigTracebackHandler):
 		parser: Type[PyProject] = resolve_class(parser_class, "parser-class")
-		encoder: Type[TomlEncoder] = resolve_class(encoder_class, "encoder-class")
+		encoder: Type["TomlEncoder"] = resolve_class(encoder_class, "encoder-class")
 
 		original_content: List[str] = pyproject_file.read_lines()
 
 		config = parser.load(filename=pyproject_file, set_defaults=False)
 
 		if config.project is not None and isinstance(config.project["name"], _NormalisedName):
 			config.project["name"] = config.project["name"].unnormalized
```

### Comparing `pyproject-parser-0.8.0/pyproject_parser/classes.py` & `pyproject-parser-0.9.0b1/pyproject_parser/classes.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/pyproject_parser/cli/__init__.py` & `pyproject-parser-0.9.0b1/pyproject_parser/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Pattern, TextIO, Type, Union
 
 # 3rd party
 import click  # nodep
 from consolekit.tracebacks import TracebackHandler  # nodep
-from consolekit.utils import abort  # nodep
 from dom_toml.parser import BadConfigError
 from packaging.specifiers import InvalidSpecifier
 from packaging.version import InvalidVersion
 
 # this package
 from pyproject_parser.utils import PyProjectDeprecationWarning
```

### Comparing `pyproject-parser-0.8.0/pyproject_parser/cli/_json_encoders.py` & `pyproject-parser-0.9.0b1/pyproject_parser/cli/_json_encoders.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/pyproject_parser/parsers.py` & `pyproject-parser-0.9.0b1/pyproject_parser/parsers.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/pyproject_parser/type_hints.py` & `pyproject-parser-0.9.0b1/pyproject_parser/type_hints.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/pyproject_parser/utils.py` & `pyproject-parser-0.9.0b1/pyproject_parser/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,28 @@
 #
 
 # stdlib
 import functools
 import io
 import os
 import sys
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 # 3rd party
 from dom_toml.parser import BadConfigError
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.typing import PathLike
 
+if sys.version_info < (3, 11):
+	# 3rd party
+	import tomli as tomllib
+else:
+	# 3rd party
+	import tomllib
+
 if TYPE_CHECKING:
 	# this package
 	from pyproject_parser.type_hints import ContentTypes
 
 __all__ = ["render_markdown", "render_rst", "content_type_from_filename", "PyProjectDeprecationWarning"]
 
 
@@ -169,7 +176,19 @@
 
 	This is a user-facing warning which will be shown by default.
 	For developer-facing warnings intended for direct consumers of this library,
 	use a standard :class:`DeprecationWarning`.
 
 	.. versionadded:: 0.5.0
 	"""
+
+
+def _load_toml(filename: PathLike, ) -> Dict[str, Any]:
+	r"""
+	Parse TOML from the given file.
+
+	:param filename: The filename to read from to.
+
+	:returns: A mapping containing the ``TOML`` data.
+	"""
+
+	return tomllib.loads(PathPlus(filename).read_text())
```

### Comparing `pyproject-parser-0.8.0/pyproject_parser.egg-info/PKG-INFO` & `pyproject-parser-0.9.0b1/pyproject_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-parser
-Version: 0.8.0
+Version: 0.9.0b1
 Summary: Parser for 'pyproject.toml'
 Home-page: https://github.com/repo-helper/pyproject-parser
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -156,15 +156,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/pyproject-parser
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.8.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/pyproject-parser/v0.9.0b1
 	:target: https://github.com/repo-helper/pyproject-parser/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/pyproject-parser
 	:target: https://github.com/repo-helper/pyproject-parser/commit/master
 	:alt: GitHub last commit
```

### Comparing `pyproject-parser-0.8.0/pyproject_parser.egg-info/SOURCES.txt` & `pyproject-parser-0.9.0b1/pyproject_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/setup.cfg` & `pyproject-parser-0.9.0b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyproject-parser
-version = 0.8.0
+version = 0.9.0b1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = pep518, pep621, pyproject, toml, metadata, packaging
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `pyproject-parser-0.8.0/setup.py` & `pyproject-parser-0.9.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/tests/test_classes.py` & `pyproject-parser-0.9.0b1/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/tests/test_cli.py` & `pyproject-parser-0.9.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/tests/test_cli_module.py` & `pyproject-parser-0.9.0b1/tests/test_cli_module.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/tests/test_config.py` & `pyproject-parser-0.9.0b1/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 		bad_pep621_config,
 		valid_buildsystem_config,
 		valid_pep621_config
 		)
 
 # this package
 from pyproject_parser.parsers import BuildSystemParser, PEP621Parser, RequiredKeysConfigParser
-from pyproject_parser.utils import PyProjectDeprecationWarning
+from pyproject_parser.utils import PyProjectDeprecationWarning, _load_toml
 
 
 @pytest.mark.parametrize("set_defaults", [True, False])
 @pytest.mark.parametrize(
 		"toml_config",
 		[
 				*valid_pep621_config,
@@ -36,15 +36,15 @@
 		set_defaults: bool,
 		):
 
 	(tmp_pathplus / "pyproject.toml").write_clean(toml_config)
 
 	with in_directory(tmp_pathplus):
 		config = PEP621Parser().parse(
-				dom_toml.load(tmp_pathplus / "pyproject.toml")["project"],
+				_load_toml(tmp_pathplus / "pyproject.toml")["project"],
 				set_defaults=set_defaults,
 				)
 
 	advanced_data_regression.check(config)
 
 
 class ReducedPEP621Parser(PEP621Parser, inherit_defaults=True):
@@ -57,15 +57,15 @@
 		tmp_pathplus: PathPlus,
 		advanced_data_regression: AdvancedDataRegressionFixture,
 		):
 
 	(tmp_pathplus / "pyproject.toml").write_clean(toml_config)
 
 	with in_directory(tmp_pathplus):
-		config = ReducedPEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		config = ReducedPEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 	advanced_data_regression.check(config)
 
 
 @pytest.mark.parametrize("filename", ["README.rst", "README.md", "INTRODUCTION.md", "readme.txt"])
 def test_pep621_class_valid_config_readme(
 		filename: str,
@@ -78,15 +78,15 @@
 			'name = "spam"',
 			'version = "2020.0.0"',
 			f'readme = {filename!r}',
 			])
 	(tmp_pathplus / filename).write_text("This is the readme.")
 
 	with in_directory(tmp_pathplus):
-		config = PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		config = PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 	advanced_data_regression.check(config)
 
 
 @pytest.mark.parametrize(
 		"readme",
 		[
@@ -121,15 +121,15 @@
 			])
 	(tmp_pathplus / "README.rst").write_text("This is the reStructuredText README.")
 	(tmp_pathplus / "README.md").write_text("This is the markdown README.")
 	(tmp_pathplus / "README.txt").write_text("This is the plaintext README.")
 	(tmp_pathplus / "README").write_text("This is the README.")
 
 	with in_directory(tmp_pathplus):
-		config = PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		config = PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 	advanced_data_regression.check(config)
 
 
 @pytest.mark.parametrize(
 		"readme, expected, exception",
 		[
@@ -209,15 +209,15 @@
 			"[project]",
 			'name = "spam"',
 			'version = "2020.0.0"',
 			readme,
 			])
 
 	with in_directory(tmp_pathplus), pytest.raises(exception, match=expected):
-		PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 
 @pytest.mark.parametrize("filename", ["LICENSE.rst", "LICENSE.md", "LICENSE.txt", "LICENSE"])
 def test_pep621_class_valid_config_license(
 		filename: str,
 		tmp_pathplus: PathPlus,
 		advanced_data_regression: AdvancedDataRegressionFixture,
@@ -228,15 +228,15 @@
 			f'name = "spam"',
 			f'version = "2020.0.0"',
 			f'license = {{file = "{filename}"}}',
 			])
 	(tmp_pathplus / filename).write_text("This is the license.")
 
 	with in_directory(tmp_pathplus):
-		config = PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		config = PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 	advanced_data_regression.check(config)
 
 
 def test_pep621_class_valid_config_license_dict(
 		tmp_pathplus: PathPlus,
 		advanced_data_regression: AdvancedDataRegressionFixture,
@@ -246,15 +246,15 @@
 			f'[project]',
 			f'name = "spam"',
 			f'version = "2020.0.0"',
 			f'license = {{text = "This is the MIT License"}}',
 			])
 
 	with in_directory(tmp_pathplus):
-		config = PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		config = PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 	advanced_data_regression.check(config)
 
 
 @pytest.mark.parametrize(
 		"license_key, expected",
 		[
@@ -280,15 +280,15 @@
 			f'[project]',
 			f'name = "spam"',
 			f'version = "2020.0.0"',
 			license_key,
 			])
 
 	with in_directory(tmp_pathplus), pytest.raises(BadConfigError, match=expected):
-		PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 
 @pytest.mark.parametrize(
 		"config, expects, match",
 		[
 				*bad_pep621_config,
 				# pytest.param(
@@ -316,15 +316,15 @@
 		expects: Type[Exception],
 		match: str,
 		tmp_pathplus: PathPlus,
 		):
 	(tmp_pathplus / "pyproject.toml").write_clean(config)
 
 	with in_directory(tmp_pathplus), pytest.raises(expects, match=match):
-		PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 
 @pytest.mark.parametrize(
 		"config, match",
 		[
 				pytest.param(
 						'[project]\nname = "foo"\nversion = "1.2.3"\n[project.optional-dependencies]\n"dev_test" = []\n"dev-test" = []',
@@ -348,57 +348,57 @@
 		match: str,
 		tmp_pathplus: PathPlus,
 		):
 
 	(tmp_pathplus / "pyproject.toml").write_clean(config)
 
 	with in_directory(tmp_pathplus), pytest.warns(PyProjectDeprecationWarning, match=match):
-		PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 
 @pytest.mark.parametrize("filename", ["README", "README.rtf"])
 def test_parse_config_readme_errors(filename: str, tmp_pathplus: PathPlus):
 	config = dedent(f"""
 [project]
 name = "spam"
 version = "2020.0.0"
 readme = "{filename}"
 """)
 	(tmp_pathplus / "pyproject.toml").write_clean(config)
 	(tmp_pathplus / filename).write_text("This is the readme.")
 
 	with in_directory(tmp_pathplus), pytest.raises(ValueError, match=f"Unsupported extension for '{filename}'"):
-		PEP621Parser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["project"])
+		PEP621Parser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["project"])
 
 
 @pytest.mark.parametrize("set_defaults", [True, False])
 @pytest.mark.parametrize("toml_config", valid_buildsystem_config)
 def test_buildsystem_parser_valid_config(
 		toml_config: str,
 		tmp_pathplus: PathPlus,
 		advanced_data_regression: AdvancedDataRegressionFixture,
 		set_defaults: bool,
 		):
 	(tmp_pathplus / "pyproject.toml").write_clean(toml_config)
 	config = BuildSystemParser().parse(
-			dom_toml.load(tmp_pathplus / "pyproject.toml")["build-system"],
+			_load_toml(tmp_pathplus / "pyproject.toml")["build-system"],
 			set_defaults=set_defaults,
 			)
 
 	config["requires"] = list(map(str, config["requires"]))  # type: ignore[arg-type]
 
 	advanced_data_regression.check(config)
 
 
 @pytest.mark.parametrize("config, expects, match", bad_buildsystem_config)
 def test_buildsystem_parser_errors(config: str, expects: Type[Exception], match: str, tmp_pathplus: PathPlus):
 	(tmp_pathplus / "pyproject.toml").write_clean(config)
 
 	with in_directory(tmp_pathplus), pytest.raises(expects, match=match):
-		BuildSystemParser().parse(dom_toml.load(tmp_pathplus / "pyproject.toml")["build-system"])
+		BuildSystemParser().parse(_load_toml(tmp_pathplus / "pyproject.toml")["build-system"])
 
 
 def test_RequiredKeysConfigParser():
 
 	class MyConfigParser(RequiredKeysConfigParser):
 		table_name = "my_table"
 		required_keys = ["foo"]
```

### Comparing `pyproject-parser-0.8.0/tests/test_dumping.py` & `pyproject-parser-0.9.0b1/tests/test_dumping.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/tests/test_pyproject_class.py` & `pyproject-parser-0.9.0b1/tests/test_pyproject_class.py`

 * *Files identical despite different names*

### Comparing `pyproject-parser-0.8.0/tests/test_utils.py` & `pyproject-parser-0.9.0b1/tests/test_utils.py`

 * *Files identical despite different names*

