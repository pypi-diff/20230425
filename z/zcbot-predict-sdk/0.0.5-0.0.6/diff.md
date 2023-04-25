# Comparing `tmp/zcbot-predict-sdk-0.0.5.tar.gz` & `tmp/zcbot-predict-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-predict-sdk-0.0.5.tar", last modified: Tue Apr 25 02:03:29 2023, max compression
+gzip compressed data, was "dist\zcbot-predict-sdk-0.0.6.tar", last modified: Tue Apr 25 02:54:34 2023, max compression
```

## Comparing `zcbot-predict-sdk-0.0.5.tar` & `zcbot-predict-sdk-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.256355 zcbot-predict-sdk-0.0.5/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      384 2023-04-25 02:03:29.255357 zcbot-predict-sdk-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-25 02:03:29.256355 zcbot-predict-sdk-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-04-25 02:03:28.000000 zcbot-predict-sdk-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.233356 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/__init__.py
--rw-rw-rw-   0        0        0     7158 2023-04-23 02:14:35.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.245356 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/decator.py
--rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/exceptions.py
--rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/keys.py
--rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/thread_pool.py
--rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.248355 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/
--rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/callback.py
--rw-rw-rw-   0        0        0      205 2023-04-24 14:12:16.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/param.py
--rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/monitor.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.253357 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/
--rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-27 05:56:52.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/base.py
--rw-rw-rw-   0        0        0      751 2023-04-25 01:27:05.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/info_extract.py
--rw-rw-rw-   0        0        0     4741 2023-04-25 02:02:41.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/sku_tag.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:03:29.238357 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/
--rw-rw-rw-   0        0        0      384 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 02:03:29.000000 zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 02:54:34.266538 zcbot-predict-sdk-0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      384 2023-04-25 02:54:34.265539 zcbot-predict-sdk-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-25 02:54:34.266538 zcbot-predict-sdk-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-04-25 02:54:10.000000 zcbot-predict-sdk-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:54:34.239539 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/__init__.py
+-rw-rw-rw-   0        0        0     7165 2023-04-25 02:51:14.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:54:34.254538 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/decator.py
+-rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/exceptions.py
+-rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/keys.py
+-rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/thread_pool.py
+-rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:54:34.258539 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/model/
+-rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/model/callback.py
+-rw-rw-rw-   0        0        0      205 2023-04-24 14:12:16.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/model/param.py
+-rw-rw-rw-   0        0        0     3668 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:54:34.263544 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/
+-rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-04-25 02:51:14.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/base.py
+-rw-rw-rw-   0        0        0      751 2023-04-25 01:27:05.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/info_extract.py
+-rw-rw-rw-   0        0        0     4741 2023-04-25 02:02:41.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/sku_tag.py
+drwxrwxrwx   0        0        0        0 2023-04-25 02:54:34.246538 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-04-25 02:54:34.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2023-04-25 02:54:34.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 02:54:34.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 02:54:34.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 02:54:34.000000 zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-predict-sdk-0.0.5/setup.py` & `zcbot-predict-sdk-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-predict-sdk',
-      version='0.0.5',
+      version='0.0.6',
       description='zcbot predict sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['celery', 'redis'],
       python_requires='>=3.7',
```

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/client.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from .common.keys import get_result_key
 from .model.callback import Callback
 
 LOGGER = get_task_logger(__name__)
 
 
 # @singleton
-class CeleryClient(object):
+class PredictClient(object):
     """
     Celery服务客户端
-    注意：此类不建议手动初始化，可通过CeleryClientHolder初始化，方便各service类自动获取
+    注意：此类不建议手动初始化，可通过PredictClientHolder初始化，方便各service类自动获取
     """
     def __init__(self, celery_broker_url: str, celery_result_backend: str, client_redis_uri: str, app_code: str):
         self.broker_url = celery_broker_url
         self.backend_uri = celery_result_backend
         self.client_redis_uri = client_redis_uri
         self.app_code = app_code
         self.default_expire_seconds = 12 * 3600
@@ -143,19 +143,19 @@
             callback.callback_func = callback_func
         else:
             callback.callback_func = obj_to_ref(callback_func)
 
         return callback
 
 
-class CeleryClientHolder(object):
+class PredictClientHolder(object):
     __default_instance = None
 
     @staticmethod
     def init_default_instance(celery_broker_url: str, celery_result_backend: str, client_redis_uri: str, app_code: str):
-        CeleryClientHolder.__default_instance = CeleryClient(celery_broker_url, celery_result_backend, client_redis_uri, app_code)
+        PredictClientHolder.__default_instance = PredictClient(celery_broker_url, celery_result_backend, client_redis_uri, app_code)
 
     @staticmethod
     def get_default_instance():
-        if not CeleryClientHolder.__default_instance:
+        if not PredictClientHolder.__default_instance:
             raise BizException(f'默认实例尚未初始化，请先初始化实例！')
-        return CeleryClientHolder.__default_instance
+        return PredictClientHolder.__default_instance
```

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/exceptions.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/thread_pool.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/common/utils.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/model/callback.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/model/callback.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/monitor.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/info_extract.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/info_extract.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk/service/sku_tag.py` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk/service/sku_tag.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.5/zcbot_predict_sdk.egg-info/SOURCES.txt` & `zcbot-predict-sdk-0.0.6/zcbot_predict_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

