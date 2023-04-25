# Comparing `tmp/zcbot-predict-sdk-0.0.4.tar.gz` & `tmp/zcbot-predict-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-predict-sdk-0.0.4.tar", last modified: Tue Apr 25 00:50:31 2023, max compression
+gzip compressed data, was "dist\zcbot-predict-sdk-0.0.5.tar", last modified: Tue Apr 25 02:03:29 2023, max compression
```

## Comparing `zcbot-predict-sdk-0.0.4.tar` & `zcbot-predict-sdk-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 00:50:31.852610 zcbot-predict-sdk-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      384 2023-04-25 00:50:31.852610 zcbot-predict-sdk-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-25 00:50:31.853611 zcbot-predict-sdk-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-04-24 14:40:44.000000 zcbot-predict-sdk-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:50:31.829610 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/__init__.py
--rw-rw-rw-   0        0        0     7158 2023-04-23 02:14:35.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:50:31.841610 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/decator.py
--rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/exceptions.py
--rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/keys.py
--rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/thread_pool.py
--rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:50:31.845610 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/model/
--rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/model/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/model/callback.py
--rw-rw-rw-   0        0        0      205 2023-04-24 14:12:16.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/model/param.py
--rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/monitor.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:50:31.850610 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/service/
--rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/service/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/service/base.py
--rw-rw-rw-   0        0        0      563 2023-04-24 14:12:11.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/service/info_extract.py
--rw-rw-rw-   0        0        0     4396 2023-04-24 14:39:56.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/service/sku_tag.py
-drwxrwxrwx   0        0        0        0 2023-04-25 00:50:31.834611 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/
--rw-rw-rw-   0        0        0      384 2023-04-25 00:50:31.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-04-25 00:50:31.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 00:50:31.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 00:50:31.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 00:50:31.000000 zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.256355 zcbot-predict-sdk-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      384 2023-04-25 02:03:29.255357 zcbot-predict-sdk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-25 02:03:29.256355 zcbot-predict-sdk-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-04-25 02:03:28.000000 zcbot-predict-sdk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.233356 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/__init__.py
+-rw-rw-rw-   0        0        0     7158 2023-04-23 02:14:35.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.245356 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/decator.py
+-rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/exceptions.py
+-rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/keys.py
+-rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/thread_pool.py
+-rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.248355 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/
+-rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/callback.py
+-rw-rw-rw-   0        0        0      205 2023-04-24 14:12:16.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/param.py
+-rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.253357 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/
+-rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/base.py
+-rw-rw-rw-   0        0        0      751 2023-04-25 01:27:05.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/info_extract.py
+-rw-rw-rw-   0        0        0     4741 2023-04-25 02:02:41.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/sku_tag.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.238357 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-predict-sdk-0.0.4/setup.py` & `zcbot-predict-sdk-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-predict-sdk',
-      version='0.0.4',
+      version='0.0.5',
       description='zcbot predict sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['celery', 'redis'],
       python_requires='>=3.7',
```

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/client.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/client.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/exceptions.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/thread_pool.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/common/utils.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/model/callback.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/callback.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/monitor.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk/service/sku_tag.py` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/sku_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 from typing import Dict, List, Union
 
 from .base import BaseService
 from ..model.callback import Callback
 from ..model.param import TextParam
 
 
-def _params_convert(task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]]):
+def _params_convert(task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]]):
     text_list = list()
-    # 单个
-    if isinstance(task_params, Dict):
+    # 批量
+    if isinstance(task_params, List):
+        for task_param in task_params:
+            if isinstance(task_param, TextParam):
+                text_list.append(task_param.dict())
+            elif isinstance(task_params, str):
+                text_list.append({'text': task_params})
+            else:
+                text_list.append(task_param)
+    else:
+        # 单个
         if isinstance(task_params, TextParam):
             text_list.append(task_params.dict())
+        elif isinstance(task_params, str):
+            text_list.append({'text': task_params})
         else:
             text_list.append(task_params)
-    # 批量
-    for task_param in task_params:
-        if isinstance(task_param, TextParam):
-            text_list.append(task_param.dict())
-        else:
-            text_list.append(task_param)
 
     return text_list
 
 
 class StaplesSkuTagService(BaseService):
 
-    def predict_catalog1(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog1(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.catalog1', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_catalog4(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog4(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.catalog4', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_catalog6(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog6(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.catalog6', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_brand(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_brand(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.staples.brand', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
 
 class JslinkSkuTagService(BaseService):
 
-    def predict_catalog1(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog1(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.catalog1', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_catalog4(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog4(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.catalog4', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_brand(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_brand(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.jslink.brand', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
 
 class ZjmiSkuTagService(BaseService):
 
-    def predict_catalog1(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog1(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.zjmi.catalog1', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_catalog3(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+    def predict_catalog3(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
         return self.celery_client.apply(task_name='sku_tag.zjmi.catalog3', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
 
-    def predict_brand(self, task_params: Union[Dict, TextParam, List[Union[TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
-        return self.celery_client.apply(task_name='sku_tag.jslink.brand', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
+    def predict_brand(self, task_params: Union[str, Dict, TextParam, List[Union[str, TextParam, Dict]]] = None, threshold: float = 0.7, callback: Callback = None, **kwargs):
+        return self.celery_client.apply(task_name='sku_tag.zjmi.brand', task_params={'text_list': _params_convert(task_params), 'threshold': threshold}, callback=callback, **kwargs)
```

### Comparing `zcbot-predict-sdk-0.0.4/zcbot_predict_sdk.egg-info/SOURCES.txt` & `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

