# Comparing `tmp/electrickiwi-api-0.8.2.tar.gz` & `tmp/electrickiwi-api-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrickiwi-api-0.8.2.tar", last modified: Tue Apr 25 06:42:18 2023, max compression
+gzip compressed data, was "electrickiwi-api-0.8.3.tar", last modified: Tue Apr 25 09:20:51 2023, max compression
```

## Comparing `electrickiwi-api-0.8.2.tar` & `electrickiwi-api-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 06:42:18.109495 electrickiwi-api-0.8.2/
--rw-rw-r--   0 michael   (1000) michael   (1000)    35149 2022-10-20 08:35:26.000000 electrickiwi-api-0.8.2/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-25 06:42:18.109495 electrickiwi-api-0.8.2/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     1678 2023-04-25 06:41:37.000000 electrickiwi-api-0.8.2/README.md
--rw-rw-r--   0 michael   (1000) michael   (1000)      914 2023-04-25 06:41:37.000000 electrickiwi-api-0.8.2/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      177 2023-04-25 06:42:18.110495 electrickiwi-api-0.8.2/setup.cfg
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 06:42:18.100494 electrickiwi-api-0.8.2/src/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 06:42:18.107495 electrickiwi-api-0.8.2/src/electrickiwi_api/
--rw-rw-r--   0 michael   (1000) michael   (1000)      428 2023-04-25 06:41:37.000000 electrickiwi-api-0.8.2/src/electrickiwi_api/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9031 2023-04-17 05:33:03.000000 electrickiwi-api-0.8.2/src/electrickiwi_api/api.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1428 2023-04-25 06:38:42.000000 electrickiwi-api-0.8.2/src/electrickiwi_api/auth.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      483 2023-03-22 18:50:16.000000 electrickiwi-api-0.8.2/src/electrickiwi_api/exceptions.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    21334 2023-04-17 05:26:30.000000 electrickiwi-api-0.8.2/src/electrickiwi_api/model.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 06:42:18.109495 electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-25 06:42:18.000000 electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      439 2023-04-25 06:42:18.000000 electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-25 06:42:18.000000 electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       15 2023-04-25 06:42:18.000000 electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       17 2023-04-25 06:42:18.000000 electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/top_level.txt
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 06:42:18.109495 electrickiwi-api-0.8.2/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1382 2022-12-16 23:22:54.000000 electrickiwi-api-0.8.2/tests/test_instance.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:20:51.366998 electrickiwi-api-0.8.3/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35149 2022-10-20 08:35:26.000000 electrickiwi-api-0.8.3/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-25 09:20:51.366998 electrickiwi-api-0.8.3/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1678 2023-04-25 09:20:38.000000 electrickiwi-api-0.8.3/README.md
+-rw-rw-r--   0 michael   (1000) michael   (1000)      914 2023-04-25 09:20:38.000000 electrickiwi-api-0.8.3/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      177 2023-04-25 09:20:51.367998 electrickiwi-api-0.8.3/setup.cfg
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:20:51.361999 electrickiwi-api-0.8.3/src/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:20:51.365998 electrickiwi-api-0.8.3/src/electrickiwi_api/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      428 2023-04-25 09:20:38.000000 electrickiwi-api-0.8.3/src/electrickiwi_api/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9031 2023-04-17 05:33:03.000000 electrickiwi-api-0.8.3/src/electrickiwi_api/api.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1588 2023-04-25 08:16:42.000000 electrickiwi-api-0.8.3/src/electrickiwi_api/auth.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      483 2023-03-22 18:50:16.000000 electrickiwi-api-0.8.3/src/electrickiwi_api/exceptions.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    21334 2023-04-17 05:26:30.000000 electrickiwi-api-0.8.3/src/electrickiwi_api/model.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:20:51.366998 electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-25 09:20:51.000000 electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      439 2023-04-25 09:20:51.000000 electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-25 09:20:51.000000 electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       15 2023-04-25 09:20:51.000000 electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       17 2023-04-25 09:20:51.000000 electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/top_level.txt
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:20:51.366998 electrickiwi-api-0.8.3/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1382 2022-12-16 23:22:54.000000 electrickiwi-api-0.8.3/tests/test_instance.py
```

### Comparing `electrickiwi-api-0.8.2/LICENSE` & `electrickiwi-api-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.2/PKG-INFO` & `electrickiwi-api-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: electrickiwi-api
-Version: 0.8.2
+Version: 0.8.3
 Author-email: Michael Arthur <michael@jumblesoft.co.nz>
 License: GNU-3.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Electric Kiwi Python API
 
-[![SemVer 0.8.2][img_version]][url_version]
+[![SemVer 0.8.3][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
-[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.2&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.3&color=blue
 [url_version]: https://pypi.org/project/electrickiwi-api/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/electrickiwi-api/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/electrickiwi-api.svg
 [url_pyversions]: https://pypi.python.org/pypi/electrickiwi-api
```

### Comparing `electrickiwi-api-0.8.2/README.md` & `electrickiwi-api-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Electric Kiwi Python API
 
-[![SemVer 0.8.2][img_version]][url_version]
+[![SemVer 0.8.3][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
-[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.2&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.3&color=blue
 [url_version]: https://pypi.org/project/electrickiwi-api/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/electrickiwi-api/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/electrickiwi-api.svg
 [url_pyversions]: https://pypi.python.org/pypi/electrickiwi-api
```

### Comparing `electrickiwi-api-0.8.2/pyproject.toml` & `electrickiwi-api-0.8.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "electrickiwi-api"
-version     = "0.8.2"
+version     = "0.8.3"
 license     = {text = "GNU-3.0"}
 description = ""
 readme      = "README.md"
 authors     = [
     {name = "Michael Arthur", email = "michael@jumblesoft.co.nz"}
 ]
 
 
 requires-python = ">=3.9.0"
 dependencies    = [
     "aiohttp>=3.8.1"
     ]
 
 [tool.bumpver]
-current_version = "0.8.2"
+current_version = "0.8.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `electrickiwi-api-0.8.2/src/electrickiwi_api/api.py` & `electrickiwi-api-0.8.3/src/electrickiwi_api/api.py`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.2/src/electrickiwi_api/auth.py` & `electrickiwi-api-0.8.3/src/electrickiwi_api/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+"""abstract auth implementation for electric kiwi"""
+from __future__ import annotations
+
 import logging
 from abc import abstractmethod, ABC
+from typing import Any, Mapping, Optional
 
 from aiohttp import ClientSession, ClientResponse, ClientError
 
 from electrickiwi_api.exceptions import AuthException
 
 AUTHORIZATION_HEADER = "Authorization"
 
@@ -20,15 +24,15 @@
         self._websession = websession
         self._host = host if host is not None else API_BASE_URL
 
     @abstractmethod
     async def async_get_access_token(self) -> str:
         """Return a valid access token."""
 
-    async def request(self, method: str, url: str, **kwargs) -> ClientResponse:
+    async def request(self, method: str, url: str, **kwargs: Optional[Mapping[str, Any]]) -> ClientResponse:
         """Make a request."""
         try:
             access_token = await self.async_get_access_token()
         except ClientError as err:
             raise AuthException(f"Access token failure: {err}") from err
         headers = {AUTHORIZATION_HEADER: f"Bearer {access_token}"}
         if not (url.startswith("https://")):
```

### Comparing `electrickiwi-api-0.8.2/src/electrickiwi_api/model.py` & `electrickiwi-api-0.8.3/src/electrickiwi_api/model.py`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.2/src/electrickiwi_api.egg-info/PKG-INFO` & `electrickiwi-api-0.8.3/src/electrickiwi_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: electrickiwi-api
-Version: 0.8.2
+Version: 0.8.3
 Author-email: Michael Arthur <michael@jumblesoft.co.nz>
 License: GNU-3.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Electric Kiwi Python API
 
-[![SemVer 0.8.2][img_version]][url_version]
+[![SemVer 0.8.3][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
-[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.2&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.3&color=blue
 [url_version]: https://pypi.org/project/electrickiwi-api/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/electrickiwi-api/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/electrickiwi-api.svg
 [url_pyversions]: https://pypi.python.org/pypi/electrickiwi-api
```

### Comparing `electrickiwi-api-0.8.2/tests/test_instance.py` & `electrickiwi-api-0.8.3/tests/test_instance.py`

 * *Files identical despite different names*

