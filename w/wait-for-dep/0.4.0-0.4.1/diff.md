# Comparing `tmp/wait-for-dep-0.4.0.tar.gz` & `tmp/wait-for-dep-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wait-for-dep-0.4.0.tar", last modified: Wed Jun 29 19:06:46 2022, max compression
+gzip compressed data, was "wait-for-dep-0.4.1.tar", last modified: Mon Apr 24 19:33:18 2023, max compression
```

## Comparing `wait-for-dep-0.4.0.tar` & `wait-for-dep-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:46.927619 wait-for-dep-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-06-29 19:06:46.927619 wait-for-dep-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:46.923619 wait-for-dep-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/base.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:46.923619 wait-for-dep-0.4.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/kafka.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/memcached.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/redis.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/extras/websockets.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-29 19:06:46.927619 wait-for-dep-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:46.923619 wait-for-dep-0.4.0/wait_for_dep/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-29 19:06:37.000000 wait-for-dep-0.4.0/wait_for_dep/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:46.927619 wait-for-dep-0.4.0/wait_for_dep/checks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/amqp.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/http.py
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/https.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/kafka.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/memcached.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/postgres.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/psql.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/tcp.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/checks/unix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-06-29 19:06:34.000000 wait-for-dep-0.4.0/wait_for_dep/wait_for_dep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 19:06:46.927619 wait-for-dep-0.4.0/wait_for_dep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-06-29 19:06:46.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-06-29 19:06:46.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 19:06:46.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-29 19:06:46.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 19:06:44.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-06-29 19:06:46.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-29 19:06:46.000000 wait-for-dep-0.4.0/wait_for_dep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:18.426016 wait-for-dep-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 19:33:18.426016 wait-for-dep-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:18.422016 wait-for-dep-0.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/base.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:18.422016 wait-for-dep-0.4.1/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/kafka.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/extras/websockets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:33:18.426016 wait-for-dep-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:18.422016 wait-for-dep-0.4.1/wait_for_dep/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 19:33:11.000000 wait-for-dep-0.4.1/wait_for_dep/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:18.426016 wait-for-dep-0.4.1/wait_for_dep/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/psql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/checks/unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-24 19:33:09.000000 wait-for-dep-0.4.1/wait_for_dep/wait_for_dep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:33:18.426016 wait-for-dep-0.4.1/wait_for_dep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 19:33:18.000000 wait-for-dep-0.4.1/wait_for_dep.egg-info/top_level.txt
```

### Comparing `wait-for-dep-0.4.0/LICENSE` & `wait-for-dep-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wait-for-dep-0.4.0/PKG-INFO` & `wait-for-dep-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wait-for-dep
-Version: 0.4.0
+Version: 0.4.1
 Summary: Waits for dependencies before running the app
 Home-page: http://github.com/wlatanowicz/wait-for-dep
 Author: Wiktor Latanowicz
 Author-email: wait-for-dep@wiktor.latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wait-for-dep-0.4.0/README.md` & `wait-for-dep-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wait-for-dep-0.4.0/setup.py` & `wait-for-dep-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 setup(
     name="wait-for-dep",
     entry_points={
         "console_scripts": [
             "wait-for-dep = wait_for_dep.wait_for_dep:main",
         ],
     },
-    version="0.4.0",
+    version="0.4.1",
     description="Waits for dependencies before running the app",
     url="http://github.com/wlatanowicz/wait-for-dep",
     author="Wiktor Latanowicz",
     author_email="wait-for-dep@wiktor.latanowicz.com",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `wait-for-dep-0.4.0/wait_for_dep/checks/amqp.py` & `wait-for-dep-0.4.1/wait_for_dep/checks/amqp.py`

 * *Files identical despite different names*

### Comparing `wait-for-dep-0.4.0/wait_for_dep/checks/mysql.py` & `wait-for-dep-0.4.1/wait_for_dep/checks/mysql.py`

 * *Files identical despite different names*

### Comparing `wait-for-dep-0.4.0/wait_for_dep/wait_for_dep.py` & `wait-for-dep-0.4.1/wait_for_dep/wait_for_dep.py`

 * *Files identical despite different names*

### Comparing `wait-for-dep-0.4.0/wait_for_dep.egg-info/PKG-INFO` & `wait-for-dep-0.4.1/wait_for_dep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wait-for-dep
-Version: 0.4.0
+Version: 0.4.1
 Summary: Waits for dependencies before running the app
 Home-page: http://github.com/wlatanowicz/wait-for-dep
 Author: Wiktor Latanowicz
 Author-email: wait-for-dep@wiktor.latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wait-for-dep-0.4.0/wait_for_dep.egg-info/SOURCES.txt` & `wait-for-dep-0.4.1/wait_for_dep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

