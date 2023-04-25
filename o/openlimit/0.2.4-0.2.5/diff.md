# Comparing `tmp/openlimit-0.2.4.tar.gz` & `tmp/openlimit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.2.4.tar", last modified: Sun Apr 23 14:05:53 2023, max compression
+gzip compressed data, was "openlimit-0.2.5.tar", last modified: Tue Apr 25 12:10:09 2023, max compression
```

## Comparing `openlimit-0.2.4.tar` & `openlimit-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.342349 openlimit-0.2.4/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 14:05:53.342236 openlimit-0.2.4/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.4/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.340301 openlimit-0.2.4/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.4/openlimit/__init__.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.341293 openlimit-0.2.4/openlimit/buckets/
--rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.4/openlimit/buckets/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.4/openlimit/buckets/bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.4/openlimit/buckets/redis_bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1750 2023-04-23 14:04:33.000000 openlimit-0.2.4/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2823 2023-04-23 14:05:00.000000 openlimit-0.2.4/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.341884 openlimit-0.2.4/openlimit/utilities/
--rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.4/openlimit/utilities/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.4/openlimit/utilities/context_decorators.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1681 2023-04-20 01:13:53.000000 openlimit-0.2.4/openlimit/utilities/token_counters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-23 14:05:53.340799 openlimit-0.2.4/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-23 14:05:53.000000 openlimit-0.2.4/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-23 14:05:53.342409 openlimit-0.2.4/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-04-23 14:05:17.000000 openlimit-0.2.4/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.808933 openlimit-0.2.5/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-25 12:10:09.808765 openlimit-0.2.5/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.5/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.806305 openlimit-0.2.5/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.5/openlimit/__init__.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.807598 openlimit-0.2.5/openlimit/buckets/
+-rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.5/openlimit/buckets/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.5/openlimit/buckets/bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.5/openlimit/buckets/redis_bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1792 2023-04-25 12:08:59.000000 openlimit-0.2.5/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     2928 2023-04-25 12:09:39.000000 openlimit-0.2.5/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.808400 openlimit-0.2.5/openlimit/utilities/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.5/openlimit/utilities/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.5/openlimit/utilities/context_decorators.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1681 2023-04-20 01:13:53.000000 openlimit-0.2.5/openlimit/utilities/token_counters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-04-25 12:10:09.807016 openlimit-0.2.5/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-04-25 12:10:09.000000 openlimit-0.2.5/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-04-25 12:10:09.809013 openlimit-0.2.5/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-04-25 12:10:05.000000 openlimit-0.2.5/setup.py
```

### Comparing `openlimit-0.2.4/README.md` & `openlimit-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.4/openlimit/buckets/bucket.py` & `openlimit-0.2.5/openlimit/buckets/bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.4/openlimit/buckets/redis_bucket.py` & `openlimit-0.2.5/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.4/openlimit/rate_limiters.py` & `openlimit-0.2.5/openlimit/rate_limiters.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 
 
 class ChatRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
             request_limit=3500,
             token_limit=90000,
-            utils.num_tokens_consumed_by_chat_request
+            token_counter=utils.num_tokens_consumed_by_chat_request
         )
 
 
 class CompletionRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
             request_limit=3500,
             token_limit=350000,
-            utils.num_tokens_consumed_by_completion_request
+            token_counter=utils.num_tokens_consumed_by_completion_request
         )
 
 
 class EmbeddingRateLimiter(RateLimiter):
     def __init__(self, request_limit, token_limit):
         super().__init__(
             request_limit=3500, 
             token_limit=70000000, 
-            utils.num_tokens_consumed_by_embedding_request
+            token_counter=utils.num_tokens_consumed_by_embedding_request
         )
```

### Comparing `openlimit-0.2.4/openlimit/redis_rate_limiters.py` & `openlimit-0.2.5/openlimit/redis_rate_limiters.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,33 +71,33 @@
 
 
 class ChatRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
             request_limit=3500, 
             token_limit=90000, 
-            utils.num_tokens_consumed_by_chat_request,
-            "chat", 
-            redis_url
+            token_counter=utils.num_tokens_consumed_by_chat_request,
+            bucket_key="chat", 
+            redis_url=redis_url
         )
 
 
 class CompletionRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
             request_limit=3500, 
             token_limit=350000, 
-            utils.num_tokens_consumed_by_completion_request,
-            "completion", 
-            redis_url
+            token_counter=utils.num_tokens_consumed_by_completion_request,
+            bucket_key="completion", 
+            redis_url=redis_url
         )
 
 
 class EmbeddingRateLimiterWithRedis(RateLimiterWithRedis):
     def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
         super().__init__(
             request_limit=3500, 
             token_limit=70000000, 
-            utils.num_tokens_consumed_by_embedding_request,
-            "embedding", 
-            redis_url
+            token_counter=utils.num_tokens_consumed_by_embedding_request,
+            bucket_key="embedding", 
+            redis_url=redis_url
         )
```

### Comparing `openlimit-0.2.4/openlimit/utilities/context_decorators.py` & `openlimit-0.2.5/openlimit/utilities/context_decorators.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.4/openlimit/utilities/token_counters.py` & `openlimit-0.2.5/openlimit/utilities/token_counters.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.4/setup.py` & `openlimit-0.2.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.2.4",
+    version="v0.2.5",
     packages=["openlimit", "openlimit.utilities", "openlimit.buckets"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

