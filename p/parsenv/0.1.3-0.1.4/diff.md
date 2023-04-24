# Comparing `tmp/parsenv-0.1.3.tar.gz` & `tmp/parsenv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsenv-0.1.3.tar", last modified: Fri Apr 14 15:00:54 2023, max compression
+gzip compressed data, was "parsenv-0.1.4.tar", last modified: Mon Apr 24 23:09:18 2023, max compression
```

## Comparing `parsenv-0.1.3.tar` & `parsenv-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.3/env/__init__.py
--rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.3/env/core.py
--rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.3/env/main.py
--rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.3/env/parsers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.3/env/py.typed
--rw-r--r--   0        0        0      449 2023-04-14 15:00:50.420182 parsenv-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      665 2023-04-14 15:00:50.440285 parsenv-0.1.3/README.md
--rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.3/tests/__main__.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 parsenv-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      130 2023-04-24 23:04:40.337356 parsenv-0.1.4/env/__init__.py
+-rw-r--r--   0        0        0      997 2023-04-14 15:15:41.479758 parsenv-0.1.4/env/core.py
+-rw-r--r--   0        0        0      647 2023-04-24 23:04:40.258226 parsenv-0.1.4/env/main.py
+-rw-r--r--   0        0        0      475 2023-04-24 23:04:40.310184 parsenv-0.1.4/env/parsers.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.4/env/py.typed
+-rw-r--r--   0        0        0      457 2023-04-24 23:09:09.040135 parsenv-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      665 2023-04-14 15:00:50.440285 parsenv-0.1.4/README.md
+-rw-r--r--   0        0        0      828 2023-04-24 23:06:24.195561 parsenv-0.1.4/tests/__main__.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 parsenv-0.1.4/PKG-INFO
```

### Comparing `parsenv-0.1.3/env/core.py` & `parsenv-0.1.4/env/core.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.3/env/main.py` & `parsenv-0.1.4/env/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from .core import get_var, DT, UNDEFINED
-from .parsers import parse_ints, parse_strs
+from .parsers import parse_ints, parse_strs, parse_bool
 
 
 def get(key: str, default: DT = UNDEFINED) -> str | DT:
     return get_var(key, default)
 
 
 def get_int(key: str, default: DT = UNDEFINED) -> int | DT:
     return get_var(key, default, int)
 
 
+def get_bool(key: str, default: DT = UNDEFINED) -> bool | DT:
+    return get_var(key, default, parse_bool)
+
+
 def get_strs(key: str, default: DT = UNDEFINED) -> list[str] | DT:
     return get_var(key, default, parse_strs)
 
 
 def get_ints(key: str, default: DT = UNDEFINED) -> list[int] | DT:
     return get_var(key, default, parse_ints)
```

### Comparing `parsenv-0.1.3/README.md` & `parsenv-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.3/tests/__main__.py` & `parsenv-0.1.4/tests/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,30 @@
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", False) is False
 assert env.get_int("PORT") == 123
 assert env.get_strs("KEYS", []) == ["word1", "F402", "12"]
 assert env.get_ints("ADMIN_IDS") == [1, 2, 3]
 assert env.get_ints("X", 0) == 0
+assert env.get_bool("T_BOOL")
+assert not env.get_bool("F_BOOL")
 
 try:
     env.get("X")
 except KeyError as e:
     assert str(e) == "Environment variable `X` not set"
 
 try:
     env.get_ints("BAD_NUMS")
 except ValueError as e:
     assert (
         str(e) == "Can't parse environment variable `BAD_NUMS`: "
         "invalid literal for int() with base 10: 'a'"
     )
+
+try:
+    env.get_bool("BAD_BOOL")
+except ValueError as e:
+    assert (
+        str(e)
+        == "Can't parse environment variable `BAD_BOOL`: Can't parse bool from `ok`"
+    )
```

### Comparing `parsenv-0.1.3/PKG-INFO` & `parsenv-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsenv
-Version: 0.1.3
+Version: 0.1.4
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Env parser
```

