# Comparing `tmp/flexypy-0.0.7.tar.gz` & `tmp/flexypy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.0.7.tar", last modified: Sun Apr 23 10:16:07 2023, max compression
+gzip compressed data, was "flexypy-0.0.8.tar", last modified: Mon Apr 24 10:23:56 2023, max compression
```

## Comparing `flexypy-0.0.7.tar` & `flexypy-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.284161 flexypy-0.0.7/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-23 10:16:07.284161 flexypy-0.0.7/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.096160 flexypy-0.0.7/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.7/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.7/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.184160 flexypy-0.0.7/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.7/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.7/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.7/flexypy/exceptions/extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.7/flexypy/exceptions/render.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.7/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.7/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.188160 flexypy-0.0.7/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.7/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.7/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.7/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.208160 flexypy-0.0.7/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.7/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.7/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.220161 flexypy-0.0.7/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.7/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.220161 flexypy-0.0.7/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.7/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.0.7/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.7/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.0.7/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.244161 flexypy-0.0.7/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.7/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.0.7/flexypy/http/cookie.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2431 2023-04-23 10:12:45.000000 flexypy-0.0.7/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2635 2023-04-17 09:53:46.000000 flexypy-0.0.7/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     9611 2023-04-22 20:34:05.000000 flexypy-0.0.7/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.248161 flexypy-0.0.7/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.7/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.264161 flexypy-0.0.7/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.7/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.7/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.7/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.7/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.272161 flexypy-0.0.7/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.7/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.7/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-23 10:16:07.132160 flexypy-0.0.7/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-23 10:16:07.000000 flexypy-0.0.7/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-04-23 10:15:55.000000 flexypy-0.0.7/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-23 10:16:07.284161 flexypy-0.0.7/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-24 10:23:56.328381 flexypy-0.0.8/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.324381 flexypy-0.0.8/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.8/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.8/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.324381 flexypy-0.0.8/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.8/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.8/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.8/flexypy/exceptions/extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.8/flexypy/exceptions/render.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.8/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.8/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.8/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.8/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.8/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.8/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.8/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.8/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.8/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.0.8/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.8/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.0.8/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.8/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.0.8/flexypy/http/cookie.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2431 2023-04-23 10:12:45.000000 flexypy-0.0.8/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2682 2023-04-24 10:03:31.000000 flexypy-0.0.8/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     9797 2023-04-24 10:05:14.000000 flexypy-0.0.8/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.8/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.8/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.8/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.8/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.8/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.328381 flexypy-0.0.8/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.8/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.8/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-24 10:23:56.324381 flexypy-0.0.8/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-24 10:23:56.000000 flexypy-0.0.8/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-04-24 10:23:56.000000 flexypy-0.0.8/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-24 10:23:56.000000 flexypy-0.0.8/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-04-24 10:23:56.000000 flexypy-0.0.8/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-24 10:23:56.000000 flexypy-0.0.8/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-04-24 10:23:47.000000 flexypy-0.0.8/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-24 10:23:56.328381 flexypy-0.0.8/setup.cfg
```

### Comparing `flexypy-0.0.7/flexypy/exceptions/web/server.py` & `flexypy-0.0.8/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy/generate_templates/generator.py` & `flexypy-0.0.8/flexypy/generate_templates/generator.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy/http/cookie.py` & `flexypy-0.0.8/flexypy/http/cookie.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy/http/request.py` & `flexypy-0.0.8/flexypy/http/request.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy/http/routing.py` & `flexypy-0.0.8/flexypy/http/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 
 @dataclass
 class SlugData:
     count: int
     params: dict
 
 
+@dataclass
+class Redirect:
+    path: str
+
+
 class Route:
     def __init__(self, path, template_path):
         self.path = path
         self.template_path = template_path
         self.method = ''
         self.get_func = None
         self.post_func = None
@@ -86,10 +91,10 @@
         else:
             return path
 
     def post(self):
         pass
 
 
-def redirect(path):
-    return path
+# def redirect(path):
+#     return path
```

### Comparing `flexypy-0.0.7/flexypy/http/server.py` & `flexypy-0.0.8/flexypy/http/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from flexypy.http.request import Request
 from dataclasses import dataclass
 import mimetypes
 from config.apps import PATH_TO_FXP_APPS
 from config.dirs import MDDL_LIST_PATH
 import importlib
 from wsgiref import util
-from flexypy.http.routing import UserRoute
+from flexypy.http.routing import UserRoute, Redirect
 from typing import Type
 import os
 from flexypy.exceptions.web.server import PathNotFound
 from urllib import parse
 from cgi import FieldStorage
 from flexypy.middlewares.mddl import Middleware
 import re
@@ -33,15 +33,15 @@
     current_app_path = ''
 
     def __init__(self, environ: dict, start_response):
         self.environ = environ
         self.start_response = start_response
         self.root_url = util.shift_path_info(self.environ)
         self.full_url = self.root_url + util.request_uri(self.environ).replace(util.application_uri(self.environ), '')
-        self.server_address = util.application_uri(self.environ).replace(self.root_url, '')
+        self.server_address = util.application_uri(self.environ).replace('/' + self.root_url, '') + '/'
         self.render: RenderTemplate = RenderTemplate()
         self.routes: list[Type[UserRoute]] = []
         self.router = None
         self.request = Request
         self._get_fxp_apps()
         self.router = Router(self.environ, self.routes, self.full_url)
         self._set_server_cookie()
@@ -100,20 +100,24 @@
                         if mddl_redirect.from_path and mddl_redirect.to_path:
                             if self.full_url == mddl_redirect.from_path:
                                 return self.render.render_redirect(mddl_redirect.to_path)
 
                     return self._method_post(mddl_app)
 
     def _method_get(self, app: UserRoute) -> HtmlResponse:
-        mime_type = mimetypes.guess_type(app.template_path)[0]
-        resp = self.render.render_html('200 OK', [('Content-type', mime_type)], app.get())
-        return resp
+        get_data = app.get()
+        if isinstance(get_data, Redirect):
+            return self.render.render_redirect(get_data.path)
+        else:
+            mime_type = mimetypes.guess_type(app.template_path)[0]
+            resp = self.render.render_html('200 OK', [('Content-type', mime_type)], get_data)
+            return resp
 
     def _method_post(self, app: UserRoute):
-        resp = self.render.render_redirect(app.post())
+        resp = self.render.render_redirect(app.post().path)
         return resp
 
     def _method_get_static_files(self, filepath) -> HtmlResponse:
         # get static filepath
         if 'HTTP_REFERER' in self.environ:
             current_url: str = self.environ['HTTP_REFERER'].replace(self.server_address, '')
             if current_url.endswith('/'):
```

### Comparing `flexypy-0.0.7/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.0.8/flexypy/http/template/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy/http/template/extensions/template_ext.py` & `flexypy-0.0.8/flexypy/http/template/extensions/template_ext.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy/http/template/render.py` & `flexypy-0.0.8/flexypy/http/template/render.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.7/flexypy.egg-info/SOURCES.txt` & `flexypy-0.0.8/flexypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

