# Comparing `tmp/dist-meta-0.7.0.tar.gz` & `tmp/dist-meta-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist-meta-0.7.0.tar", last modified: Thu Mar  9 13:13:38 2023, max compression
+gzip compressed data, was "dist-meta-0.8.0.tar", last modified: Tue Apr 25 08:56:44 2023, max compression
```

## Comparing `dist-meta-0.7.0.tar` & `dist-meta-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 13:13:38.490944 dist-meta-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-03-09 13:13:10.000000 dist-meta-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-03-09 13:13:10.000000 dist-meta-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-03-09 13:13:38.490944 dist-meta-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5116 2023-03-09 13:13:10.000000 dist-meta-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 13:13:38.490944 dist-meta-0.7.0/dist_meta/
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18820 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/distributions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10350 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (122)     7042 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     8649 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/metadata_mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7956 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/record.py
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-03-09 13:13:10.000000 dist-meta-0.7.0/dist_meta/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 13:13:38.490944 dist-meta-0.7.0/dist_meta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-03-09 13:13:38.000000 dist-meta-0.7.0/dist_meta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-03-09 13:13:38.000000 dist-meta-0.7.0/dist_meta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 13:13:38.000000 dist-meta-0.7.0/dist_meta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 13:13:38.000000 dist-meta-0.7.0/dist_meta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-03-09 13:13:38.000000 dist-meta-0.7.0/dist_meta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-09 13:13:38.000000 dist-meta-0.7.0/dist_meta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4842 2023-03-09 13:13:10.000000 dist-meta-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-03-09 13:13:10.000000 dist-meta-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-03-09 13:13:38.490944 dist-meta-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-03-09 13:13:10.000000 dist-meta-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.012237 dist-meta-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-25 08:56:05.000000 dist-meta-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-25 08:56:05.000000 dist-meta-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-04-25 08:56:44.012237 dist-meta-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5116 2023-04-25 08:56:05.000000 dist-meta-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.008237 dist-meta-0.8.0/dist_meta/
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18820 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10350 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6810 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8649 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/metadata_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     8678 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4541 2023-04-25 08:56:05.000000 dist-meta-0.8.0/dist_meta/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.008237 dist-meta-0.8.0/dist_meta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-25 08:56:44.000000 dist-meta-0.8.0/dist_meta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-25 08:56:43.000000 dist-meta-0.8.0/dist_meta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-04-25 08:56:05.000000 dist-meta-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-25 08:56:05.000000 dist-meta-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-04-25 08:56:44.012237 dist-meta-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-04-25 08:56:05.000000 dist-meta-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:56:44.012237 dist-meta-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    19121 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10134 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10319 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3975 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_metadata_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_metadata_top_packages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4729 2023-04-25 08:56:05.000000 dist-meta-0.8.0/tests/test_wheel.py
```

### Comparing `dist-meta-0.7.0/LICENSE` & `dist-meta-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dist-meta-0.7.0/PKG-INFO` & `dist-meta-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dist-meta
-Version: 0.7.0
+Version: 0.8.0
 Summary: Parse and create Python distribution metadata.
 Home-page: https://github.com/repo-helper/dist-meta
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -152,15 +153,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/dist-meta
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.0
 	:target: https://github.com/repo-helper/dist-meta/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/commit/master
 	:alt: GitHub last commit
```

### Comparing `dist-meta-0.7.0/README.rst` & `dist-meta-0.8.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/dist-meta
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.0
 	:target: https://github.com/repo-helper/dist-meta/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/commit/master
 	:alt: GitHub last commit
```

### Comparing `dist-meta-0.7.0/dist_meta/__init__.py` & `dist-meta-0.8.0/dist_meta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 # this package
 from dist_meta.distributions import get_distribution, iter_distributions  # noqa: F401
 from dist_meta.entry_points import get_all_entry_points, get_entry_points  # noqa: F401
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0"
+__version__: str = "0.8.0"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `dist-meta-0.7.0/dist_meta/_utils.py` & `dist-meta-0.8.0/dist_meta/_utils.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.7.0/dist_meta/distributions.py` & `dist-meta-0.8.0/dist_meta/distributions.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.7.0/dist_meta/entry_points.py` & `dist-meta-0.8.0/dist_meta/entry_points.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.7.0/dist_meta/metadata.py` & `dist-meta-0.8.0/dist_meta/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,34 +23,30 @@
 #  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
 #  DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
-import re
 import sys
 from typing import List
 
 # 3rd party
 from domdf_python_tools.paths import PathPlus
 from domdf_python_tools.typing import PathLike
 from domdf_python_tools.utils import divide
 
 # this package
 from dist_meta.metadata_mapping import MetadataEmitter, MetadataMapping
 
 __all__ = ("dump", "dumps", "load", "loads", "MissingFieldError")
 
-WSP = " \t"
 DELIMITER = "\n\n"
 NEWLINE_MARK = '\uf8ff'
 
-_unfold_re = re.compile(rf"\n([{WSP}])")
-
 
 def _clean_desc(lines: List[str], wsp: str) -> List[str]:
 	#  Adapted from inspect.cleandoc
 	#  Licensed under the Python Software Foundation License Version 2.
 	#  Copyright © 2001-2020 Python Software Foundation. All rights reserved.
 	#  Copyright © 2000 BeOpen.com. All rights reserved.
 	#  Copyright © 1995-2000 Corporation for National Research Initiatives. All rights reserved.
@@ -90,31 +86,30 @@
 	"""
 	Parse Python core metadata from the given string.
 
 	:param rawtext:
 
 	:returns: A mapping of the metadata fields, and the long description
 	"""
-	rawtext = rawtext.replace('\r', '')
+
+	rawtext = rawtext.replace("\r\n", '\n')
 
 	if DELIMITER in rawtext:
 		rawtext, body = rawtext.split(DELIMITER, maxsplit=1)
 	else:
 		body = ''
 
 	# unfold per RFC 5322 § 2.2.3
-	rawtext = _unfold_re.sub(fr"{NEWLINE_MARK}\1", rawtext)
+	rawtext = rawtext.replace("\n\t", f"{NEWLINE_MARK}\t").replace("\n ", f"{NEWLINE_MARK} ")
 
 	file_content: List[str] = rawtext.split('\n')
-	file_content.reverse()
 
 	fields: MetadataMapping = MetadataMapping()
 
-	while file_content:
-		line = file_content.pop()
+	for line in file_content:
 		if not line:
 			continue
 
 		field_name, field_value = divide(line, ':')
 
 		# pylint: disable=loop-global-usage
 		if field_name.lower() != "description":
@@ -123,23 +118,17 @@
 			# Unwrap
 			description_lines = field_value.split(NEWLINE_MARK)
 			description_lines = _clean_desc(description_lines, ' ')
 			description_lines = _clean_desc(description_lines, '\t')
 			description_lines = _clean_desc(description_lines, '|')
 			# pylint: enable=loop-global-usage
 
-			# Remove any trailing or leading blank lines.
-			while description_lines and not description_lines[-1]:
-				description_lines.pop()
-			while description_lines and not description_lines[0]:
-				description_lines.pop(0)
-
-			field_value = '\n'.join(description_lines).strip() + '\n'
-
-			fields["Description"] = field_value
+			# pylint: disable=loop-invariant-statement
+			fields["Description"] = '\n'.join(description_lines).strip() + '\n'
+			# pylint: enable=loop-invariant-statement
 
 	if body.strip():
 		if "Description" in fields:
 			raise ValueError(
 					"A value was given for the 'Description' field "
 					"but the body of the file is not empty."
 					)
```

### Comparing `dist-meta-0.7.0/dist_meta/metadata_mapping.py` & `dist-meta-0.8.0/dist_meta/metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.7.0/dist_meta/record.py` & `dist-meta-0.8.0/dist_meta/record.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import csv
 import os
 import pathlib
+import posixpath
+import sys
 from base64 import urlsafe_b64decode, urlsafe_b64encode
 from typing import TYPE_CHECKING, NamedTuple, Optional, Type, TypeVar
 
 # 3rd party
 from domdf_python_tools.stringlist import DelimitedList
 from domdf_python_tools.typing import PathLike
 
@@ -93,33 +95,55 @@
 	def __init__(
 			self,
 			path: PathLike,
 			hash: Optional["FileHash"] = None,  # noqa: A002  # pylint: disable=redefined-builtin
 			size: Optional[int] = None,
 			distro: Optional["Distribution"] = None,
 			):
-		super().__init__()
+		if sys.version_info < (3, 12):  # pragma: no cover (py312+)
+			super().__init__()
+		else:  # pragma: no cover (<py312)
+			super().__init__(self._coerce_path(path))
 
 	def __new__(
 			cls: Type[_RE],
 			path: PathLike,
 			hash: Optional["FileHash"] = None,  # noqa: A002  # pylint: disable=redefined-builtin
 			size: Optional[int] = None,
 			distro: Optional["Distribution"] = None,
 			) -> _RE:
 		"""
 		Construct a :class:`RecordEntry` from one a string or an existing :class:`pathlib.PurePath` object.
 		"""
 
-		self = cls._from_parts((path, ))  # type: ignore[attr-defined]
+		self = super().__new__(cls, cls._coerce_path(path))
 		self.hash = hash
 		self.size = size
 		self.distro = distro
 		return self
 
+	@classmethod
+	def _coerce_path(cls, path: PathLike) -> PathLike:
+		"""
+		Necessary to fix issue in Python 3.12 where path separators are no longer converted.
+		"""
+
+		if os.path.isabs(path):
+			raise ValueError("RecordEntry paths cannot be absolute")
+
+		if isinstance(path, pathlib.PurePath):
+			if path.is_absolute():
+				# Catch absolute paths from other platform
+				raise ValueError("RecordEntry paths cannot be absolute")
+			path = path.as_posix()
+			if posixpath.isabs(path):
+				raise ValueError("RecordEntry paths cannot be absolute")
+
+		return path
+
 	def read_text(
 			self,
 			encoding: Optional[str] = "UTF-8",
 			errors: Optional[str] = None,
 			) -> str:
 		"""
 		Open the file in text mode, read it, and close the file.
@@ -166,15 +190,15 @@
 		return f"{self.__class__.__name__}({parts:, })"
 
 	def as_record_entry(self) -> str:
 		"""
 		Returns an entry for a ``RECORD`` file, in the form ``<name>,<hash>,<size>``.
 		"""
 
-		parts = [os.fspath(self)]
+		parts = [self.as_posix()]
 
 		if self.hash is not None:
 			parts.append(self.hash.to_string())
 		else:
 			parts.append('')
 
 		if self.size is not None:
```

### Comparing `dist-meta-0.7.0/dist_meta/wheel.py` & `dist-meta-0.8.0/dist_meta/wheel.py`

 * *Files identical despite different names*

### Comparing `dist-meta-0.7.0/dist_meta.egg-info/PKG-INFO` & `dist-meta-0.8.0/dist_meta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dist-meta
-Version: 0.7.0
+Version: 0.8.0
 Summary: Parse and create Python distribution metadata.
 Home-page: https://github.com/repo-helper/dist-meta
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2021 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Typing :: Typed
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
@@ -152,15 +153,15 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/dist-meta
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/dist-meta/v0.8.0
 	:target: https://github.com/repo-helper/dist-meta/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/dist-meta
 	:target: https://github.com/repo-helper/dist-meta/commit/master
 	:alt: GitHub last commit
```

### Comparing `dist-meta-0.7.0/pyproject.toml` & `dist-meta-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dist-meta"
-version = "0.7.0"
+version = "0.8.0"
 description = "Parse and create Python distribution metadata."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "dist-info", "metadata", "packaging", "pypi",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
 dynamic = [ "dependencies",]
@@ -136,15 +137,15 @@
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving :: Packaging",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "dist_meta"
 
 [tool.mypy]
 python_version = "3.8"
```

### Comparing `dist-meta-0.7.0/setup.cfg` & `dist-meta-0.8.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dist-meta
-version = 0.7.0
+version = 0.8.0
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = packaging, dist-info, metadata, pypi
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
@@ -21,14 +21,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Archiving :: Packaging
 	Typing :: Typed
 
 [options]
```

### Comparing `dist-meta-0.7.0/setup.py` & `dist-meta-0.8.0/setup.py`

 * *Files identical despite different names*

