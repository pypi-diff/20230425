# Comparing `tmp/python_regius-0.1.1.tar.gz` & `tmp/python_regius-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_regius-0.1.1.tar", max compression
+gzip compressed data, was "python_regius-0.2.0.tar", max compression
```

## Comparing `python_regius-0.1.1.tar` & `python_regius-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       59 2023-04-23 23:35:15.384800 python_regius-0.1.1/README.md
--rw-r--r--   0        0        0      728 2023-04-24 00:24:41.815654 python_regius-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       94 2023-04-23 21:27:23.659621 python_regius-0.1.1/regius/__init__.py
--rw-r--r--   0        0        0     1151 2023-04-24 00:21:25.420313 python_regius-0.1.1/regius/client.py
--rw-r--r--   0        0        0     3185 2023-04-24 00:23:31.372352 python_regius-0.1.1/regius/server.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 python_regius-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      342 2023-04-25 03:42:05.138597 python_regius-0.2.0/README.md
+-rw-r--r--   0        0        0      797 2023-04-25 03:54:34.750789 python_regius-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-04-25 04:04:07.413681 python_regius-0.2.0/regius/__init__.py
+-rw-r--r--   0        0        0     2201 2023-04-25 03:54:25.854134 python_regius-0.2.0/regius/app.py
+-rw-r--r--   0        0        0      211 2023-04-25 01:48:07.293166 python_regius-0.2.0/regius/asyncio.py
+-rw-r--r--   0        0        0     1893 2023-04-25 03:56:12.643851 python_regius-0.2.0/regius/module.py
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 python_regius-0.2.0/PKG-INFO
```

### Comparing `python_regius-0.1.1/regius/client.py` & `python_regius-0.2.0/regius/module.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,69 @@
+from logging import getLogger
 from os import environ
 
-from httpx import AsyncClient
+from httpx import AsyncClient, Client
 
-__all__ = ["import_module", "RegiusModule"]
+__all__ = ["RegiusModule", "RegiusAsyncModule"]
 
-_environ = environ.copy()
+_endpoint_override: dict[str, str] = {}
+_endpoint_template = "http://{name}"
+
+getLogger("httpx").setLevel("INFO")
 
 try:
     from dotenv import dotenv_values
 
-    _environ = {**dotenv_values(".env"), **_environ}
+    dotenv = dotenv_values(".env")
+    env = environ.copy()
+    env.update(**dotenv)
 except ImportError:
-    pass
+    env = environ
 
+if "REGIUS_ENDPOINT_TEMPLATE" in env:
+    _endpoint_template = env["REGIUS_ENDPOINT_TEMPLATE"]
 
-class RegiusModule(object):
-    _endpoint_override: dict[str, str] = {}
-    _endpoint_template = _environ.get("REGIUS_ENDPOINT_TEMPLATE", "http://{name}")
 
+class RegiusModule(object):
     def __init__(self, name: str):
-        endpoint = self._endpoint_override.get(name)
-        if endpoint is None:
-            endpoint = self._endpoint_template.format(name=name)
+        if name in _endpoint_override:
+            endpoint = _endpoint_override[name]
+        else:
+            endpoint = _endpoint_template.format(name=name)
 
-        self._client = AsyncClient(base_url=endpoint)
+        self._client = Client(base_url=endpoint)
 
     def __getattr__(self, name: str):
-        return _create_rpc(self._client, name)
+        def regius_method(*args, **kwargs):
+            if args and kwargs:
+                raise ValueError("Cannot specify both args and kwargs")
+
+            response = self._client.post(name, json=kwargs or args)
+            response.raise_for_status()
+            return response.json()
 
+        regius_method.__name__ = name
 
-def import_module(name: str):
-    return RegiusModule(name)
+        return regius_method
 
 
-def _create_rpc(client: AsyncClient, name: str):
-    async def rpc(*args, **kwargs):
-        if args and kwargs:
-            raise ValueError("Cannot specify both args and kwargs")
+class RegiusAsyncModule(object):
+    def __init__(self, name: str):
+        if name in _endpoint_override:
+            endpoint = _endpoint_override[name]
+        else:
+            endpoint = _endpoint_template.format(name=name)
+
+        self._client = AsyncClient(base_url=endpoint)
+
+    def __getattr__(self, name: str):
+        async def regius_method(*args, **kwargs):
+            if args and kwargs:
+                raise ValueError("Cannot specify both args and kwargs")
 
-        response = await client.post(name, json=kwargs or args)
-        response.raise_for_status()
-        return response.json()
+            response = await self._client.post(name, json=kwargs or args)
+            response.raise_for_status()
+            return response.json()
 
-    rpc.__name__ = name
+        regius_method.__name__ = name
 
-    return rpc
+        return regius_method
```

### Comparing `python_regius-0.1.1/regius/server.py` & `python_regius-0.2.0/regius/app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,77 @@
-import os.path
 from importlib.util import module_from_spec, spec_from_file_location
-from inspect import iscoroutinefunction, isfunction
-from typing import Callable
+from inspect import iscoroutine, isfunction
+from types import ModuleType
 
-from sanic import BadRequest, Request, Sanic, json
+from sanic import BadRequest, NotFound, Request, Sanic, json
 from sanic.log import logger
 
-__all__ = ["app", "RegiusApp"]
+__all__ = ["RegiusApp"]
 
 
 class RegiusApp(Sanic):
-    def __init__(self, path: str, *args, **kwargs):
-        super().__init__(name="regius_app", *args, **kwargs)
+    _logger = logger.getChild("regius")
 
-        path = os.path.join(path, "__init__.py")
-        module = _load_module(path)
-        _install_handlers(self, module.__dict__)
-
-
-def app(*args, **kwargs):
-    import os
+    def __init__(self, module: ModuleType, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.ctx._module = module
 
-    return RegiusApp(path=os.getcwd(), *args, **kwargs)
+        self.add_route(self._handler, "/<name>", methods=["POST"])
 
-
-def _load_module(path: str):
-    try:
-        spec = spec_from_file_location("regius_module", path)
-        assert spec is not None, "Could not get module spec"
+    def refresh(self, *args, **kwargs):
+        spec = self.ctx._module.__spec__
+        assert spec is not None
 
         loader = spec.loader
-        assert loader is not None, "Could not get module loader from spec"
-
-        module = module_from_spec(spec)
-        loader.exec_module(module)
-
-        return module
-    except (FileNotFoundError, AssertionError) as exc:
-        raise ModuleNotFoundError(f"Could not find module at {path}") from exc
-
-
-def _install_handlers(app: Sanic, func_dict: dict[str, Callable]):
-    for name, value in func_dict.items():
-        if name.startswith("_"):
-            continue
-
-        if not isfunction(value):
-            logger.warning("Skipping %s because it is not a function", name)
-            continue
-
-        logger.info("Registering function %s", name)
-        handler = _create_handler(value)
-        app.add_route(handler, f"/{name}", methods=["POST"], name=name)
-
-
-def _create_handler(func: Callable):
-    if iscoroutinefunction(func):
-        return _handle_async(func)
-    else:
-        return _handle_sync(func)
+        assert loader is not None
 
+        loader.exec_module(self.ctx._module)
 
-def _handle_async(func: Callable):
-    async def handler(request: Request):
-        data = request.json
+        return super().refresh(*args, **kwargs)
 
-        if isinstance(data, dict):
-            logger.debug("Calling %r with dict %r", func, data)
-
-            body = await func(**data)
-
-            logger.debug("Calling %r with list %r got %r", func, data, body)
-
-            return json(body)
-        elif isinstance(data, list):
-            logger.debug("Calling %r with list %r", func, data)
-
-            body = await func(*data)
+    @classmethod
+    def from_path(cls, path: str, *args, **kwargs):
+        module = _load_module(path)
 
-            logger.debug("Calling %r with list %r got %r", func, data, body)
+        return cls(module, *args, **kwargs)
 
-            return json(body)
+    async def _handler(self, request: Request, name: str):
+        try:
+            assert not name.startswith("_")
+            func = getattr(self.ctx._module, name)
+            assert isfunction(func)
+        except (AttributeError, AssertionError):
+            raise NotFound
+
+        body = request.json
+
+        if isinstance(body, list):
+            self._logger.info("--> %s(%r)", name, body)
+            result = func(*body)
+        elif isinstance(body, dict):
+            self._logger.info("--> %s(%r)", name, body)
+            result = func(**body)
         else:
             raise BadRequest("Invalid request body, expected array or object")
 
-    return handler
+        if iscoroutine(result):
+            result = await result
 
+        self._logger.info("<-- %s(%r) = %r", name, body, result)
 
-def _handle_sync(func: Callable):
-    async def handler(request: Request):
-        data = request.json
+        return json(result)
 
-        if isinstance(data, dict):
-            logger.debug("Calling %r with dict %r", func, data)
 
-            body = func(**data)
-
-            logger.debug("Calling %r with list %r got %r", func, data, body)
-
-            return json(body)
-        elif isinstance(data, list):
-            logger.debug("Calling %r with list %r", func, data)
-
-            body = func(*data)
+def _load_module(path: str):
+    try:
+        spec = spec_from_file_location("regius_module", path)
+        assert spec is not None
 
-            logger.debug("Calling %r with list %r got %r", func, data, body)
+        loader = spec.loader
+        assert loader is not None
 
-            return json(body)
-        else:
-            raise BadRequest("Invalid request body, expected array or object")
+        module = module_from_spec(spec)
+        loader.exec_module(module)
 
-    return handler
+        return module
+    except (FileNotFoundError, AssertionError) as exc:
+        raise ModuleNotFoundError(f"Could not find module at {path}") from exc
```

### Comparing `python_regius-0.1.1/PKG-INFO` & `python_regius-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,51 @@
 Metadata-Version: 2.1
 Name: python-regius
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python Regius - A simple & friendly Python RPC framework.
 Home-page: https://jihulab.com/Sya/Regius/regius.git
 License: Proprietary
 Author: 王见充
 Author-email: gerhut@sya.org.cn
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: sanic (>=23.3.0,<24.0.0)
 Project-URL: Repository, https://jihulab.com/Sya/Regius/regius.git
 Description-Content-Type: text/markdown
 
 # Python Regius
 
 A simple & friendly Python RPC framework.
 
+## Install
+
+```bash
+pip install python-regius
+```
+
+## Server Usage
+
+Write a file named `__init__.py` in current directory.
+
+```python
+def add(a, b):
+    return a + b
+```
+
+And Run
+
+```bash
+sanic regius:app
+```
+
+## Client Usage
+
+```python
+from regius import add
+
+print(add(1, 2))
+```
+
```

