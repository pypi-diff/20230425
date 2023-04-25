# Comparing `tmp/obsutil-1.0.4.tar.gz` & `tmp/obsutil-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsutil-1.0.4.tar", last modified: Tue Apr 11 03:11:45 2023, max compression
+gzip compressed data, was "obsutil-1.0.5.tar", last modified: Tue Apr 25 08:15:16 2023, max compression
```

## Comparing `obsutil-1.0.4.tar` & `obsutil-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 03:11:45.487135 obsutil-1.0.4/
--rw-r--r--   0 chen       (501) staff       (20)      120 2023-04-11 03:11:45.486994 obsutil-1.0.4/PKG-INFO
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 03:11:45.485711 obsutil-1.0.4/obsutil/
--rw-r--r--   0 chen       (501) staff       (20)      181 2023-02-07 00:50:51.000000 obsutil-1.0.4/obsutil/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     4039 2023-03-17 07:13:18.000000 obsutil-1.0.4/obsutil/file.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-11 03:11:45.486771 obsutil-1.0.4/obsutil.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      120 2023-04-11 03:11:45.000000 obsutil-1.0.4/obsutil.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      198 2023-04-11 03:11:45.000000 obsutil-1.0.4/obsutil.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-11 03:11:45.000000 obsutil-1.0.4/obsutil.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       16 2023-04-11 03:11:45.000000 obsutil-1.0.4/obsutil.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)        8 2023-04-11 03:11:45.000000 obsutil-1.0.4/obsutil.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-11 03:11:45.487179 obsutil-1.0.4/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      723 2023-03-01 02:59:07.000000 obsutil-1.0.4/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 08:15:16.436035 obsutil-1.0.5/
+-rw-r--r--   0 chen       (501) staff       (20)      120 2023-04-25 08:15:16.435824 obsutil-1.0.5/PKG-INFO
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 08:15:16.434937 obsutil-1.0.5/obsutil/
+-rw-r--r--   0 chen       (501) staff       (20)      190 2023-04-25 08:15:00.000000 obsutil-1.0.5/obsutil/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     4473 2023-04-25 08:15:00.000000 obsutil-1.0.5/obsutil/file.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 08:15:16.435632 obsutil-1.0.5/obsutil.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      120 2023-04-25 08:15:16.000000 obsutil-1.0.5/obsutil.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      198 2023-04-25 08:15:16.000000 obsutil-1.0.5/obsutil.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-25 08:15:16.000000 obsutil-1.0.5/obsutil.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       16 2023-04-25 08:15:16.000000 obsutil-1.0.5/obsutil.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)        8 2023-04-25 08:15:16.000000 obsutil-1.0.5/obsutil.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-25 08:15:16.436087 obsutil-1.0.5/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      686 2023-04-25 08:15:00.000000 obsutil-1.0.5/setup.py
```

### Comparing `obsutil-1.0.4/obsutil/file.py` & `obsutil-1.0.5/obsutil/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,50 @@
+import logging
 import os
 import time
 from obs import ObsClient
 from urllib.parse import urlparse
 
-AK = os.environ.get('HW_OBS_AK')
-SK = os.environ.get('HW_OBS_SK')
-server = os.environ.get('HW_OBS_SERVER')
+_AK = os.environ.get('HW_OBS_AK')
+_SK = os.environ.get('HW_OBS_SK')
+_server = os.environ.get('HW_OBS_SERVER')
 
 _obsClient = None
 _last_time = None
 
+logger = logging.getLogger(__name__)
+
+
+def init(ak, sk, server):
+    global _AK, _SK, _server
+    _AK = ak
+    _SK = sk
+    _server = server
 
 # 检查字符串是否为合法的obs路径
 # obs路径格式为：obs://bucketname/objectname
 def _is_obs_path(path):
     if path.startswith('obs://'):
         return True
     else:
         return False
 
 
 def copy(src, dest):
     global _obsClient
     if _obsClient is None:
-        _obsClient = ObsClient(access_key_id=AK, secret_access_key=SK, server=server)
+        _obsClient = ObsClient(access_key_id=_AK, secret_access_key=_SK, server=_server)
 
     _download_folder(src, dest)
 
 
 def download(obs_url):
     global _obsClient
     if _obsClient is None:
-        _obsClient = ObsClient(access_key_id=AK, secret_access_key=SK, server=server)
+        _obsClient = ObsClient(access_key_id=_AK, secret_access_key=_SK, server=_server)
 
     if not _is_obs_path(obs_url):
         raise Exception('obs url is invalid')
 
     url = urlparse(obs_url)
     bucket_name = url.hostname
     try:
@@ -48,30 +57,42 @@
             return resp.body.buffer
 
         else:
             print('errorCode:', resp.errorCode)
             print('errorMessage:', resp.errorMessage)
     except:
         import traceback
-        print(traceback.format_exc())
+        logger.error(traceback.format_exc())
+
+
+def _retry(times=3):
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            for i in range(times):
+                try:
+                    return func(*args, **kwargs)
+                except:
+                    if i == times - 1:
+                        raise
 
+        return wrapper
 
+    return decorator
+
+
+@_retry(times=3)
 def _download_one_file(bucketName, src, dest):
-    try:
-        resp = _obsClient.getObject(bucketName, src, downloadPath=dest,
-                                    progressCallback=download_progress_callback)
-        if resp.status < 300:
-            print('requestId:', resp.requestId)
-            print('url:', resp.body.url)
-        else:
-            print('errorCode:', resp.errorCode)
-            print('errorMessage:', resp.errorMessage)
-    except:
-        import traceback
-        print(traceback.format_exc())
+    resp = _obsClient.getObject(bucketName, src, downloadPath=dest,
+                                progressCallback=download_progress_callback)
+    if resp.status < 300:
+        print('requestId:', resp.requestId)
+        print('url:', resp.body.url)
+    else:
+        print('errorCode:', resp.errorCode)
+        print('errorMessage:', resp.errorMessage)
 
 
 # 流式下载
 def _download_one_file_stream(bucketName, src):
     try:
         resp = _obsClient.getObject(bucketName, src, loadStreamInMemory=False)
 
@@ -85,15 +106,15 @@
                 yield chunk
             resp.body.response.close()
         else:
             print('errorCode:', resp.errorCode)
             print('errorMessage:', resp.errorMessage)
     except:
         import traceback
-        print(traceback.format_exc())
+        logger.error(traceback.format_exc())
 
 
 def _download_folder(obs_url, dest_path):
     url = urlparse(obs_url)
     bucket_name = url.hostname
     try:
         max_num = 1000
@@ -111,18 +132,19 @@
                 else:
                     break
             else:
                 print('errorCode:', resp.errorCode)
                 print('errorMessage:', resp.errorMessage)
     except:
         import traceback
-        print(traceback.format_exc())
+        logger.error(traceback.format_exc())
 
 
 def download_progress_callback(transferred_amount, total_amount, total_seconds):
     global _last_time
     if _last_time is None:
         _last_time = time.time()
     if time.time() - _last_time > 3:
-        print("正在下载中，平均速率： {} (KB/S), 进度： {}%".format(int(transferred_amount * 1.0 / total_seconds / 1024),
-                                                                 int(transferred_amount * 100.0 / total_amount)))
+        logger.info(
+            "正在下载中，平均速率： {} (KB/S), 进度： {}%".format(int(transferred_amount * 1.0 / total_seconds / 1024),
+                                                               int(transferred_amount * 100.0 / total_amount)))
         _last_time = time.time()
```

### Comparing `obsutil-1.0.4/setup.py` & `obsutil-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from datetime import date
-import sys
 from setuptools import setup, find_packages
 # pylint: disable = relative-import
 import obsutil
 
 pkgs = find_packages()
 
 if __name__ == '__main__':
     name = 'obsutil'
 
     requirements = ['esdk-obs-python']
 
     setup(
         name=name,
-        version='1.0.4',
+        version='1.0.5',
         description='hw modelarts obs utils',
         # long_description='',
         # author='Taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         # keywords='Serving Deep Learning Inference AI',
```

