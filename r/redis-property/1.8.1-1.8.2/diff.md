# Comparing `tmp/redis-property-1.8.1.tar.gz` & `tmp/redis-property-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/redis-property-1.8.1.tar", last modified: Fri Feb  3 02:17:29 2023, max compression
+gzip compressed data, was "dist/redis-property-1.8.2.tar", last modified: Tue Apr 25 12:53:28 2023, max compression
```

## Comparing `redis-property-1.8.1.tar` & `redis-property-1.8.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 02:17:29.000000 redis-property-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-02-03 02:17:29.000000 redis-property-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-03 02:17:15.000000 redis-property-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 02:17:29.000000 redis-property-1.8.1/redis_property.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-02-03 02:17:29.000000 redis-property-1.8.1/redis_property.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-03 02:17:29.000000 redis-property-1.8.1/redis_property.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 02:17:29.000000 redis-property-1.8.1/redis_property.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-03 02:17:29.000000 redis-property-1.8.1/redis_property.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-03 02:17:29.000000 redis-property-1.8.1/redis_property.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-02-03 02:17:15.000000 redis-property-1.8.1/redis_property.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 02:17:29.000000 redis-property-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-03 02:17:15.000000 redis-property-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:53:28.000000 redis-property-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-25 12:53:28.000000 redis-property-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-25 12:53:18.000000 redis-property-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:53:28.000000 redis-property-1.8.2/redis_property.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-25 12:53:28.000000 redis-property-1.8.2/redis_property.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 12:53:28.000000 redis-property-1.8.2/redis_property.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:53:28.000000 redis-property-1.8.2/redis_property.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 12:53:28.000000 redis-property-1.8.2/redis_property.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 12:53:28.000000 redis-property-1.8.2/redis_property.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-25 12:53:18.000000 redis-property-1.8.2/redis_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 12:53:28.000000 redis-property-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-25 12:53:18.000000 redis-property-1.8.2/setup.py
```

### Comparing `redis-property-1.8.1/PKG-INFO` & `redis-property-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-property
-Version: 1.8.1
+Version: 1.8.2
 Summary: A decorator for caching properties in Redis.
 Home-page: https://github.com/Ed-XCF/redis-property
 Author: Ed__xu__Ed
 Author-email: m.tofu@qq.com
 License: UNKNOWN
 Description: # redis-property
         ![GitHub](https://img.shields.io/github/license/Ed-XCF/redis-property)
```

### Comparing `redis-property-1.8.1/README.md` & `redis-property-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `redis-property-1.8.1/redis_property.egg-info/PKG-INFO` & `redis-property-1.8.2/redis_property.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-property
-Version: 1.8.1
+Version: 1.8.2
 Summary: A decorator for caching properties in Redis.
 Home-page: https://github.com/Ed-XCF/redis-property
 Author: Ed__xu__Ed
 Author-email: m.tofu@qq.com
 License: UNKNOWN
 Description: # redis-property
         ![GitHub](https://img.shields.io/github/license/Ed-XCF/redis-property)
```

### Comparing `redis-property-1.8.1/redis_property.py` & `redis-property-1.8.2/redis_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,14 @@
 
     return wrapper
 
 
 def use_cache(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        token = cache_disable.set(False)
+        cache_disable.set(False)
         try:
             return func(*args, **kwargs)
         finally:
-            cache_disable.reset(token)
+            cache_disable.set(_default_cache_disable)
 
     return wrapper
```

### Comparing `redis-property-1.8.1/setup.py` & `redis-property-1.8.2/setup.py`

 * *Files identical despite different names*

