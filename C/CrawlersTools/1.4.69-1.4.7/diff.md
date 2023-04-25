# Comparing `tmp/CrawlersTools-1.4.69.tar.gz` & `tmp/CrawlersTools-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrawlersTools-1.4.69.tar", last modified: Wed Apr 19 10:31:10 2023, max compression
+gzip compressed data, was "CrawlersTools-1.4.7.tar", last modified: Mon Apr 24 09:47:18 2023, max compression
```

## Comparing `CrawlersTools-1.4.69.tar` & `CrawlersTools-1.4.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.235205 CrawlersTools-1.4.69/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.223204 CrawlersTools-1.4.69/CrawlersTools/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.227204 CrawlersTools-1.4.69/CrawlersTools/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/attachment_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/content_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/list_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.227204 CrawlersTools-1.4.69/CrawlersTools/extractors/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/schemas/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/time_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/title_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.227204 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/extractors/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.231204 CrawlersTools-1.4.69/CrawlersTools/js_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/js_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/js_crawler/font_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/js_crawler/transfer_js.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.231204 CrawlersTools-1.4.69/CrawlersTools/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/logs/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.231204 CrawlersTools-1.4.69/CrawlersTools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/pipelines/mongo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/pipelines/mysql_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/pipelines/redis_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.231204 CrawlersTools-1.4.69/CrawlersTools/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/preprocess/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/preprocess/time_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.235205 CrawlersTools-1.4.69/CrawlersTools/projects/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/projects/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/projects/upload_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.235205 CrawlersTools-1.4.69/CrawlersTools/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/requests/base_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/requests/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/requests/random_ua.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.235205 CrawlersTools-1.4.69/CrawlersTools/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/CrawlersTools/schedules/auto_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:31:10.223204 CrawlersTools-1.4.69/CrawlersTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-19 10:31:10.000000 CrawlersTools-1.4.69/CrawlersTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-19 10:31:10.000000 CrawlersTools-1.4.69/CrawlersTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:31:10.000000 CrawlersTools-1.4.69/CrawlersTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-19 10:31:10.000000 CrawlersTools-1.4.69/CrawlersTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 10:31:10.000000 CrawlersTools-1.4.69/CrawlersTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-19 10:31:10.235205 CrawlersTools-1.4.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 10:31:10.235205 CrawlersTools-1.4.69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-19 10:30:57.000000 CrawlersTools-1.4.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.520623 CrawlersTools-1.4.7/CrawlersTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.520623 CrawlersTools-1.4.7/CrawlersTools/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/attachment_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/content_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/list_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.520623 CrawlersTools-1.4.7/CrawlersTools/extractors/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/schemas/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/time_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/title_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.520623 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/extractors/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/js_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/js_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/js_crawler/font_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/js_crawler/transfer_js.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/logs/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/pipelines/mongo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/pipelines/mysql_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/pipelines/redis_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/preprocess/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/preprocess/time_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/projects/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/projects/upload_oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/requests/base_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/requests/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/requests/random_ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/CrawlersTools/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/CrawlersTools/schedules/auto_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:47:18.520623 CrawlersTools-1.4.7/CrawlersTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42683 2023-04-24 09:47:18.000000 CrawlersTools-1.4.7/CrawlersTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-24 09:47:18.000000 CrawlersTools-1.4.7/CrawlersTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:47:18.000000 CrawlersTools-1.4.7/CrawlersTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 09:47:18.000000 CrawlersTools-1.4.7/CrawlersTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 09:47:18.000000 CrawlersTools-1.4.7/CrawlersTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42683 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:47:18.524623 CrawlersTools-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-24 09:47:01.000000 CrawlersTools-1.4.7/setup.py
```

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/__init__.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/attachment_extractor.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/attachment_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/base.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/base.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/content_extractor.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/content_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/list_extractor.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/list_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/schemas/element.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/schemas/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/time_extractor.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/time_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/title_extractor.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/title_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/utils/cluster.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/utils/element.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/utils/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/utils/preprocess.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/utils/settings.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/utils/settings.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/extractors/utils/similarity.py` & `CrawlersTools-1.4.7/CrawlersTools/extractors/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/js_crawler/font_decrypt.py` & `CrawlersTools-1.4.7/CrawlersTools/js_crawler/font_decrypt.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/js_crawler/transfer_js.py` & `CrawlersTools-1.4.7/CrawlersTools/js_crawler/transfer_js.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/logs/log.py` & `CrawlersTools-1.4.7/CrawlersTools/logs/log.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/pipelines/mongo_pipeline.py` & `CrawlersTools-1.4.7/CrawlersTools/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/pipelines/mysql_pipeline.py` & `CrawlersTools-1.4.7/CrawlersTools/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/pipelines/redis_pipeline.py` & `CrawlersTools-1.4.7/CrawlersTools/pipelines/redis_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/preprocess/bloom_filter.py` & `CrawlersTools-1.4.7/CrawlersTools/preprocess/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/preprocess/time_process.py` & `CrawlersTools-1.4.7/CrawlersTools/preprocess/time_process.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 # @File    : time_process.py
 
 import re
 from datetime import datetime, timedelta
 
 from sinan import Sinan
 
-from CrawlersTools.projects.filters import empty_title
+from CrawlersTools.projects.filters import empty_text
 
 
 class TimeProcessor:
 
     datetime_pattern = r"([0-9]{4}).*?([0-1]{0,1}[0-9]).*?([0-3]{0,1}[0-9])"
 
     def __init__(self):
         self.fmt = "%Y-%m-%d"  # 暂时只处理年月日
 
     def format(self, string, struct=False):
-        string = empty_title(string)
+        string = empty_text(string)
         try:
             return self.process_timestamp(string, struct)
         except ValueError:
             # print(f"非时间戳格式：{string}")
             pass
 
         date = Sinan(string).parse(display_status=False).get("datetime", [""])[0].split(' ')[0]  # 错误的时分秒
```

### Comparing `CrawlersTools-1.4.69/CrawlersTools/projects/filters.py` & `CrawlersTools-1.4.7/CrawlersTools/projects/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 from functools import reduce
 from urllib.parse import urlparse
 
 from loguru import logger
 
 
-def empty_title(lis):
+def empty_text(lis):
     word = ""
     for i in lis:
         word += i.strip()
     return word
 
 
 def filter_title(title: str, remove_list: list):
@@ -27,15 +27,15 @@
     """
     if not title:
         return False
     for r in remove_list:
         and_lists = r.split("and")
         if len(and_lists) == 1:
             if and_lists[0] in title:
-                logger.debug(f"[DEBUG] 过滤标题: {title}   过滤词:{r}")
+                logger.debug(f"过滤标题: {title}  过滤词: {r}")
                 return True
         else:
             total = [1 for a in and_lists if a in title]
             result = reduce(lambda x, y: x + y, total)
             if len(and_lists) != result:
                 continue
             return True
```

### Comparing `CrawlersTools-1.4.69/CrawlersTools/projects/upload_oss.py` & `CrawlersTools-1.4.7/CrawlersTools/projects/upload_oss.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 # @Author  : MuggleK
 # @File    : upload_oss.py
 
 import base64
 import hashlib
 import re
 
-from loguru import logger
 import httpx
+from loguru import logger
 
+from CrawlersTools import base_requests
 from CrawlersTools.requests.proxy import get_proxies
 
 
 class UploadOss(object):
     """
     A Class for QZD Upload file to oss
 
@@ -22,30 +23,33 @@
 
     ```python
     >>> upload = UploadOss('(pdf|txt|doc|docx|xlsx|xls|csv|wps|hlp|rtf|ppt|pptx|zip|rar|jar|gz|jpg|jpeg|png|tif|gif|bmp)', "https://***")
     >>> oss_url, oss_uuid = upload.download("http://xxgk.haiyan.gov.cn/gov/jcms_files/jcms1/web7/site/zfxxgk/download/downfile.jsp?classid=0&filename=140901165845693.xls", '附件')
     ```
     """
 
-    def __init__(self, oss_url, suffix_reg):
+    def __init__(self, oss_url, suffix_reg, oss_code=None, client_code=None):
         self.suffix_reg = suffix_reg
         self.oss_url = oss_url
+        self.oss_code = oss_code
+        self.client_code = client_code
 
     def download(self, file_url, file_name, headers=None, verify=True):
         """
 
         :param file_url:
         :param file_name:
         :param headers:
         :param verify:
         :return:
         """
         location = global_uuid = ""
         proxy = None
-        headers = headers if headers else {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36"}
+        headers = headers if headers else {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.116 Safari/537.36"}
         for _ in range(3):
             try:
                 if ";base64," in file_url:
                     suffix = "png"
                     logger.debug(f"正在上传base64图片: {file_name}: {file_url}")
                     hl = hashlib.md5()
                     hl.update(file_url.encode(encoding='utf-8'))
@@ -59,53 +63,54 @@
                     logger.debug(f"文件上传成功: {file_name}: {file_url}")
                 else:
                     suffix = self.complete_name(file_url, file_name, self.suffix_reg)
                     if not file_url.startswith("http") and not suffix:
                         return location, global_uuid
                     file_name = f"{file_name}.{suffix}"
                     logger.debug(f"正在上传文件: {file_name}: {file_url}")
-                    res = httpx.get(file_url, timeout=60, headers=headers, verify=verify, proxies=proxy)
+                    res = base_requests(file_url, timeout=60, headers=headers, verify=verify, proxies=proxy)
                     if 200 <= res.status_code < 400:
                         upload_result = self.post_file(file_name, res)
                         location = upload_result.get("downloadLocation")
                         global_uuid = upload_result.get("globalUuid")
                         logger.debug(f"文件上传成功: {file_name}: {file_url}")
                         break
                     elif res.status_code == 404 or res.status_code == 500:
                         logger.debug(f"文件地址无效: {file_name}: {file_url}")
                         break
             except Exception as e:
                 logger.warning(f"文件上传异常: {file_name}: {e}")
-                proxy = get_proxies()
+                proxy = get_proxies(http2=True)
                 continue
         else:
             logger.error(f"文件上传失败: {file_name}: {file_url}")
 
         return location, global_uuid
 
     def post_file(self, name, resp):
         params_json = {
             "name": name,
-            "appCode": "spider-project",
-            "appClientCode": "policy",
+            "appCode": self.oss_code,
+            "appClientCode": self.client_code,
             "appOrgCode": "",
             "appUserId": "",
             "ownCatalogUuid": ""
         }
         json_data = httpx.post(self.oss_url, json=params_json).json()
         if json_data.get("msg") == "SUCCESS":
             token_data = json_data.get("data", {})
 
-            str_dic = {"key": token_data.get("dir") + token_data.get("name"),
-                       "policy": token_data.get("policy"),
-                       "OSSAccessKeyId": token_data.get("accessid"),
-                       "success_action_status": 200,
-                       "callback": token_data.get("callback"),
-                       "signature": token_data.get("signature"),
-                       }
+            str_dic = {
+                "key": token_data.get("dir") + token_data.get("name"),
+                "policy": token_data.get("policy"),
+                "OSSAccessKeyId": token_data.get("accessid"),
+                "success_action_status": 200,
+                "callback": token_data.get("callback"),
+                "signature": token_data.get("signature"),
+            }
 
             files = {'file': resp.content}
             response = httpx.post(token_data.get("host"), data=str_dic, files=files)
             if response.status_code == 200:
                 res_data = response.json()
                 if res_data.get("msg") == "SUCCESS":
                     return res_data["data"]
```

### Comparing `CrawlersTools-1.4.69/CrawlersTools/requests/base_requests.py` & `CrawlersTools-1.4.7/CrawlersTools/requests/base_requests.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/requests/proxy.py` & `CrawlersTools-1.4.7/CrawlersTools/requests/proxy.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/requests/random_ua.py` & `CrawlersTools-1.4.7/CrawlersTools/requests/random_ua.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools/schedules/auto_thread.py` & `CrawlersTools-1.4.7/CrawlersTools/schedules/auto_thread.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/CrawlersTools.egg-info/PKG-INFO` & `CrawlersTools-1.4.7/CrawlersTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.69
+Version: 1.4.7
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.69/CrawlersTools.egg-info/SOURCES.txt` & `CrawlersTools-1.4.7/CrawlersTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/LICENSE` & `CrawlersTools-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/PKG-INFO` & `CrawlersTools-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.69
+Version: 1.4.7
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.69/README.md` & `CrawlersTools-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.69/setup.py` & `CrawlersTools-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='CrawlersTools',  # 包名
-    version='1.4.69',  # 版本号
+    version='1.4.7',  # 版本号
     description='Tools for Crawlers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='MuggleK',
     author_email='peichangchuan@gmail.com',
     url='https://github.com/MuggleK/CrawlersTools',
     install_requires=[
```

