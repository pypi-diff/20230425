# Comparing `tmp/cyberdrop-dl-4.1.12.tar.gz` & `tmp/cyberdrop-dl-4.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.12.tar", last modified: Fri Apr 21 04:46:29 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.13.tar", last modified: Mon Apr 24 23:15:10 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.12.tar` & `cyberdrop-dl-4.1.13.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.059224 cyberdrop-dl-4.1.12/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.063224 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.063224 cyberdrop-dl-4.1.12/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.067224 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:46:29.059224 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 04:46:29.000000 cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-21 04:46:29.071224 cyberdrop-dl-4.1.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:46:16.000000 cyberdrop-dl-4.1.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.025434 cyberdrop-dl-4.1.13/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-24 23:15:10.025434 cyberdrop-dl-4.1.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.017434 cyberdrop-dl-4.1.13/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.021434 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.021434 cyberdrop-dl-4.1.13/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.025434 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19384 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.025434 cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.025434 cyberdrop-dl-4.1.13/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:15:10.021434 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-24 23:15:10.000000 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-24 23:15:10.000000 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:15:10.000000 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 23:15:10.000000 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 23:15:10.000000 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 23:15:10.000000 cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-24 23:15:10.025434 cyberdrop-dl-4.1.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:15:00.000000 cyberdrop-dl-4.1.13/setup.py
```

### Comparing `cyberdrop-dl-4.1.12/LICENSE` & `cyberdrop-dl-4.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/PKG-INFO` & `cyberdrop-dl-4.1.13/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.12
+Version: 4.1.13
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `cyberdrop-dl`
-**Bulk downloader for multiple file hosts** 
+
+**Bulk downloader for multiple file hosts**
 
 [![PyPI version](https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-dl)
 
 [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp)
 
-
 Brand new and improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top of this it also downloads from different domains simultaneously.
 
 ![Screenshot 2023-02-19 183052](https://user-images.githubusercontent.com/61347133/219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png)
 
-# Support Cyberdrop-DL Development
+## Support Cyberdrop-DL Development
 
 <a href="https://www.buymeacoffee.com/juleswinnft" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 If you want to support me and my effort you can buy me a coffee or send me some crypto:
 
 BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn
 
 ETH: 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B
 
 XMR: 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 
-# More Information
-
-Read the Wiki!
+## More Information
 
-https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/
+Read the [Wiki](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/)!
 
-# Supported Sites
+## Supported Sites
 
 | Website                 | Supported Link Types                                                                                                                                                                                                                   |
 |-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Anonfiles               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
 | Bayfiles                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
 | Bunkr (ru/su/la)        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
-| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      | 
+| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
 | Cyberdrop               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
-| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    | 
+| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
 | E-Hentai                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
 | Erome                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
 | Fapello                 | Models: fapello.com/...                                                                                                                                                                                                                |
 | Gallery.DeltaPorno.com  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
 | GoFile                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
 | Gfycat                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
 | HGameCG                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
@@ -65,127 +63,130 @@
 | jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
-| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            | 
+| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
 | SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
 | XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
 | XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
-# Information
+## Information
 
 **Requires Python 3.7 or higher (3.10 recommended)**
 
-You can get Python from here: https://www.python.org/downloads/
+You can get Python from here: <https://www.python.org/downloads/>
 
 Make sure you tick the check box for "Add python to path"
 ![alt text](https://simp2.jpg.church/PATHe426c23371048def.png)
 
 Mac users will also likely need to open terminal and execute the following command: `xcode-select --install`
 
-# Script Method
+## Script Method
+
 Go to the [releases page](https://github.com/Jules-WinnfieldX/CyberDropDownloader/releases) and download the Cyberdrop_DL.zip file. Extract it to wherever you want the program to be.
 
 Put the links in the URLs.txt file then run `Start Windows.bat` (Windows) or `Start Mac.command` (OS X) or `Start Linux.sh` (Linux).
 
 ** Mac users will need to run the command `chmod +x 'Start Mac.command'` to make the file executable.
 
-# CLI Method
+## CLI Method
 
 Run `pip3 install cyberdrop-dl` in command prompt/terminal
 
 Advanced users may want to use virtual environments (via `pipx`), but it's **NOT** required.
 
 1. Run `cyberdrop-dl` once to generate an empty `URLs.txt` file.
 2. Copy and paste your links into `URLs.txt`.
 Each link you add has to go on its own line (paste link, press enter, repeat).
 3. Run `cyberdrop-dl` again.
 It will begin to download everything.
 4. Enjoy!
 
-## Arguments & Config
+### Arguments & Config
+
 If you know what you're doing, you can use the available options to adjust how the program runs.
 
 You can read more about all of these options [here](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/Config-Options). As they directly correlate with the config options.
 
-```
+```raw
 $ cyberdrop-dl -h
 usage: cyberdrop-dl [-h] [-V] [-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads THREADS] [--attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-images] [--exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
 
 Bulk downloader for multiple file hosts
 
 positional arguments:
   link                  link to content to download (passing multiple links is supported)
 
 optional arguments:
 -h, --help                                         show this help message and exit
 -V, --version                                      show program's version number and exit
 -i INPUT_FILE, --input-file INPUT_FILE             file containing links to download
 -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER    folder to download files to
 
---config-file 	                config file to read arguments from
---db-file 	                history database file to write to
+--config-file                   config file to read arguments from
+--db-file                       history database file to write to
 --errored-urls-file             csv file to write failed download information to
---log-file 	                log file to write to
---output-last-forum-post-file 	text file to output last scraped post from a forum thread for re-feeding into CDL
---unsupported-urls-file 	csv file to output unsupported links into
-
---exclude-audio 	skip downloading of audio files
---exclude-images 	skip downloading of image files
---exclude-other 	skip downloading of images
---exclude-videos 	skip downloading of video files
---ignore-cache 	        ignores previous runs cached scrape history
---ignore-history 	ignores previous download history
---only-hosts 	        only allows downloads and scraping from these hosts
---skip-hosts 	        doesn't allow downloads and scraping from these hosts
-
---allow-insecure-connections 	        allows insecure connections from content hosts
---attempts 	                        number of attempts to download each file
---block-sub-folders 	                block sub folders from being created
---disable-attempt-limit 	        disables the attempt limitation
---include-id 	                        include the ID in the download folder name
---skip-download-mark-completed 	        sets the scraped files as downloaded without downloading
---output-errored-urls 	                sets the failed urls to be output to the errored urls file
---output-unsupported-urls 	        sets the unsupported urls to be output to the unsupported urls file
---proxy 	                        HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
---remove-bunkr-identifier 	        removes the bunkr added identifier from output filenames
---required-free-space 	                required free space (in gigabytes) for the program to run
---simultaneous-downloads-per-domain 	number of simultaneous downloads to use per domain
-
---sort-downloads 	sorts downloaded files after downloads have finished
---sort-directory 	folder to download files to
---sorted-audio 	        schema to sort audio
---sorted-images 	schema to sort images
---sorted-others 	schema to sort other
---sorted-videos 	schema to sort videos
-
---connection-timeout 	number of seconds to wait attempting to connect to a URL during the downloading phase
---ratelimit 	        this applies to requests made in the program during scraping, the number you provide is in requests/seconds
---throttle 	        this is a throttle between requests during the downloading phase, the number is in seconds
-
---output-last-forum-post 	outputs the last post of a forum scrape to use as a starting point for future runs
---separate-posts 	        separates forum scraping into folders by post number
-	
---pixeldrain-api-key 	        api key for premium pixeldrain
---simpcity-password 	        password to login to simpcity
---simpcity-username 	        username to login to simpcity
---socialmediagirls-password 	password to login to socialmediagirls
---socialmediagirls-username 	username to login to socialmediagirls
---xbunker-password 	        password to login to xbunker
---xbunker-username 	        username to login to xbunker
-
---apply-jdownloader 	enables sending unsupported URLs to a running jdownloader2 instance to download
---jdownloader-username 	username to login to jdownloader
---jdownloader-password 	password to login to jdownloader
---jdownloader-device 	device name to login to for jdownloader
+--log-file                      log file to write to
+--output-last-forum-post-file   text file to output last scraped post from a forum thread for re-feeding into CDL
+--unsupported-urls-file         csv file to output unsupported links into
+
+--exclude-audio         skip downloading of audio files
+--exclude-images        skip downloading of image files
+--exclude-other         skip downloading of images
+--exclude-videos        skip downloading of video files
+--ignore-cache          ignores previous runs cached scrape history
+--ignore-history        ignores previous download history
+--only-hosts            only allows downloads and scraping from these hosts
+--skip-hosts            doesn't allow downloads and scraping from these hosts
+
+--allow-insecure-connections            allows insecure connections from content hosts
+--attempts                              number of attempts to download each file
+--block-sub-folders                     block sub folders from being created
+--disable-attempt-limit                 disables the attempt limitation
+--include-id                            include the ID in the download folder name
+--skip-download-mark-completed          sets the scraped files as downloaded without downloading
+--output-errored-urls                   sets the failed urls to be output to the errored urls file
+--output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
+--proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
+--remove-bunkr-identifier               removes the bunkr added identifier from output filenames
+--required-free-space                   required free space (in gigabytes) for the program to run
+--simultaneous-downloads-per-domain     number of simultaneous downloads to use per domain
+
+--sort-downloads        sorts downloaded files after downloads have finished
+--sort-directory        folder to download files to
+--sorted-audio          schema to sort audio
+--sorted-images         schema to sort images
+--sorted-others         schema to sort other
+--sorted-videos         schema to sort videos
+
+--connection-timeout    number of seconds to wait attempting to connect to a URL during the downloading phase
+--ratelimit             this applies to requests made in the program during scraping, the number you provide is in requests/seconds
+--throttle              this is a throttle between requests during the downloading phase, the number is in seconds
+
+--output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
+--separate-posts                separates forum scraping into folders by post number
+
+--gofile-api-key                api key for premium gofile
+--pixeldrain-api-key            api key for premium pixeldrain
+--simpcity-username             username to login to simpcity
+--simpcity-password             password to login to simpcity
+--socialmediagirls-username     username to login to socialmediagirls
+--socialmediagirls-password     password to login to socialmediagirls
+--xbunker-username              username to login to xbunker
+--xbunker-password              password to login to xbunker
+
+--apply-jdownloader     enables sending unsupported URLs to a running jdownloader2 instance to download
+--jdownloader-username  username to login to jdownloader
+--jdownloader-password  password to login to jdownloader
+--jdownloader-device    device name to login to for jdownloader
 
 --hide-new-progress             disables the new rich progress entirely and uses older methods
 --hide-overall-progress         removes overall progress section while downloading
 --hide-forum-progress           removes forum progress section while downloading
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.12 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.13 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -11,26 +11,26 @@
 dl/month)](https://pepy.tech/project/cyberdrop-dl) [![Downloads](https://
 static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-
 dl) [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/
 widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp) Brand new and
 improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top
 of this it also downloads from different domains simultaneously. ![Screenshot
 2023-02-19 183052](https://user-images.githubusercontent.com/61347133/
-219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png) # Support Cyberdrop-DL
+219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png) ## Support Cyberdrop-DL
 Development [Buy_Me_A_Coffee] If you want to support me and my effort you can
 buy me a coffee or send me some crypto: BTC:
 bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
-# More Information Read the Wiki! https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/wiki/ # Supported Sites | Website | Supported Link Types |
-|-------------------------|----------------------------------------------------
+## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
+CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
+| |-------------------------|--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------| | Anonfiles | Download page: Anonfiles.com/... | |
+------------------------| | Anonfiles | Download page: Anonfiles.com/... | |
 Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/su/la) | Albums:
 bunkr.ru/a/...
 Direct Videos: stream.bunkr.ru/v/...
 Direct links: cdn.bunkr.ru/...
 Direct links: i.bunkr.ru/...
 Direct links: files.bunkr.ru/...
 Direct links: media-files.bunkr.ru/... | | Coomer.party | Profiles:
@@ -78,42 +78,42 @@
 Continue from (will download this post and after): simpcity.st/threads/...post-
 NUMBER | | SocialMediaGirls | Thread: forum.socialmediagirls.com/threads/...
 Continue from (will download this post and after): forum.socialmediagirls.com/
 threads/...post-NUMBER | | XBunker | Thread: xbunker.nu/threads/...
 Continue from (will download this post and after): xbunker.nu/threads/...post-
 NUMBER | | XBunkr | Album: xbunkr.com/a/...
 Direct Links: media.xbunkr.com/... | Reminder to leave the link full (include
-the https://) # Information **Requires Python 3.7 or higher (3.10
-recommended)** You can get Python from here: https://www.python.org/downloads/
-Make sure you tick the check box for "Add python to path" ![alt text](https://
-simp2.jpg.church/PATHe426c23371048def.png) Mac users will also likely need to
-open terminal and execute the following command: `xcode-select --install` #
-Script Method Go to the [releases page](https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/releases) and download the Cyberdrop_DL.zip file. Extract
-it to wherever you want the program to be. Put the links in the URLs.txt file
-then run `Start Windows.bat` (Windows) or `Start Mac.command` (OS X) or `Start
-Linux.sh` (Linux). ** Mac users will need to run the command `chmod +x 'Start
-Mac.command'` to make the file executable. # CLI Method Run `pip3 install
-cyberdrop-dl` in command prompt/terminal Advanced users may want to use virtual
-environments (via `pipx`), but it's **NOT** required. 1. Run `cyberdrop-dl`
-once to generate an empty `URLs.txt` file. 2. Copy and paste your links into
-`URLs.txt`. Each link you add has to go on its own line (paste link, press
-enter, repeat). 3. Run `cyberdrop-dl` again. It will begin to download
-everything. 4. Enjoy! ## Arguments & Config If you know what you're doing, you
-can use the available options to adjust how the program runs. You can read more
-about all of these options [here](https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/wiki/Config-Options). As they directly correlate with the
-config options. ``` $ cyberdrop-dl -h usage: cyberdrop-dl [-h] [-V] [-
-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads THREADS] [--
-attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-images] [--
-exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-username
-"USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...] Bulk
-downloader for multiple file hosts positional arguments: link link to content
-to download (passing multiple links is supported) optional arguments: -h, --
-help show this help message and exit -V, --version show program's version
+the https://) ## Information **Requires Python 3.7 or higher (3.10
+recommended)** You can get Python from here:
+www.python.org/downloads/> Make sure you tick the check box for "Add python to
+path" ![alt text](https://simp2.jpg.church/PATHe426c23371048def.png) Mac users
+will also likely need to open terminal and execute the following command:
+`xcode-select --install` ## Script Method Go to the [releases page](https://
+github.com/Jules-WinnfieldX/CyberDropDownloader/releases) and download the
+Cyberdrop_DL.zip file. Extract it to wherever you want the program to be. Put
+the links in the URLs.txt file then run `Start Windows.bat` (Windows) or `Start
+Mac.command` (OS X) or `Start Linux.sh` (Linux). ** Mac users will need to run
+the command `chmod +x 'Start Mac.command'` to make the file executable. ## CLI
+Method Run `pip3 install cyberdrop-dl` in command prompt/terminal Advanced
+users may want to use virtual environments (via `pipx`), but it's **NOT**
+required. 1. Run `cyberdrop-dl` once to generate an empty `URLs.txt` file. 2.
+Copy and paste your links into `URLs.txt`. Each link you add has to go on its
+own line (paste link, press enter, repeat). 3. Run `cyberdrop-dl` again. It
+will begin to download everything. 4. Enjoy! ### Arguments & Config If you know
+what you're doing, you can use the available options to adjust how the program
+runs. You can read more about all of these options [here](https://github.com/
+Jules-WinnfieldX/CyberDropDownloader/wiki/Config-Options). As they directly
+correlate with the config options. ```raw $ cyberdrop-dl -h usage: cyberdrop-dl
+[-h] [-V] [-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads
+THREADS] [--attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-
+images] [--exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-
+username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
+Bulk downloader for multiple file hosts positional arguments: link link to
+content to download (passing multiple links is supported) optional arguments: -
+h, --help show this help message and exit -V, --version show program's version
 number and exit -i INPUT_FILE, --input-file INPUT_FILE file containing links to
 download -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER folder to download
 files to --config-file config file to read arguments from --db-file history
 database file to write to --errored-urls-file csv file to write failed download
 information to --log-file log file to write to --output-last-forum-post-file
 text file to output last scraped post from a forum thread for re-feeding into
 CDL --unsupported-urls-file csv file to output unsupported links into --
@@ -140,30 +140,30 @@
 sorted-videos schema to sort videos --connection-timeout number of seconds to
 wait attempting to connect to a URL during the downloading phase --ratelimit
 this applies to requests made in the program during scraping, the number you
 provide is in requests/seconds --throttle this is a throttle between requests
 during the downloading phase, the number is in seconds --output-last-forum-post
 outputs the last post of a forum scrape to use as a starting point for future
 runs --separate-posts separates forum scraping into folders by post number --
-pixeldrain-api-key api key for premium pixeldrain --simpcity-password password
-to login to simpcity --simpcity-username username to login to simpcity --
-socialmediagirls-password password to login to socialmediagirls --
-socialmediagirls-username username to login to socialmediagirls --xbunker-
-password password to login to xbunker --xbunker-username username to login to
-xbunker --apply-jdownloader enables sending unsupported URLs to a running
-jdownloader2 instance to download --jdownloader-username username to login to
-jdownloader --jdownloader-password password to login to jdownloader --
-jdownloader-device device name to login to for jdownloader --hide-new-progress
-disables the new rich progress entirely and uses older methods --hide-overall-
-progress removes overall progress section while downloading --hide-forum-
-progress removes forum progress section while downloading --hide-thread-
-progress removes thread progress section while downloading --hide-domain-
-progress removes domain progress section while downloading --hide-album-
-progress removes album progress section while downloading --hide-file-progress
-removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
-use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
-"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+gofile-api-key api key for premium gofile --pixeldrain-api-key api key for
+premium pixeldrain --simpcity-username username to login to simpcity --
+simpcity-password password to login to simpcity --socialmediagirls-username
+username to login to socialmediagirls --socialmediagirls-password password to
+login to socialmediagirls --xbunker-username username to login to xbunker --
+xbunker-password password to login to xbunker --apply-jdownloader enables
+sending unsupported URLs to a running jdownloader2 instance to download --
+jdownloader-username username to login to jdownloader --jdownloader-password
+password to login to jdownloader --jdownloader-device device name to login to
+for jdownloader --hide-new-progress disables the new rich progress entirely and
+uses older methods --hide-overall-progress removes overall progress section
+while downloading --hide-forum-progress removes forum progress section while
+downloading --hide-thread-progress removes thread progress section while
+downloading --hide-domain-progress removes domain progress section while
+downloading --hide-album-progress removes album progress section while
+downloading --hide-file-progress removes file progress section while
+downloading --refresh-rate changes the refresh rate of the progress table ```
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
+"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
+"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
 "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost",
 "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls",
 "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.12/README.md` & `cyberdrop-dl-4.1.13/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 # `cyberdrop-dl`
-**Bulk downloader for multiple file hosts** 
+
+**Bulk downloader for multiple file hosts**
 
 [![PyPI version](https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-dl)
 
 [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp)
 
-
 Brand new and improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top of this it also downloads from different domains simultaneously.
 
 ![Screenshot 2023-02-19 183052](https://user-images.githubusercontent.com/61347133/219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png)
 
-# Support Cyberdrop-DL Development
+## Support Cyberdrop-DL Development
 
 <a href="https://www.buymeacoffee.com/juleswinnft" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 If you want to support me and my effort you can buy me a coffee or send me some crypto:
 
 BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn
 
 ETH: 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B
 
 XMR: 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 
-# More Information
-
-Read the Wiki!
+## More Information
 
-https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/
+Read the [Wiki](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/)!
 
-# Supported Sites
+## Supported Sites
 
 | Website                 | Supported Link Types                                                                                                                                                                                                                   |
 |-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Anonfiles               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
 | Bayfiles                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
 | Bunkr (ru/su/la)        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
-| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      | 
+| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
 | Cyberdrop               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
-| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    | 
+| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
 | E-Hentai                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
 | Erome                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
 | Fapello                 | Models: fapello.com/...                                                                                                                                                                                                                |
 | Gallery.DeltaPorno.com  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
 | GoFile                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
 | Gfycat                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
 | HGameCG                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
@@ -53,127 +51,130 @@
 | jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
-| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            | 
+| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
 | SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
 | XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
 | XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
-# Information
+## Information
 
 **Requires Python 3.7 or higher (3.10 recommended)**
 
-You can get Python from here: https://www.python.org/downloads/
+You can get Python from here: <https://www.python.org/downloads/>
 
 Make sure you tick the check box for "Add python to path"
 ![alt text](https://simp2.jpg.church/PATHe426c23371048def.png)
 
 Mac users will also likely need to open terminal and execute the following command: `xcode-select --install`
 
-# Script Method
+## Script Method
+
 Go to the [releases page](https://github.com/Jules-WinnfieldX/CyberDropDownloader/releases) and download the Cyberdrop_DL.zip file. Extract it to wherever you want the program to be.
 
 Put the links in the URLs.txt file then run `Start Windows.bat` (Windows) or `Start Mac.command` (OS X) or `Start Linux.sh` (Linux).
 
 ** Mac users will need to run the command `chmod +x 'Start Mac.command'` to make the file executable.
 
-# CLI Method
+## CLI Method
 
 Run `pip3 install cyberdrop-dl` in command prompt/terminal
 
 Advanced users may want to use virtual environments (via `pipx`), but it's **NOT** required.
 
 1. Run `cyberdrop-dl` once to generate an empty `URLs.txt` file.
 2. Copy and paste your links into `URLs.txt`.
 Each link you add has to go on its own line (paste link, press enter, repeat).
 3. Run `cyberdrop-dl` again.
 It will begin to download everything.
 4. Enjoy!
 
-## Arguments & Config
+### Arguments & Config
+
 If you know what you're doing, you can use the available options to adjust how the program runs.
 
 You can read more about all of these options [here](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/Config-Options). As they directly correlate with the config options.
 
-```
+```raw
 $ cyberdrop-dl -h
 usage: cyberdrop-dl [-h] [-V] [-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads THREADS] [--attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-images] [--exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
 
 Bulk downloader for multiple file hosts
 
 positional arguments:
   link                  link to content to download (passing multiple links is supported)
 
 optional arguments:
 -h, --help                                         show this help message and exit
 -V, --version                                      show program's version number and exit
 -i INPUT_FILE, --input-file INPUT_FILE             file containing links to download
 -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER    folder to download files to
 
---config-file 	                config file to read arguments from
---db-file 	                history database file to write to
+--config-file                   config file to read arguments from
+--db-file                       history database file to write to
 --errored-urls-file             csv file to write failed download information to
---log-file 	                log file to write to
---output-last-forum-post-file 	text file to output last scraped post from a forum thread for re-feeding into CDL
---unsupported-urls-file 	csv file to output unsupported links into
-
---exclude-audio 	skip downloading of audio files
---exclude-images 	skip downloading of image files
---exclude-other 	skip downloading of images
---exclude-videos 	skip downloading of video files
---ignore-cache 	        ignores previous runs cached scrape history
---ignore-history 	ignores previous download history
---only-hosts 	        only allows downloads and scraping from these hosts
---skip-hosts 	        doesn't allow downloads and scraping from these hosts
-
---allow-insecure-connections 	        allows insecure connections from content hosts
---attempts 	                        number of attempts to download each file
---block-sub-folders 	                block sub folders from being created
---disable-attempt-limit 	        disables the attempt limitation
---include-id 	                        include the ID in the download folder name
---skip-download-mark-completed 	        sets the scraped files as downloaded without downloading
---output-errored-urls 	                sets the failed urls to be output to the errored urls file
---output-unsupported-urls 	        sets the unsupported urls to be output to the unsupported urls file
---proxy 	                        HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
---remove-bunkr-identifier 	        removes the bunkr added identifier from output filenames
---required-free-space 	                required free space (in gigabytes) for the program to run
---simultaneous-downloads-per-domain 	number of simultaneous downloads to use per domain
-
---sort-downloads 	sorts downloaded files after downloads have finished
---sort-directory 	folder to download files to
---sorted-audio 	        schema to sort audio
---sorted-images 	schema to sort images
---sorted-others 	schema to sort other
---sorted-videos 	schema to sort videos
-
---connection-timeout 	number of seconds to wait attempting to connect to a URL during the downloading phase
---ratelimit 	        this applies to requests made in the program during scraping, the number you provide is in requests/seconds
---throttle 	        this is a throttle between requests during the downloading phase, the number is in seconds
-
---output-last-forum-post 	outputs the last post of a forum scrape to use as a starting point for future runs
---separate-posts 	        separates forum scraping into folders by post number
-	
---pixeldrain-api-key 	        api key for premium pixeldrain
---simpcity-password 	        password to login to simpcity
---simpcity-username 	        username to login to simpcity
---socialmediagirls-password 	password to login to socialmediagirls
---socialmediagirls-username 	username to login to socialmediagirls
---xbunker-password 	        password to login to xbunker
---xbunker-username 	        username to login to xbunker
-
---apply-jdownloader 	enables sending unsupported URLs to a running jdownloader2 instance to download
---jdownloader-username 	username to login to jdownloader
---jdownloader-password 	password to login to jdownloader
---jdownloader-device 	device name to login to for jdownloader
+--log-file                      log file to write to
+--output-last-forum-post-file   text file to output last scraped post from a forum thread for re-feeding into CDL
+--unsupported-urls-file         csv file to output unsupported links into
+
+--exclude-audio         skip downloading of audio files
+--exclude-images        skip downloading of image files
+--exclude-other         skip downloading of images
+--exclude-videos        skip downloading of video files
+--ignore-cache          ignores previous runs cached scrape history
+--ignore-history        ignores previous download history
+--only-hosts            only allows downloads and scraping from these hosts
+--skip-hosts            doesn't allow downloads and scraping from these hosts
+
+--allow-insecure-connections            allows insecure connections from content hosts
+--attempts                              number of attempts to download each file
+--block-sub-folders                     block sub folders from being created
+--disable-attempt-limit                 disables the attempt limitation
+--include-id                            include the ID in the download folder name
+--skip-download-mark-completed          sets the scraped files as downloaded without downloading
+--output-errored-urls                   sets the failed urls to be output to the errored urls file
+--output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
+--proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
+--remove-bunkr-identifier               removes the bunkr added identifier from output filenames
+--required-free-space                   required free space (in gigabytes) for the program to run
+--simultaneous-downloads-per-domain     number of simultaneous downloads to use per domain
+
+--sort-downloads        sorts downloaded files after downloads have finished
+--sort-directory        folder to download files to
+--sorted-audio          schema to sort audio
+--sorted-images         schema to sort images
+--sorted-others         schema to sort other
+--sorted-videos         schema to sort videos
+
+--connection-timeout    number of seconds to wait attempting to connect to a URL during the downloading phase
+--ratelimit             this applies to requests made in the program during scraping, the number you provide is in requests/seconds
+--throttle              this is a throttle between requests during the downloading phase, the number is in seconds
+
+--output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
+--separate-posts                separates forum scraping into folders by post number
+
+--gofile-api-key                api key for premium gofile
+--pixeldrain-api-key            api key for premium pixeldrain
+--simpcity-username             username to login to simpcity
+--simpcity-password             password to login to simpcity
+--socialmediagirls-username     username to login to socialmediagirls
+--socialmediagirls-password     password to login to socialmediagirls
+--xbunker-username              username to login to xbunker
+--xbunker-password              password to login to xbunker
+
+--apply-jdownloader     enables sending unsupported URLs to a running jdownloader2 instance to download
+--jdownloader-username  username to login to jdownloader
+--jdownloader-password  password to login to jdownloader
+--jdownloader-device    device name to login to for jdownloader
 
 --hide-new-progress             disables the new rich progress entirely and uses older methods
 --hide-overall-progress         removes overall progress section while downloading
 --hide-forum-progress           removes forum progress section while downloading
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
```

#### html2text {}

```diff
@@ -6,25 +6,25 @@
 cyberdrop-dl) [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/week)]
 (https://pepy.tech/project/cyberdrop-dl) [![Discord Banner 3](https://
 discordapp.com/api/guilds/1070206871564197908/widget.png?style=banner3)](https:
 //discord.com/invite/kbZCxz22Qp) Brand new and improved! Cyberdrop-DL now has
 an updated paint job, fantastic new look. On top of this it also downloads from
 different domains simultaneously. ![Screenshot 2023-02-19 183052](https://user-
 images.githubusercontent.com/61347133/219989561-759bd8b1-34d2-4d61-8fa7-
-0d0b3680e83f.png) # Support Cyberdrop-DL Development [Buy_Me_A_Coffee] If you
+0d0b3680e83f.png) ## Support Cyberdrop-DL Development [Buy_Me_A_Coffee] If you
 want to support me and my effort you can buy me a coffee or send me some
 crypto: BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
-# More Information Read the Wiki! https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/wiki/ # Supported Sites | Website | Supported Link Types |
-|-------------------------|----------------------------------------------------
+## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
+CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
+| |-------------------------|--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------| | Anonfiles | Download page: Anonfiles.com/... | |
+------------------------| | Anonfiles | Download page: Anonfiles.com/... | |
 Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/su/la) | Albums:
 bunkr.ru/a/...
 Direct Videos: stream.bunkr.ru/v/...
 Direct links: cdn.bunkr.ru/...
 Direct links: i.bunkr.ru/...
 Direct links: files.bunkr.ru/...
 Direct links: media-files.bunkr.ru/... | | Coomer.party | Profiles:
@@ -72,42 +72,42 @@
 Continue from (will download this post and after): simpcity.st/threads/...post-
 NUMBER | | SocialMediaGirls | Thread: forum.socialmediagirls.com/threads/...
 Continue from (will download this post and after): forum.socialmediagirls.com/
 threads/...post-NUMBER | | XBunker | Thread: xbunker.nu/threads/...
 Continue from (will download this post and after): xbunker.nu/threads/...post-
 NUMBER | | XBunkr | Album: xbunkr.com/a/...
 Direct Links: media.xbunkr.com/... | Reminder to leave the link full (include
-the https://) # Information **Requires Python 3.7 or higher (3.10
-recommended)** You can get Python from here: https://www.python.org/downloads/
-Make sure you tick the check box for "Add python to path" ![alt text](https://
-simp2.jpg.church/PATHe426c23371048def.png) Mac users will also likely need to
-open terminal and execute the following command: `xcode-select --install` #
-Script Method Go to the [releases page](https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/releases) and download the Cyberdrop_DL.zip file. Extract
-it to wherever you want the program to be. Put the links in the URLs.txt file
-then run `Start Windows.bat` (Windows) or `Start Mac.command` (OS X) or `Start
-Linux.sh` (Linux). ** Mac users will need to run the command `chmod +x 'Start
-Mac.command'` to make the file executable. # CLI Method Run `pip3 install
-cyberdrop-dl` in command prompt/terminal Advanced users may want to use virtual
-environments (via `pipx`), but it's **NOT** required. 1. Run `cyberdrop-dl`
-once to generate an empty `URLs.txt` file. 2. Copy and paste your links into
-`URLs.txt`. Each link you add has to go on its own line (paste link, press
-enter, repeat). 3. Run `cyberdrop-dl` again. It will begin to download
-everything. 4. Enjoy! ## Arguments & Config If you know what you're doing, you
-can use the available options to adjust how the program runs. You can read more
-about all of these options [here](https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/wiki/Config-Options). As they directly correlate with the
-config options. ``` $ cyberdrop-dl -h usage: cyberdrop-dl [-h] [-V] [-
-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads THREADS] [--
-attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-images] [--
-exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-username
-"USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...] Bulk
-downloader for multiple file hosts positional arguments: link link to content
-to download (passing multiple links is supported) optional arguments: -h, --
-help show this help message and exit -V, --version show program's version
+the https://) ## Information **Requires Python 3.7 or higher (3.10
+recommended)** You can get Python from here:
+www.python.org/downloads/> Make sure you tick the check box for "Add python to
+path" ![alt text](https://simp2.jpg.church/PATHe426c23371048def.png) Mac users
+will also likely need to open terminal and execute the following command:
+`xcode-select --install` ## Script Method Go to the [releases page](https://
+github.com/Jules-WinnfieldX/CyberDropDownloader/releases) and download the
+Cyberdrop_DL.zip file. Extract it to wherever you want the program to be. Put
+the links in the URLs.txt file then run `Start Windows.bat` (Windows) or `Start
+Mac.command` (OS X) or `Start Linux.sh` (Linux). ** Mac users will need to run
+the command `chmod +x 'Start Mac.command'` to make the file executable. ## CLI
+Method Run `pip3 install cyberdrop-dl` in command prompt/terminal Advanced
+users may want to use virtual environments (via `pipx`), but it's **NOT**
+required. 1. Run `cyberdrop-dl` once to generate an empty `URLs.txt` file. 2.
+Copy and paste your links into `URLs.txt`. Each link you add has to go on its
+own line (paste link, press enter, repeat). 3. Run `cyberdrop-dl` again. It
+will begin to download everything. 4. Enjoy! ### Arguments & Config If you know
+what you're doing, you can use the available options to adjust how the program
+runs. You can read more about all of these options [here](https://github.com/
+Jules-WinnfieldX/CyberDropDownloader/wiki/Config-Options). As they directly
+correlate with the config options. ```raw $ cyberdrop-dl -h usage: cyberdrop-dl
+[-h] [-V] [-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads
+THREADS] [--attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-
+images] [--exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-
+username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
+Bulk downloader for multiple file hosts positional arguments: link link to
+content to download (passing multiple links is supported) optional arguments: -
+h, --help show this help message and exit -V, --version show program's version
 number and exit -i INPUT_FILE, --input-file INPUT_FILE file containing links to
 download -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER folder to download
 files to --config-file config file to read arguments from --db-file history
 database file to write to --errored-urls-file csv file to write failed download
 information to --log-file log file to write to --output-last-forum-post-file
 text file to output last scraped post from a forum thread for re-feeding into
 CDL --unsupported-urls-file csv file to output unsupported links into --
@@ -134,30 +134,30 @@
 sorted-videos schema to sort videos --connection-timeout number of seconds to
 wait attempting to connect to a URL during the downloading phase --ratelimit
 this applies to requests made in the program during scraping, the number you
 provide is in requests/seconds --throttle this is a throttle between requests
 during the downloading phase, the number is in seconds --output-last-forum-post
 outputs the last post of a forum scrape to use as a starting point for future
 runs --separate-posts separates forum scraping into folders by post number --
-pixeldrain-api-key api key for premium pixeldrain --simpcity-password password
-to login to simpcity --simpcity-username username to login to simpcity --
-socialmediagirls-password password to login to socialmediagirls --
-socialmediagirls-username username to login to socialmediagirls --xbunker-
-password password to login to xbunker --xbunker-username username to login to
-xbunker --apply-jdownloader enables sending unsupported URLs to a running
-jdownloader2 instance to download --jdownloader-username username to login to
-jdownloader --jdownloader-password password to login to jdownloader --
-jdownloader-device device name to login to for jdownloader --hide-new-progress
-disables the new rich progress entirely and uses older methods --hide-overall-
-progress removes overall progress section while downloading --hide-forum-
-progress removes forum progress section while downloading --hide-thread-
-progress removes thread progress section while downloading --hide-domain-
-progress removes domain progress section while downloading --hide-album-
-progress removes album progress section while downloading --hide-file-progress
-removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
-use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
-"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+gofile-api-key api key for premium gofile --pixeldrain-api-key api key for
+premium pixeldrain --simpcity-username username to login to simpcity --
+simpcity-password password to login to simpcity --socialmediagirls-username
+username to login to socialmediagirls --socialmediagirls-password password to
+login to socialmediagirls --xbunker-username username to login to xbunker --
+xbunker-password password to login to xbunker --apply-jdownloader enables
+sending unsupported URLs to a running jdownloader2 instance to download --
+jdownloader-username username to login to jdownloader --jdownloader-password
+password to login to jdownloader --jdownloader-device device name to login to
+for jdownloader --hide-new-progress disables the new rich progress entirely and
+uses older methods --hide-overall-progress removes overall progress section
+while downloading --hide-forum-progress removes forum progress section while
+downloading --hide-thread-progress removes thread progress section while
+downloading --hide-domain-progress removes domain progress section while
+downloading --hide-album-progress removes album progress section while
+downloading --hide-file-progress removes file progress section while
+downloading --refresh-rate changes the refresh rate of the progress table ```
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
+"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
+"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
 "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost",
 "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls",
 "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 import logging
 import os
 import re
 from typing import TYPE_CHECKING
 
 import rich
 
+from cyberdrop_dl.base_functions.data_classes import MediaItem
 from cyberdrop_dl.base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from yarl import URL
+    
+    from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 
 
 FILE_FORMATS = {
     'Images': {
         '.jpg', '.jpeg', '.png', '.gif',
         '.gifv', '.webp', '.jpe', '.svg',
         '.jfif', '.tif', '.tiff', '.jif',
@@ -51,15 +56,15 @@
     logger.debug(text)
     if not quiet:
         if style:
             text = f"[{style}]{text}[/{style}]"
         rich.print(text)
 
 
-async def purge_dir(dirname) -> None:
+async def purge_dir(dirname: Path) -> None:
     """Purges empty directories"""
     deleted = []
     dir_tree = list(os.walk(dirname, topdown=False))
 
     for tree_element in dir_tree:
         sub_dir = tree_element[0]
         dir_count = len(os.listdir(sub_dir))
@@ -99,7 +104,14 @@
     if filename_parts[-1].isnumeric() and forum:
         filename_parts = filename_parts[0].rsplit('-', 1)
     ext = "." + filename_parts[-1].lower()
     filename = filename_parts[0][:MAX_FILENAME_LENGTH] if len(filename_parts[0]) > MAX_FILENAME_LENGTH else filename_parts[0]
     filename = filename.strip()
     filename = await sanitize(filename + ext)
     return filename, ext
+
+
+async def create_media_item(url: URL, referer: URL, sql_helper: SQLHelper, domain: str) -> MediaItem:
+    """Returns the MediaItem of a given url, throws NoExtensionFailure if url.name doesn't have extension"""
+    filename, ext = await get_filename_and_ext(url.name)
+    complete = await sql_helper.check_complete_singular(domain, url)
+    return MediaItem(url, referer, complete, filename, ext, filename)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,83 @@
 import asyncio
-import os
+import itertools
 from pathlib import Path
-from .base_functions import FILE_FORMATS, log
+
+from .base_functions import FILE_FORMATS, log, purge_dir
 
 
 class Sorter:
     def __init__(self, download_dir: Path, sorted_downloads: Path, audio_dir: str, image_dir: str, video_dir: str,
                  other_dir: str):
         self.download_dir = download_dir
         self.sorted_downloads = sorted_downloads
 
         self.audio_dir = audio_dir
         self.image_dir = image_dir
         self.video_dir = video_dir
         self.other_dir = other_dir
 
-        self.audio = 0
-        self.images = 0
-        self.videos = 0
-        self.other = 0
-
     async def find_files_in_dir(self, directory: Path):
         file_list = []
         for x in directory.iterdir():
             if x.is_file():
                 file_list.append(x)
             elif x.is_dir():
                 file_list.extend(await self.find_files_in_dir(x))
         return file_list
 
     async def sort(self):
+        audio_count = 0
+        image_count = 0
+        video_count = 0
+        other_count = 0
+
         for folder in self.download_dir.iterdir():
             if not folder.is_dir():
                 continue
 
             audio_destination = Path(self.audio_dir.format(sort_dir=self.sorted_downloads, base_dir=folder.name))
             image_destination = Path(self.image_dir.format(sort_dir=self.sorted_downloads, base_dir=folder.name))
             video_destination = Path(self.video_dir.format(sort_dir=self.sorted_downloads, base_dir=folder.name))
             other_destination = Path(self.other_dir.format(sort_dir=self.sorted_downloads, base_dir=folder.name))
 
             files = await self.find_files_in_dir(folder)
             for file in files:
                 ext = file.suffix.lower()
                 if '.part' in ext:
                     continue
-                elif ext in FILE_FORMATS['Audio']:
+                if ext in FILE_FORMATS['Audio']:
                     audio_destination.mkdir(parents=True, exist_ok=True)
                     await self.move_cd(file, audio_destination)
-                    self.audio += 1
+                    audio_count += 1
                 elif ext in FILE_FORMATS['Images']:
                     image_destination.mkdir(parents=True, exist_ok=True)
                     await self.move_cd(file, image_destination)
-                    self.images += 1
+                    image_count += 1
                 elif ext in FILE_FORMATS['Videos']:
                     video_destination.mkdir(parents=True, exist_ok=True)
                     await self.move_cd(file, video_destination)
-                    self.videos += 1
+                    video_count += 1
                 else:
                     other_destination.mkdir(parents=True, exist_ok=True)
                     await self.move_cd(file, other_destination)
-                    self.other += 1
+                    other_count += 1
         await asyncio.sleep(5)
-        await self.purge_dir(str(self.download_dir))
-        await log(f"Organized: {self.audio} Audio Files", style="green")
-        await log(f"Organized: {self.images} Image Files", style="green")
-        await log(f"Organized: {self.videos} Video Files", style="green")
-        await log(f"Organized: {self.other} Other Files", style="green")
+        await purge_dir(self.download_dir)
+        await log(f"Organized: {audio_count} Audio Files", style="green")
+        await log(f"Organized: {image_count} Image Files", style="green")
+        await log(f"Organized: {video_count} Video Files", style="green")
+        await log(f"Organized: {other_count} Other Files", style="green")
 
     async def move_cd(self, file: Path, dest: Path):
         try:
-            file.rename((dest / file.name))
+            dest_file = dest / file.name
+            file.rename(dest_file)
         except FileExistsError:
-            stem = file.stem
-            temp_stem = stem
-            ext = file.suffix
-            i = 1
-            while (dest / f"{temp_stem}{ext}").is_file() and file.is_file():
-                if file.stat().st_size == (dest / file.name).stat().st_size:
-                    file.unlink()
-                temp_stem = f"{stem} ({i})"
-                i += 1
-            if file.is_file():
-                file.rename((dest / f"{temp_stem}{ext}"))
-
-    async def purge_dir(self, directory: str):
-        dir_tree = list(os.walk(directory, topdown=False))
-        for tree_element in dir_tree:
-            sub_dir = tree_element[0]
-            is_empty = not len(os.listdir(sub_dir))
-            if is_empty:
-                os.rmdir(sub_dir)
+            if file.stat().st_size == dest_file.stat().st_size:
+                file.unlink()
+                return
+            for i in itertools.count(1):
+                dest_file = dest / f"{file.stem} ({i}){file.suffix}"
+                if not dest_file.is_file():
+                    break
+            file.rename(dest_file)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from __future__ import annotations
+
 import atexit
 import logging
 import sqlite3
-from pathlib import Path
-from typing import List, Optional
+from typing import TYPE_CHECKING, List, Optional
+
+if TYPE_CHECKING:
+    from pathlib import Path
 
-from yarl import URL
+    from yarl import URL
 
-from cyberdrop_dl.base_functions.data_classes import (
-    AlbumItem,
-    CascadeItem,
-    DomainItem,
-    MediaItem,
-)
+    from cyberdrop_dl.base_functions.data_classes import (
+        AlbumItem,
+        CascadeItem,
+        DomainItem,
+        MediaItem,
+    )
 
 
 async def get_db_path(url: URL, referer: str = None) -> str:
     """Gets the URL path to be put into the DB and checked from the DB"""
     url_path = url.path
 
     if url.host and ('anonfiles' in url.host or 'bayfiles' in url.host):
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import ssl
+import time
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Callable
 
 import aiofiles
 import aiohttp
 import certifi
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 from yarl import URL
 
 from ..base_functions.base_functions import adjust, logger
 from ..base_functions.error_classes import DownloadFailure, InvalidContentTypeFailure
 from ..downloader.downloader_utils import CustomHTTPStatus
 from ..downloader.progress_definitions import file_progress
-from .rate_limiting import AsyncRateLimiter, throttle
+from .rate_limiting import AsyncRateLimiter
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from rich.progress import TaskID
 
     from ..base_functions.data_classes import MediaItem
@@ -128,29 +129,47 @@
                 await f.write(chunk)
                 update_progress(len(chunk))
 
     async def _download(self, media: MediaItem, current_throttle: int, proxy: str, headers: dict,
                         save_content: Callable[[aiohttp.StreamReader, int], None]) -> None:
         headers['Referer'] = str(media.referer)
         headers['user-agent'] = self.client.user_agent
-        await throttle(self, current_throttle, media.url.host)
+        await self._throttle(current_throttle, media.url.host)
         async with self.client_session.get(media.url, headers=headers, ssl=self.client.ssl_context,
                                            raise_for_status=True, proxy=proxy) as resp:
             content_type = resp.headers.get('Content-Type')
             if not content_type:
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="No content-type in response header")
             if resp.url in self.bunkr_maintenance:
                 raise DownloadFailure(code=HTTPStatus.SERVICE_UNAVAILABLE, message="Bunkr under maintenance")
             if any(s in content_type.lower() for s in ('html', 'text')):
                 logger.debug("Server for %s is experiencing issues, you are being ratelimited, or cookies have expired", str(media.url))
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="Unexpectedly got text as response")
 
             size = int(resp.headers.get('Content-Length', '0'))
             await save_content(resp.content, size)
 
+    async def _throttle(self, delay: int, host: str) -> None:
+        """Throttles requests to domains by a parameter amount of time"""
+        if delay is None or delay == 0:
+            return
+
+        key = f'throttle:{host}'
+        while True:
+            now = time.time()
+            last = self.throttle_times.get(key, 0.0)
+            elapsed = now - last
+
+            if elapsed >= delay:
+                self.throttle_times[key] = now
+                return
+
+            remaining = delay - elapsed + 0.1
+            await asyncio.sleep(remaining)
+
     async def download_file(self, media: MediaItem, file: Path, current_throttle: int, resume_point: int,
                             proxy: str, headers: dict, file_task: TaskID):
 
         async def save_content(content: aiohttp.StreamReader, size: int):
             file_progress.update(file_task, total=size + resume_point)
             file_progress.advance(file_task, resume_point)
             await self._append_content(file, content, lambda chunk_len: file_progress.advance(file_task, chunk_len))
@@ -166,15 +185,15 @@
                       initial=resume_point, desc=task_description) as progress:
                 await self._append_content(file, content, lambda chunk_len: progress.update(chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
     async def get_filesize(self, url: URL, referer: str, current_throttle: int):
         headers = {'Referer': referer, 'user-agent': self.client.user_agent}
-        await throttle(self, current_throttle, url.host)
+        await self._throttle(current_throttle, url.host)
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context,
                                            raise_for_status=True) as resp:
             return int(resp.headers.get('Content-Length', str(0)))
 
     async def exit_handler(self):
         try:
             await self.client_session.close()
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/client/rate_limiting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 import asyncio
 import collections
-import time
-
 from datetime import datetime
-from types import TracebackType
-from typing import Optional, Callable, Awaitable, Any, Type
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Optional, Type
+
+if TYPE_CHECKING:
+    from types import TracebackType
 
 
 class AsyncRateLimiter:
     """Provides rate limiting for an operation with a configurable number of requests for a time period."""
 
     __lock: asyncio.Lock
     callback: Optional[Callable[[float], Awaitable[Any]]]
@@ -56,28 +58,7 @@
 
             while self._timespan >= self.period:
                 self.calls.popleft()
 
     @property
     def _timespan(self) -> float:
         return self.calls[-1] - self.calls[0]
-
-
-async def throttle(self, delay: int, host: str) -> None:
-    """Throttles requests to domains by a parameter amount of time"""
-    if delay is None or delay == 0:
-        return
-
-    key: Optional[str] = None
-    while True:
-        if key is None:
-            key = f'throttle:{host}'
-        now = time.time()
-        last = self.throttle_times.get(key, 0.0)
-        elapsed = now - last
-
-        if elapsed >= delay:
-            self.throttle_times[key] = now
-            return
-
-        remaining = delay - elapsed + 0.1
-        await asyncio.sleep(remaining)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
 from ..base_functions.base_functions import get_filename_and_ext, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class AnonfilesCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.api_link = URL("https://api.anonfiles.com/v2/file")
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from __future__ import annotations
+
 import re
+from typing import TYPE_CHECKING
 
 from yarl import URL
 
 from ..base_functions.base_functions import (
     FILE_FORMATS,
     get_filename_and_ext,
     log,
     logger,
     make_title_safe,
 )
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class BunkrCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper, remove_bunkr_id: bool):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
@@ -146,15 +151,14 @@
 
                 try:
                     filename, ext = await get_filename_and_ext(link.name)
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
 
-                referer = link
                 if "v" in link.parts or "d" in link.parts:
                     media = await self.get_file(session, link)
                     link = media.url
                 elif ext in FILE_FORMATS["Images"]:
                     link = URL(str(link).replace("https://cdn", "https://i"))
                 else:
                     link = URL(f"https://media-files{media_loc}.bunkr.ru" + link.path)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from __future__ import annotations
+
 import asyncio
+from typing import TYPE_CHECKING
 
 from bs4 import BeautifulSoup
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import CascadeItem, MediaItem
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import CascadeItem
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class CoomenoCrawler:
     def __init__(self, *, include_id=False, scraping_mapper, separate_posts=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.scraping_mapper = scraping_mapper
@@ -45,23 +50,19 @@
         text_selector = 'div[class=post__content] a'
 
         title = "Loose Coomer Files"
         if "thumbnail" in url.parts:
             parts = [x for x in url.parts if x not in ("thumbnail", "/")]
             link = URL("https://coomer.party/" + "/".join(parts))
 
-            complete = await self.SQL_Helper.check_complete_singular("coomer", link)
-            filename, ext = await get_filename_and_ext(link.name)
-            media_item = MediaItem(link, url, complete, filename, ext, filename)
+            media_item = await create_media_item(link, url, self.SQL_Helper, "coomer")
             await cascade.add_to_album("coomer", title, media_item)
 
         elif "data" in url.parts:
-            complete = await self.SQL_Helper.check_complete_singular("coomer", url)
-            filename, ext = await get_filename_and_ext(url.name)
-            media_item = MediaItem(url, url, complete, filename, ext, filename)
+            media_item = await create_media_item(url, url, self.SQL_Helper, "coomer")
             await cascade.add_to_album("coomer", title, media_item)
 
         elif "post" in url.parts:
             title = await self.parse_post(session, url, "coomer", cascade, images_selector, downloads_selector,
                                           text_selector)
 
         else:
@@ -79,23 +80,19 @@
         text_selector = 'div[class=post__content] a'
 
         title = "Loose Kemono Files"
         if "thumbnail" in url.parts:
             parts = [x for x in url.parts if x not in ("thumbnail", "/")]
             link = URL("https://kemono.party/" + "/".join(parts))
 
-            complete = await self.SQL_Helper.check_complete_singular("kemono", link)
-            filename, ext = await get_filename_and_ext(link.name)
-            media_item = MediaItem(link, url, complete, filename, ext, filename)
+            media_item = await create_media_item(link, url, self.SQL_Helper, "kemono")
             await cascade.add_to_album("kemono", title, media_item)
 
         elif "data" in url.parts:
-            complete = await self.SQL_Helper.check_complete_singular("kemono", url)
-            filename, ext = await get_filename_and_ext(url.name)
-            media_item = MediaItem(url, url, complete, filename, ext, filename)
+            media_item = await create_media_item(url, url, self.SQL_Helper, "kemono")
             await cascade.add_to_album("kemono", title, media_item)
 
         elif "post" in url.parts:
             title = await self.parse_post(session, url, "kemono", cascade, images_selector, downloads_selector,
                                           text_selector)
 
         else:
@@ -172,29 +169,25 @@
             images = soup.select(images_selector)
             for image in images:
                 href = image.get('href')
                 if href.startswith("/"):
                     link = URL("https://" + url.host + href)
                 else:
                     link = URL(href)
-                complete = await self.SQL_Helper.check_complete_singular(domain, link)
-                filename, ext = await get_filename_and_ext(link.name)
-                media_item = MediaItem(link, url, complete, filename, ext, filename)
+                media_item = await create_media_item(link, url, self.SQL_Helper, domain)
                 await cascade.add_to_album(domain, title, media_item)
 
             downloads = soup.select(downloads_selector)
             for download in downloads:
                 href = download.get('href')
                 if href.startswith("/"):
                     link = URL("https://" + url.host + href)
                 else:
                     link = URL(href)
-                complete = await self.SQL_Helper.check_complete_singular(domain, link)
-                filename, ext = await get_filename_and_ext(link.name)
-                media_item = MediaItem(link, url, complete, filename, ext, filename)
+                media_item = await create_media_item(link, url, self.SQL_Helper, domain)
                 await cascade.add_to_album(domain, title, media_item)
 
             text_content = soup.select(text_selector)
             await self.map_links(text_content, title, url)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+from __future__ import annotations
+
+import contextlib
+from typing import TYPE_CHECKING
+
 from bs4 import BeautifulSoup
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import DomainItem, MediaItem
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class CyberFileCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.load_files = URL('https://cyberfile.me/account/ajax/load_files')
@@ -76,22 +83,19 @@
                 title = await make_title_safe(title)
 
 
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
             total_pages = int(soup.select("a[onclick*=loadImages]")[-1].get('onclick').split(',')[2])
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
-                try:
+                with contextlib.suppress(TypeError):
                     nodes.append(int(listing.get('folderid')))
-                except TypeError:
-                    pass
-                try:
+
+                with contextlib.suppress(TypeError):
                     contents.append((title, int(listing.get('fileid'))))
-                except TypeError:
-                    pass
 
             if page < total_pages:
                 contents.extend(await self.get_folder_content(session, url, nodeId, page+1, original_title))
             for node in nodes:
                 contents.extend(await self.get_folder_content(session, url, node, 1, title))
             return contents
 
@@ -135,23 +139,20 @@
             content = await session.post(self.load_files, data)
             text = content['html']
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
             total_pages = int(soup.select_one('input[id=rspTotalPages]').get('value'))
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 title = await make_title_safe(content['page_title'])
-                try:
+                with contextlib.suppress(TypeError, AttributeError):
                     title = title + '/' + await make_title_safe(listing.select_one('span[class=filename]').text)
                     nodes.append((title, int(listing.get('folderid'))))
-                except (TypeError, AttributeError):
-                    pass
-                try:
+
+                with contextlib.suppress(TypeError):
                     contents.append((title, int(listing.get('fileid'))))
-                except TypeError:
-                    pass
 
             if page < total_pages:
                 nodes_temp, content_temp = await self.get_shared_ids_and_content(session, url, page + 1)
                 nodes.extend(nodes_temp)
                 contents.extend(content_temp)
             return nodes, contents
 
@@ -173,24 +174,21 @@
 
             title = title if title else content['page_title']
 
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
             total_pages = int(soup.select("a[onclick*=loadImages]")[-1].get('onclick').split(',')[2])
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
-                try:
+                with contextlib.suppress(TypeError, AttributeError):
                     filename = listing.select_one('span[class=filename]')
                     temp_title = title + '/' + await make_title_safe(filename.text)
                     nodes.append((temp_title, int(listing.get('folderid'))))
-                except (TypeError, AttributeError):
-                    pass
-                try:
+
+                with contextlib.suppress(TypeError):
                     contents.append((title, int(listing.get('fileid'))))
-                except TypeError:
-                    pass
 
             if page < total_pages:
                 contents.extend(await self.get_shared_content(session, url, nodeId, page + 1, title))
             for title, node in nodes:
                 contents.extend(await self.get_shared_content(session, url, node, 1, title))
             return contents
 
@@ -214,21 +212,19 @@
 
                 if menu:
                     html_download_text = menu.get("onclick")
                     link = URL(html_download_text.replace("openUrl('", "").replace("'); return false;", ""))
                 elif button:
                     html_download_text = button.get("onclick")
                     link = URL(html_download_text.replace("openUrl('", "").replace("'); return false;", ""))
-                complete = await self.SQL_Helper.check_complete_singular("cyberfile", link)
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    media = await create_media_item(link, url, self.SQL_Helper, "cyberfile")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
-                media = MediaItem(link, url, complete, filename, ext, filename)
 
                 download_links.append((title, media))
             return download_links
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,51 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
 from ..base_functions.base_functions import (
     check_direct,
-    get_filename_and_ext,
+    create_media_item,
     log,
     logger,
     make_title_safe,
 )
-from ..base_functions.data_classes import AlbumItem, MediaItem
-from ..base_functions.error_classes import NoExtensionFailure, InvalidContentTypeFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+from ..base_functions.data_classes import AlbumItem
+from ..base_functions.error_classes import InvalidContentTypeFailure, NoExtensionFailure
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class CyberdropCrawler:
     def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Cyberdrop scraper"""
         album_obj = AlbumItem("Loose Cyberdrop Files", [])
 
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         if await check_direct(url):
-            complete = await self.SQL_Helper.check_complete_singular("cyberdrop", url)
-            filename, ext = await get_filename_and_ext(url.name)
-            media = MediaItem(url, url, complete, filename, ext, filename)
+            media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
             await album_obj.add_media(media)
             await self.SQL_Helper.insert_album("cyberdrop", URL(""), album_obj)
             await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
             return album_obj
 
         try:
             try:
                 soup = await session.get_BS4(url)
             except InvalidContentTypeFailure:
-                complete = await self.SQL_Helper.check_complete_singular("cyberdrop", url)
-                filename, ext = await get_filename_and_ext(url.name)
-                media = MediaItem(url, url, complete, filename, ext, filename)
+                media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
                 await album_obj.add_media(media)
                 await self.SQL_Helper.insert_album("cyberdrop", URL(""), album_obj)
                 await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
                 return album_obj
 
             title = soup.select_one("h1[id=title]").get_text()
             title = await make_title_safe(title)
@@ -54,21 +56,19 @@
                 title = title + " - " + titlep2
             await album_obj.set_new_title(title)
 
             links = soup.select('div[class="image-container column"] a')
             for link in links:
                 link = URL(link.get('href'))
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    media = await create_media_item(link, url, self.SQL_Helper, "cyberdrop")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
 
-                complete = await self.SQL_Helper.check_complete_singular("cyberdrop", link)
-                media = MediaItem(link, url, complete, filename, ext, filename)
                 await album_obj.add_media(media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import AlbumItem, MediaItem
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import AlbumItem
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class EHentaiCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
@@ -56,17 +62,14 @@
     async def get_image(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets media items from image links"""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("img[id=img]")
             link = URL(image.get('src'))
 
-            complete = await self.SQL_Helper.check_complete_singular("e-hentai", link)
-
-            filename, ext = await get_filename_and_ext(link.name)
-            media_item = MediaItem(link, url, complete, filename, ext, filename)
+            media_item = await create_media_item(link, url, self.SQL_Helper, "e-hentai")
             await album_obj.add_media(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import DomainItem, MediaItem
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class EromeCrawler:
     def __init__(self, *, include_id: bool, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
@@ -38,32 +44,28 @@
                 title = title + " - " + url.name
             title = await make_title_safe(title)
 
             # Images
             for link in soup.select('img[class="img-front lasyload"]'):
                 link = URL(link['data-src'])
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    media = await create_media_item(link, url, self.SQL_Helper, "erome")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(url))
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("erome", link)
-                media = MediaItem(link, url, complete, filename, ext, filename)
                 await domain_obj.add_media(title, media)
 
             # Videos
             for link in soup.select('div[class=media-group] div[class=video-lg] video source'):
                 link = URL(link['src'])
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    media = await create_media_item(link, url, self.SQL_Helper, "erome")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("erome", link)
-                media = MediaItem(link, url, complete, filename, ext, filename)
                 await domain_obj.add_media(title, media)
 
             await self.SQL_Helper.insert_domain("erome", url, domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-from typing import Optional
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Optional
 
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import AlbumItem, MediaItem
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.data_classes import MediaItem
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class FapelloCrawler:
     def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
@@ -56,44 +61,40 @@
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return None
 
-    async def parse_post(self, session: ScrapeSession, url: URL):
-        """Parses posts, returns list of media_items"""
+    async def parse_post(self, session: ScrapeSession, url: URL) -> list[MediaItem]:
+        """Parses posts, returns list of MediaItem"""
+        results = []
         try:
             soup = await session.get_BS4(url)
-            results = []
 
             content_section = soup.select_one('div[class="flex justify-between items-center"]')
 
             images = content_section.select("img")
             for image in images:
                 download_link = URL(image.get('src'))
                 try:
-                    filename, ext = await get_filename_and_ext(download_link.name)
+                    media_item = await create_media_item(download_link, url, self.SQL_Helper, "fapello")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(download_link))
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("fapello", download_link)
-                results.append(MediaItem(download_link, url, complete, filename, ext, filename))
+                results.append(media_item)
 
             videos = content_section.select("source")
             for video in videos:
                 download_link = URL(video.get('src'))
                 try:
-                    filename, ext = await get_filename_and_ext(download_link.name)
+                    media_item = await create_media_item(download_link, url, self.SQL_Helper, "fapello")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(download_link))
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("fapello", download_link)
-                results.append(MediaItem(download_link, url, complete, filename, ext, filename))
-
-            return results
-
+                results.append(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
-            return
+
+        return results
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger
-from ..base_functions.data_classes import AlbumItem, MediaItem
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+from ..base_functions.base_functions import create_media_item, log, logger
+from ..base_functions.data_classes import AlbumItem
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class GfycatCrawler:
     def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
@@ -26,17 +32,15 @@
                 link = URL(src.get("src"))
                 if "giant" in link.host:
                     video_link = link
                     break
             if video_link is None:
                 video_link = URL(video_srcs[0].get("src"))
 
-            complete = await self.SQL_Helper.check_complete_singular("gfycat", video_link)
-            filename, ext = await get_filename_and_ext(video_link.name)
-            media_item = MediaItem(video_link, url, complete, filename, ext, filename)
+            media_item = await create_media_item(video_link, url, self.SQL_Helper, "gfycat")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("gfycat", video_link, album_obj)
             await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+from __future__ import annotations
+
 import http
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 from yarl import URL
 
 from ..base_functions.base_functions import log, logger, make_title_safe, get_filename_and_ext
 from ..base_functions.data_classes import DomainItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class GoFileCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import AlbumItem, MediaItem
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import AlbumItem
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class HGameCGCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
@@ -30,18 +36,15 @@
 
             images = soup.select("div[class=image] a")
             for image in images:
                 image = image.get('href')
                 image = URL("https://" + url.host + image)
                 link = await self.get_image(session, image)
 
-                complete = await self.SQL_Helper.check_complete_singular("hgamecg", link)
-
-                filename, ext = await get_filename_and_ext(link.name)
-                media_item = MediaItem(link, image, complete, filename, ext, filename)
+                media_item = await create_media_item(link, image, self.SQL_Helper, "hgamecg")
                 await album_obj.add_media(media_item)
 
             next_page = soup.find("a", text="Next Page")
             if next_page is not None:
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL("https://" + url.host + next_page)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,71 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import (
-    check_direct,
-    get_filename_and_ext,
-    log,
-    logger,
-    make_title_safe,
-)
-from ..base_functions.data_classes import AlbumItem, MediaItem
-from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import AlbumItem
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
-class ImgBoxCrawler:
-    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
+class PimpAndHostCrawler:
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
-        """Director func for ImgBox scraping"""
-        album_obj = AlbumItem("Loose ImgBox Files", [])
+        """Director for pimpandhost scraping"""
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
-        try:
-            if await check_direct(url):
-                filename, ext = await get_filename_and_ext(url.name)
-                complete = await self.SQL_Helper.check_complete_singular("imgbox", url)
-                media_item = MediaItem(url, url, complete, filename, ext, filename)
-                await album_obj.add_media(media_item)
-
-            elif "g" in url.parts:
-                title, images = await self.folder(session, url)
-                if not title:
-                    title = url.raw_name
-                title = await make_title_safe(title)
-                await album_obj.set_new_title(title)
-                for img in images:
-                    try:
-                        filename, ext = await get_filename_and_ext(img.name)
-                    except NoExtensionFailure:
-                        logger.debug("Couldn't get extension for %s", str(img))
-                        continue
-                    complete = await self.SQL_Helper.check_complete_singular("imgbox", img)
-                    media_item = MediaItem(img, url, complete, filename, ext, filename)
+        if url.parts[1] == 'album':
+            media_items, title = await self.get_listings(session, url)
+            await album_obj.set_new_title(title)
+            if media_items:
+                for media_item in media_items:
                     await album_obj.add_media(media_item)
-            else:
-                img = await self.singular(session, url)
-                filename, ext = await get_filename_and_ext(img.name)
-                complete = await self.SQL_Helper.check_complete_singular("imgbox", img)
-                media_item = MediaItem(img, url, complete, filename, ext, filename)
-                await album_obj.add_media(media_item)
+        else:
+            media_item = await self.get_singular(session, url)
+            await album_obj.add_media(media_item)
+
+        await self.SQL_Helper.insert_album("pimpandhost", url, album_obj)
+        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        return album_obj
+
+    async def get_listings(self, session: ScrapeSession, url: URL):
+        """Handles album media"""
+        media_items = []
+        try:
+            soup = await session.get_BS4(url)
+            title = soup.select_one("div[class=image-header]")
+            user_link = title.select_one("span[class=details]")
+            user_link.decompose()
+            title = await make_title_safe(title.get_text())
+
+            for file in soup.select('a[class*="image-wrapper center-cropped im-wr"]'):
+                link = file.get("href")
+                media_items.append(await self.get_singular(session, link))
+            return media_items, title
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-        await self.SQL_Helper.insert_album("imgbox", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
-        return album_obj
-
-    async def folder(self, session: ScrapeSession, url: URL):
-        """Gets links from a folder"""
-        soup = await session.get_BS4(url)
-        output = []
-        title = soup.select_one("div[id=gallery-view] h1").get_text()
-
-        images = soup.find('div', attrs={'id': 'gallery-view-content'})
-        images = images.findAll("img")
-        for link in images:
-            link = link.get('src').replace("thumbs", "images").replace("_b", "_o")
-            output.append(URL(link))
-
-        return title, output
-
-    async def singular(self, session: ScrapeSession, url: URL) -> URL:
-        """Gets individual links"""
-        soup = await session.get_BS4(url)
-        return URL(soup.select_one("img[id=img]").get('src'))
+    async def get_singular(self, session: ScrapeSession, url: URL):
+        """Handles singular files"""
+        try:
+            soup = await session.get_BS4(url)
+            img = soup.select_one("a img")
+            img = img.get("src")
+            if img.startswith("//"):
+                img = URL("https:" + img)
+            return await create_media_item(img, url, self.SQL_Helper, "pimpandhost")
+        except Exception as e:
+            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
+            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,73 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import (
-    check_direct,
-    get_filename_and_ext,
-    log,
-    logger,
-    make_title_safe,
-)
+from ..base_functions.base_functions import get_filename_and_ext, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
-class LoveFapCrawler:
+class PixelDrainCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
-        self.SQL_Helper = SQL_Helper
         self.quiet = quiet
+        self.SQL_Helper = SQL_Helper
+        self.api = URL('https://pixeldrain.com/api/')
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
-        """Director for lovefap scraping"""
-        album_obj = AlbumItem("Loose LoveFap Files", [])
-
+        """Director for pixeldrain scraping"""
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
-        if await check_direct(url):
-            complete = await self.SQL_Helper.check_complete_singular("lovefap", url)
-            filename, ext = await get_filename_and_ext(url.name)
-            media = MediaItem(url, url, complete, filename, ext, filename)
-            await album_obj.add_media(media)
-            await self.SQL_Helper.insert_album("lovefap", URL(""), album_obj)
-            await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
-            return album_obj
-
-        try:
-            if "video" in url.parts:
-                await self.fetch_video(session, url, album_obj)
-            else:
-                await self.fetch_album(session, url, album_obj)
+        album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
-        except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
-            logger.debug(e)
-            return album_obj
+        identifier = str(url).split('/')[-1]
+        if url.parts[1] == 'l':
+            await album_obj.set_new_title(url.name)
+            media_items = await self.get_listings(session, identifier, url)
+            for media_item in media_items:
+                await album_obj.add_media(media_item)
+        else:
+            link = await self.create_download_link(identifier)
+            complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
+            filename, ext = await get_filename_and_ext(await self.get_file_name(session, identifier))
+            media_item = MediaItem(link, url, complete, filename, ext, filename)
+            await album_obj.add_media(media_item)
 
-        await self.SQL_Helper.insert_album("lovefap", url, album_obj)
+        await self.SQL_Helper.insert_album("pixeldrain", url, album_obj)
         await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
-    async def fetch_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
-        """Gets media_items for albums, and adds them to the Album_obj"""
-        soup = await session.get_BS4(url)
-
-        title = soup.select_one('div[class=albums-content-header] span[style*="float: left"]').get_text()
-        if title is None:
-            title = url.name
-        title = await make_title_safe(title)
-        await album_obj.set_new_title(title)
-
-        links = soup.select('div[class="file picture"] a')
-        links.extend(soup.select('div[class="file picture"] a'))
-        for link in links:
-            link = link.get('href')
-            if link.startswith('/'):
-                link = url.host + link
-            link = URL(link)
-            if "video" in link.parts:
-                await self.fetch_video(session, url, album_obj)
-            else:
+    async def get_listings(self, session: ScrapeSession, identifier: str, url: URL) -> list[MediaItem]:
+        """Handles album scraping"""
+        media_items = []
+        try:
+            content = await session.get_json(self.api / "list" / identifier)
+            for file in content['files']:
+                link = await self.create_download_link(file['id'])
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    filename, ext = await get_filename_and_ext(file['name'])
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
+                complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
+                media_item = MediaItem(link, url, complete, filename, ext, filename)
+                media_items.append(media_item)
+        except Exception as e:
+            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
+            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug(e)
+
+        return media_items
 
-                complete = await self.SQL_Helper.check_complete_singular("lovefap", link)
-                media = MediaItem(link, url, complete, filename, ext, filename)
-                await album_obj.add_media(media)
-
-    async def fetch_video(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
-        """Gets media_items for video links"""
-        soup = await session.get_BS4(url)
-        video = soup.select_one("video[id=main-video] source")
-        if video:
-            link = URL(video.get("src"))
-            try:
-                filename, ext = await get_filename_and_ext(link.name)
-            except NoExtensionFailure:
-                logger.debug("Couldn't get extension for %s", str(link))
-                return
-
-            complete = await self.SQL_Helper.check_complete_singular("lovefap", link)
-            media = MediaItem(link, url, complete, filename, ext, filename)
-            await album_obj.add_media(media)
+    async def get_file_name(self, session: ScrapeSession, identifier: str) -> str:
+        """Gets filename for the given file identifier"""
+        content = await session.get_json(self.api / 'file' / identifier / 'info')
+        return content['name']
+
+    async def create_download_link(self, file: str) -> URL:
+        """Gets download links for the file given"""
+        return (self.api / 'file' / file).with_query('download')
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from __future__ import annotations
+
 import itertools
+from typing import TYPE_CHECKING
 
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import MediaItem, DomainItem
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class NSFWXXXCrawler:
     def __init__(self, quiet: bool, separate_posts: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
@@ -74,21 +79,19 @@
             content_obj.extend(soup.select("video source"))
             content_obj.extend(soup.select('div[class="sh-section__images sh-section__images_gallery row"] div a img'))
 
             for content in content_obj:
                 link = URL(content.get("src"))
                 if "-mobile" in link.name or ".webm" in link.name:
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("nsfw.xxx", link)
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    media = await create_media_item(link, url, self.SQL_Helper, "nsfw.xxx")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
-                media = MediaItem(link, url, complete, filename, ext, filename)
 
                 title = f"{model}/{post_name}" if self.separate_posts else model
                 await domain_obj.add_media(title, media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,81 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger
-from ..base_functions.data_classes import AlbumItem, MediaItem
+from ..base_functions.base_functions import (
+    check_direct,
+    create_media_item,
+    log,
+    logger,
+    make_title_safe,
+)
+from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
-class PixelDrainCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
+class ImgBoxCrawler:
+    def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
-        self.api = URL('https://pixeldrain.com/api/')
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
-        """Director for pixeldrain scraping"""
+        """Director func for ImgBox scraping"""
+        album_obj = AlbumItem("Loose ImgBox Files", [])
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
-        album_obj = AlbumItem("Loose Pixeldrain Files", [])
-
-        identifier = str(url).split('/')[-1]
-        if url.parts[1] == 'l':
-            await album_obj.set_new_title(url.name)
-            media_items = await self.get_listings(session, identifier, url)
-            if media_items:
-                for media_item in media_items:
-                    await album_obj.add_media(media_item)
-        else:
-            link = await self.create_download_link(identifier)
-            complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
-            filename, ext = await get_filename_and_ext(await self.get_file_name(session, identifier))
-            media_item = MediaItem(link, url, complete, filename, ext, filename)
-            await album_obj.add_media(media_item)
-
-        await self.SQL_Helper.insert_album("pixeldrain", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
-        return album_obj
 
-    async def get_listings(self, session: ScrapeSession, identifier: str, url: URL):
-        """Handles album scraping"""
-        media_items = []
         try:
-            content = await session.get_json(self.api / "list" / identifier)
-            for file in content['files']:
-                link = await self.create_download_link(file['id'])
-                try:
-                    filename, ext = await get_filename_and_ext(file['name'])
-                except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
-                    continue
-                complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
-                media_item = MediaItem(link, url, complete, filename, ext, filename)
-                media_items.append(media_item)
-            return media_items
+            if await check_direct(url):
+                media_item = await create_media_item(url, url, self.SQL_Helper, "imgbox")
+                await album_obj.add_media(media_item)
+
+            elif "g" in url.parts:
+                title, images = await self.folder(session, url)
+                if not title:
+                    title = url.raw_name
+                title = await make_title_safe(title)
+                await album_obj.set_new_title(title)
+                for img in images:
+                    try:
+                        media_item = await create_media_item(img, url, self.SQL_Helper, "imgbox")
+                    except NoExtensionFailure:
+                        logger.debug("Couldn't get extension for %s", str(img))
+                        continue
+                    await album_obj.add_media(media_item)
+            else:
+                img = await self.singular(session, url)
+                media_item = await create_media_item(img, url, self.SQL_Helper, "imgbox")
+                await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_file_name(self, session: ScrapeSession, identifier: str) -> str:
-        """Gets filename for the given file identifier"""
-        content = await session.get_json(self.api / 'file' / identifier / 'info')
-        return content['name']
-
-    async def create_download_link(self, file: str) -> URL:
-        """Gets download links for the file given"""
-        return (self.api / 'file' / file).with_query('download')
+        await self.SQL_Helper.insert_album("imgbox", url, album_obj)
+        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        return album_obj
+
+    async def folder(self, session: ScrapeSession, url: URL):
+        """Gets links from a folder"""
+        soup = await session.get_BS4(url)
+        output = []
+        title = soup.select_one("div[id=gallery-view] h1").get_text()
+
+        images = soup.find('div', attrs={'id': 'gallery-view-content'})
+        images = images.findAll("img")
+        for link in images:
+            link = link.get('src').replace("thumbs", "images").replace("_b", "_o")
+            output.append(URL(link))
+
+        return title, output
+
+    async def singular(self, session: ScrapeSession, url: URL) -> URL:
+        """Gets individual links"""
+        soup = await session.get_BS4(url)
+        return URL(soup.select_one("img[id=img]").get('src'))
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+from __future__ import annotations
+
 import itertools
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger
+from ..base_functions.base_functions import create_media_item, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class PostImgCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
@@ -40,36 +45,30 @@
 
     async def get_folder(self, session: ScrapeSession, url: URL):
         """Handles folder scraping"""
         album = url.raw_name
         data = {"action": "list", "album": album}
         content = []
         for i in itertools.count(1):
-            data_used = data
-            data_used["page"] = i
-            data_out = await session.post(URL("https://postimg.cc/json"), data_used)
+            data["page"] = i
+            data_out = await session.post(URL("https://postimg.cc/json"), data)
             if data_out['status_code'] != HTTPStatus.OK or not data_out['images']:
                 break
             for item in data_out['images']:
                 referer = URL("https://postimg.cc/" + item[0])
                 img = URL(item[4].replace(item[0], item[1]))
 
                 try:
-                    filename, ext = await get_filename_and_ext(img.name)
+                    media_item = await create_media_item(img, referer, self.SQL_Helper, "postimg")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(img))
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("postimg", img)
-                media_item = MediaItem(img, referer, complete, filename, ext, filename)
 
                 content.append(media_item)
         return content
 
     async def get_singular(self, session: ScrapeSession, url: URL) -> MediaItem:
         """Handles singular folder scraping"""
         soup = await session.get_BS4(url)
         link = URL(soup.select_one("a[id=download]").get('href').replace("?dl=1", ""))
 
-        filename, ext = await get_filename_and_ext(link.name)
-        complete = await self.SQL_Helper.check_complete_singular("postimg", link)
-
-        return MediaItem(link, url, complete, filename, ext, filename)
+        return await create_media_item(link, url, self.SQL_Helper, "postimg")
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from __future__ import annotations
+
 import asyncio
 import re
+from typing import TYPE_CHECKING
 
 from yarl import URL
 
 from ..base_functions.base_functions import (
     check_direct,
-    get_filename_and_ext,
+    create_media_item,
     log,
     logger,
     make_title_safe,
 )
-from ..base_functions.data_classes import DomainItem, MediaItem
+from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class ShareXCrawler:
     def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
@@ -27,17 +32,15 @@
         domain_obj = DomainItem(url.host.lower(), {})
 
         await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         if await check_direct(url):
             url = url.with_name(url.name.replace('.md.', '.').replace('.th.', '.'))
             url = await self.jpg_fish_from_church(url)
-            complete = await self.SQL_Helper.check_complete_singular("sharex", url)
-            filename, ext = await get_filename_and_ext(url.name)
-            media_item = MediaItem(url, url, complete, filename, ext, filename)
+            media_item = await create_media_item(url, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         elif "album" in url.parts or "a" in url.parts:
             await self.parse(session=session, url=url, domain_obj=domain_obj)
         elif "albums" in url.parts:
             await self.get_albums(session, url, domain_obj)
         elif 'image' in url.parts or 'img' in url.parts or 'images' in url.parts:
             await self.get_singular(session, url, domain_obj)
@@ -80,17 +83,15 @@
         await asyncio.sleep(1)
         try:
             soup = await session.get_BS4(url)
             link = URL(soup.select_one("input[id=embed-code-2]").get('value'))
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
             link = await self.jpg_fish_from_church(link)
 
-            complete = await self.SQL_Helper.check_complete_singular("sharex", link)
-            filename, ext = await get_filename_and_ext(link.name)
-            media_item = MediaItem(link, url, complete, filename, ext, filename)
+            media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str, domain_obj: DomainItem):
@@ -135,20 +136,18 @@
                 links = soup.select("a[href*=image] img")
             for link in links:
                 link = URL(link.get('src'))
                 link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
                 link = await self.jpg_fish_from_church(link)
 
                 try:
-                    filename, ext = await get_filename_and_ext(link.name)
+                    media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
-                complete = await self.SQL_Helper.check_complete_singular("sharex", link)
-                media_item = MediaItem(link, url, complete, filename, ext, filename)
                 await domain_obj.add_media(title, media_item)
 
             next_page = soup.select_one('li.pagination-next a')
             if not next_page:
                 next_page = soup.select_one('a[data-pagination=next]')
             if next_page is not None:
                 next_page = next_page.get('href')
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,49 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from yarl import URL
 
-from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
-from ..base_functions.data_classes import AlbumItem, MediaItem
+from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
+from ..base_functions.data_classes import AlbumItem
 from ..base_functions.error_classes import NoExtensionFailure
-from ..base_functions.sql_helper import SQLHelper
-from ..client.client import ScrapeSession
+
+if TYPE_CHECKING:
+    from ..base_functions.sql_helper import SQLHelper
+    from ..client.client import ScrapeSession
 
 
 class XBunkrCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for XBunkr scraping"""
         album_obj = AlbumItem("Loose XBunkr Files", [])
 
         try:
             if "media" in url.host:
-                complete = await self.SQL_Helper.check_complete_singular("xbunkr", url)
-                filename, ext = await get_filename_and_ext(url.name)
-                media_item = MediaItem(url, url, complete, filename, ext, filename)
+                media_item = await create_media_item(url, url, self.SQL_Helper, "xbunkr")
                 await album_obj.add_media(media_item)
 
             else:
                 soup = await session.get_BS4(url)
                 links = soup.select("a[class=image]")
                 title = await make_title_safe(soup.select_one("h1[id=title]").text)
                 title = title.strip()
                 await album_obj.set_new_title(title)
                 for link in links:
                     link = URL(link.get('href'))
                     try:
-                        filename, ext = await get_filename_and_ext(link.name)
+                        media_item = await create_media_item(link, url, self.SQL_Helper, "xbunkr")
                     except NoExtensionFailure:
                         logger.debug("Couldn't get extension for %s", str(link))
                         continue
-                    complete = await self.SQL_Helper.check_complete_singular("xbunkr", link)
-                    media_item = MediaItem(link, url, complete, filename, ext, filename)
                     await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             await log("Error scraping " + str(url), quiet=self.quiet)
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+from __future__ import annotations
+
 import multiprocessing
 import shutil
 from base64 import b64encode
 from enum import IntEnum
 from functools import wraps
 from http import HTTPStatus
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from cyberdrop_dl.base_functions.base_functions import FILE_FORMATS, logger
-from cyberdrop_dl.base_functions.data_classes import MediaItem
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from cyberdrop_dl.base_functions.data_classes import MediaItem
+
 
 class CustomHTTPStatus(IntEnum):
     WEB_SERVER_IS_DOWN = 521
     IM_A_TEAPOT = 418
 
 
 async def allowed_filetype(media: MediaItem, block_images: bool, block_video: bool, block_audio: bool, block_other: bool):
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import itertools
 import logging
 from http import HTTPStatus
 from random import gauss
 from typing import TYPE_CHECKING
 
 import aiofiles
@@ -246,23 +247,19 @@
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
                 aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
                 DownloadFailure, FileNotFoundError, PermissionError) as e:
             if await self.File_Lock.check_lock(filename):
                 await self.File_Lock.remove_lock(filename)
 
-            new_error = DownloadFailure(code=1)
-            try:
+            with contextlib.suppress(Exception):
                 file_progress.update(file_task, visible=False)
-            except Exception:
-                pass
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
-            new_error.message = repr(e)
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", str(e.code))
                     await log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
@@ -279,17 +276,16 @@
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
 
                 logger.debug("Error status code: " + str(e.code))
-                new_error.code = e.code
 
-            raise new_error
+            raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     async def output_failed(self, media, e):
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
     async def check_file_exists(self, complete_file, partial_file, media, album, url_path, original_filename,
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,19 +196,16 @@
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
                 aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
                 DownloadFailure, PermissionError) as e:
             if await self.File_Lock.check_lock(original_filename):
                 await self.File_Lock.remove_lock(original_filename)
 
-            new_error = DownloadFailure(code=1)
-
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
-            new_error.message = repr(e)
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", str(e.code))
                     await log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
@@ -223,17 +220,16 @@
                     await log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 logger.debug("Error status code: " + str(e.code))
-                new_error.code = e.code
 
-            raise new_error
+            raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     async def output_failed(self, media, e):
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
     async def check_file_exists(self, complete_file, partial_file, media, album, url_path, original_filename,
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import asyncio
+import contextlib
 import logging
 import re
 from pathlib import Path
 
 import aiofiles
 from yarl import URL
 
@@ -290,18 +291,16 @@
     logging.basicConfig(
         filename=args["Files"]["log_file"],
         level=logging.DEBUG,
         format="%(asctime)s:%(levelname)s:%(module)s:%(filename)s:%(lineno)d:%(message)s",
         filemode="w"
     )
 
-    try:
+    with contextlib.suppress(RuntimeError):
         loop = asyncio.get_event_loop()
         loop.run_until_complete(director(args, links))
-    except RuntimeError:
-        pass
 
 
 if __name__ == '__main__':
     print("""STOP! If you're just trying to download files, check the README.md file for instructions.
     If you're developing this project, use start.py instead.""")
     exit()
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from __future__ import annotations
+
 import logging
+from typing import TYPE_CHECKING
 
 from myjdapi import myjdapi
-from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.error_classes import JDownloaderFailure
 
+if TYPE_CHECKING:
+    from yarl import URL
+
 
 class JDownloader:
     """Class that handles connecting and passing links to JDownloader"""
     def __init__(self, jdownloader_args: dict, quiet: bool):
         self.jdownloader_device = jdownloader_args['jdownloader_device']
         self.jdownloader_username = jdownloader_args['jdownloader_username']
         self.jdownloader_password = jdownloader_args['jdownloader_password']
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.13/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
+
 import asyncio
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 
 import aiofiles
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
-from cyberdrop_dl.base_functions.data_classes import SkipData, CascadeItem, ForumItem, AlbumItem, DomainItem
-from cyberdrop_dl.base_functions.sql_helper import SQLHelper
+from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, ForumItem, SkipData
 from cyberdrop_dl.client.client import Client, ScrapeSession
 from cyberdrop_dl.client.rate_limiting import AsyncRateLimiter
 from cyberdrop_dl.crawlers.Anonfiles_Spider import AnonfilesCrawler
 from cyberdrop_dl.crawlers.Bunkr_Spider import BunkrCrawler
 from cyberdrop_dl.crawlers.Coomeno_Spider import CoomenoCrawler
 from cyberdrop_dl.crawlers.CyberFile_Spider import CyberFileCrawler
 from cyberdrop_dl.crawlers.Cyberdrop_Spider import CyberdropCrawler
@@ -28,14 +29,17 @@
 from cyberdrop_dl.crawlers.PostImg_Spider import PostImgCrawler
 from cyberdrop_dl.crawlers.Saint_Spider import SaintCrawler
 from cyberdrop_dl.crawlers.ShareX_Spider import ShareXCrawler
 from cyberdrop_dl.crawlers.XBunkr_Spider import XBunkrCrawler
 from cyberdrop_dl.crawlers.Xenforo_Spider import XenforoCrawler
 from cyberdrop_dl.scraper.JDownloader_Integration import JDownloader
 
+if TYPE_CHECKING:
+    from cyberdrop_dl.base_functions.sql_helper import SQLHelper
+
 
 class ScrapeMapper:
     """This class maps links to their respective handlers, or JDownloader if they are unsupported"""
     def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool):
         self.args = args
         self.client = client
         self.SQL_Helper = SQL_Helper
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.12
+Version: 4.1.13
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `cyberdrop-dl`
-**Bulk downloader for multiple file hosts** 
+
+**Bulk downloader for multiple file hosts**
 
 [![PyPI version](https://badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/month)](https://pepy.tech/project/cyberdrop-dl)
 [![Downloads](https://static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-dl)
 
 [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp)
 
-
 Brand new and improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top of this it also downloads from different domains simultaneously.
 
 ![Screenshot 2023-02-19 183052](https://user-images.githubusercontent.com/61347133/219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png)
 
-# Support Cyberdrop-DL Development
+## Support Cyberdrop-DL Development
 
 <a href="https://www.buymeacoffee.com/juleswinnft" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
 
 If you want to support me and my effort you can buy me a coffee or send me some crypto:
 
 BTC: bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn
 
 ETH: 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B
 
 XMR: 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
 
-# More Information
-
-Read the Wiki!
+## More Information
 
-https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/
+Read the [Wiki](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/)!
 
-# Supported Sites
+## Supported Sites
 
 | Website                 | Supported Link Types                                                                                                                                                                                                                   |
 |-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Anonfiles               | Download page: Anonfiles.com/...                                                                                                                                                                                                       |
 | Bayfiles                | Download page: Bayfiles.com/...                                                                                                                                                                                                        |
 | Bunkr (ru/su/la)        | Albums: bunkr.ru/a/... <br> Direct Videos: stream.bunkr.ru/v/... <br> Direct links: cdn.bunkr.ru/... <br> Direct links: i.bunkr.ru/... <br> Direct links: files.bunkr.ru/... <br> Direct links: media-files.bunkr.ru/...               |
-| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      | 
+| Coomer.party            | Profiles: coomer.party/... <br> Thumbnail Links: coomer.party/thumbnail/... <br> Data Links: coomer.party/data/... <br> coomer.party/.../post/...                                                                                      |
 | Cyberdrop               | Albums: cyberdrop.me/a/... <br> Direct Videos: fs-0#.cyberdrop.me/... <br> Direct Videos: f.cyberdrop.me/... <br> Direct Images: img-0#.cyberdrop.me/... <br> Direct Images: f.cyberdrop.me/... <br> Also works with .cc, .to, and .nl |
-| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    | 
+| Cyberfile               | folders: cyberfile.su/folder/... <br> shared: cyberfile.su/shared/... <br> Direct: cyberfile.su/...                                                                                                                                    |
 | E-Hentai                | Albums: e-hentai.org/g/... <br> Posts: e-hentai.org/s/...                                                                                                                                                                              |
 | Erome                   | Albums: erome.com/a/...                                                                                                                                                                                                                |
 | Fapello                 | Models: fapello.com/...                                                                                                                                                                                                                |
 | Gallery.DeltaPorno.com  | Albums: Gallery.DeltaPorno.com/album/... <br> Direct Images: Gallery.DeltaPorno.com/image/... <br> User Profile: Gallery.DeltaPorno.com/#USER# <br> All User Albums: Gallery.DeltaPorno.com/#USER#/albums                              |
 | GoFile                  | Albums: gofile.io/d/...                                                                                                                                                                                                                |
 | Gfycat                  | Gif: gfycat.com/...                                                                                                                                                                                                                    |
 | HGameCG                 | Albums: hgamecg.com/.../index.html                                                                                                                                                                                                     |
@@ -65,127 +63,130 @@
 | jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
-| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            | 
+| SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
 | SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
 | XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
 | XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
-# Information
+## Information
 
 **Requires Python 3.7 or higher (3.10 recommended)**
 
-You can get Python from here: https://www.python.org/downloads/
+You can get Python from here: <https://www.python.org/downloads/>
 
 Make sure you tick the check box for "Add python to path"
 ![alt text](https://simp2.jpg.church/PATHe426c23371048def.png)
 
 Mac users will also likely need to open terminal and execute the following command: `xcode-select --install`
 
-# Script Method
+## Script Method
+
 Go to the [releases page](https://github.com/Jules-WinnfieldX/CyberDropDownloader/releases) and download the Cyberdrop_DL.zip file. Extract it to wherever you want the program to be.
 
 Put the links in the URLs.txt file then run `Start Windows.bat` (Windows) or `Start Mac.command` (OS X) or `Start Linux.sh` (Linux).
 
 ** Mac users will need to run the command `chmod +x 'Start Mac.command'` to make the file executable.
 
-# CLI Method
+## CLI Method
 
 Run `pip3 install cyberdrop-dl` in command prompt/terminal
 
 Advanced users may want to use virtual environments (via `pipx`), but it's **NOT** required.
 
 1. Run `cyberdrop-dl` once to generate an empty `URLs.txt` file.
 2. Copy and paste your links into `URLs.txt`.
 Each link you add has to go on its own line (paste link, press enter, repeat).
 3. Run `cyberdrop-dl` again.
 It will begin to download everything.
 4. Enjoy!
 
-## Arguments & Config
+### Arguments & Config
+
 If you know what you're doing, you can use the available options to adjust how the program runs.
 
 You can read more about all of these options [here](https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/Config-Options). As they directly correlate with the config options.
 
-```
+```raw
 $ cyberdrop-dl -h
 usage: cyberdrop-dl [-h] [-V] [-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads THREADS] [--attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-images] [--exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
 
 Bulk downloader for multiple file hosts
 
 positional arguments:
   link                  link to content to download (passing multiple links is supported)
 
 optional arguments:
 -h, --help                                         show this help message and exit
 -V, --version                                      show program's version number and exit
 -i INPUT_FILE, --input-file INPUT_FILE             file containing links to download
 -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER    folder to download files to
 
---config-file 	                config file to read arguments from
---db-file 	                history database file to write to
+--config-file                   config file to read arguments from
+--db-file                       history database file to write to
 --errored-urls-file             csv file to write failed download information to
---log-file 	                log file to write to
---output-last-forum-post-file 	text file to output last scraped post from a forum thread for re-feeding into CDL
---unsupported-urls-file 	csv file to output unsupported links into
-
---exclude-audio 	skip downloading of audio files
---exclude-images 	skip downloading of image files
---exclude-other 	skip downloading of images
---exclude-videos 	skip downloading of video files
---ignore-cache 	        ignores previous runs cached scrape history
---ignore-history 	ignores previous download history
---only-hosts 	        only allows downloads and scraping from these hosts
---skip-hosts 	        doesn't allow downloads and scraping from these hosts
-
---allow-insecure-connections 	        allows insecure connections from content hosts
---attempts 	                        number of attempts to download each file
---block-sub-folders 	                block sub folders from being created
---disable-attempt-limit 	        disables the attempt limitation
---include-id 	                        include the ID in the download folder name
---skip-download-mark-completed 	        sets the scraped files as downloaded without downloading
---output-errored-urls 	                sets the failed urls to be output to the errored urls file
---output-unsupported-urls 	        sets the unsupported urls to be output to the unsupported urls file
---proxy 	                        HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
---remove-bunkr-identifier 	        removes the bunkr added identifier from output filenames
---required-free-space 	                required free space (in gigabytes) for the program to run
---simultaneous-downloads-per-domain 	number of simultaneous downloads to use per domain
-
---sort-downloads 	sorts downloaded files after downloads have finished
---sort-directory 	folder to download files to
---sorted-audio 	        schema to sort audio
---sorted-images 	schema to sort images
---sorted-others 	schema to sort other
---sorted-videos 	schema to sort videos
-
---connection-timeout 	number of seconds to wait attempting to connect to a URL during the downloading phase
---ratelimit 	        this applies to requests made in the program during scraping, the number you provide is in requests/seconds
---throttle 	        this is a throttle between requests during the downloading phase, the number is in seconds
-
---output-last-forum-post 	outputs the last post of a forum scrape to use as a starting point for future runs
---separate-posts 	        separates forum scraping into folders by post number
-	
---pixeldrain-api-key 	        api key for premium pixeldrain
---simpcity-password 	        password to login to simpcity
---simpcity-username 	        username to login to simpcity
---socialmediagirls-password 	password to login to socialmediagirls
---socialmediagirls-username 	username to login to socialmediagirls
---xbunker-password 	        password to login to xbunker
---xbunker-username 	        username to login to xbunker
-
---apply-jdownloader 	enables sending unsupported URLs to a running jdownloader2 instance to download
---jdownloader-username 	username to login to jdownloader
---jdownloader-password 	password to login to jdownloader
---jdownloader-device 	device name to login to for jdownloader
+--log-file                      log file to write to
+--output-last-forum-post-file   text file to output last scraped post from a forum thread for re-feeding into CDL
+--unsupported-urls-file         csv file to output unsupported links into
+
+--exclude-audio         skip downloading of audio files
+--exclude-images        skip downloading of image files
+--exclude-other         skip downloading of images
+--exclude-videos        skip downloading of video files
+--ignore-cache          ignores previous runs cached scrape history
+--ignore-history        ignores previous download history
+--only-hosts            only allows downloads and scraping from these hosts
+--skip-hosts            doesn't allow downloads and scraping from these hosts
+
+--allow-insecure-connections            allows insecure connections from content hosts
+--attempts                              number of attempts to download each file
+--block-sub-folders                     block sub folders from being created
+--disable-attempt-limit                 disables the attempt limitation
+--include-id                            include the ID in the download folder name
+--skip-download-mark-completed          sets the scraped files as downloaded without downloading
+--output-errored-urls                   sets the failed urls to be output to the errored urls file
+--output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
+--proxy                                 HTTP/HTTPS proxy used for downloading, format [protocal]://[ip]:[port]
+--remove-bunkr-identifier               removes the bunkr added identifier from output filenames
+--required-free-space                   required free space (in gigabytes) for the program to run
+--simultaneous-downloads-per-domain     number of simultaneous downloads to use per domain
+
+--sort-downloads        sorts downloaded files after downloads have finished
+--sort-directory        folder to download files to
+--sorted-audio          schema to sort audio
+--sorted-images         schema to sort images
+--sorted-others         schema to sort other
+--sorted-videos         schema to sort videos
+
+--connection-timeout    number of seconds to wait attempting to connect to a URL during the downloading phase
+--ratelimit             this applies to requests made in the program during scraping, the number you provide is in requests/seconds
+--throttle              this is a throttle between requests during the downloading phase, the number is in seconds
+
+--output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
+--separate-posts                separates forum scraping into folders by post number
+
+--gofile-api-key                api key for premium gofile
+--pixeldrain-api-key            api key for premium pixeldrain
+--simpcity-username             username to login to simpcity
+--simpcity-password             password to login to simpcity
+--socialmediagirls-username     username to login to socialmediagirls
+--socialmediagirls-password     password to login to socialmediagirls
+--xbunker-username              username to login to xbunker
+--xbunker-password              password to login to xbunker
+
+--apply-jdownloader     enables sending unsupported URLs to a running jdownloader2 instance to download
+--jdownloader-username  username to login to jdownloader
+--jdownloader-password  password to login to jdownloader
+--jdownloader-device    device name to login to for jdownloader
 
 --hide-new-progress             disables the new rich progress entirely and uses older methods
 --hide-overall-progress         removes overall progress section while downloading
 --hide-forum-progress           removes forum progress section while downloading
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.12 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.13 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -11,26 +11,26 @@
 dl/month)](https://pepy.tech/project/cyberdrop-dl) [![Downloads](https://
 static.pepy.tech/badge/cyberdrop-dl/week)](https://pepy.tech/project/cyberdrop-
 dl) [![Discord Banner 3](https://discordapp.com/api/guilds/1070206871564197908/
 widget.png?style=banner3)](https://discord.com/invite/kbZCxz22Qp) Brand new and
 improved! Cyberdrop-DL now has an updated paint job, fantastic new look. On top
 of this it also downloads from different domains simultaneously. ![Screenshot
 2023-02-19 183052](https://user-images.githubusercontent.com/61347133/
-219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png) # Support Cyberdrop-DL
+219989561-759bd8b1-34d2-4d61-8fa7-0d0b3680e83f.png) ## Support Cyberdrop-DL
 Development [Buy_Me_A_Coffee] If you want to support me and my effort you can
 buy me a coffee or send me some crypto: BTC:
 bc1qzw7l9d8ju2qnag3skfarrd0t5mkn0zyapnrcsn ETH:
 0xf36ef155C43Ed220BfBb2CBe9c5Ae172A8640e9B XMR:
 46vMP5MXVZqQeGzkA1mbX9WQKU8fbWRBJGAktDcjYkCMRDY7HMdLzi1DFsHCPLgms968cyUz1gCWVhy9cZir9Ae7M6anQ8Q
-# More Information Read the Wiki! https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/wiki/ # Supported Sites | Website | Supported Link Types |
-|-------------------------|----------------------------------------------------
+## More Information Read the [Wiki](https://github.com/Jules-WinnfieldX/
+CyberDropDownloader/wiki/)! ## Supported Sites | Website | Supported Link Types
+| |-------------------------|--------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-----------------------| | Anonfiles | Download page: Anonfiles.com/... | |
+------------------------| | Anonfiles | Download page: Anonfiles.com/... | |
 Bayfiles | Download page: Bayfiles.com/... | | Bunkr (ru/su/la) | Albums:
 bunkr.ru/a/...
 Direct Videos: stream.bunkr.ru/v/...
 Direct links: cdn.bunkr.ru/...
 Direct links: i.bunkr.ru/...
 Direct links: files.bunkr.ru/...
 Direct links: media-files.bunkr.ru/... | | Coomer.party | Profiles:
@@ -78,42 +78,42 @@
 Continue from (will download this post and after): simpcity.st/threads/...post-
 NUMBER | | SocialMediaGirls | Thread: forum.socialmediagirls.com/threads/...
 Continue from (will download this post and after): forum.socialmediagirls.com/
 threads/...post-NUMBER | | XBunker | Thread: xbunker.nu/threads/...
 Continue from (will download this post and after): xbunker.nu/threads/...post-
 NUMBER | | XBunkr | Album: xbunkr.com/a/...
 Direct Links: media.xbunkr.com/... | Reminder to leave the link full (include
-the https://) # Information **Requires Python 3.7 or higher (3.10
-recommended)** You can get Python from here: https://www.python.org/downloads/
-Make sure you tick the check box for "Add python to path" ![alt text](https://
-simp2.jpg.church/PATHe426c23371048def.png) Mac users will also likely need to
-open terminal and execute the following command: `xcode-select --install` #
-Script Method Go to the [releases page](https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/releases) and download the Cyberdrop_DL.zip file. Extract
-it to wherever you want the program to be. Put the links in the URLs.txt file
-then run `Start Windows.bat` (Windows) or `Start Mac.command` (OS X) or `Start
-Linux.sh` (Linux). ** Mac users will need to run the command `chmod +x 'Start
-Mac.command'` to make the file executable. # CLI Method Run `pip3 install
-cyberdrop-dl` in command prompt/terminal Advanced users may want to use virtual
-environments (via `pipx`), but it's **NOT** required. 1. Run `cyberdrop-dl`
-once to generate an empty `URLs.txt` file. 2. Copy and paste your links into
-`URLs.txt`. Each link you add has to go on its own line (paste link, press
-enter, repeat). 3. Run `cyberdrop-dl` again. It will begin to download
-everything. 4. Enjoy! ## Arguments & Config If you know what you're doing, you
-can use the available options to adjust how the program runs. You can read more
-about all of these options [here](https://github.com/Jules-WinnfieldX/
-CyberDropDownloader/wiki/Config-Options). As they directly correlate with the
-config options. ``` $ cyberdrop-dl -h usage: cyberdrop-dl [-h] [-V] [-
-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads THREADS] [--
-attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-images] [--
-exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-username
-"USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...] Bulk
-downloader for multiple file hosts positional arguments: link link to content
-to download (passing multiple links is supported) optional arguments: -h, --
-help show this help message and exit -V, --version show program's version
+the https://) ## Information **Requires Python 3.7 or higher (3.10
+recommended)** You can get Python from here:
+www.python.org/downloads/> Make sure you tick the check box for "Add python to
+path" ![alt text](https://simp2.jpg.church/PATHe426c23371048def.png) Mac users
+will also likely need to open terminal and execute the following command:
+`xcode-select --install` ## Script Method Go to the [releases page](https://
+github.com/Jules-WinnfieldX/CyberDropDownloader/releases) and download the
+Cyberdrop_DL.zip file. Extract it to wherever you want the program to be. Put
+the links in the URLs.txt file then run `Start Windows.bat` (Windows) or `Start
+Mac.command` (OS X) or `Start Linux.sh` (Linux). ** Mac users will need to run
+the command `chmod +x 'Start Mac.command'` to make the file executable. ## CLI
+Method Run `pip3 install cyberdrop-dl` in command prompt/terminal Advanced
+users may want to use virtual environments (via `pipx`), but it's **NOT**
+required. 1. Run `cyberdrop-dl` once to generate an empty `URLs.txt` file. 2.
+Copy and paste your links into `URLs.txt`. Each link you add has to go on its
+own line (paste link, press enter, repeat). 3. Run `cyberdrop-dl` again. It
+will begin to download everything. 4. Enjoy! ### Arguments & Config If you know
+what you're doing, you can use the available options to adjust how the program
+runs. You can read more about all of these options [here](https://github.com/
+Jules-WinnfieldX/CyberDropDownloader/wiki/Config-Options). As they directly
+correlate with the config options. ```raw $ cyberdrop-dl -h usage: cyberdrop-dl
+[-h] [-V] [-i INPUT_FILE] [-o OUTPUT_FOLDER] [--log-file LOG_FILE] [--threads
+THREADS] [--attempts ATTEMPTS] [--include-id] [--exclude-videos] [--exclude-
+images] [--exclude-audio] [--exclude-other] [--ignore-history] [--simpcity-
+username "USERNAME"] [--simpcity-password "PASSWORD"] [--skip SITE] [link ...]
+Bulk downloader for multiple file hosts positional arguments: link link to
+content to download (passing multiple links is supported) optional arguments: -
+h, --help show this help message and exit -V, --version show program's version
 number and exit -i INPUT_FILE, --input-file INPUT_FILE file containing links to
 download -o OUTPUT_FOLDER, --output-folder OUTPUT_FOLDER folder to download
 files to --config-file config file to read arguments from --db-file history
 database file to write to --errored-urls-file csv file to write failed download
 information to --log-file log file to write to --output-last-forum-post-file
 text file to output last scraped post from a forum thread for re-feeding into
 CDL --unsupported-urls-file csv file to output unsupported links into --
@@ -140,30 +140,30 @@
 sorted-videos schema to sort videos --connection-timeout number of seconds to
 wait attempting to connect to a URL during the downloading phase --ratelimit
 this applies to requests made in the program during scraping, the number you
 provide is in requests/seconds --throttle this is a throttle between requests
 during the downloading phase, the number is in seconds --output-last-forum-post
 outputs the last post of a forum scrape to use as a starting point for future
 runs --separate-posts separates forum scraping into folders by post number --
-pixeldrain-api-key api key for premium pixeldrain --simpcity-password password
-to login to simpcity --simpcity-username username to login to simpcity --
-socialmediagirls-password password to login to socialmediagirls --
-socialmediagirls-username username to login to socialmediagirls --xbunker-
-password password to login to xbunker --xbunker-username username to login to
-xbunker --apply-jdownloader enables sending unsupported URLs to a running
-jdownloader2 instance to download --jdownloader-username username to login to
-jdownloader --jdownloader-password password to login to jdownloader --
-jdownloader-device device name to login to for jdownloader --hide-new-progress
-disables the new rich progress entirely and uses older methods --hide-overall-
-progress removes overall progress section while downloading --hide-forum-
-progress removes forum progress section while downloading --hide-thread-
-progress removes thread progress section while downloading --hide-domain-
-progress removes domain progress section while downloading --hide-album-
-progress removes album progress section while downloading --hide-file-progress
-removes file progress section while downloading --refresh-rate changes the
-refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
-use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
-"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+gofile-api-key api key for premium gofile --pixeldrain-api-key api key for
+premium pixeldrain --simpcity-username username to login to simpcity --
+simpcity-password password to login to simpcity --socialmediagirls-username
+username to login to socialmediagirls --socialmediagirls-password password to
+login to socialmediagirls --xbunker-username username to login to xbunker --
+xbunker-password password to login to xbunker --apply-jdownloader enables
+sending unsupported URLs to a running jdownloader2 instance to download --
+jdownloader-username username to login to jdownloader --jdownloader-password
+password to login to jdownloader --jdownloader-device device name to login to
+for jdownloader --hide-new-progress disables the new rich progress entirely and
+uses older methods --hide-overall-progress removes overall progress section
+while downloading --hide-forum-progress removes forum progress section while
+downloading --hide-thread-progress removes thread progress section while
+downloading --hide-domain-progress removes domain progress section while
+downloading --hide-album-progress removes album progress section while
+downloading --hide-file-progress removes file progress section while
+downloading --refresh-rate changes the refresh rate of the progress table ```
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
+"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
+"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
 "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost",
 "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls",
 "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.12/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.13/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.12/setup.cfg` & `cyberdrop-dl-4.1.13/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 [options]
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires = 
 	aiofiles>=23.1.0
-	aiohttp>=3.8.3
-	beautifulsoup4>=4.11.2
+	aiohttp>=3.8.4
+	beautifulsoup4>=4.12.2
 	certifi>=2022.12.7
 	myjdapi>=1.1.6
 	PyYAML>=6.0
-	rich>=13.3.1
-	setuptools>=65.6.3
-	yarl>=1.8.2
-	tqdm>=4.64.1
+	rich>=13.3.4
+	setuptools>=67.7.2
+	yarl>=1.9.1
+	tqdm>=4.65.0
 
 [options.entry_points]
 console_scripts = 
 	cyberdrop-dl = cyberdrop_dl.main:main
 
 [egg_info]
 tag_build =
```

