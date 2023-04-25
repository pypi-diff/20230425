# Comparing `tmp/obsutils-1.0.6.tar.gz` & `tmp/obsutils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsutils-1.0.6.tar", last modified: Tue Apr 25 08:51:55 2023, max compression
+gzip compressed data, was "obsutils-1.0.7.tar", last modified: Tue Apr 25 11:01:08 2023, max compression
```

## Comparing `obsutils-1.0.6.tar` & `obsutils-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 08:51:55.315167 obsutils-1.0.6/
--rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-25 08:51:55.315034 obsutils-1.0.6/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      125 2023-04-25 08:51:01.000000 obsutils-1.0.6/README.md
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 08:51:55.314074 obsutils-1.0.6/obsutils/
--rw-r--r--   0 chen       (501) staff       (20)       60 2023-04-25 08:51:54.000000 obsutils-1.0.6/obsutils/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     4561 2023-04-25 08:41:32.000000 obsutils-1.0.6/obsutils/file.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 08:51:55.314829 obsutils-1.0.6/obsutils.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-25 08:51:55.000000 obsutils-1.0.6/obsutils.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      215 2023-04-25 08:51:55.000000 obsutils-1.0.6/obsutils.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-25 08:51:55.000000 obsutils-1.0.6/obsutils.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       16 2023-04-25 08:51:55.000000 obsutils-1.0.6/obsutils.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)        9 2023-04-25 08:51:55.000000 obsutils-1.0.6/obsutils.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-25 08:51:55.315221 obsutils-1.0.6/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      688 2023-04-25 08:51:09.000000 obsutils-1.0.6/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 11:01:08.414178 obsutils-1.0.7/
+-rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-25 11:01:08.414051 obsutils-1.0.7/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      167 2023-04-25 09:00:58.000000 obsutils-1.0.7/README.md
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 11:01:08.413053 obsutils-1.0.7/obsutils/
+-rw-r--r--   0 chen       (501) staff       (20)       60 2023-04-25 08:51:54.000000 obsutils-1.0.7/obsutils/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     4876 2023-04-25 10:59:56.000000 obsutils-1.0.7/obsutils/file.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-25 11:01:08.413853 obsutils-1.0.7/obsutils.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      173 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      215 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       16 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)        9 2023-04-25 11:01:08.000000 obsutils-1.0.7/obsutils.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-25 11:01:08.414229 obsutils-1.0.7/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      688 2023-04-25 11:00:58.000000 obsutils-1.0.7/setup.py
```

### Comparing `obsutils-1.0.6/obsutils/file.py` & `obsutils-1.0.7/obsutils/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import logging
 import os
+import sys
 import time
 from obs import ObsClient
 from urllib.parse import urlparse
 
 _AK = os.environ.get('HW_OBS_AK')
 _SK = os.environ.get('HW_OBS_SK')
 _server = os.environ.get('HW_OBS_SERVER')
 
 _obsClient = None
 _last_time = None
 
+logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
+
+
 def init(ak, sk, server):
     global _AK, _SK, _server
     _AK = ak
     _SK = sk
     _server = server
+    logger.info("init obsutil done")
 
 # 检查字符串是否为合法的obs路径
 # obs路径格式为：obs://bucketname/objectname
 def _is_obs_path(path):
     if path.startswith('obs://'):
         return True
     else:
@@ -47,78 +52,80 @@
 
     url = urlparse(obs_url)
     bucket_name = url.hostname
     try:
         resp = _obsClient.getObject(bucket_name, url.path[1:], loadStreamInMemory=True)
 
         if resp.status < 300:
-            print('requestId:', resp.requestId)
+            logger.info('requestId:', resp.requestId)
             # 获取对象内容
-            print('size:', resp.body.size)
+            logger.info('size:', resp.body.size)
             return resp.body.buffer
 
         else:
-            print('errorCode:', resp.errorCode)
-            print('errorMessage:', resp.errorMessage)
+            logger.info('errorCode:', resp.errorCode)
+            logger.info('errorMessage:', resp.errorMessage)
     except:
         import traceback
         logger.error(traceback.format_exc())
 
 
 def _retry(times=3):
     def decorator(func):
         def wrapper(*args, **kwargs):
             for i in range(times):
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     logger.error('retry %d times, error: %s', i, str(e))
+                    time.sleep(1)
                     if i == times - 1:
                         raise
 
         return wrapper
 
     return decorator
 
 
-@_retry(times=3)
+@_retry(times=5)
 def _download_one_file(bucketName, src, dest):
     resp = _obsClient.getObject(bucketName, src, downloadPath=dest,
                                 progressCallback=download_progress_callback)
     if resp.status < 300:
-        print('requestId:', resp.requestId)
-        print('url:', resp.body.url)
+        logger.info('requestId:', resp.requestId)
+        logger.info('url:', resp.body.url)
     else:
-        print('errorCode:', resp.errorCode)
-        print('errorMessage:', resp.errorMessage)
+        logger.info('errorCode:', resp.errorCode)
+        logger.info('errorMessage:', resp.errorMessage)
 
 
 # 流式下载
 def _download_one_file_stream(bucketName, src):
     try:
         resp = _obsClient.getObject(bucketName, src, loadStreamInMemory=False)
 
         if resp.status < 300:
-            print('requestId:', resp.requestId)
+            logger.info('requestId:', resp.requestId)
             # 读取对象内容
             while True:
                 chunk = resp.body.response.read(65536)
                 if not chunk:
                     break
                 yield chunk
             resp.body.response.close()
         else:
-            print('errorCode:', resp.errorCode)
-            print('errorMessage:', resp.errorMessage)
+            logger.info('errorCode:', resp.errorCode)
+            logger.info('errorMessage:', resp.errorMessage)
     except:
         import traceback
         logger.error(traceback.format_exc())
 
 
 def _download_folder(obs_url, dest_path):
+    logger.info('download folder: %s to %s', obs_url, dest_path)
     url = urlparse(obs_url)
     bucket_name = url.hostname
     try:
         max_num = 1000
         mark = None
         while True:
             resp = _obsClient.listObjects(bucket_name, url.path[1:], marker=mark, max_keys=max_num)
@@ -129,16 +136,16 @@
                         _download_one_file(bucket_name, name,
                                            os.path.join(dest_path, os.path.relpath('/' + name, url.path)))
                 if resp.body.is_truncated is True:
                     mark = resp.body.next_marker
                 else:
                     break
             else:
-                print('errorCode:', resp.errorCode)
-                print('errorMessage:', resp.errorMessage)
+                logger.info('errorCode:', resp.errorCode)
+                logger.info('errorMessage:', resp.errorMessage)
     except:
         import traceback
         logger.error(traceback.format_exc())
 
 
 def download_progress_callback(transferred_amount, total_amount, total_seconds):
     global _last_time
```

### Comparing `obsutils-1.0.6/setup.py` & `obsutils-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if __name__ == '__main__':
     name = 'obsutils'
 
     requirements = ['esdk-obs-python']
 
     setup(
         name=name,
-        version='1.0.6',
+        version='1.0.7',
         description='hw modelarts obs utils',
         # long_description='',
         # author='Taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         # keywords='Serving Deep Learning Inference AI',
```

