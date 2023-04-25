# Comparing `tmp/spring-config-client-0.2.tar.gz` & `tmp/spring-config-client-1.0.0.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spring-config-client-0.2.tar", last modified: Sun Sep 29 15:30:59 2019, max compression
+gzip compressed data, was "spring-config-client-1.0.0.linux-x86_64.tar", last modified: Tue Apr 25 11:55:36 2023, max compression
```

## Comparing `spring-config-client-0.2.tar` & `spring-config-client-1.0.0.linux-x86_64.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 jgodara   (1000) users      (985)        0 2019-09-29 15:30:59.000000 spring-config-client-0.2/
--rw-r--r--   0 jgodara   (1000) users      (985)     4026 2019-09-29 15:30:59.000000 spring-config-client-0.2/PKG-INFO
--rw-r--r--   0 jgodara   (1000) users      (985)     2454 2019-09-29 15:26:43.000000 spring-config-client-0.2/README.md
--rw-r--r--   0 jgodara   (1000) users      (985)       38 2019-09-29 15:30:59.000000 spring-config-client-0.2/setup.cfg
--rw-r--r--   0 jgodara   (1000) users      (985)     1321 2019-09-29 14:37:14.000000 spring-config-client-0.2/setup.py
-drwxr-xr-x   0 jgodara   (1000) users      (985)        0 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config/
--rw-r--r--   0 jgodara   (1000) users      (985)     2276 2019-09-29 14:59:17.000000 spring-config-client-0.2/spring_config/__init__.py
--rw-r--r--   0 jgodara   (1000) users      (985)     2121 2019-09-29 14:39:55.000000 spring-config-client-0.2/spring_config/client.py
--rw-r--r--   0 jgodara   (1000) users      (985)       89 2019-09-29 14:01:48.000000 spring-config-client-0.2/spring_config/utils.py
-drwxr-xr-x   0 jgodara   (1000) users      (985)        0 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config_client.egg-info/
--rw-r--r--   0 jgodara   (1000) users      (985)     4026 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config_client.egg-info/PKG-INFO
--rw-r--r--   0 jgodara   (1000) users      (985)      310 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config_client.egg-info/SOURCES.txt
--rw-r--r--   0 jgodara   (1000) users      (985)        1 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config_client.egg-info/dependency_links.txt
--rw-r--r--   0 jgodara   (1000) users      (985)       17 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config_client.egg-info/requires.txt
--rw-r--r--   0 jgodara   (1000) users      (985)       14 2019-09-29 15:30:59.000000 spring-config-client-0.2/spring_config_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.420450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-25 11:55:27.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.420450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-25 11:55:36.420450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-25 11:55:36.416450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-25 11:55:27.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 11:55:27.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:55:36.420450 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-25 11:55:36.360449 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-25 11:55:36.368449 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:55:36.360449 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 11:55:36.360449 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 11:55:36.360449 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spring-config-client-0.2/README.md` & `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config_client-1.0.0-py3.11.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: spring-config-client
+Version: 1.0.0
+Summary: A client for Spring Config Server
+Home-page: https://realbucksavage.github.io/spring-config-client
+Author: realbucksavage
+License: MIT
+Project-URL: Documentation, https://github.com/realbucksavage/spring-config-client
+Project-URL: Code, https://github.com/realbucksavage/spring-config-client
+Project-URL: Issue tracker, https://github.com/realbucksavage/spring-config-client/issues
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Java Libraries
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # spring-config-client
 
 A Python client for [Spring Config Server](https://spring.io/projects/spring-cloud-config).
 
 This library is inspired by [amenezes/config-client](https://github.com/amenezes/config-client) and is essentially a toned-down fork that I customized to fit my own needs.
 
 ## Project goals
@@ -77,8 +98,8 @@
 - Application Name : `app_name("some-app")` - Default `None`, required.
 - Server Address : `address("http://some-server")` - Default `http://localhost:8888`, optional.
 - Profile : `profile("production")` - Default `development`, optional.
 - Branch : `branch("devel/0.1")` - Default `master`, optional.
 
 ## Requesting features
 
-Please use the [issues section](https://github.com/realbucksavage/spring-config-client/issues) to request new features and I will try to take out my time to work on them. Contributions in any sorts are always welcome :)
+Please use the [issues section](https://github.com/realbucksavage/spring-config-client/issues) to request new features and I will try to take out my time to work on them. Contributions in any sorts are always welcome :)
```

### Comparing `spring-config-client-0.2/spring_config/__init__.py` & `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/spring_config/__init__.py`

 * *Files identical despite different names*

