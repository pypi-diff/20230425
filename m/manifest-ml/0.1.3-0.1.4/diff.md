# Comparing `tmp/manifest-ml-0.1.3.tar.gz` & `tmp/manifest-ml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-ml-0.1.3.tar", last modified: Wed Apr 12 20:14:11 2023, max compression
+gzip compressed data, was "manifest-ml-0.1.4.tar", last modified: Mon Apr 24 22:34:12 2023, max compression
```

## Comparing `manifest-ml-0.1.3.tar` & `manifest-ml-0.1.4.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.040597 manifest-ml-0.1.3/
--rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/LICENSE
--rw-r--r--   0 laurelorr   (501) staff       (20)     8190 2023-04-12 20:14:11.040463 manifest-ml-0.1.3/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     7502 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/README.md
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.032367 manifest-ml-0.1.3/manifest/
--rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.3/manifest/__init__.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.033006 manifest-ml-0.1.3/manifest/api/
--rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/api/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/app.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.033971 manifest-ml-0.1.3/manifest/api/models/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/api/models/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    23121 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/model.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/sentence_transformer.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1801 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/response.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.035386 manifest-ml-0.1.3/manifest/caches/
--rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4463 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/caches/cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/noop.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.3/manifest/caches/postgres.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/redis.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5773 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/caches/serializers.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/sqlite.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.037502 manifest-ml-0.1.3/manifest/clients/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/clients/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3301 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/ai21.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    11825 2023-04-12 19:53:13.000000 manifest-ml-0.1.3/manifest/clients/client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3459 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/cohere.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2819 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3738 2023-03-27 02:06:27.000000 manifest-ml-0.1.3/manifest/clients/dummy.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3463 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2334 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/huggingface_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3997 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/openai.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5132 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/openai_chat.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6558 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/openai_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5162 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/toma.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1938 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/toma_diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    17784 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2811 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     7558 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-04-12 20:13:56.000000 manifest-ml-0.1.3/manifest/version.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.038214 manifest-ml-0.1.3/manifest_ml.egg-info/
--rw-r--r--   0 laurelorr   (501) staff       (20)     8190 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     1415 2023-04-12 20:14:11.000000 manifest-ml-0.1.3/manifest_ml.egg-info/SOURCES.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/dependency_links.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)     1615 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/requires.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/top_level.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)      786 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/pyproject.toml
--rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-04-12 20:14:11.040650 manifest-ml-0.1.3/setup.cfg
--rw-r--r--   0 laurelorr   (501) staff       (20)     5349 2023-04-12 20:13:43.000000 manifest-ml-0.1.3/setup.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.039721 manifest-ml-0.1.3/tests/
--rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/tests/test_array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     9111 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2053 2023-04-08 21:15:06.000000 manifest-ml-0.1.3/tests/test_client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_huggingface_api.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    31611 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.3/tests/test_request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5756 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/tests/test_response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      997 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_serializer.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.040181 manifest-ml-0.1.3/web_app/
--rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/web_app/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1733 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/web_app/main.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/web_app/schemas.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.988283 manifest-ml-0.1.4/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/LICENSE
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10067 2023-04-24 22:34:12.988099 manifest-ml-0.1.4/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9379 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/README.md
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.978902 manifest-ml-0.1.4/manifest/
+-rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.4/manifest/__init__.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.979548 manifest-ml-0.1.4/manifest/api/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/api/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.4/manifest/api/app.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.981051 manifest-ml-0.1.4/manifest/api/models/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/api/models/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    23121 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/model.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/api/models/sentence_transformer.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/api/response.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.982433 manifest-ml-0.1.4/manifest/caches/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/caches/cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/noop.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.4/manifest/caches/postgres.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/redis.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/caches/serializers.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/caches/sqlite.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.984583 manifest-ml-0.1.4/manifest/clients/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/manifest/clients/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3303 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/ai21.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    13421 2023-04-24 18:39:09.000000 manifest-ml-0.1.4/manifest/clients/client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3461 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/cohere.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2821 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4510 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/dummy.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3751 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2336 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/huggingface_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4810 2023-04-24 19:18:15.000000 manifest-ml-0.1.4/manifest/clients/openai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5132 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/manifest/clients/openai_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6560 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/openai_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5164 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/toma.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1940 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/clients/toma_diffuser.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.985183 manifest-ml-0.1.4/manifest/connections/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/connections/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5947 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/connections/client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/manifest/connections/scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    18277 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3000 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/manifest/request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10750 2023-04-24 19:16:26.000000 manifest-ml-0.1.4/manifest/response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-04-12 20:16:25.000000 manifest-ml-0.1.4/manifest/version.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.985822 manifest-ml-0.1.4/manifest_ml.egg-info/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10067 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1568 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1615 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/requires.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-04-24 22:34:12.000000 manifest-ml-0.1.4/manifest_ml.egg-info/top_level.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)      786 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/pyproject.toml
+-rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-04-24 22:34:12.988327 manifest-ml-0.1.4/setup.cfg
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5349 2023-04-12 20:13:43.000000 manifest-ml-0.1.4/setup.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.987443 manifest-ml-0.1.4/tests/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/tests/test_array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2294 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/tests/test_client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.4/tests/test_huggingface_api.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    36113 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.4/tests/test_request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10431 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-04-17 05:07:52.000000 manifest-ml-0.1.4/tests/test_scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/tests/test_serializer.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-24 22:34:12.987870 manifest-ml-0.1.4/web_app/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/web_app/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.4/web_app/main.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.4/web_app/schemas.py
```

### Comparing `manifest-ml-0.1.3/LICENSE` & `manifest-ml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/PKG-INFO` & `manifest-ml-0.1.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,18 @@
-Metadata-Version: 2.1
-Name: manifest-ml
-Version: 0.1.3
-Summary: Manifest for Prompting Foundation Models.
-Home-page: https://github.com/HazyResearch/manifest
-Author: Laurel Orr
-Author-email: laurel.orr@numbersstation.ai
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: api
-Provides-Extra: app
-Provides-Extra: diffusers
-Provides-Extra: gcp
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
-
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
 - [Embedding Models](#embedding-models)
+- [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
 ```bash
@@ -76,15 +53,15 @@
 We have example notebook and python scripts located at [examples](examples). These show how to use different models, model types (i.e. text, diffusers, or embedding models), and async running.
 
 # Manifest Components
 Manifest is meant to be a very light weight package to help with prompt design and iteration. Three key design decisions of Manifest are
 
 * All models are behind APIs
 * Supports caching of model inputs/outputs for iteration, reproducibility, and cost saving
-* Unified API of generate, score, and embed
+* Unified API to support generate, score, and embed
 
 ## Models
 Manifest provides model clients for [OpenAI](https://openai.com/), [AI21](https://studio.ai21.com/), [Cohere](https://cohere.ai/), [Together](https://together.xyz/), and HuggingFace (see [below](#huggingface-models) for how to use locally hosted HuggingFace models). You can toggle between the models by changing `client_name` and `client_connection`. For example, if a HuggingFace model is loaded locally, run
 ```python
 manifest = Manifest(
     client_name = "huggingface",
     client_connection = "http://127.0.0.1:5000",
@@ -145,29 +122,56 @@
 import asyncio
 results = asyncio.run(manifest.arun_batch(["Where are the cats?", "Where are the dogs?"]))
 ```
 
 If something doesn't go right, you can also ask to get a raw manifest Response.
 ```python
 result_object = manifest.run(["Where are the cats?", "Where are the dogs?"], return_response=True)
-print(result_object.get_request())
+print(result_object.get_request_obj())
 print(result_object.is_cached())
-print(result_object.get_json_response())
+print(result_object.get_response_obj())
 ```
 
 By default, we do not truncate results based on a stop token. You can change this by either passing a new stop token to a Manifest session or to a `run`.
 ```python
 result = manifest.run(prompt, "Laurel", stop_token="and")
 ```
 
 If you want to change default parameters to a model, we pass those as `kwargs` to the client.
 ```python
 result = manifest.run(prompt, "Laurel", max_tokens=50)
 ```
 
+## Model Pools
+Manifest supports querying multiple models with different schedulers. This is very much a work in progress effort, but Manifest will round robin select (or randomly select) the clients you want. You can use the same client multiple times with different connection strings (e.g. different API keys), or you can mix and match. The only requirement is that all clients are the same request type. I.e. you can't have a pool of generation models and embedding models.
+
+To query between a local model and OpenAI,
+```python
+from manifest.connections.client_pool import ClientConnection
+from manifest import Manifest
+
+client_connection1 = ClientConnection(
+    client_name="huggingface",
+    client_connection="http://127.0.0.1:5000",
+)
+client_connection2 = ClientConnection(client_name="openai", engine="text-ada-001")
+manifest = Manifest(
+    client_pool=[client_connection1, client_connection2],
+    cache_name="sqlite",
+    client_connection=sqlite_cache,
+)
+manifest.run(...)
+```
+
+The speed benefit comes in with async batched runs. When calling `arun_batch` with a list of prompts, Manifest supports a `chunk_size` param. This will break the prompts into `chunk_size` chunks to spread across the client pool. By default `chunk_size` is `-1` which means only one client will get all the prompts to run asynchronously. You must set `chunk_size > 1` to distribute across the pool. There is a further `batch_size` param which control the individual client `batch_size` to send to the model.
+
+```python
+responses = asyncio.run(manifest.arun_batch(prompts, max_tokens=30, chunk_size=20))
+```
+
 # Local Huggingface Models
 To use a HuggingFace generative model, in `manifest/api` we have a Flask application that hosts the models for you.
 
 In a separate terminal or Tmux/Screen session, to load 6B parameters models, run
 ```bash
 python3 -m manifest.api.app \
     --model_type huggingface \
@@ -225,14 +229,27 @@
 ```bash
 python3 -m manifest.api.app \
     --model_type sentence_transformers \
     --model_name_or_path all-mpnet-base-v2 \
     --device 0
 ```
 
+# Road Map
+Here's what's coming up next
+- [ ] Clients
+  - [ ] HuggingFace Hub
+  - [ ] Azure OpenAI
+  - [ ] Anthropic
+- [ ] Data Types
+  - [ ] Diffusion Models
+- [ ] Orchestration
+  - [x] Connection pools
+- [ ] Local Inference
+  - [ ] FlexGen
+
 # Development
 Before submitting a PR, run
 ```bash
 export REDIS_PORT="6379"  # or whatever PORT local redis is running for those tests
 cd <REDIS_PATH>
 docker run -d -p 127.0.0.1:${REDIS_PORT}:6379 -v `pwd`:`pwd` -w `pwd` --name manifest_redis_test redis
 make test
@@ -245,9 +262,7 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
-
-
```

### Comparing `manifest-ml-0.1.3/README.md` & `manifest-ml-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,42 @@
+Metadata-Version: 2.1
+Name: manifest-ml
+Version: 0.1.4
+Summary: Manifest for Prompting Foundation Models.
+Home-page: https://github.com/HazyResearch/manifest
+Author: Laurel Orr
+Author-email: laurel.orr@numbersstation.ai
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: api
+Provides-Extra: app
+Provides-Extra: diffusers
+Provides-Extra: gcp
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
+
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
 - [Embedding Models](#embedding-models)
+- [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
 ```bash
@@ -52,15 +77,15 @@
 We have example notebook and python scripts located at [examples](examples). These show how to use different models, model types (i.e. text, diffusers, or embedding models), and async running.
 
 # Manifest Components
 Manifest is meant to be a very light weight package to help with prompt design and iteration. Three key design decisions of Manifest are
 
 * All models are behind APIs
 * Supports caching of model inputs/outputs for iteration, reproducibility, and cost saving
-* Unified API of generate, score, and embed
+* Unified API to support generate, score, and embed
 
 ## Models
 Manifest provides model clients for [OpenAI](https://openai.com/), [AI21](https://studio.ai21.com/), [Cohere](https://cohere.ai/), [Together](https://together.xyz/), and HuggingFace (see [below](#huggingface-models) for how to use locally hosted HuggingFace models). You can toggle between the models by changing `client_name` and `client_connection`. For example, if a HuggingFace model is loaded locally, run
 ```python
 manifest = Manifest(
     client_name = "huggingface",
     client_connection = "http://127.0.0.1:5000",
@@ -121,29 +146,56 @@
 import asyncio
 results = asyncio.run(manifest.arun_batch(["Where are the cats?", "Where are the dogs?"]))
 ```
 
 If something doesn't go right, you can also ask to get a raw manifest Response.
 ```python
 result_object = manifest.run(["Where are the cats?", "Where are the dogs?"], return_response=True)
-print(result_object.get_request())
+print(result_object.get_request_obj())
 print(result_object.is_cached())
-print(result_object.get_json_response())
+print(result_object.get_response_obj())
 ```
 
 By default, we do not truncate results based on a stop token. You can change this by either passing a new stop token to a Manifest session or to a `run`.
 ```python
 result = manifest.run(prompt, "Laurel", stop_token="and")
 ```
 
 If you want to change default parameters to a model, we pass those as `kwargs` to the client.
 ```python
 result = manifest.run(prompt, "Laurel", max_tokens=50)
 ```
 
+## Model Pools
+Manifest supports querying multiple models with different schedulers. This is very much a work in progress effort, but Manifest will round robin select (or randomly select) the clients you want. You can use the same client multiple times with different connection strings (e.g. different API keys), or you can mix and match. The only requirement is that all clients are the same request type. I.e. you can't have a pool of generation models and embedding models.
+
+To query between a local model and OpenAI,
+```python
+from manifest.connections.client_pool import ClientConnection
+from manifest import Manifest
+
+client_connection1 = ClientConnection(
+    client_name="huggingface",
+    client_connection="http://127.0.0.1:5000",
+)
+client_connection2 = ClientConnection(client_name="openai", engine="text-ada-001")
+manifest = Manifest(
+    client_pool=[client_connection1, client_connection2],
+    cache_name="sqlite",
+    client_connection=sqlite_cache,
+)
+manifest.run(...)
+```
+
+The speed benefit comes in with async batched runs. When calling `arun_batch` with a list of prompts, Manifest supports a `chunk_size` param. This will break the prompts into `chunk_size` chunks to spread across the client pool. By default `chunk_size` is `-1` which means only one client will get all the prompts to run asynchronously. You must set `chunk_size > 1` to distribute across the pool. There is a further `batch_size` param which control the individual client `batch_size` to send to the model.
+
+```python
+responses = asyncio.run(manifest.arun_batch(prompts, max_tokens=30, chunk_size=20))
+```
+
 # Local Huggingface Models
 To use a HuggingFace generative model, in `manifest/api` we have a Flask application that hosts the models for you.
 
 In a separate terminal or Tmux/Screen session, to load 6B parameters models, run
 ```bash
 python3 -m manifest.api.app \
     --model_type huggingface \
@@ -201,14 +253,27 @@
 ```bash
 python3 -m manifest.api.app \
     --model_type sentence_transformers \
     --model_name_or_path all-mpnet-base-v2 \
     --device 0
 ```
 
+# Road Map
+Here's what's coming up next
+- [ ] Clients
+  - [ ] HuggingFace Hub
+  - [ ] Azure OpenAI
+  - [ ] Anthropic
+- [ ] Data Types
+  - [ ] Diffusion Models
+- [ ] Orchestration
+  - [x] Connection pools
+- [ ] Local Inference
+  - [ ] FlexGen
+
 # Development
 Before submitting a PR, run
 ```bash
 export REDIS_PORT="6379"  # or whatever PORT local redis is running for those tests
 cd <REDIS_PATH>
 docker run -d -p 127.0.0.1:${REDIS_PORT}:6379 -v `pwd`:`pwd` -w `pwd` --name manifest_redis_test redis
 make test
@@ -221,7 +286,9 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
+
+
```

### Comparing `manifest-ml-0.1.3/manifest/api/app.py` & `manifest-ml-0.1.4/manifest/api/app.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/api/models/diffuser.py` & `manifest-ml-0.1.4/manifest/api/models/diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/api/models/huggingface.py` & `manifest-ml-0.1.4/manifest/api/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/api/models/model.py` & `manifest-ml-0.1.4/manifest/api/models/model.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/api/models/sentence_transformer.py` & `manifest-ml-0.1.4/manifest/api/models/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/api/response.py` & `manifest-ml-0.1.4/manifest/api/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         self.response_id = str(uuid.uuid4())
         self.created = int(time.time())
 
     def __dict__(self) -> Dict[str, Any]:  # type: ignore
         """Return dictionary representation of response."""
         key = (
             "text"
-            if self.response_type
-            not in {"prompt_logit_score", "image_generation", "embedding_generation"}
+            if self.response_type not in {"image_generation", "embedding_generation"}
             else "array"
         )
         return {
             "id": self.response_id,
             "object": self.response_type,
             "created": self.created,
             "model": "flask_model",
```

### Comparing `manifest-ml-0.1.3/manifest/caches/array_cache.py` & `manifest-ml-0.1.4/manifest/caches/array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/caches/cache.py` & `manifest-ml-0.1.4/manifest/caches/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 """Cache for queries and responses."""
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Union
+from typing import Any, Dict, Type, Union
 
 from manifest.caches.serializers import ArraySerializer, NumpyByteSerializer, Serializer
-from manifest.response import RESPONSE_CONSTRUCTORS, Response
+from manifest.request import DiffusionRequest, EmbeddingRequest, LMRequest, Request
+from manifest.response import Response
 
 # Non-text return type caches
-ARRAY_CACHE_TYPES = {
-    "diffuser",
-    "tomadiffuser",
-    "openaiembedding",
-    "huggingfaceembedding",
-}
+ARRAY_CACHE_TYPES = {EmbeddingRequest, DiffusionRequest}
 
 
 class Cache(ABC):
     """A cache for request/response pairs."""
 
     def __init__(
         self,
         connection_str: str,
-        client_name: str = "None",
+        request_type: Type[Request] = LMRequest,
         cache_args: Dict[str, Any] = {},
     ):
         """
         Initialize cache.
 
         Args:
             connection_str: connection string.
-            client_name: name of client.
+            request_type: request type.
             cache_args: arguments for cache.
 
         cache_args are any arguments needed to initialize the cache.
 
         Further, cache_args can contain `array_serializer` as a string
         for embedding or image return types (e.g. diffusers) with values
         as `local_file` or `byte_string`. `local_file` will save the
         array in a local file and cache a pointer to the file.
         `byte_string` will convert the array to a byte string and cache
         the entire byte string. `byte_string` is default.
 
         Args:
-            connection_str: connection string for client.
+            connection_str: connection string for cache.
             cache_args: cache arguments.
         """
-        self.client_name = client_name
+        self.request_type = request_type
         self.connect(connection_str, cache_args)
-        if self.client_name in ARRAY_CACHE_TYPES:
+        if self.request_type in ARRAY_CACHE_TYPES:
             array_serializer = cache_args.pop("array_serializer", "byte_string")
             if array_serializer not in ["local_file", "byte_string"]:
                 raise ValueError(
                     "array_serializer must be local_file or byte_string,"
                     f" not {array_serializer}"
                 )
             self.serializer = (
@@ -61,21 +57,21 @@
         else:
             # If user has array_serializer type, it will throw an error as
             # it is not recognized for non-array return types.
             self.serializer = Serializer()
 
     @abstractmethod
     def close(self) -> None:
-        """Close the client."""
+        """Close the cache."""
         raise NotImplementedError()
 
     @abstractmethod
     def connect(self, connection_str: str, cache_args: Dict[str, Any]) -> None:
         """
-        Connect to client.
+        Connect to cache.
 
         Args:
             connection_str: connection string.
         """
         raise NotImplementedError()
 
     @abstractmethod
@@ -119,22 +115,17 @@
 
         Returns:
             Response object or None if not in cache.
         """
         key = self.serializer.request_to_key(request)
         cached_response = self.get_key(key)
         if cached_response:
-            cached = True
             response = self.serializer.key_to_response(cached_response)
-            return Response(
-                response,
-                cached,
-                request,
-                **RESPONSE_CONSTRUCTORS.get(self.client_name, {}),
-            )
+            response["cached"] = True
+            return Response.from_dict(response, request_dict=request)
         return None
 
     def set(self, request: Dict, response: Dict) -> None:
         """Set the value for the key.
 
         Args:
             request: request to set.
```

### Comparing `manifest-ml-0.1.3/manifest/caches/noop.py` & `manifest-ml-0.1.4/manifest/caches/noop.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/caches/postgres.py` & `manifest-ml-0.1.4/manifest/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/caches/redis.py` & `manifest-ml-0.1.4/manifest/caches/redis.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/caches/serializers.py` & `manifest-ml-0.1.4/manifest/caches/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,22 +73,23 @@
 
         Args:
             response: response to normalize.
 
         Returns:
             normalized key.
         """
+        sub_response = response["response"]
         # Assume response is a dict with keys "choices" -> List dicts
         # with keys "array".
-        choices = response["choices"]
+        choices = sub_response["choices"]
         # We don't want to modify the response in place
         # but we want to avoid calling deepcopy on an array
-        del response["choices"]
-        response_copy = response.copy()
-        response["choices"] = choices
+        del sub_response["choices"]
+        response_copy = sub_response.copy()
+        sub_response["choices"] = choices
         response_copy["choices"] = []
         for choice in choices:
             if "array" not in choice:
                 raise ValueError(
                     f"Choice with keys {choice.keys()} does not have array key."
                 )
             arr = choice["array"]
@@ -97,28 +98,29 @@
             new_choice = choice.copy()
             choice["array"] = arr
             with io.BytesIO() as f:
                 np.savez_compressed(f, data=arr)
                 hash_str = f.getvalue().hex()
             new_choice["array"] = hash_str
             response_copy["choices"].append(new_choice)
-        return json.dumps(response_copy, sort_keys=True)
+        response["response"] = response_copy
+        return json.dumps(response, sort_keys=True)
 
     def key_to_response(self, key: str) -> Dict:
         """
         Convert the normalized version to the response.
 
         Args:
             key: normalized key to convert.
 
         Returns:
             unnormalized response dict.
         """
         response = json.loads(key)
-        for choice in response["choices"]:
+        for choice in response["response"]["choices"]:
             hash_str = choice["array"]
             byte_str = bytes.fromhex(hash_str)
             with io.BytesIO(byte_str) as f:
                 choice["array"] = np.load(f)["data"]
         return response
 
 
@@ -148,22 +150,23 @@
 
         Args:
             response: response to normalize.
 
         Returns:
             normalized key.
         """
+        sub_response = response["response"]
         # Assume response is a dict with keys "choices" -> List dicts
         # with keys "array".
-        choices = response["choices"]
+        choices = sub_response["choices"]
         # We don't want to modify the response in place
         # but we want to avoid calling deepcopy on an array
-        del response["choices"]
-        response_copy = response.copy()
-        response["choices"] = choices
+        del sub_response["choices"]
+        response_copy = sub_response.copy()
+        sub_response["choices"] = choices
         response_copy["choices"] = []
         for choice in choices:
             if "array" not in choice:
                 raise ValueError(
                     f"Choice with keys {choice.keys()} does not have array key."
                 )
             arr = choice["array"]
@@ -175,26 +178,27 @@
             self.hash.update(arr)
             hash_str = self.hash.hexdigest()
             self.hash.reset()
             new_choice["array"] = hash_str
             response_copy["choices"].append(new_choice)
             if not self.writer.contains_key(hash_str):
                 self.writer.put(hash_str, arr)
-        return json.dumps(response_copy, sort_keys=True)
+        response["response"] = response_copy
+        return json.dumps(response, sort_keys=True)
 
     def key_to_response(self, key: str) -> Dict:
         """
         Convert the normalized version to the response.
 
         Convert the hash string keys to the arrays.
 
         Args:
             key: normalized key to convert.
 
         Returns:
             unnormalized response dict.
         """
         response = json.loads(key)
-        for choice in response["choices"]:
+        for choice in response["response"]["choices"]:
             hash_str = choice["array"]
             choice["array"] = self.writer.get(hash_str)
         return response
```

### Comparing `manifest-ml-0.1.3/manifest/caches/sqlite.py` & `manifest-ml-0.1.4/manifest/caches/sqlite.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/clients/ai21.py` & `manifest-ml-0.1.4/manifest/clients/ai21.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/clients/client.py` & `manifest-ml-0.1.4/manifest/clients/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,29 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import aiohttp
 import requests
 from tenacity import RetryCallState, retry, stop_after_attempt, wait_random_exponential
 
-from manifest.request import DEFAULT_REQUEST_KEYS, NOT_CACHE_KEYS, Request
-from manifest.response import RESPONSE_CONSTRUCTORS, Response
+from manifest.request import (
+    DEFAULT_REQUEST_KEYS,
+    NOT_CACHE_KEYS,
+    LMScoreRequest,
+    Request,
+)
+from manifest.response import (
+    RESPONSE_CONSTRUCTORS,
+    ArrayModelChoice,
+    LMModelChoice,
+    ModelChoices,
+    Response,
+    Usage,
+    Usages,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def retry_if_ratelimit(retry_base: RetryCallState) -> bool:
     """Return whether to retry if ratelimited."""
     try:
@@ -124,50 +137,71 @@
             prompt: prompt.
             request_args: request arguments.
 
         Returns:
             request.
         """
         params = {"prompt": prompt}
+        # Adds default values from self.PARAMS if not in request_args
         for key in self.PARAMS:
             params[key] = request_args.pop(key, getattr(self, key))
+        # Allows for overriding DEFAULT_REQUEST_KEYS even if they are not
+        # in self.PARAMS. Note that DEFAULT_REQUEST_KEYS match the default
+        # values in Request.
         for key in DEFAULT_REQUEST_KEYS:
             if key not in params and key in request_args:
                 params[key] = request_args.pop(key)
         return self.REQUEST_CLS(**params)  # type: ignore
 
     def get_request_params(self, request: Request) -> Dict[str, Any]:
         """Get request params.
 
         Add default keys that we need for requests such as batch_size.
         We drop these before sending to the model.
         """
         params_to_add = DEFAULT_REQUEST_KEYS.copy()
+        # This will override DEFAULT_REQUEST_KEYS with those in PARAMS
         params_to_add.update(self.PARAMS)
+        # to_dict will handle parameter renaming but not any
+        # default value handling - that is done in get_request()
         request_params = request.to_dict(params_to_add)
         return request_params
 
     def get_cache_key(self, request: Request) -> Dict[str, Any]:
         """Get cache key for request.
 
         Skip keys that are not cache keys such as batch_size.
         """
         request_params = self.get_request_params(request)
         for key in NOT_CACHE_KEYS:
             request_params.pop(key, None)
+        # Make sure to add model params and request class
         request_params.update(self.get_model_params())
+        request_params["request_cls"] = request.__class__.__name__
         return request_params
 
     def split_usage(self, request: Dict, choices: List[str]) -> List[Dict[str, int]]:
         """Split usage into list of usages for each prompt."""
         return []
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def get_model_choices(self, response: Dict) -> ModelChoices:
+        """Format response to ModelChoices."""
+        # Array or text response
+        response_type = RESPONSE_CONSTRUCTORS[self.REQUEST_CLS]["response_type"]
+        if response_type == "array":
+            choices: List[Union[LMModelChoice, ArrayModelChoice]] = [
+                ArrayModelChoice(**choice) for choice in response["choices"]
+            ]
+        else:
+            choices = [LMModelChoice(**choice) for choice in response["choices"]]
+        return ModelChoices(choices=choices)
+
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
-        Format response to dict.
+        Validate response as dict.
 
         Args:
             response: response
             request: request
 
         Return:
             response as dict
@@ -235,15 +269,15 @@
             timeout=retry_timeout,
         )
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError:
             logger.error(res.json())
             raise requests.exceptions.HTTPError(res.json())
-        return self.format_response(res.json(), request_params)
+        return self.validate_response(res.json(), request_params)
 
     @retry(
         reraise=True,
         retry=retry_if_ratelimit,
         wait=wait_random_exponential(min=1, max=60),
         stop=stop_after_attempt(10),
     )
@@ -266,15 +300,15 @@
                 post_str,
                 headers=self.get_generation_header(),
                 json=request_params,
                 timeout=retry_timeout,
             ) as res:
                 res.raise_for_status()
                 res_json = await res.json(content_type=None)
-                return self.format_response(res_json, request_params)
+                return self.validate_response(res_json, request_params)
 
     def run_request(self, request: Request) -> Response:
         """
         Get request string function.
 
         Args:
             request: request.
@@ -290,19 +324,24 @@
         request_params = self.get_request_params(request)
         # Take the default keys we need and drop the rest as they
         # are not part of the model request.
         retry_timeout = request_params.pop("client_timeout")
         for key in DEFAULT_REQUEST_KEYS:
             request_params.pop(key, None)
         response_dict = self._run_completion(request_params, retry_timeout)
+        usages = None
+        if "usage" in response_dict:
+            usages = [Usage(**usage) for usage in response_dict["usage"]]
+
         return Response(
-            response_dict,
+            response=self.get_model_choices(response_dict),
             cached=False,
-            request_params=request_params,
-            **RESPONSE_CONSTRUCTORS.get(self.NAME, {}),  # type: ignore
+            request=request,
+            usages=Usages(usages=usages) if usages else None,
+            **RESPONSE_CONSTRUCTORS[self.REQUEST_CLS],  # type: ignore
         )
 
     async def arun_batch_request(self, request: Request) -> Response:
         """
         Get async request string function.
 
         Args:
@@ -342,26 +381,28 @@
         choices = []
         usages = []
         for res_dict in responses:
             choices.extend(res_dict["choices"])
             if "usage" in res_dict:
                 usages.extend(res_dict["usage"])
         final_response_dict = {"choices": choices}
+        final_usages = None
         if usages:
-            final_response_dict["usage"] = usages
+            final_usages = Usages(usages=[Usage(**usage) for usage in usages])
         return Response(
-            final_response_dict,
+            self.get_model_choices(final_response_dict),
             cached=False,
-            request_params=request_params,
-            **RESPONSE_CONSTRUCTORS.get(self.NAME, {}),  # type: ignore
+            request=request,
+            usages=final_usages,
+            **RESPONSE_CONSTRUCTORS[self.REQUEST_CLS],  # type: ignore
         )
 
     def get_score_prompt_request(
         self,
-        request: Request,
+        request: LMScoreRequest,
     ) -> Response:
         """
         Get the logit score of the prompt via a forward pass of the model.
 
         Args:
             request: request.
```

### Comparing `manifest-ml-0.1.3/manifest/clients/cohere.py` & `manifest-ml-0.1.4/manifest/clients/cohere.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/clients/diffuser.py` & `manifest-ml-0.1.4/manifest/clients/diffuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         Returns:
             model params.
         """
         res = requests.post(self.host + "/params").json()
         res["client_name"] = self.NAME
         return res
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/clients/huggingface.py` & `manifest-ml-0.1.4/manifest/clients/huggingface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Hugging Face client."""
 import logging
 from typing import Any, Dict, Optional
 
 import requests
 
 from manifest.clients.client import Client
-from manifest.request import DEFAULT_REQUEST_KEYS, LMRequest, Request
-from manifest.response import Response
+from manifest.request import DEFAULT_REQUEST_KEYS, LMRequest, LMScoreRequest
+from manifest.response import LMModelChoice, ModelChoices, Response
 
 logger = logging.getLogger(__name__)
 
 
 class HuggingFaceClient(Client):
     """HuggingFace client."""
 
@@ -78,15 +78,15 @@
         """
         res = requests.post(self.host + "/params").json()
         res["client_name"] = self.NAME
         return res
 
     def get_score_prompt_request(
         self,
-        request: Request,
+        request: LMScoreRequest,
     ) -> Response:
         """
         Get the logit score of the prompt via a forward pass of the model.
 
         Args:
             request: request.
 
@@ -112,8 +112,17 @@
         except requests.Timeout as e:
             logger.error("HF request timed out. Increase client_timeout.")
             raise e
         except requests.exceptions.HTTPError as e:
             logger.error(res.text)
             raise e
         response_dict = res.json()
-        return Response(response_dict, cached=False, request_params=request_params)
+        return Response(
+            response=ModelChoices(
+                choices=[LMModelChoice(**choice) for choice in response_dict["choices"]]
+            ),
+            cached=False,
+            request=request,
+            usages=None,
+            response_type="text",
+            request_type=LMScoreRequest,
+        )
```

### Comparing `manifest-ml-0.1.3/manifest/clients/huggingface_embedding.py` & `manifest-ml-0.1.4/manifest/clients/huggingface_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         Returns:
             model params.
         """
         res = requests.post(self.host + "/params").json()
         res["client_name"] = self.NAME
         return res
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/clients/openai.py` & `manifest-ml-0.1.4/manifest/clients/openai.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,17 +33,19 @@
     PARAMS = {
         "engine": ("model", "text-davinci-003"),
         "temperature": ("temperature", 1.0),
         "max_tokens": ("max_tokens", 10),
         "n": ("n", 1),
         "top_p": ("top_p", 1.0),
         "top_k": ("best_of", 1),
+        "logprobs": ("logprobs", None),
         "stop_sequences": ("stop", None),  # OpenAI doesn't like empty lists
         "presence_penalty": ("presence_penalty", 0.0),
         "frequency_penalty": ("frequency_penalty", 0.0),
+        "batch_size": ("batch_size", 20),
     }
     REQUEST_CLS: Type[Request] = LMRequest
     NAME = "openai"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
@@ -101,14 +103,35 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+        """
+        Validate response as dict.
+
+        Args:
+            response: response
+            request: request
+
+        Return:
+            response as dict
+        """
+        validated_response = super().validate_response(response, request)
+        # Handle logprobs
+        for choice in validated_response["choices"]:
+            if "logprobs" in choice:
+                logprobs = choice.pop("logprobs")
+                if logprobs and "token_logprobs" in logprobs:
+                    choice["token_logprobs"] = logprobs["token_logprobs"]
+                    choice["tokens"] = logprobs["tokens"]
+        return validated_response
+
     def split_usage(self, request: Dict, choices: List[str]) -> List[Dict[str, int]]:
         """Split usage into list of usages for each prompt."""
         try:
             encoding = tiktoken.encoding_for_model(getattr(self, "engine"))
         except Exception:
             return []
         prompt = request["prompt"]
```

### Comparing `manifest-ml-0.1.3/manifest/clients/openai_chat.py` & `manifest-ml-0.1.4/manifest/clients/openai_chat.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/manifest/clients/openai_embedding.py` & `manifest-ml-0.1.4/manifest/clients/openai_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/clients/toma.py` & `manifest-ml-0.1.4/manifest/clients/toma.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             now = datetime.now(mod_time.tzinfo)
             heartbeats[mod["name"]] = {
                 "last_ping": (now - mod_time).total_seconds(),
                 "expected_runtime": mod["expected_runtime"],
             }
         return heartbeats
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/clients/toma_diffuser.py` & `manifest-ml-0.1.4/manifest/clients/toma_diffuser.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.3/manifest/manifest.py` & `manifest-ml-0.1.4/manifest/manifest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,162 +1,108 @@
 """Manifest class."""
+import asyncio
 import copy
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
 
 import numpy as np
 
 from manifest.caches.noop import NoopCache
 from manifest.caches.postgres import PostgresCache
 from manifest.caches.redis import RedisCache
 from manifest.caches.sqlite import SQLiteCache
-from manifest.clients.ai21 import AI21Client
-from manifest.clients.cohere import CohereClient
-from manifest.clients.dummy import DummyClient
+from manifest.clients.client import Client
 from manifest.clients.huggingface import HuggingFaceClient
-from manifest.clients.huggingface_embedding import HuggingFaceEmbeddingClient
-from manifest.clients.openai import OpenAIClient
-from manifest.clients.openai_chat import OpenAIChatClient
-from manifest.clients.openai_embedding import OpenAIEmbeddingClient
-from manifest.clients.toma import TOMAClient
-from manifest.request import Request
-from manifest.response import Response
+from manifest.connections.client_pool import (
+    CLIENT_CONSTRUCTORS,
+    ClientConnection,
+    ClientConnectionPool,
+)
+from manifest.request import LMScoreRequest, Request
+from manifest.response import ModelChoices, Response, Usage, Usages
 
 logging.getLogger("openai").setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
 
-CLIENT_CONSTRUCTORS = {
-    OpenAIClient.NAME: OpenAIClient,
-    OpenAIChatClient.NAME: OpenAIChatClient,
-    OpenAIEmbeddingClient.NAME: OpenAIEmbeddingClient,
-    CohereClient.NAME: CohereClient,
-    AI21Client.NAME: AI21Client,
-    HuggingFaceClient.NAME: HuggingFaceClient,
-    HuggingFaceEmbeddingClient.NAME: HuggingFaceEmbeddingClient,
-    DummyClient.NAME: DummyClient,
-    TOMAClient.NAME: TOMAClient,
-}
-
-# Diffusion
-DIFFUSION_CLIENTS = ["diffuser", "tomadiffuser"]
-try:
-    from manifest.clients.diffuser import DiffuserClient
-    from manifest.clients.toma_diffuser import TOMADiffuserClient
-
-    CLIENT_CONSTRUCTORS[DiffuserClient.NAME] = DiffuserClient
-    CLIENT_CONSTRUCTORS[TOMADiffuserClient.NAME] = TOMADiffuserClient
-except Exception:
-    logger.info("Diffusion not supported. Skipping import.")
-    pass
-
 
 CACHE_CONSTRUCTORS = {
     "redis": RedisCache,
     "sqlite": SQLiteCache,
     "noop": NoopCache,
     "postgres": PostgresCache,
 }
 
 
 class Manifest:
     """Manifest session object."""
 
     def __init__(
         self,
-        client_name: str = "openai",
+        client_name: Optional[str] = None,
         client_connection: Optional[str] = None,
+        client_pool: Optional[List[ClientConnection]] = None,
+        client_pool_schedule: str = "round_robin",
         cache_name: str = "noop",
         cache_connection: Optional[str] = None,
         stop_token: str = "",
         **kwargs: Any,
     ):
         """
         Initialize manifest.
 
         Args:
             client_name: name of client.
             client_connection: connection string for client.
+            client_pool: list of client connections for multi-client.
+            client_pool_schedule: schedule for client pool.
             cache_name: name of cache.
             cache_connection: connection string for cache.
             stop_token: stop token prompt generation.
                         Can be overridden in run
 
         Remaining kwargs sent to client and cache.
         """
-        if client_name not in CLIENT_CONSTRUCTORS:
-            if client_name in DIFFUSION_CLIENTS:
-                raise ImportError(
-                    f"Diffusion client {client_name} requires the proper install. "
-                    "Make sure to run `pip install manifest-ml[diffusers]` "
-                    "or install Pillow."
-                )
-            else:
-                raise ValueError(
-                    f"Unknown client name: {client_name}. "
-                    f"Choices are {list(CLIENT_CONSTRUCTORS.keys())}"
+        if not client_name and not client_pool:
+            raise ValueError(
+                "Must specify client_name or client_pool. "
+                f"Choices are {list(CLIENT_CONSTRUCTORS.keys())}"
+            )
+        if client_name and client_pool:
+            raise ValueError("Cannot specify both client_name and client_pool")
+        if client_name:
+            client_pool = [
+                ClientConnection(
+                    client_name=client_name,
+                    client_connection=client_connection,
+                    # Remove engine from kwargs
+                    engine=kwargs.pop("engine", None),
                 )
+            ]
+        self.client_pool = ClientConnectionPool(
+            client_pool, client_pool_schedule, client_args=kwargs
+        )
         if cache_name not in CACHE_CONSTRUCTORS:
             raise ValueError(
                 f"Unknown cache name: {cache_name}. "
                 f"Choices are {list(CACHE_CONSTRUCTORS.keys())}"
             )
-        self.client_name = client_name
         # Must pass kwargs as dict for client "pop" methods removed used arguments
         self.cache = CACHE_CONSTRUCTORS[cache_name](  # type: ignore
-            cache_connection, self.client_name, cache_args=kwargs
-        )
-        self.client = CLIENT_CONSTRUCTORS[self.client_name](  # type: ignore
-            client_connection, client_args=kwargs
+            cache_connection, self.client_pool.request_type, cache_args=kwargs
         )
         if len(kwargs) > 0:
             raise ValueError(f"{list(kwargs.items())} arguments are not recognized.")
 
         self.stop_token = stop_token
 
     def close(self) -> None:
         """Close the client and cache."""
-        self.client.close()
+        self.client_pool.close()
         self.cache.close()
 
-    def change_client(
-        self,
-        client_name: Optional[str] = None,
-        client_connection: Optional[str] = None,
-        stop_token: Optional[str] = None,
-        **kwargs: Any,
-    ) -> None:
-        """
-        Change manifest client.
-
-        Args:
-            client_name: name of client.
-            client_connection: connection string for client.
-            stop_token: stop token prompt generation.
-                        Can be overridden in run
-
-        Remaining kwargs sent to client.
-        """
-        if client_name:
-            if client_name not in CLIENT_CONSTRUCTORS:
-                raise ValueError(
-                    f"Unknown client name: {client_name}. "
-                    f"Choices are {list(CLIENT_CONSTRUCTORS.keys())}"
-                )
-            self.client_name = client_name
-            self.client = CLIENT_CONSTRUCTORS[client_name](  # type: ignore
-                client_connection, client_args=kwargs
-            )
-            if len(kwargs) > 0:
-                raise ValueError(
-                    f"{list(kwargs.items())} arguments are not recognized."
-                )
-
-        if stop_token is not None:
-            self.stop_token = stop_token
-
     def _validate_kwargs(self, kwargs: Dict, request_params: Request) -> None:
         """Validate kwargs.
 
         Args:
             kwargs: kwargs to validate.
             request_params: request object to validate against.
         """
@@ -176,14 +122,15 @@
         if len(request_unused_kwargs) > 0:
             logger.warning(f"{list(request_unused_kwargs)} arguments are unused.")
         return
 
     def _split_cached_requests(
         self,
         request: Request,
+        client: Client,
         overwrite_cache: bool,
     ) -> Tuple[Dict[int, Response], Request]:
         """Split a request into cached responses and Requests to run.
 
         Args:
             request: request object.
             overwrite_cache: whether to overwrite cache.
@@ -197,121 +144,110 @@
         if not overwrite_cache:
             if isinstance(new_request.prompt, list):
                 new_request.prompt = []
                 for idx, prompt_str in enumerate(request.prompt):
                     single_request = copy.deepcopy(request)
                     single_request.prompt = prompt_str
                     possible_response = self.cache.get(
-                        self.client.get_cache_key(single_request)
+                        client.get_cache_key(single_request)
                     )
                     if possible_response:
                         cached_idx_to_response[idx] = possible_response
                     else:
                         new_request.prompt.append(prompt_str)
             else:
-                possible_response = self.cache.get(
-                    self.client.get_cache_key(new_request)
-                )
+                possible_response = self.cache.get(client.get_cache_key(new_request))
                 if possible_response:
                     cached_idx_to_response[0] = possible_response
                     new_request.prompt = None
         return cached_idx_to_response, new_request
 
     def _stitch_responses_and_cache(
         self,
         request: Request,
+        client: Client,
         response: Union[Response, None],
         cached_idx_to_response: Dict[int, Response],
     ) -> Response:
         """Stich together the cached and uncached responses."""
         # We stitch the responses (the choices) here from both the new request the
         # cached entries.
         all_model_choices = []
         all_usages = []
         all_input_prompts = []
         response_idx = 0
         number_prompts = len(cached_idx_to_response)
         single_output = False
         if response:
-            if isinstance(response.get_request()["prompt"], str):
+            if isinstance(response.get_request_obj().prompt, str):
                 single_output = True
                 number_prompts += 1
             else:
-                number_prompts += len(response.get_request()["prompt"])
-        response_gen_key = None
-        response_logits_key = None
-        response_item_key = None
+                number_prompts += len(response.get_request_obj().prompt)
+        response_type = None
+        request_type: Type[Request] = None
         for idx in range(number_prompts):
             if idx in cached_idx_to_response:
                 cached_res = cached_idx_to_response[idx]
-                response_gen_key = cached_res.generation_key
-                response_logits_key = cached_res.logits_key
-                response_item_key = cached_res.item_key
-                response_usage_key = cached_res.usage_key
-                all_input_prompts.append(cached_res.get_request()["prompt"])
-                json_response = cached_res.get_json_response()
+                response_type = cached_res._response_type
+                request_type = cached_res._request_type
+                all_input_prompts.append(cached_res.get_request_obj().prompt)
                 if request.n == 1:
                     assert (
-                        len(json_response[response_gen_key]) == 1
+                        len(cached_res.get_response_obj().choices) == 1
                     ), "cached response should have only one choice"
-                all_model_choices.extend(json_response[response_gen_key])
-                if response_usage_key:
-                    all_usages.extend(json_response[response_usage_key])
+                all_model_choices.extend(cached_res.get_response_obj().choices)
+                if cached_res.get_usage_obj().usages:
+                    all_usages.extend(cached_res.get_usage_obj().usages)
             else:
                 assert response is not None, "response should not be None"
                 response = cast(Response, response)
-                response_gen_key = response.generation_key
-                response_logits_key = response.logits_key
-                response_item_key = response.item_key
-                response_usage_key = response.usage_key
+                response_type = response._response_type
+                request_type = response._request_type
                 # the choices list in the response is a flat one.
                 # length is request.n * num_prompts
-                current_choices = response.get_json_response()[response_gen_key][
+                current_choices = response.get_response_obj().choices[
                     response_idx * request.n : (response_idx + 1) * request.n
                 ]
                 all_model_choices.extend(current_choices)
 
-                if isinstance(response.get_request()["prompt"], list):
-                    prompt = response.get_request()["prompt"][response_idx]
+                if isinstance(response.get_request_obj().prompt, list):
+                    prompt = response.get_request_obj().prompt[response_idx]
                 else:
-                    prompt = str(response.get_request()["prompt"])
-                if response_usage_key:
-                    usage = response.get_json_response()[response_usage_key][
+                    prompt = str(response.get_request_obj().prompt)
+                usages: Optional[List[Usage]] = None
+                if response.get_usage_obj().usages:
+                    usages = response.get_usage_obj().usages[
                         response_idx * request.n : (response_idx + 1) * request.n
                     ]
-                    all_usages.extend(usage)
+                    all_usages.extend(usages)
                 all_input_prompts.append(prompt)
                 # set cache
                 new_request = copy.deepcopy(request)
                 new_request.prompt = prompt
-                cache_key = self.client.get_cache_key(new_request)
-                new_response_key = copy.deepcopy(response.get_json_response())
-                new_response_key[response_gen_key] = current_choices
-                if response_usage_key:
-                    new_response_key[response_usage_key] = usage
-                self.cache.set(cache_key, new_response_key)
+                cache_key = client.get_cache_key(new_request)
+                new_response = copy.deepcopy(response)
+                new_response._response.choices = current_choices
+                new_response._usages = Usages(usages=(usages or []))
+                self.cache.set(cache_key, new_response.to_dict(drop_request=True))
                 response_idx += 1
 
         new_request = copy.deepcopy(request)
         new_request.prompt = (
-            all_input_prompts
+            all_input_prompts  # type: ignore
             if len(all_input_prompts) > 1 or not single_output
             else all_input_prompts[0]
         )
-        new_response = {response_gen_key: all_model_choices}
-        if response_usage_key:
-            new_response[response_usage_key] = all_usages
         response_obj = Response(
-            new_response,
+            response=ModelChoices(choices=all_model_choices),
             cached=len(cached_idx_to_response) > 0,
-            request_params=self.client.get_cache_key(new_request),
-            generation_key=response_gen_key,
-            logits_key=response_logits_key,
-            item_key=response_item_key,
-            usage_key=response_usage_key,
+            request=new_request,
+            usages=Usages(usages=all_usages),
+            response_type=response_type,
+            request_type=request_type,
         )
         return response_obj
 
     def run(
         self,
         prompt: Union[str, List[str]],
         overwrite_cache: bool = False,
@@ -330,35 +266,40 @@
                         "" for no stop token.
             return_response: whether to return Response object.
 
         Returns:
             response from prompt.
         """
         is_batch = isinstance(prompt, list)
-
+        # Get the client to run
+        client = self.client_pool.get_client()
         stop_token = stop_token if stop_token is not None else self.stop_token
         # Must pass kwargs as dict for client "pop" methods removed used arguments
-        request_params = self.client.get_request(prompt, kwargs)
+        request_params = client.get_request(prompt, kwargs)
         # Avoid nested list of results - enforce n = 1 for batch
         if is_batch and request_params.n > 1:
             raise ValueError("Batch mode does not support n > 1.")
         self._validate_kwargs(kwargs, request_params)
 
         cached_idx_to_response, request_params = self._split_cached_requests(
-            request_params, overwrite_cache
+            request_params, client, overwrite_cache
         )
         # If not None value or empty list - run new request
         if request_params.prompt:
-            response = self.client.run_request(request_params)
+            # Start timing metrics
+            self.client_pool.start_timer()
+            response = client.run_request(request_params)
+            self.client_pool.end_timer()
         else:
             # Nothing to run
             response = None
 
         final_response = self._stitch_responses_and_cache(
             request=request_params,
+            client=client,
             response=response,
             cached_idx_to_response=cached_idx_to_response,
         )
 
         # Extract text results
         if return_response:
             return final_response
@@ -367,62 +308,127 @@
 
     async def arun_batch(
         self,
         prompts: List[str],
         overwrite_cache: bool = False,
         stop_token: Optional[str] = None,
         return_response: bool = False,
+        chunk_size: int = -1,
         **kwargs: Any,
     ) -> Union[List[str], List[np.ndarray], Response]:
         """
         Run a batch of prompts with async.
 
+        If the client pool is a single client, all prompts will be sent
+        to one client and batch_size (which is passed it as kwargs) will
+        determine how the prompts are split.
+
+        If the client pool is a pool of clients, the prompts will be split
+        into chunks and sent to the clients. Each client will split the
+        chunk into batch_size prompts to send to the model.
+
         Args:
             prompts: prompts to run.
             overwrite_cache: whether to overwrite cache.
             stop_token: stop token for prompt generation.
-                        Default is self.stop_token.
-                        "" for no stop token.
+                Default is self.stop_token.
+                "" for no stop token.
             return_response: whether to return Response object.
+            chunk_size: number of prompts to send to a client in chunks.
+                For each chunk, the client will split the chunk into
+                batch_sized prompts to send to the model.
+                For a single manifest client, there is no impact to
+                setting chunk_size. For a client pool, chunk_size
+                can be used to distribute the load across the clients.
 
         Returns:
             response from prompt.
         """
+        # Split the prompts into chunks
+        prompt_chunks: List[Tuple[Client, List[str]]] = []
+        if chunk_size > 0:
+            for i in range(0, len(prompts), chunk_size):
+                prompt_chunks.append(
+                    (self.client_pool.get_client(), prompts[i : i + chunk_size])
+                )
+        else:
+            prompt_chunks = [(self.client_pool.get_client(), prompts)]
+
+        # Run the chunks
+        tasks = []
+        for client, chunk in prompt_chunks:
+            tasks.append(
+                asyncio.create_task(
+                    self._arun_batch_client(
+                        prompts=chunk,
+                        client=client,
+                        overwrite_cache=overwrite_cache,
+                        **kwargs,
+                    )
+                )
+            )
+        print(f"Running {len(tasks)} tasks across all clients.")
+        logger.info(f"Running {len(tasks)} tasks across all clients.")
+        responses = await asyncio.gather(*tasks)
+        final_response = Response.union_all(responses)
         stop_token = stop_token if stop_token is not None else self.stop_token
+
+        # Extract text results
+        if return_response:
+            return final_response
+        else:
+            return cast(
+                Union[List[str], List[np.ndarray]],
+                final_response.get_response(stop_token, True),
+            )
+
+    async def _arun_batch_client(
+        self,
+        prompts: List[str],
+        client: Client,
+        overwrite_cache: bool = False,
+        **kwargs: Any,
+    ) -> Response:
+        """
+        Run a batch of prompts with async for single client.
+
+        Args:
+            prompts: prompts to run.
+            client: client to run.
+            overwrite_cache: whether to overwrite cache.
+
+        Returns:
+            response from prompt.
+        """
         # Must pass kwargs as dict for client "pop" methods removed used arguments
-        request_params = self.client.get_request(prompts, kwargs)
+        request_params = client.get_request(prompts, kwargs)
         # Avoid nested list of results - enforce n = 1 for batch
         if request_params.n > 1:
             raise ValueError("Batch mode does not support n > 1.")
         self._validate_kwargs(kwargs, request_params)
 
         cached_idx_to_response, request_params = self._split_cached_requests(
-            request_params, overwrite_cache
+            request_params, client, overwrite_cache
         )
         # If not None value or empty list - run new request
         if request_params.prompt:
-            response = await self.client.arun_batch_request(request_params)
+            self.client_pool.start_timer()
+            response = await client.arun_batch_request(request_params)
+            self.client_pool.end_timer()
         else:
             # Nothing to run
             response = None
 
         final_response = self._stitch_responses_and_cache(
             request=request_params,
+            client=client,
             response=response,
             cached_idx_to_response=cached_idx_to_response,
         )
-
-        # Extract text results
-        if return_response:
-            return final_response
-        else:
-            return cast(
-                Union[List[str], List[np.ndarray]],
-                final_response.get_response(stop_token, True),
-            )
+        return final_response
 
     def score_prompt(
         self,
         prompt: Union[str, List[str]],
         overwrite_cache: bool = False,
         **kwargs: Any,
     ) -> Dict:
@@ -434,36 +440,38 @@
         Args:
             prompt: prompt(s) to run.
             overwrite_cache: whether to overwrite cache.
 
         Returns:
             response from prompt.
         """
+        client = self.client_pool.get_client()
         # Must pass kwargs as dict for client "pop" methods removed used arguments
-        request_params = self.client.get_request(prompt, kwargs)
-        request_params.request_type = "score_prompt"
+        request_params = client.get_request(prompt, kwargs)
+        request_params_as_score = LMScoreRequest(**request_params.to_dict())
 
-        if request_params.n > 1:
+        if request_params_as_score.n > 1:
             raise ValueError("Sequence scoring does not support n > 1.")
-        self._validate_kwargs(kwargs, request_params)
+        self._validate_kwargs(kwargs, request_params_as_score)
 
-        cached_idx_to_response, request_params = self._split_cached_requests(
-            request_params, overwrite_cache
+        cached_idx_to_response, request_params_as_score = self._split_cached_requests(  # type: ignore # noqa: E501
+            request_params_as_score, client, overwrite_cache
         )
         # If not None value or empty list - run new request
-        if request_params.prompt:
+        if request_params_as_score.prompt:
             try:
-                response = cast(
-                    HuggingFaceClient, self.client
-                ).get_score_prompt_request(request_params)
+                response = cast(HuggingFaceClient, client).get_score_prompt_request(
+                    request_params_as_score
+                )
             except AttributeError:
                 raise ValueError("`score_prompt` only supported for HF models.")
         else:
             # Nothing to run
             response = None
 
         final_response = self._stitch_responses_and_cache(
-            request=request_params,
+            request=request_params_as_score,
+            client=client,
             response=response,
             cached_idx_to_response=cached_idx_to_response,
         )
         return final_response.to_dict()
```

### Comparing `manifest-ml-0.1.3/manifest/request.py` & `manifest-ml-0.1.4/manifest/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Request object."""
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from pydantic import BaseModel
 
+# Used when unioning requests after async connection pool
+ENGINE_SEP = "::"
 NOT_CACHE_KEYS = {"client_timeout", "batch_size"}
+# The below should match those in Request.
 DEFAULT_REQUEST_KEYS = {
     "client_timeout": ("client_timeout", 60),  # seconds
-    "batch_size": ("batch_size", 1),
+    "batch_size": ("batch_size", 8),
     "run_id": ("run_id", None),
-    "request_type": ("request_type", None),
 }
 
 
 class Request(BaseModel):
     """Request object."""
 
     # Prompt
@@ -21,31 +23,31 @@
     # Engine
     engine: str = "text-ada-001"
 
     # Number completions
     n: int = 1
 
     # Timeout
-    client_timeout: int = 120
+    client_timeout: int = 60
 
     # Run id used to repeat run with same parameters
     run_id: Optional[str] = None
 
     # Batch size for async batch run
     batch_size: int = 8
 
-    # Request type None is for completion. Used to scoring prompt
-    request_type: str = None
-
     def to_dict(
         self, allowable_keys: Dict[str, Tuple[str, Any]] = None, add_prompt: bool = True
     ) -> Dict[str, Any]:
         """
         Convert request to a dictionary.
 
+        Handles parameter renaming but does not fill in default values.
+        It will drop any None values.
+
         Add prompt ensures the prompt is always in the output dictionary.
         """
         if allowable_keys:
             include_keys = set(allowable_keys.keys())
             if add_prompt and "prompt":
                 include_keys.add("prompt")
         else:
@@ -70,14 +72,17 @@
 
     # Nucleus sampling taking top_p probability mass tokens
     top_p: float = 1.0
 
     # Top k sampling taking top_k highest probability tokens
     top_k: int = 50
 
+    # Logprobs return value
+    logprobs: Optional[int] = None
+
     # Stop sequences
     stop_sequences: Optional[List[str]] = None
 
     # Number beams beam search (HF)
     num_beams: int = 1
 
     # Whether to sample or do greedy (HF)
@@ -92,26 +97,29 @@
     # Penalize resence
     presence_penalty: float = 0
 
     # Penalize frequency
     frequency_penalty: float = 0
 
 
+class LMScoreRequest(LMRequest):
+    """Language Model Score Request object."""
+
+    pass
+
+
 class EmbeddingRequest(Request):
     """Embedding Request object."""
 
     pass
 
 
 class DiffusionRequest(Request):
     """Diffusion Model Request object."""
 
-    # Request type
-    request_type: str = "diffusion"
-
     # Number of steps
     num_inference_steps: int = 50
 
     # Height of image
     height: int = 512
 
     # Width of image
```

### Comparing `manifest-ml-0.1.3/manifest_ml.egg-info/PKG-INFO` & `manifest-ml-0.1.4/manifest_ml.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -28,14 +28,15 @@
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
 - [Embedding Models](#embedding-models)
+- [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
 ```bash
@@ -76,15 +77,15 @@
 We have example notebook and python scripts located at [examples](examples). These show how to use different models, model types (i.e. text, diffusers, or embedding models), and async running.
 
 # Manifest Components
 Manifest is meant to be a very light weight package to help with prompt design and iteration. Three key design decisions of Manifest are
 
 * All models are behind APIs
 * Supports caching of model inputs/outputs for iteration, reproducibility, and cost saving
-* Unified API of generate, score, and embed
+* Unified API to support generate, score, and embed
 
 ## Models
 Manifest provides model clients for [OpenAI](https://openai.com/), [AI21](https://studio.ai21.com/), [Cohere](https://cohere.ai/), [Together](https://together.xyz/), and HuggingFace (see [below](#huggingface-models) for how to use locally hosted HuggingFace models). You can toggle between the models by changing `client_name` and `client_connection`. For example, if a HuggingFace model is loaded locally, run
 ```python
 manifest = Manifest(
     client_name = "huggingface",
     client_connection = "http://127.0.0.1:5000",
@@ -145,29 +146,56 @@
 import asyncio
 results = asyncio.run(manifest.arun_batch(["Where are the cats?", "Where are the dogs?"]))
 ```
 
 If something doesn't go right, you can also ask to get a raw manifest Response.
 ```python
 result_object = manifest.run(["Where are the cats?", "Where are the dogs?"], return_response=True)
-print(result_object.get_request())
+print(result_object.get_request_obj())
 print(result_object.is_cached())
-print(result_object.get_json_response())
+print(result_object.get_response_obj())
 ```
 
 By default, we do not truncate results based on a stop token. You can change this by either passing a new stop token to a Manifest session or to a `run`.
 ```python
 result = manifest.run(prompt, "Laurel", stop_token="and")
 ```
 
 If you want to change default parameters to a model, we pass those as `kwargs` to the client.
 ```python
 result = manifest.run(prompt, "Laurel", max_tokens=50)
 ```
 
+## Model Pools
+Manifest supports querying multiple models with different schedulers. This is very much a work in progress effort, but Manifest will round robin select (or randomly select) the clients you want. You can use the same client multiple times with different connection strings (e.g. different API keys), or you can mix and match. The only requirement is that all clients are the same request type. I.e. you can't have a pool of generation models and embedding models.
+
+To query between a local model and OpenAI,
+```python
+from manifest.connections.client_pool import ClientConnection
+from manifest import Manifest
+
+client_connection1 = ClientConnection(
+    client_name="huggingface",
+    client_connection="http://127.0.0.1:5000",
+)
+client_connection2 = ClientConnection(client_name="openai", engine="text-ada-001")
+manifest = Manifest(
+    client_pool=[client_connection1, client_connection2],
+    cache_name="sqlite",
+    client_connection=sqlite_cache,
+)
+manifest.run(...)
+```
+
+The speed benefit comes in with async batched runs. When calling `arun_batch` with a list of prompts, Manifest supports a `chunk_size` param. This will break the prompts into `chunk_size` chunks to spread across the client pool. By default `chunk_size` is `-1` which means only one client will get all the prompts to run asynchronously. You must set `chunk_size > 1` to distribute across the pool. There is a further `batch_size` param which control the individual client `batch_size` to send to the model.
+
+```python
+responses = asyncio.run(manifest.arun_batch(prompts, max_tokens=30, chunk_size=20))
+```
+
 # Local Huggingface Models
 To use a HuggingFace generative model, in `manifest/api` we have a Flask application that hosts the models for you.
 
 In a separate terminal or Tmux/Screen session, to load 6B parameters models, run
 ```bash
 python3 -m manifest.api.app \
     --model_type huggingface \
@@ -225,14 +253,27 @@
 ```bash
 python3 -m manifest.api.app \
     --model_type sentence_transformers \
     --model_name_or_path all-mpnet-base-v2 \
     --device 0
 ```
 
+# Road Map
+Here's what's coming up next
+- [ ] Clients
+  - [ ] HuggingFace Hub
+  - [ ] Azure OpenAI
+  - [ ] Anthropic
+- [ ] Data Types
+  - [ ] Diffusion Models
+- [ ] Orchestration
+  - [x] Connection pools
+- [ ] Local Inference
+  - [ ] FlexGen
+
 # Development
 Before submitting a PR, run
 ```bash
 export REDIS_PORT="6379"  # or whatever PORT local redis is running for those tests
 cd <REDIS_PATH>
 docker run -d -p 127.0.0.1:${REDIS_PORT}:6379 -v `pwd`:`pwd` -w `pwd` --name manifest_redis_test redis
 make test
```

### Comparing `manifest-ml-0.1.3/manifest_ml.egg-info/SOURCES.txt` & `manifest-ml-0.1.4/manifest_ml.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,28 @@
 manifest/clients/huggingface.py
 manifest/clients/huggingface_embedding.py
 manifest/clients/openai.py
 manifest/clients/openai_chat.py
 manifest/clients/openai_embedding.py
 manifest/clients/toma.py
 manifest/clients/toma_diffuser.py
+manifest/connections/__init__.py
+manifest/connections/client_pool.py
+manifest/connections/scheduler.py
 manifest_ml.egg-info/PKG-INFO
 manifest_ml.egg-info/SOURCES.txt
 manifest_ml.egg-info/dependency_links.txt
 manifest_ml.egg-info/requires.txt
 manifest_ml.egg-info/top_level.txt
 tests/test_array_cache.py
 tests/test_cache.py
 tests/test_client.py
+tests/test_client_pool.py
 tests/test_huggingface_api.py
 tests/test_manifest.py
 tests/test_request.py
 tests/test_response.py
+tests/test_scheduler.py
 tests/test_serializer.py
 web_app/__init__.py
 web_app/main.py
 web_app/schemas.py
```

### Comparing `manifest-ml-0.1.3/manifest_ml.egg-info/requires.txt` & `manifest-ml-0.1.4/manifest_ml.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 aiohttp>=3.8.0
 sqlitedict>=2.0.0
 tenacity>=8.2.0
 tiktoken>=0.3.0
 xxhash>=3.0.0
 
 [all]
-types-xxhash>=3.0.0
-uvicorn>=0.18.0
-python-dotenv>=0.20.0
 types-requests>=2.27.29
-sphinx-rtd-theme>=0.5.1
-pre-commit>=2.14.0
-sphinx-autobuild
-sqlalchemy
-pg8000
-pillow>=9.0.0
-types-protobuf>=3.19.21
-twine
 accelerate>=0.10.0
-flake8>=4.0.0
-cloud-sql-python-connector[pg8000]>=1.0.0
-pep8-naming>=0.12.1
-recommonmark>=0.7.1
-sentence_transformers>=2.2.0
+Flask>=2.1.2
+transformers<4.26.0,>=4.20.0
 types-redis>=4.2.6
 pytest>=7.0.0
-types-pillow>=9.0.0
+pytest-cov>=3.0.0
+diffusers>=0.6.0
+black>=22.3.0
+flake8>=4.0.0
 torch>=1.8.0
-autopep8>=1.6.0
+pillow>=9.0.0
+python-dotenv>=0.20.0
+sqlalchemy
+types-protobuf>=3.19.21
+recommonmark>=0.7.1
+sentence_transformers>=2.2.0
+types-xxhash>=3.0.0
+pg8000
+pep8-naming>=0.12.1
+deepspeed>=0.7.0
+sphinx-rtd-theme>=0.5.1
 nbsphinx>=0.8.0
-fastapi>=0.70.0
-types-python-dateutil>=2.8.16
+twine
 types-PyYAML>=6.0.7
-transformers<4.26.0,>=4.20.0
-Flask>=2.1.2
-deepspeed>=0.7.0
-pytest-cov>=3.0.0
+types-python-dateutil>=2.8.16
+mypy>=0.950
+types-pillow>=9.0.0
+sphinx-autobuild
 docformatter>=1.4
-types-setuptools>=57.4.17
+autopep8>=1.6.0
+uvicorn>=0.18.0
+fastapi>=0.70.0
+cloud-sql-python-connector[pg8000]>=1.0.0
+pre-commit>=2.14.0
 isort>=5.9.3
-diffusers>=0.6.0
-black>=22.3.0
-mypy>=0.950
+types-setuptools>=57.4.17
 flake8-docstrings>=1.6.0
 
 [api]
 accelerate>=0.10.0
 deepspeed>=0.7.0
 diffusers>=0.6.0
 Flask>=2.1.2
```

### Comparing `manifest-ml-0.1.3/pyproject.toml` & `manifest-ml-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/setup.py` & `manifest-ml-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/tests/test_array_cache.py` & `manifest-ml-0.1.4/tests/test_array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/tests/test_cache.py` & `manifest-ml-0.1.4/tests/test_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Cache test."""
-from typing import Dict, cast
+from typing import Dict, Type, cast
 
 import numpy as np
 import pytest
 from redis import Redis
 from sqlitedict import SqliteDict
 
 from manifest.caches.cache import Cache
 from manifest.caches.noop import NoopCache
 from manifest.caches.postgres import PostgresCache
 from manifest.caches.redis import RedisCache
 from manifest.caches.sqlite import SQLiteCache
+from manifest.request import DiffusionRequest, LMRequest, Request
+from manifest.response import ArrayModelChoice, ModelChoices, Response
 
 
 def _get_postgres_cache(
-    client_name: str = "", cache_args: Dict = {}
+    request_type: Type[Request] = LMRequest, cache_args: Dict = {}
 ) -> Cache:  # type: ignore
     """Get postgres cache."""
     cache_args.update({"cache_user": "", "cache_password": "", "cache_db": ""})
     return PostgresCache(
         "postgres",
-        client_name=client_name,
+        request_type=request_type,
         cache_args=cache_args,
     )
 
 
 @pytest.mark.usefixtures("sqlite_cache")
 @pytest.mark.usefixtures("redis_cache")
 @pytest.mark.usefixtures("postgres_cache")
@@ -73,171 +75,148 @@
 
 
 @pytest.mark.usefixtures("sqlite_cache")
 @pytest.mark.usefixtures("redis_cache")
 @pytest.mark.usefixtures("postgres_cache")
 @pytest.mark.parametrize("cache_type", ["sqlite", "redis", "postgres"])
 def test_get(
-    sqlite_cache: str, redis_cache: str, postgres_cache: str, cache_type: str
+    sqlite_cache: str,
+    redis_cache: str,
+    postgres_cache: str,
+    cache_type: str,
+    model_choice: ModelChoices,
+    model_choice_single: ModelChoices,
+    model_choice_arr_int: ModelChoices,
+    request_lm: LMRequest,
+    request_lm_single: LMRequest,
+    request_diff: DiffusionRequest,
 ) -> None:
     """Test cache save prompt."""
     if cache_type == "sqlite":
         cache = cast(Cache, SQLiteCache(sqlite_cache))
     elif cache_type == "redis":
         cache = cast(Cache, RedisCache(redis_cache))
     elif cache_type == "postgres":
         cache = cast(Cache, _get_postgres_cache())
 
-    test_request = {"test": "hello", "testA": "world"}
-    test_response = {"choices": [{"text": "hello"}]}
+    response = Response(
+        response=model_choice_single,
+        cached=False,
+        request=request_lm_single,
+        usages=None,
+        request_type=LMRequest,
+        response_type="text",
+    )
+
+    cache_response = cache.get(request_lm_single.dict())
+    assert cache_response is None
 
-    response = cache.get(test_request)
-    assert response is None
+    cache.set(request_lm_single.dict(), response.to_dict(drop_request=True))
+    cache_response = cache.get(request_lm_single.dict())
+    assert cache_response.get_response() == "helloo"
+    assert cache_response.is_cached()
+    assert cache_response.get_request_obj() == request_lm_single
+
+    response = Response(
+        response=model_choice,
+        cached=False,
+        request=request_lm,
+        usages=None,
+        request_type=LMRequest,
+        response_type="text",
+    )
 
-    cache.set(test_request, test_response)
-    response = cache.get(test_request)
-    assert response.get_response() == "hello"
-    assert response.is_cached()
-    assert response.get_request() == test_request
+    cache_response = cache.get(request_lm.dict())
+    assert cache_response is None
+
+    cache.set(request_lm.dict(), response.to_dict(drop_request=True))
+    cache_response = cache.get(request_lm.dict())
+    assert cache_response.get_response() == ["hello", "bye"]
+    assert cache_response.is_cached()
+    assert cache_response.get_request_obj() == request_lm
 
     # Test array
-    arr = np.random.rand(4, 4)
-    test_request = {"test": "hello", "testA": "world of images"}
-    compute_arr_response = {"choices": [{"array": arr}]}
+    response = Response(
+        response=model_choice_arr_int,
+        cached=False,
+        request=request_diff,
+        usages=None,
+        request_type=DiffusionRequest,
+        response_type="array",
+    )
 
     if cache_type == "sqlite":
-        cache = SQLiteCache(sqlite_cache, client_name="diffuser")
+        cache = SQLiteCache(sqlite_cache, request_type=DiffusionRequest)
     elif cache_type == "redis":
-        cache = RedisCache(redis_cache, client_name="diffuser")
+        cache = RedisCache(redis_cache, request_type=DiffusionRequest)
     elif cache_type == "postgres":
-        cache = _get_postgres_cache(client_name="diffuser")
+        cache = _get_postgres_cache(request_type=DiffusionRequest)
 
-    response = cache.get(test_request)
-    assert response is None
+    cache_response = cache.get(request_diff.dict())
+    assert cache_response is None
 
-    cache.set(test_request, compute_arr_response)
-    response = cache.get(test_request)
-    assert np.allclose(response.get_response(), arr)
-    assert response.is_cached()
-    assert response.get_request() == test_request
+    cache.set(request_diff.dict(), response.to_dict(drop_request=True))
+    cached_response = cache.get(request_diff.dict())
+    assert np.allclose(
+        cached_response.get_response()[0],
+        cast(ArrayModelChoice, model_choice_arr_int.choices[0]).array,
+    )
+    assert np.allclose(
+        cached_response.get_response()[1],
+        cast(ArrayModelChoice, model_choice_arr_int.choices[1]).array,
+    )
+    assert cached_response.is_cached()
+    assert cached_response.get_request_obj() == request_diff
 
     # Test array byte string
-    arr = np.random.rand(4, 4)
-    test_request = {"test": "hello", "testA": "world of images 2"}
-    compute_arr_response = {"choices": [{"array": arr}]}
+    # Make sure to not hit the cache
+    new_request_diff = DiffusionRequest(**request_diff.dict())
+    new_request_diff.prompt = ["blahhh", "yayayay"]
+    response = Response(
+        response=model_choice_arr_int,
+        cached=False,
+        request=new_request_diff,
+        usages=None,
+        request_type=DiffusionRequest,
+        response_type="array",
+    )
 
     if cache_type == "sqlite":
         cache = SQLiteCache(
             sqlite_cache,
-            client_name="diffuser",
+            request_type=DiffusionRequest,
             cache_args={"array_serializer": "byte_string"},
         )
     elif cache_type == "redis":
         cache = RedisCache(
             redis_cache,
-            client_name="diffuser",
+            request_type=DiffusionRequest,
             cache_args={"array_serializer": "byte_string"},
         )
     elif cache_type == "postgres":
         cache = _get_postgres_cache(
-            client_name="diffuser", cache_args={"array_serializer": "byte_string"}
-        )
-
-    response = cache.get(test_request)
-    assert response is None
-
-    cache.set(test_request, compute_arr_response)
-    response = cache.get(test_request)
-    assert np.allclose(response.get_response(), arr)
-    assert response.is_cached()
-    assert response.get_request() == test_request
-
-
-@pytest.mark.usefixtures("sqlite_cache")
-@pytest.mark.usefixtures("redis_cache")
-@pytest.mark.usefixtures("postgres_cache")
-@pytest.mark.parametrize("cache_type", ["sqlite", "redis", "postgres"])
-def test_get_batch_prompt(
-    sqlite_cache: str, redis_cache: str, postgres_cache: str, cache_type: str
-) -> None:
-    """Test cache save prompt."""
-    if cache_type == "sqlite":
-        cache = cast(Cache, SQLiteCache(sqlite_cache))
-    elif cache_type == "redis":
-        cache = cast(Cache, RedisCache(redis_cache))
-    elif cache_type == "postgres":
-        cache = cast(Cache, _get_postgres_cache())
-
-    test_request = {"test": ["hello", "goodbye"], "testA": "world"}
-    test_response = {"choices": [{"text": "hello"}, {"text": "goodbye"}]}
-
-    response = cache.get(test_request)
-    assert response is None
-
-    cache.set(test_request, test_response)
-    response = cache.get(test_request)
-    assert response.get_response() == ["hello", "goodbye"]
-    assert response.is_cached()
-    assert response.get_request() == test_request
-
-    # Test arrays
-    arr = np.random.rand(4, 4)
-    arr2 = np.random.rand(4, 4)
-    test_request = {"test": ["hello", "goodbye"], "testA": "world of images"}
-    compute_arr_response = {"choices": [{"array": arr}, {"array": arr2}]}
-
-    if cache_type == "sqlite":
-        cache = SQLiteCache(sqlite_cache, client_name="diffuser")
-    elif cache_type == "redis":
-        cache = RedisCache(redis_cache, client_name="diffuser")
-    elif cache_type == "postgres":
-        cache = _get_postgres_cache(client_name="diffuser")
-
-    response = cache.get(test_request)
-    assert response is None
-
-    cache.set(test_request, compute_arr_response)
-    response = cache.get(test_request)
-    assert np.allclose(response.get_response()[0], arr)
-    assert np.allclose(response.get_response()[1], arr2)
-    assert response.is_cached()
-    assert response.get_request() == test_request
-
-    # Test arrays byte serializer
-    arr = np.random.rand(4, 4)
-    arr2 = np.random.rand(4, 4)
-    test_request = {"test": ["hello", "goodbye"], "testA": "world of images 2"}
-    compute_arr_response = {"choices": [{"array": arr}, {"array": arr2}]}
-
-    if cache_type == "sqlite":
-        cache = SQLiteCache(
-            sqlite_cache,
-            client_name="diffuser",
-            cache_args={"array_serializer": "byte_string"},
-        )
-    elif cache_type == "redis":
-        cache = RedisCache(
-            redis_cache,
-            client_name="diffuser",
+            request_type=DiffusionRequest,
             cache_args={"array_serializer": "byte_string"},
         )
-    elif cache_type == "postgres":
-        cache = _get_postgres_cache(
-            client_name="diffuser", cache_args={"array_serializer": "byte_string"}
-        )
 
-    response = cache.get(test_request)
-    assert response is None
+    cached_response = cache.get(new_request_diff.dict())
+    assert cached_response is None
 
-    cache.set(test_request, compute_arr_response)
-    response = cache.get(test_request)
-    assert np.allclose(response.get_response()[0], arr)
-    assert np.allclose(response.get_response()[1], arr2)
-    assert response.is_cached()
-    assert response.get_request() == test_request
+    cache.set(new_request_diff.dict(), response.to_dict(drop_request=True))
+    cached_response = cache.get(new_request_diff.dict())
+    assert np.allclose(
+        cached_response.get_response()[0],
+        cast(ArrayModelChoice, model_choice_arr_int.choices[0]).array,
+    )
+    assert np.allclose(
+        cached_response.get_response()[1],
+        cast(ArrayModelChoice, model_choice_arr_int.choices[1]).array,
+    )
+    assert cached_response.is_cached()
+    assert cached_response.get_request_obj() == new_request_diff
 
 
 def test_noop_cache() -> None:
     """Test cache that is a no-op cache."""
     cache = NoopCache(None)
     cache.set_key("test", "valueA")
     cache.set_key("testA", "valueB")
```

### Comparing `manifest-ml-0.1.3/tests/test_huggingface_api.py` & `manifest-ml-0.1.4/tests/test_huggingface_api.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/tests/test_manifest.py` & `manifest-ml-0.1.4/tests/test_manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import requests
 from requests import HTTPError
 
 from manifest import Manifest, Response
 from manifest.caches.noop import NoopCache
 from manifest.caches.sqlite import SQLiteCache
 from manifest.clients.dummy import DummyClient
+from manifest.connections.client_pool import ClientConnection
 
 URL = "http://localhost:6000"
 try:
     _ = requests.post(URL + "/params").json()
     MODEL_ALIVE = True
 except Exception:
     MODEL_ALIVE = False
@@ -37,54 +38,32 @@
     assert str(exc_info.value) == "[('sep_tok', '')] arguments are not recognized."
 
     manifest = Manifest(
         client_name="dummy",
         cache_name="sqlite",
         cache_connection=sqlite_cache,
     )
-    assert manifest.client_name == "dummy"
-    assert isinstance(manifest.client, DummyClient)
+    assert len(manifest.client_pool.client_pool) == 1
+    client = manifest.client_pool.get_client()
+    assert isinstance(client, DummyClient)
     assert isinstance(manifest.cache, SQLiteCache)
-    assert manifest.client.n == 1  # type: ignore
+    assert client.n == 1  # type: ignore
     assert manifest.stop_token == ""
 
     manifest = Manifest(
         client_name="dummy",
         cache_name="noop",
         n=3,
         stop_token="\n",
     )
-    assert manifest.client_name == "dummy"
-    assert isinstance(manifest.client, DummyClient)
+    assert len(manifest.client_pool.client_pool) == 1
+    client = manifest.client_pool.get_client()
+    assert isinstance(client, DummyClient)
     assert isinstance(manifest.cache, NoopCache)
-    assert manifest.client.n == 3  # type: ignore
-    assert manifest.stop_token == "\n"
-
-
-@pytest.mark.usefixtures("sqlite_cache")
-def test_change_manifest(sqlite_cache: str) -> None:
-    """Test manifest change."""
-    manifest = Manifest(
-        client_name="dummy",
-        cache_name="sqlite",
-        cache_connection=sqlite_cache,
-    )
-
-    manifest.change_client()
-    assert manifest.client_name == "dummy"
-    assert isinstance(manifest.client, DummyClient)
-    assert isinstance(manifest.cache, SQLiteCache)
-    assert manifest.client.n == 1  # type: ignore
-    assert manifest.stop_token == ""
-
-    manifest.change_client(stop_token="\n")
-    assert manifest.client_name == "dummy"
-    assert isinstance(manifest.client, DummyClient)
-    assert isinstance(manifest.cache, SQLiteCache)
-    assert manifest.client.n == 1  # type: ignore
+    assert client.n == 3  # type: ignore
     assert manifest.stop_token == "\n"
 
 
 @pytest.mark.usefixtures("sqlite_cache")
 @pytest.mark.parametrize("n", [1, 2])
 @pytest.mark.parametrize("return_response", [True, False])
 def test_run(sqlite_cache: str, n: int, return_response: bool) -> None:
@@ -98,34 +77,35 @@
 
     prompt = "This is a prompt"
     with pytest.raises(ValueError) as exc_info:
         result = manifest.run(prompt, return_response=return_response, bad_input=5)
     assert str(exc_info.value) == "[('bad_input', 5)] arguments are not recognized."
 
     # Allow params in the request object but not in the client to go through
-    assert "top_k" not in manifest.client.PARAMS
+    assert "top_k" not in manifest.client_pool.get_client().PARAMS
     result = manifest.run(prompt, return_response=return_response, top_k=5)
     assert result is not None
 
     prompt = "This is a prompt"
     result = manifest.run(prompt, return_response=return_response)
     if return_response:
         assert isinstance(result, Response)
         result = cast(Response, result)
-        assert len(result.get_json_response()["usage"]) == len(
-            result.get_json_response()["choices"]
+        assert len(result.get_usage_obj().usages) == len(
+            result.get_response_obj().choices
         )
         res = result.get_response(manifest.stop_token)
     else:
         res = cast(str, result)
     assert (
         manifest.cache.get(
             {
                 "prompt": "This is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": n,
             },
         )
         is not None
     )
     if n == 1:
         assert res == "hello"
@@ -133,25 +113,26 @@
         assert res == ["hello", "hello"]
 
     prompt = "This is a prompt"
     result = manifest.run(prompt, run_id="34", return_response=return_response)
     if return_response:
         assert isinstance(result, Response)
         result = cast(Response, result)
-        assert len(result.get_json_response()["usage"]) == len(
-            result.get_json_response()["choices"]
+        assert len(result.get_usage_obj().usages) == len(
+            result.get_response_obj().choices
         )
         res = result.get_response(manifest.stop_token)
     else:
         res = cast(str, result)
     assert (
         manifest.cache.get(
             {
                 "prompt": "This is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": n,
                 "run_id": "34",
             }
         )
         is not None
     )
     if n == 1:
@@ -160,25 +141,26 @@
         assert res == ["hello", "hello"]
 
     prompt = "Hello is a prompt"
     result = manifest.run(prompt, return_response=return_response)
     if return_response:
         assert isinstance(result, Response)
         result = cast(Response, result)
-        assert len(result.get_json_response()["usage"]) == len(
-            result.get_json_response()["choices"]
+        assert len(result.get_usage_obj().usages) == len(
+            result.get_response_obj().choices
         )
         res = result.get_response(manifest.stop_token)
     else:
         res = cast(str, result)
     assert (
         manifest.cache.get(
             {
                 "prompt": "Hello is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": n,
             },
         )
         is not None
     )
     if n == 1:
         assert res == "hello"
@@ -186,25 +168,26 @@
         assert res == ["hello", "hello"]
 
     prompt = "Hello is a prompt"
     result = manifest.run(prompt, stop_token="ll", return_response=return_response)
     if return_response:
         assert isinstance(result, Response)
         result = cast(Response, result)
-        assert len(result.get_json_response()["usage"]) == len(
-            result.get_json_response()["choices"]
+        assert len(result.get_usage_obj().usages) == len(
+            result.get_response_obj().choices
         )
         res = result.get_response(stop_token="ll")
     else:
         res = cast(str, result)
     assert (
         manifest.cache.get(
             {
                 "prompt": "Hello is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": n,
             },
         )
         is not None
     )
     if n == 1:
         assert res == "he"
@@ -229,49 +212,51 @@
             result = manifest.run(prompt, return_response=return_response)
         assert str(exc_info.value) == "Batch mode does not support n > 1."
     else:
         result = manifest.run(prompt, return_response=return_response)
         if return_response:
             assert isinstance(result, Response)
             result = cast(Response, result)
-            assert len(result.get_json_response()["usage"]) == len(
-                result.get_json_response()["choices"]
+            assert len(result.get_usage_obj().usages) == len(
+                result.get_response_obj().choices
             )
             res = result.get_response(manifest.stop_token, is_batch=True)
         else:
             res = cast(str, result)
         assert res == ["hello"]
         assert (
             manifest.cache.get(
                 {
                     "prompt": "This is a prompt",
                     "engine": "dummy",
+                    "request_cls": "LMRequest",
                     "num_results": n,
                 },
             )
             is not None
         )
 
         prompt = ["Hello is a prompt", "Hello is a prompt"]
         result = manifest.run(prompt, return_response=return_response)
         if return_response:
             assert isinstance(result, Response)
             result = cast(Response, result)
-            assert len(result.get_json_response()["usage"]) == len(
-                result.get_json_response()["choices"]
+            assert len(result.get_usage_obj().usages) == len(
+                result.get_response_obj().choices
             )
             res = result.get_response(manifest.stop_token, is_batch=True)
         else:
             res = cast(str, result)
         assert res == ["hello", "hello"]
         assert (
             manifest.cache.get(
                 {
                     "prompt": "Hello is a prompt",
                     "engine": "dummy",
+                    "request_cls": "LMRequest",
                     "num_results": n,
                 },
             )
             is not None
         )
 
         result = manifest.run(prompt, return_response=True)
@@ -279,41 +264,42 @@
         assert cast(Response, result).is_cached()
 
         assert (
             manifest.cache.get(
                 {
                     "prompt": "New prompt",
                     "engine": "dummy",
+                    "request_cls": "LMRequest",
                     "num_results": n,
                 },
             )
             is None
         )
         prompt = ["This is a prompt", "New prompt"]
         result = manifest.run(prompt, return_response=return_response)
         if return_response:
             assert isinstance(result, Response)
             result = cast(Response, result)
-            assert len(result.get_json_response()["usage"]) == len(
-                result.get_json_response()["choices"]
+            assert len(result.get_usage_obj().usages) == len(
+                result.get_response_obj().choices
             )
             res = result.get_response(manifest.stop_token, is_batch=True)
             # Cached because one item is in cache
             assert result.is_cached()
         else:
             res = cast(str, result)
         assert res == ["hello", "hello"]
 
         prompt = ["Hello is a prompt", "Hello is a prompt"]
         result = manifest.run(prompt, stop_token="ll", return_response=return_response)
         if return_response:
             assert isinstance(result, Response)
             result = cast(Response, result)
-            assert len(result.get_json_response()["usage"]) == len(
-                result.get_json_response()["choices"]
+            assert len(result.get_usage_obj().usages) == len(
+                result.get_response_obj().choices
             )
             res = result.get_response(stop_token="ll", is_batch=True)
         else:
             res = cast(str, result)
         assert res == ["he", "he"]
 
 
@@ -326,92 +312,85 @@
         cache_connection=sqlite_cache,
     )
     prompt = ["This is a prompt"]
     result = cast(
         Response, asyncio.run(manifest.arun_batch(prompt, return_response=True))
     )
 
-    assert len(result.get_json_response()["usage"]) == len(
-        result.get_json_response()["choices"]
-    )
+    assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response(manifest.stop_token, is_batch=True)
     assert res == ["hello"]
     assert (
         manifest.cache.get(
             {
                 "prompt": "This is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": 1,
             },
         )
         is not None
     )
 
     prompt = ["Hello is a prompt", "Hello is a prompt"]
     result = cast(
         Response, asyncio.run(manifest.arun_batch(prompt, return_response=True))
     )
 
-    assert len(result.get_json_response()["usage"]) == len(
-        result.get_json_response()["choices"]
-    )
+    assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response(manifest.stop_token, is_batch=True)
     assert res == ["hello", "hello"]
     assert (
         manifest.cache.get(
             {
                 "prompt": "Hello is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": 1,
             },
         )
         is not None
     )
 
     result = cast(
         Response, asyncio.run(manifest.arun_batch(prompt, return_response=True))
     )
 
-    assert len(result.get_json_response()["usage"]) == len(
-        result.get_json_response()["choices"]
-    )
+    assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response(manifest.stop_token, is_batch=True)
     assert result.is_cached()
 
     assert (
         manifest.cache.get(
             {
                 "prompt": "New prompt",
                 "engine": "dummy",
+                "request_cls": "LMRequest",
                 "num_results": 1,
             },
         )
         is None
     )
     prompt = ["This is a prompt", "New prompt"]
     result = cast(
         Response, asyncio.run(manifest.arun_batch(prompt, return_response=True))
     )
 
-    assert len(result.get_json_response()["usage"]) == len(
-        result.get_json_response()["choices"]
-    )
+    assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response(manifest.stop_token, is_batch=True)
     # Cached because one item is in cache
     assert result.is_cached()
     assert res == ["hello", "hello"]
 
     prompt = ["Hello is a prompt", "Hello is a prompt"]
     result = cast(
         Response, asyncio.run(manifest.arun_batch(prompt, return_response=True))
     )
 
-    assert len(result.get_json_response()["usage"]) == len(
-        result.get_json_response()["choices"]
-    )
+    assert len(result.get_usage_obj().usages) == len(result.get_response_obj().choices)
     res = result.get_response(stop_token="ll", is_batch=True)
     assert res == ["he", "he"]
 
 
 @pytest.mark.usefixtures("sqlite_cache")
 def test_score_run(sqlite_cache: str) -> None:
     """Test manifest run."""
@@ -424,77 +403,113 @@
     prompt = "This is a prompt"
     result = manifest.score_prompt(prompt)
     assert (
         manifest.cache.get(
             {
                 "prompt": "This is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMScoreRequest",
                 "num_results": 1,
-                "request_type": "score_prompt",
             },
         )
         is not None
     )
     assert result == {
-        "generation_key": "choices",
-        "logits_key": "token_logprobs",
-        "item_key": "text",
-        "item_dtype": None,
-        "response": {"choices": [{"text": "This is a prompt", "logprob": 0.3}]},
+        "response": {
+            "choices": [
+                {"text": "This is a prompt", "token_logprobs": [0.3], "tokens": None}
+            ]
+        },
+        "usages": {"usages": []},
         "cached": False,
-        "request_params": {
+        "request": {
             "prompt": "This is a prompt",
-            "engine": "dummy",
-            "num_results": 1,
-            "request_type": "score_prompt",
+            "engine": "text-ada-001",
+            "n": 1,
+            "client_timeout": 60,
+            "run_id": None,
+            "batch_size": 8,
+            "temperature": 0.7,
+            "max_tokens": 100,
+            "top_p": 1.0,
+            "top_k": 50,
+            "logprobs": None,
+            "stop_sequences": None,
+            "num_beams": 1,
+            "do_sample": False,
+            "repetition_penalty": 1.0,
+            "length_penalty": 1.0,
+            "presence_penalty": 0.0,
+            "frequency_penalty": 0.0,
         },
+        "response_type": "text",
+        "request_type": "LMScoreRequest",
+        "item_dtype": None,
     }
 
     prompt_list = ["Hello is a prompt", "Hello is another prompt"]
     result = manifest.score_prompt(prompt_list)
     assert (
         manifest.cache.get(
             {
                 "prompt": "Hello is a prompt",
                 "engine": "dummy",
+                "request_cls": "LMScoreRequest",
                 "num_results": 1,
-                "request_type": "score_prompt",
             },
         )
         is not None
     )
     assert (
         manifest.cache.get(
             {
                 "prompt": "Hello is another prompt",
                 "engine": "dummy",
+                "request_cls": "LMScoreRequest",
                 "num_results": 1,
-                "request_type": "score_prompt",
             },
         )
         is not None
     )
     assert result == {
-        "generation_key": "choices",
-        "logits_key": "token_logprobs",
-        "item_key": "text",
-        "item_dtype": None,
         "response": {
             "choices": [
-                {"text": "Hello is a prompt", "logprob": 0.3},
-                {"text": "Hello is another prompt", "logprob": 0.3},
+                {"text": "Hello is a prompt", "token_logprobs": [0.3], "tokens": None},
+                {
+                    "text": "Hello is another prompt",
+                    "token_logprobs": [0.3],
+                    "tokens": None,
+                },
             ]
         },
+        "usages": {"usages": []},
         "cached": False,
-        "request_params": {
+        "request": {
             "prompt": ["Hello is a prompt", "Hello is another prompt"],
-            "engine": "dummy",
-            "num_results": 1,
-            "request_type": "score_prompt",
+            "engine": "text-ada-001",
+            "n": 1,
+            "client_timeout": 60,
+            "run_id": None,
+            "batch_size": 8,
+            "temperature": 0.7,
+            "max_tokens": 100,
+            "top_p": 1.0,
+            "top_k": 50,
+            "logprobs": None,
+            "stop_sequences": None,
+            "num_beams": 1,
+            "do_sample": False,
+            "repetition_penalty": 1.0,
+            "length_penalty": 1.0,
+            "presence_penalty": 0.0,
+            "frequency_penalty": 0.0,
         },
+        "response_type": "text",
+        "request_type": "LMScoreRequest",
+        "item_dtype": None,
     }
 
 
 @pytest.mark.skipif(not MODEL_ALIVE, reason=f"No model at {URL}")
 @pytest.mark.usefixtures("sqlite_cache")
 def test_local_huggingface(sqlite_cache: str) -> None:
     """Test local huggingface client."""
@@ -661,16 +676,16 @@
     res = client.run("Why are there apples?")
     assert isinstance(res, str) and len(res) > 0
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert isinstance(response.get_response(), str) and len(response.get_response()) > 0
     assert response.get_response() == res
     assert response.is_cached() is True
-    assert "usage" in response.get_json_response()
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 15
+    assert response.get_usage_obj().usages
+    assert response.get_usage_obj().usages[0].total_tokens == 15
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert response.is_cached() is True
 
     res_list = client.run(["Why are there apples?", "Why are there bananas?"])
     assert isinstance(res_list, list) and len(res_list) == 2
 
@@ -679,20 +694,17 @@
         client.run(
             ["Why are there apples?", "Why are there mangos?"], return_response=True
         ),
     )
     assert (
         isinstance(response.get_response(), list) and len(response.get_response()) == 2
     )
-    assert (
-        "usage" in response.get_json_response()
-        and len(response.get_json_response()["usage"]) == 2
-    )
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 15
-    assert response.get_json_response()["usage"][1]["total_tokens"] == 16
+    assert response.get_usage_obj().usages and len(response.get_usage_obj().usages) == 2
+    assert response.get_usage_obj().usages[0].total_tokens == 15
+    assert response.get_usage_obj().usages[1].total_tokens == 16
 
     response = cast(
         Response, client.run("Why are there bananas?", return_response=True)
     )
     assert response.is_cached() is True
 
     res_list = asyncio.run(
@@ -708,20 +720,17 @@
                 return_response=True,
             )
         ),
     )
     assert (
         isinstance(response.get_response(), list) and len(response.get_response()) == 2
     )
-    assert (
-        "usage" in response.get_json_response()
-        and len(response.get_json_response()["usage"]) == 2
-    )
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 17
-    assert response.get_json_response()["usage"][1]["total_tokens"] == 15
+    assert response.get_usage_obj().usages and len(response.get_usage_obj().usages) == 2
+    assert response.get_usage_obj().usages[0].total_tokens == 17
+    assert response.get_usage_obj().usages[1].total_tokens == 15
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
     assert response.is_cached() is True
 
 
@@ -738,16 +747,16 @@
     res = client.run("Why are there apples?")
     assert isinstance(res, str) and len(res) > 0
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert isinstance(response.get_response(), str) and len(response.get_response()) > 0
     assert response.get_response() == res
     assert response.is_cached() is True
-    assert "usage" in response.get_json_response()
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 23
+    assert response.get_usage_obj().usages
+    assert response.get_usage_obj().usages[0].total_tokens == 23
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert response.is_cached() is True
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
@@ -766,20 +775,17 @@
                 return_response=True,
             )
         ),
     )
     assert (
         isinstance(response.get_response(), list) and len(response.get_response()) == 2
     )
-    assert (
-        "usage" in response.get_json_response()
-        and len(response.get_json_response()["usage"]) == 2
-    )
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 25
-    assert response.get_json_response()["usage"][1]["total_tokens"] == 23
+    assert response.get_usage_obj().usages and len(response.get_usage_obj().usages) == 2
+    assert response.get_usage_obj().usages[0].total_tokens == 25
+    assert response.get_usage_obj().usages[1].total_tokens == 23
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
     assert response.is_cached() is True
 
 
@@ -812,16 +818,16 @@
     res = client.run("Why are there apples?")
     assert isinstance(res, np.ndarray)
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert isinstance(response.get_response(), np.ndarray)
     assert np.allclose(response.get_response(), res)
     assert response.is_cached() is True
-    assert "usage" in response.get_json_response()
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 5
+    assert response.get_usage_obj().usages
+    assert response.get_usage_obj().usages[0].total_tokens == 5
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert response.is_cached() is True
 
     res_list = client.run(["Why are there apples?", "Why are there bananas?"])
     assert (
         isinstance(res_list, list)
@@ -834,20 +840,17 @@
         client.run(
             ["Why are there apples?", "Why are there mangos?"], return_response=True
         ),
     )
     assert (
         isinstance(response.get_response(), list) and len(response.get_response()) == 2
     )
-    assert (
-        "usage" in response.get_json_response()
-        and len(response.get_json_response()["usage"]) == 2
-    )
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 5
-    assert response.get_json_response()["usage"][1]["total_tokens"] == 6
+    assert response.get_usage_obj().usages and len(response.get_usage_obj().usages) == 2
+    assert response.get_usage_obj().usages[0].total_tokens == 5
+    assert response.get_usage_obj().usages[1].total_tokens == 6
 
     response = cast(
         Response, client.run("Why are there bananas?", return_response=True)
     )
     assert response.is_cached() is True
 
     response = cast(
@@ -874,27 +877,151 @@
         ),
     )
     assert (
         isinstance(response.get_response(), list)
         and len(res_list) == 2
         and isinstance(res_list[0], np.ndarray)
     )
-    assert (
-        "usage" in response.get_json_response()
-        and len(response.get_json_response()["usage"]) == 2
-    )
-    assert response.get_json_response()["usage"][0]["total_tokens"] == 7
-    assert response.get_json_response()["usage"][1]["total_tokens"] == 5
+    assert response.get_usage_obj().usages and len(response.get_usage_obj().usages) == 2
+    assert response.get_usage_obj().usages[0].total_tokens == 7
+    assert response.get_usage_obj().usages[1].total_tokens == 5
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
     assert response.is_cached() is True
 
 
+@pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
+@pytest.mark.usefixtures("sqlite_cache")
+def test_openai_pool(sqlite_cache: str) -> None:
+    """Test openai and openaichat client."""
+    client_connection1 = ClientConnection(
+        client_name="openaichat",
+    )
+    client_connection2 = ClientConnection(client_name="openai", engine="text-ada-001")
+    client = Manifest(
+        client_pool=[client_connection1, client_connection2],
+        cache_name="sqlite",
+        client_connection=sqlite_cache,
+    )
+    res = client.run("Why are there apples?")
+    assert isinstance(res, str) and len(res) > 0
+
+    res2 = client.run("Why are there apples?")
+    assert isinstance(res2, str) and len(res2) > 0
+    # Different models
+    assert res != res2
+
+    assert cast(
+        Response, client.run("Why are there apples?", return_response=True)
+    ).is_cached()
+
+    res_list = asyncio.run(
+        client.arun_batch(["Why are there pears?", "Why are there oranges?"])
+    )
+    assert isinstance(res_list, list) and len(res_list) == 2
+    res_list2 = asyncio.run(
+        client.arun_batch(["Why are there pears?", "Why are there oranges?"])
+    )
+    assert isinstance(res_list2, list) and len(res_list2) == 2
+    # Different models
+    assert res_list != res_list2
+
+    assert cast(
+        Response,
+        asyncio.run(
+            client.arun_batch(
+                ["Why are there pears?", "Why are there oranges?"], return_response=True
+            )
+        ),
+    ).is_cached()
+
+    # Test chunk size of 1
+    res_list = asyncio.run(
+        client.arun_batch(
+            ["Why are there pineapples?", "Why are there pinecones?"], chunk_size=1
+        )
+    )
+    assert isinstance(res_list, list) and len(res_list) == 2
+    res_list2 = asyncio.run(
+        client.arun_batch(
+            ["Why are there pineapples?", "Why are there pinecones?"], chunk_size=1
+        )
+    )
+    # Because we split across both models exactly in first run,
+    # we will get the same result
+    assert res_list == res_list2
+
+
+@pytest.mark.skipif(
+    not OPENAI_ALIVE or not MODEL_ALIVE, reason="No openai or local model set"
+)
+@pytest.mark.usefixtures("sqlite_cache")
+def test_mixed_pool(sqlite_cache: str) -> None:
+    """Test openai and openaichat client."""
+    client_connection1 = ClientConnection(
+        client_name="huggingface",
+        client_connection=URL,
+    )
+    client_connection2 = ClientConnection(client_name="openai", engine="text-ada-001")
+    client = Manifest(
+        client_pool=[client_connection1, client_connection2],
+        cache_name="sqlite",
+        client_connection=sqlite_cache,
+    )
+
+    res = client.run("Why are there apples?")
+    assert isinstance(res, str) and len(res) > 0
+
+    res2 = client.run("Why are there apples?")
+    assert isinstance(res2, str) and len(res2) > 0
+    # Different models
+    assert res != res2
+    assert cast(
+        Response, client.run("Why are there apples?", return_response=True)
+    ).is_cached()
+
+    res_list = asyncio.run(
+        client.arun_batch(["Why are there pears?", "Why are there oranges?"])
+    )
+    assert isinstance(res_list, list) and len(res_list) == 2
+    res_list2 = asyncio.run(
+        client.arun_batch(["Why are there pears?", "Why are there oranges?"])
+    )
+    assert isinstance(res_list2, list) and len(res_list2) == 2
+    # Different models
+    assert res_list != res_list2
+
+    assert cast(
+        Response,
+        asyncio.run(
+            client.arun_batch(
+                ["Why are there pears?", "Why are there oranges?"], return_response=True
+            )
+        ),
+    ).is_cached()
+
+    # Test chunk size of 1
+    res_list = asyncio.run(
+        client.arun_batch(
+            ["Why are there pineapples?", "Why are there pinecones?"], chunk_size=1
+        )
+    )
+    assert isinstance(res_list, list) and len(res_list) == 2
+    res_list2 = asyncio.run(
+        client.arun_batch(
+            ["Why are there pineapples?", "Why are there pinecones?"], chunk_size=1
+        )
+    )
+    # Because we split across both models exactly in first run,
+    # we will get the same result
+    assert res_list == res_list2
+
+
 def test_retry_handling() -> None:
     """Test retry handling."""
     # We'll mock the response so we won't need a real connection
     client = Manifest(client_name="openai", client_connection="fake")
     mock_create = MagicMock(
         side_effect=[
             # raise a 429 error
```

### Comparing `manifest-ml-0.1.3/tests/test_request.py` & `manifest-ml-0.1.4/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.3/web_app/main.py` & `manifest-ml-0.1.4/web_app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,12 @@
         )
         response = cast(ManifestResponse, response)
     except Exception as e:
         raise HTTPException(status_code=500, detail=str(e))
     return {
         "response": response.get_response(),
         "cached": response.is_cached(),
-        "request_params": response.get_request(),
+        "request_params": response.get_request_obj(),
     }
 
 
 app.include_router(api_router)
```

### Comparing `manifest-ml-0.1.3/web_app/schemas.py` & `manifest-ml-0.1.4/web_app/schemas.py`

 * *Files identical despite different names*

