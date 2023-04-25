# Comparing `tmp/zcbot-predict-sdk-0.0.7.tar.gz` & `tmp/zcbot-predict-sdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-predict-sdk-0.0.7.tar", last modified: Tue Apr 25 02:57:39 2023, max compression
+gzip compressed data, was "dist\zcbot-predict-sdk-0.0.8.tar", last modified: Tue Apr 25 03:39:29 2023, max compression
```

## Comparing `zcbot-predict-sdk-0.0.7.tar` & `zcbot-predict-sdk-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 02:57:39.166458 zcbot-predict-sdk-0.0.7/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      384 2023-04-25 02:57:39.165459 zcbot-predict-sdk-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-25 02:57:39.166458 zcbot-predict-sdk-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      601 2023-04-25 02:57:35.000000 zcbot-predict-sdk-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:57:39.137457 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/__init__.py
--rw-rw-rw-   0        0        0     7165 2023-04-25 02:51:14.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:57:39.152458 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/decator.py
--rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/exceptions.py
--rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/keys.py
--rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/thread_pool.py
--rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:57:39.157458 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/model/
--rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/model/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/model/callback.py
--rw-rw-rw-   0        0        0      205 2023-04-24 14:12:16.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/model/param.py
--rw-rw-rw-   0        0        0     3670 2023-04-25 02:57:17.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/monitor.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:57:39.163459 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/
--rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/__init__.py
--rw-rw-rw-   0        0        0      279 2023-04-25 02:51:14.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/base.py
--rw-rw-rw-   0        0        0      751 2023-04-25 01:27:05.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/info_extract.py
--rw-rw-rw-   0        0        0     4741 2023-04-25 02:02:41.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/sku_tag.py
-drwxrwxrwx   0        0        0        0 2023-04-25 02:57:39.143457 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/
--rw-rw-rw-   0        0        0      384 2023-04-25 02:57:38.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-04-25 02:57:39.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 02:57:38.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-25 02:57:38.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 02:57:38.000000 zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 03:39:29.293308 zcbot-predict-sdk-0.0.8/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-predict-sdk-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      384 2023-04-25 03:39:29.292308 zcbot-predict-sdk-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2023-04-18 08:45:42.000000 zcbot-predict-sdk-0.0.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:39:29.293308 zcbot-predict-sdk-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-04-25 03:37:24.000000 zcbot-predict-sdk-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:39:29.263309 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/__init__.py
+-rw-rw-rw-   0        0        0     7165 2023-04-25 02:51:14.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:39:29.277309 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/decator.py
+-rw-rw-rw-   0        0        0      705 2022-08-22 07:41:36.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/exceptions.py
+-rw-rw-rw-   0        0        0      365 2023-03-22 09:17:48.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/keys.py
+-rw-rw-rw-   0        0        0     2132 2023-03-15 06:40:08.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/thread_pool.py
+-rw-rw-rw-   0        0        0     3363 2023-03-28 08:30:17.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:39:29.284308 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/model/
+-rw-rw-rw-   0        0        0        0 2023-03-23 08:28:20.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-03-28 11:46:06.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/model/callback.py
+-rw-rw-rw-   0        0        0      283 2023-04-25 03:07:12.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/model/param.py
+-rw-rw-rw-   0        0        0     2938 2023-04-25 03:30:26.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/model/response.py
+-rw-rw-rw-   0        0        0     3670 2023-04-25 02:57:17.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/monitor.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:39:29.290309 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/
+-rw-rw-rw-   0        0        0        0 2023-03-14 05:49:28.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-04-25 02:51:14.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/base.py
+-rw-rw-rw-   0        0        0      751 2023-04-25 01:27:05.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/info_extract.py
+-rw-rw-rw-   0        0        0     4741 2023-04-25 02:02:41.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/sku_tag.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:39:29.269309 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-04-25 03:39:29.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2023-04-25 03:39:29.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:39:29.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 03:39:29.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-25 03:39:29.000000 zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-predict-sdk-0.0.7/setup.py` & `zcbot-predict-sdk-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-predict-sdk',
-      version='0.0.7',
+      version='0.0.8',
       description='zcbot predict sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['celery', 'redis'],
       python_requires='>=3.7',
```

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/client.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/client.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/exceptions.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/thread_pool.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/common/utils.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/common/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/model/callback.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/model/callback.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/monitor.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/info_extract.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/info_extract.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk/service/sku_tag.py` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk/service/sku_tag.py`

 * *Files identical despite different names*

### Comparing `zcbot-predict-sdk-0.0.7/zcbot_predict_sdk.egg-info/SOURCES.txt` & `zcbot-predict-sdk-0.0.8/zcbot_predict_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 zcbot_predict_sdk/common/exceptions.py
 zcbot_predict_sdk/common/keys.py
 zcbot_predict_sdk/common/thread_pool.py
 zcbot_predict_sdk/common/utils.py
 zcbot_predict_sdk/model/__init__.py
 zcbot_predict_sdk/model/callback.py
 zcbot_predict_sdk/model/param.py
+zcbot_predict_sdk/model/response.py
 zcbot_predict_sdk/service/__init__.py
 zcbot_predict_sdk/service/base.py
 zcbot_predict_sdk/service/info_extract.py
 zcbot_predict_sdk/service/sku_tag.py
```

