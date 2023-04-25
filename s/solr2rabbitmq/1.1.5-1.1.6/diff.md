# Comparing `tmp/solr2rabbitmq-1.1.5-py3-none-any.whl.zip` & `tmp/solr2rabbitmq-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10215 bytes, number of entries: 7
--rw-r--r--  2.0 unx    10187 b- defN 23-Mar-29 11:58 solr2rabbitmq/__init__.py
--rwxr-xr-x  2.0 unx      542 b- defN 23-Mar-29 11:58 solr2rabbitmq-1.1.5.data/scripts/solr2rabbitmq
--rw-r--r--  2.0 unx    11343 b- defN 23-Mar-29 11:58 solr2rabbitmq-1.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     5002 b- defN 23-Mar-29 11:58 solr2rabbitmq-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-29 11:58 solr2rabbitmq-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Mar-29 11:58 solr2rabbitmq-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      602 b- defN 23-Mar-29 11:58 solr2rabbitmq-1.1.5.dist-info/RECORD
-7 files, 27782 bytes uncompressed, 9141 bytes compressed:  67.1%
+Zip file size: 10208 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    10194 b- defN 23-Apr-25 06:58 solr2rabbitmq/__init__.py
+-rwxr-xr-x  2.0 unx      542 b- defN 23-Apr-25 06:58 solr2rabbitmq-1.1.6.data/scripts/solr2rabbitmq
+-rw-r--r--  2.0 unx    11343 b- defN 23-Apr-25 06:58 solr2rabbitmq-1.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4974 b- defN 23-Apr-25 06:58 solr2rabbitmq-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 06:58 solr2rabbitmq-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-25 06:58 solr2rabbitmq-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      602 b- defN 23-Apr-25 06:58 solr2rabbitmq-1.1.6.dist-info/RECORD
+7 files, 27761 bytes uncompressed, 9134 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: solr2rabbitmq/__init__.py
 Comment: 
 
-Filename: solr2rabbitmq-1.1.5.data/scripts/solr2rabbitmq
+Filename: solr2rabbitmq-1.1.6.data/scripts/solr2rabbitmq
 Comment: 
 
-Filename: solr2rabbitmq-1.1.5.dist-info/LICENSE
+Filename: solr2rabbitmq-1.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: solr2rabbitmq-1.1.5.dist-info/METADATA
+Filename: solr2rabbitmq-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: solr2rabbitmq-1.1.5.dist-info/WHEEL
+Filename: solr2rabbitmq-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: solr2rabbitmq-1.1.5.dist-info/top_level.txt
+Filename: solr2rabbitmq-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: solr2rabbitmq-1.1.5.dist-info/RECORD
+Filename: solr2rabbitmq-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## solr2rabbitmq/__init__.py

```diff
@@ -195,15 +195,15 @@
                 _j = json.loads(solr_config_file.read())
                 SOLR_BASE_URL = _j['url']
         except:
             pass
 
         SOLR_COLLECTION_NAME = os.environ.get('SOLR_COLLECTION_NAME')
 
-        config["solr_collection_url"] = f"{SOLR_BASE_URL}/{SOLR_COLLECTION_NAME}"
+        config["solr_collection_url"] = f"{SOLR_BASE_URL}/{SOLR_COLLECTION_NAME}/select"
 
     template_format = open(config.get("data_template_file_path")).read()
 
     if "worker_pool_size" in config:
         if config.get("worker_pool_size"):
             try:
                 worker_pool_size = int(config.get("worker_pool_size"))
```

## Comparing `solr2rabbitmq-1.1.5.data/scripts/solr2rabbitmq` & `solr2rabbitmq-1.1.6.data/scripts/solr2rabbitmq`

 * *Files identical despite different names*

## Comparing `solr2rabbitmq-1.1.5.dist-info/LICENSE` & `solr2rabbitmq-1.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `solr2rabbitmq-1.1.5.dist-info/METADATA` & `solr2rabbitmq-1.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solr2rabbitmq
-Version: 1.1.5
+Version: 1.1.6
 Summary: Asynchronous RabbitMQ transfer job library from Apache Solr
 Home-page: https://github.com/mantis-software-company/solr2rabbitmq
 Author: Furkan Kalkan
 Author-email: furkankalkan@mantis.com.tr
 License: UNKNOWN
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >3.6.*, <4
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aio-pika
 Requires-Dist: jinja2
 
 # solr2rabbitmq
```

## Comparing `solr2rabbitmq-1.1.5.dist-info/RECORD` & `solr2rabbitmq-1.1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-solr2rabbitmq/__init__.py,sha256=wtnX4ovDx13iRqsKw5X_aMlaiqVNU29c9Y6tJbI983Q,10187
-solr2rabbitmq-1.1.5.data/scripts/solr2rabbitmq,sha256=q8b7AY11Q_iZggAZwfwlkuTzCARhAbkERj2OkOLSNaY,542
-solr2rabbitmq-1.1.5.dist-info/LICENSE,sha256=PsX0TtjB1aacybSeDSMKdZGbIif-HaZgi3CtkAe6b-g,11343
-solr2rabbitmq-1.1.5.dist-info/METADATA,sha256=s1ztaQcGJWWtdfsfWbB8eEeAWwpF2Z9hAd_q48p5IrI,5002
-solr2rabbitmq-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-solr2rabbitmq-1.1.5.dist-info/top_level.txt,sha256=bZ6M0mx0TtECJIVMUZCyvIU2WhfIS5aRKc5syYKNTVI,14
-solr2rabbitmq-1.1.5.dist-info/RECORD,,
+solr2rabbitmq/__init__.py,sha256=_9gV4iCR8l6kUlJlXKTlYNlUc2dcuf51HhlQ5z2gpOg,10194
+solr2rabbitmq-1.1.6.data/scripts/solr2rabbitmq,sha256=q8b7AY11Q_iZggAZwfwlkuTzCARhAbkERj2OkOLSNaY,542
+solr2rabbitmq-1.1.6.dist-info/LICENSE,sha256=PsX0TtjB1aacybSeDSMKdZGbIif-HaZgi3CtkAe6b-g,11343
+solr2rabbitmq-1.1.6.dist-info/METADATA,sha256=S3AbRS9XOnMSSjwG7Jyz6sxG3oHEfQSO0gWgHvIwx70,4974
+solr2rabbitmq-1.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+solr2rabbitmq-1.1.6.dist-info/top_level.txt,sha256=bZ6M0mx0TtECJIVMUZCyvIU2WhfIS5aRKc5syYKNTVI,14
+solr2rabbitmq-1.1.6.dist-info/RECORD,,
```

