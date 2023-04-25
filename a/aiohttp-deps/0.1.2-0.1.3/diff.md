# Comparing `tmp/aiohttp_deps-0.1.2.tar.gz` & `tmp/aiohttp_deps-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.1.2.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.1.3.tar", max compression
```

## Comparing `aiohttp_deps-0.1.2.tar` & `aiohttp_deps-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/LICENSE
--rw-r--r--   0        0        0     6819 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/README.md
--rw-r--r--   0        0        0      375 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     2221 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1211 2023-04-22 15:35:11.839741 aiohttp_deps-0.1.2/aiohttp_deps/router.py
--rw-r--r--   0        0        0      890 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0     7447 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1317 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1766 2023-04-22 15:35:11.843741 aiohttp_deps-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8126 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6819 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/README.md
+-rw-r--r--   0        0        0      375 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3202 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0     7447 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1317 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1766 2023-04-25 10:54:38.961979 aiohttp_deps-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8126 1970-01-01 00:00:00.000000 aiohttp_deps-0.1.3/PKG-INFO
```

### Comparing `aiohttp_deps-0.1.2/LICENSE` & `aiohttp_deps-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.2/README.md` & `aiohttp_deps-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.2/aiohttp_deps/router.py` & `aiohttp_deps-0.1.3/aiohttp_deps/router.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,19 @@
     Because after you initialize dependencies contexts,
     handler functions won't have the same types as
     in default AioHTTP code.
 
     New types are introduced in stub file: router.pyi.
     """
 
-    def add_routes(self, router: Iterable[web.RouteDef], prefix: str = "") -> None:
+    def add_routes(
+        self,
+        router: Iterable[web.AbstractRouteDef],
+        prefix: str = "",
+    ) -> None:
         """
         Append another router's routes to this one.
 
         :param router: router to get routes from.
         :param prefix: url prefix for routes, defaults to ""
         :raises ValueError: if prefix is incorrect.
         """
```

### Comparing `aiohttp_deps-0.1.2/aiohttp_deps/router.pyi` & `aiohttp_deps-0.1.3/aiohttp_deps/router.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     def get(self, path: str, **kwargs: Any) -> _Deco: ...
     def post(self, path: str, **kwargs: Any) -> _Deco: ...
     def put(self, path: str, **kwargs: Any) -> _Deco: ...
     def patch(self, path: str, **kwargs: Any) -> _Deco: ...
     def delete(self, path: str, **kwargs: Any) -> _Deco: ...
     def options(self, path: str, **kwargs: Any) -> _Deco: ...
     def view(self, path: str, **kwargs: Any) -> _Deco: ...
-    def add_routes(self, router: Iterable[web.RouteDef], prefix: str = "") -> None: ...
+    def add_routes(self, router: Iterable[web.AbstractRouteDef], prefix: str = "") -> None: ...
```

### Comparing `aiohttp_deps-0.1.2/aiohttp_deps/utils.py` & `aiohttp_deps-0.1.3/aiohttp_deps/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.2/aiohttp_deps/view.py` & `aiohttp_deps-0.1.3/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.1.2/pyproject.toml` & `aiohttp_deps-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aiohttp_deps-0.1.2/PKG-INFO` & `aiohttp_deps-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
```

