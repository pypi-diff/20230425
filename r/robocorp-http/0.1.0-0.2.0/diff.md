# Comparing `tmp/robocorp_http-0.1.0.tar.gz` & `tmp/robocorp_http-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_http-0.1.0.tar", max compression
+gzip compressed data, was "robocorp_http-0.2.0.tar", max compression
```

## Comparing `robocorp_http-0.1.0.tar` & `robocorp_http-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2023-04-04 11:49:45.062599 robocorp_http-0.1.0/README.md
--rw-r--r--   0        0        0      557 2023-04-04 11:49:45.063064 robocorp_http-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-04-04 11:49:45.063279 robocorp_http-0.1.0/src/robo/libs/http/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-04 11:49:45.063425 robocorp_http-0.1.0/src/robo/libs/http/_http.py
--rw-r--r--   0        0        0      598 2023-04-04 11:49:45.063536 robocorp_http-0.1.0/src/robo/libs/http/_types.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 robocorp_http-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-04-04 11:49:45.062599 robocorp_http-0.2.0/README.md
+-rw-r--r--   0        0        0      545 2023-04-25 10:41:01.008843 robocorp_http-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-25 10:39:03.647640 robocorp_http-0.2.0/src/robocorp/http/__init__.py
+-rw-r--r--   0        0        0     1339 2023-04-25 10:39:03.647870 robocorp_http-0.2.0/src/robocorp/http/_http.py
+-rw-r--r--   0        0        0      598 2023-04-25 10:39:03.647969 robocorp_http-0.2.0/src/robocorp/http/_types.py
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 robocorp_http-0.2.0/PKG-INFO
```

### Comparing `robocorp_http-0.1.0/pyproject.toml` & `robocorp_http-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp-http"
-version = "0.1.0"
+version = "0.2.0"
 description = "Robocorp HTTP automation library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
-packages = [{include = "robo", from="src"}]
+packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
-libs-devdeps = {path = "..", develop = true}
+libs-devdeps = {path = ".."}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_http-0.1.0/src/robo/libs/http/_http.py` & `robocorp_http-0.2.0/src/robocorp/http/_http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import requests
 from urllib.parse import urlparse
 
 from typing import Any, Optional
-from robo.libs.http._types import PathType
+from robocorp.http._types import PathType
 
 
 def _create_or_overwrite_target_file(
     path: PathType,
     response: Any,
     overwrite: bool,
 ) -> Path:
```

### Comparing `robocorp_http-0.1.0/src/robo/libs/http/_types.py` & `robocorp_http-0.2.0/src/robocorp/http/_types.py`

 * *Files identical despite different names*

