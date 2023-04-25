# Comparing `tmp/types-ujson-5.7.0.3.tar.gz` & `tmp/types-ujson-5.7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ujson-5.7.0.3.tar", last modified: Thu Apr 13 15:15:35 2023, max compression
+gzip compressed data, was "types-ujson-5.7.0.4.tar", last modified: Tue Apr 25 06:19:37 2023, max compression
```

## Comparing `types-ujson-5.7.0.3.tar` & `types-ujson-5.7.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/types_ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 15:15:35.000000 types-ujson-5.7.0.3/types_ujson.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:15:35.116155 types-ujson-5.7.0.3/ujson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/ujson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-13 15:15:33.000000 types-ujson-5.7.0.3/ujson-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:19:37.082490 types-ujson-5.7.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-25 06:19:35.000000 types-ujson-5.7.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 06:19:35.000000 types-ujson-5.7.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-25 06:19:37.082490 types-ujson-5.7.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:19:37.082490 types-ujson-5.7.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-25 06:19:35.000000 types-ujson-5.7.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:19:37.082490 types-ujson-5.7.0.4/types_ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-25 06:19:37.000000 types-ujson-5.7.0.4/types_ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 06:19:37.000000 types-ujson-5.7.0.4/types_ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:19:37.000000 types-ujson-5.7.0.4/types_ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 06:19:37.000000 types-ujson-5.7.0.4/types_ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:19:37.082490 types-ujson-5.7.0.4/ujson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 06:19:35.000000 types-ujson-5.7.0.4/ujson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-25 06:19:35.000000 types-ujson-5.7.0.4/ujson-stubs/__init__.pyi
```

### Comparing `types-ujson-5.7.0.3/CHANGELOG.md` & `types-ujson-5.7.0.4/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 5.7.0.4 (2023-04-25)
+
+Loosen constraints on ujson file functions (#10081)
+
+Like `json.dump`, `ujson.dump` takes any object that has a
+string-accepting `.write` method.
+
+Similarly, `ujson.load` works with any object with a `.read()` that
+returns either a string or a bytes
+
 ## 5.7.0.3 (2023-04-13)
 
 Make most ujson.dump() parameters keyword-only (#10044)
 
 ## 5.7.0.2 (2023-04-12)
 
 [ujson] Update stubs with new features (#10035)
```

### Comparing `types-ujson-5.7.0.3/PKG-INFO` & `types-ujson-5.7.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.7.0.3
+Version: 5.7.0.4
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6f35e8d9faf93f8f72af1b22a8006e75f7d0961c`.
+This package was generated from typeshed commit `9abf620500644509a0ba656767e858ac2ef23dd6`.
```

### Comparing `types-ujson-5.7.0.3/setup.py` & `types-ujson-5.7.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6f35e8d9faf93f8f72af1b22a8006e75f7d0961c`.
+This package was generated from typeshed commit `9abf620500644509a0ba656767e858ac2ef23dd6`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.7.0.3",
+      version="5.7.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md",
```

### Comparing `types-ujson-5.7.0.3/types_ujson.egg-info/PKG-INFO` & `types-ujson-5.7.0.4/types_ujson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.7.0.3
+Version: 5.7.0.4
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6f35e8d9faf93f8f72af1b22a8006e75f7d0961c`.
+This package was generated from typeshed commit `9abf620500644509a0ba656767e858ac2ef23dd6`.
```

### Comparing `types-ujson-5.7.0.3/ujson-stubs/__init__.pyi` & `types-ujson-5.7.0.4/ujson-stubs/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, SupportsRead, SupportsWrite
 from collections.abc import Callable
-from typing import IO, Any, AnyStr
+from typing import Any, AnyStr
 
 __version__: str
 
 def encode(
     obj: Any,
     ensure_ascii: bool = ...,
     double_precision: int = ...,
@@ -28,25 +28,25 @@
     allow_nan: bool = ...,
     reject_bytes: bool = ...,
     default: Callable[[Incomplete], Incomplete] | None = None,
     separators: tuple[str, str] | None = None,
 ) -> str: ...
 def dump(
     obj: Any,
-    fp: IO[str],
+    fp: SupportsWrite[str],
     *,
     ensure_ascii: bool = ...,
     double_precision: int = ...,
     encode_html_chars: bool = ...,
     escape_forward_slashes: bool = ...,
     sort_keys: bool = ...,
     indent: int = ...,
     allow_nan: bool = ...,
     reject_bytes: bool = ...,
     default: Callable[[Incomplete], Incomplete] | None = None,
     separators: tuple[str, str] | None = None,
 ) -> None: ...
 def decode(s: AnyStr, precise_float: bool = ...) -> Any: ...
 def loads(s: AnyStr, precise_float: bool = ...) -> Any: ...
-def load(fp: IO[AnyStr], precise_float: bool = ...) -> Any: ...
+def load(fp: SupportsRead[str | bytes], precise_float: bool = ...) -> Any: ...
 
 class JSONDecodeError(ValueError): ...
```

