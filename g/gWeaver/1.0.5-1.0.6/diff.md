# Comparing `tmp/gWeaver-1.0.5.tar.gz` & `tmp/gWeaver-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gWeaver-1.0.5.tar", last modified: Mon Apr 24 06:52:09 2023, max compression
+gzip compressed data, was "gWeaver-1.0.6.tar", last modified: Tue Apr 25 12:39:42 2023, max compression
```

## Comparing `gWeaver-1.0.5.tar` & `gWeaver-1.0.6.tar`

### file list

```diff
@@ -1,40 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 06:51:38.000000 gWeaver-1.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 06:52:09.970904 gWeaver-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 06:51:38.000000 gWeaver-1.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/graph_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/graph_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/graph_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/node_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/base/response_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/gWeaver/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/commands/_private.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/management/commands/graph_migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/gWeaver/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/managers/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.970904 gWeaver-1.0.5/gWeaver/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:51:38.000000 gWeaver-1.0.5/gWeaver/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:52:09.966904 gWeaver-1.0.5/gWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 06:52:09.000000 gWeaver-1.0.5/gWeaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 06:52:09.970904 gWeaver-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-24 06:51:38.000000 gWeaver-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 12:38:52.000000 gWeaver-1.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-25 12:39:42.820058 gWeaver-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-25 12:38:52.000000 gWeaver-1.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.816058 gWeaver-1.0.6/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.816058 gWeaver-1.0.6/example/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-25 12:38:52.000000 gWeaver-1.0.6/example/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.816058 gWeaver-1.0.6/gWeaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/gWeaver/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/graph_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/graph_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/graph_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/node_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/response_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/base/schema_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/gWeaver/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/gWeaver/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/management/commands/_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/management/commands/graph_migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/gWeaver/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/managers/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/gWeaver/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 12:38:52.000000 gWeaver-1.0.6/gWeaver/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.816058 gWeaver-1.0.6/gWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-25 12:39:42.000000 gWeaver-1.0.6/gWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-25 12:39:42.000000 gWeaver-1.0.6/gWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:39:42.000000 gWeaver-1.0.6/gWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:39:41.000000 gWeaver-1.0.6/gWeaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-25 12:39:42.000000 gWeaver-1.0.6/gWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 12:39:42.000000 gWeaver-1.0.6/gWeaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:39:42.820058 gWeaver-1.0.6/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 12:38:52.000000 gWeaver-1.0.6/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-25 12:38:52.000000 gWeaver-1.0.6/graph/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-25 12:38:52.000000 gWeaver-1.0.6/graph/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-25 12:38:52.000000 gWeaver-1.0.6/graph/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-25 12:38:52.000000 gWeaver-1.0.6/graph/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 12:39:42.820058 gWeaver-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-25 12:38:52.000000 gWeaver-1.0.6/setup.py
```

### Comparing `gWeaver-1.0.5/LICENSE.txt` & `gWeaver-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.5/PKG-INFO` & `gWeaver-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.5
+Version: 1.0.6
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.5/gWeaver/base/graph_actions.py` & `gWeaver-1.0.6/gWeaver/base/graph_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 from .node_connector import graph_engine
 from .response_constructor import response
 from django.core.exceptions import ValidationError
 import time
 import asyncio
 
-
+class graph_actions2:
+    def __init__(self) -> None:
+        pass
 class graph_actions:
 
             
-    def __init__(self,request,actions) -> None:
+    def __init__(self,actions) -> None:
+
+        print("actions = ", actions,type(actions))
 
         self.dqquery = actions.dqquery
-        self.entity = actions.entity
-        self.addons = actions.addons
-        self.function_args = actions.function_args
-        self.request = request
-        self.res = response(request)
+        self.entity = actions.model.dgraph_type
+        self.addons = actions.add_functions
+        self.model = actions.model
+        
         self.serializer = actions.serializer
-        self.fields = actions.fields
-        self.primary_key = actions.primary_key
-        self.pk_field = actions.pk_field
+        self.fields = actions.model
+        self.primary_key = actions.model.primary_key
+        self.async_execution = False
         
     
-    def get(self,pk=None):
+    def get(self,request,pk=None):
         processed_data = {}
-        if not pk:
-            raise ValidationError("pk is required")
+        self.request = request
+        self.res = response(request)
         result = self.dqquery.all(pk).get(self.entity)
         len_data = len(result)
         if len_data == 0:
             return self.res.out(["ok", [], "no data"])
-        for processed_data in result:
-            self.function_args.update(
-                {"processed_data": processed_data})
-            if self.addons:
-                processed_data = self.plugin_func(self.addons,
-                                                  method="GET", processed_data=processed_data)
-        if processed_data:
-            return self.res.paginated(["ok", result, "success"])
         else:
-            return self.res.out(["error", [], "error"])
+            return self.res.out(["ok", result, "success"])
+        # for processed_data in result:
+        #     self.function_args.update(
+        #         {"processed_data": processed_data})
+        #     if self.addons:
+        #         processed_data = self.plugin_func(self.addons,
+        #                                           method="GET", processed_data=processed_data)
+        # if processed_data:
+        #     return self.res.paginated(["ok", result, "success"])
+        # else:
+        #     return self.res.out(["error", [], "error"])
 
-    def ser_check(self):
-        print("request data = ", self.request.data)
+    def ser_check(self,request):
+        print("request data = ", request.data)
         ser = self.serializer(
-            data=self.request.data,
-            context={'request': self.request}
+            data=request.data,
+            context={'request': request}
         )
         if ser.is_valid():
-            processed = graph_engine(ser.validated_data,
-                                     self.fields(self.entity)(), self.primary_key)
+            self.primary_key =None
+            print("&&&&&&&&&&7", ser.validated_data)
+            processed = graph_engine(dict(ser.validated_data),
+                                     self.model, self.primary_key)
             data = processed.connect()
             return True, data, ser.validated_data
         else:
             return False, ser.errors, []
 
     async def process_data(self, function, **kwargs):
         return function(**kwargs)
@@ -91,55 +98,59 @@
         for key, value in ser_data.items():
             if isinstance(value, list):
                 try:
                     getattr(self.dqquery,"delete_"+key)(self.primary_key, value)
                 except:
                     pass
 
-    def create(self, **kwargs):
+    def create(self,*args, **kwargs):
         processed_data = kwargs["processed_data"]
         print("proicessed_data = ", processed_data)
         ser_data = kwargs["ser_data"]
 
-        processed_data.update({self.entity+".created_on": time.time()})
-
-        uid = self.dqquery.create(processed_data)
+        uid = self.dqquery().create(processed_data)
         processed_data["id"] = uid
-        self.function_args.update({"processed_data": processed_data,
-                                   "ser_data": ser_data})
+        # self.function_args.update({"processed_data": processed_data,
+        #                            "ser_data": ser_data})
         if self.addons:
             processed_data = self.plugin_func(self.addons,
                                               method="POST", processed_data=processed_data)
 
-    def put(self):
-        status, processed_data, ser_data = self.ser_check()
+    def put(self,request):
+        status, processed_data, ser_data = self.ser_check(request)
         if status:
             try:
                 self.execute_async(
                     self.modify, processed_data=processed_data, ser_data=ser_data)
                 return self.res.out(["ok", [], "modified"])
             except:
                 return self.res.out(["error", processed_data, "error"])
         else:
             return self.res.out(["error", processed_data, "error"])
 
-    def post(self):
-        status, processed_data, ser_data = self.ser_check()
+    def post(self,request):
+        status, processed_data, ser_data = self.ser_check(request)
+        res = response(request)
         print("status, processed data, ser data = ", status, processed_data, ser_data)
         if status:
-            try:
-                self.execute_async(
-                    self.create, processed_data=processed_data, ser_data=ser_data)
-                return self.res.out(["ok", [], "added"])
-            except:
-                return self.res.out(["error", processed_data, "error"])
+            print(processed_data, ser_data)
+            if self.async_execution:
+                try:
+                    self.execute_async(
+                        self.create, processed_data=processed_data, ser_data=ser_data)
+                    return res.out(["ok", [], "added"])
+                except:
+                    return res.out(["error", processed_data, "error"])
+            else:
+                self.create(processed_data=processed_data, ser_data=ser_data)
+                return res.out(["ok", [], "added"])
         else:
-            return self.res.out(["error", processed_data, "error"])
+            return res.out(["error", processed_data, "error"])
 
-    def delete(self):
+    def delete(self,request):
         item = self.request.query_params.get(self.pk_field)
         if not item:
             item = self.request.data.get(self.pk_field)
         if type(item) != list:
             item = [item]
 
         try:
```

### Comparing `gWeaver-1.0.5/gWeaver/base/node_connector.py` & `gWeaver-1.0.6/gWeaver/base/node_connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 
 
 class graph_engine:
-    def __init__(self, data, fields, pk):
+    def __init__(self, data, model, pk):
         self.data = data
         self.primary_key = pk
-        self.predicates, self.edges, self.reverse_edge, self.dgraph_type, self.reverse_graph_type = fields
+        self.model = model
+        self.predicates = model.predicates
+        self.edges = model.edges
+        self.reverse_edge = model.reverse_edge
+        self.dgraph_type = model.dgraph_type
+        self.reverse_graph_type = model.reverse_graph_type
+        
         self.result = {}
         self.c_count = 0
 
     def connect_predicates(self):
         sub = {}
+        print("predicates = ", self.predicates, self.data)
         for p in self.predicates:
             if p in self.data:
                 self.c_count += 1
                 sub.update(
                     {self.dgraph_type+"."+p: self.data.get(p)})
         if self.primary_key:
             sub.update({"uid": self.primary_key})
```

### Comparing `gWeaver-1.0.5/gWeaver/base/response_constructor.py` & `gWeaver-1.0.6/gWeaver/base/response_constructor.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.5/gWeaver/management/commands/graph_migrate.py` & `gWeaver-1.0.6/gWeaver/management/commands/graph_migrate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from django.core.management.base import CommandError, BaseCommand
 from django.apps import apps
-from ...base.graph_models import SchemaGenerator
+from ...base.schema_generator import SchemaGenerator
 
 class Command(BaseCommand):
     help = 'Generate a Dgraph schema based on the models in your project.'
 
     def handle(self, *args, **options):
         # Get all models from all apps
         models = apps.get_models()
 
         # Filter models that have a `dgraph_type` attribute
         graph_models = [model for model in models if hasattr(model, 'dgraph_type')]
 
         # Generate the schema
         schema_generator = SchemaGenerator(graph_models)
-        schema = schema_generator.generate_schema()
+        
+        schema = schema_generator.generate_dgraph_schema()
+        print(schema)
+        schema_generator.post_to_dgraph()
         # write schema to a file 
         with open('schema.txt', 'w') as f:
             f.write(schema)
         self.stdout.write(
                 self.style.SUCCESS('Successfully created schema for Dgraph.')
         )
```

### Comparing `gWeaver-1.0.5/gWeaver/managers/client.py` & `gWeaver-1.0.6/gWeaver/managers/client.py`

 * *Files identical despite different names*

### Comparing `gWeaver-1.0.5/gWeaver.egg-info/PKG-INFO` & `gWeaver-1.0.6/gWeaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gWeaver
-Version: 1.0.5
+Version: 1.0.6
 Summary: dgraph operation module for Django REST Framework
 Home-page: https://github.com/iamr2k/gWeaver
 Author: Rahul Babu K
 Author-email: rahulbabu101@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `gWeaver-1.0.5/setup.py` & `gWeaver-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     + extras_require["doc"]
     + extras_require["python-jose"]
 )
 
 
 setup(
     name="gWeaver",
-    version = "1.0.5",
+    version = "1.0.6",
     url="https://github.com/iamr2k/gWeaver",
     license="MIT",
     description="dgraph operation module for Django REST Framework",
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     author="Rahul Babu K",
     author_email="rahulbabu101@gmail.com",
     install_requires=[
```

