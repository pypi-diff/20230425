# Comparing `tmp/dead_simple_framework-1.3.3.tar.gz` & `tmp/dead_simple_framework-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dead_simple_framework-1.3.3.tar", last modified: Sun Apr 23 02:51:27 2023, max compression
+gzip compressed data, was "dead_simple_framework-1.3.4.tar", last modified: Tue Apr 25 09:40:15 2023, max compression
```

## Comparing `dead_simple_framework-1.3.3.tar` & `dead_simple_framework-1.3.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.164383 dead_simple_framework-1.3.3/
--rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-23 02:51:27.163915 dead_simple_framework-1.3.3/PKG-INFO
--rw-r--r--   0 pswanson   (502) staff       (20)     4847 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/README.md
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.123235 dead_simple_framework-1.3.3/dead_simple_framework/
--rw-r--r--   0 pswanson   (502) staff       (20)      433 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/__init__.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.129879 dead_simple_framework-1.3.3/dead_simple_framework/api/
--rw-r--r--   0 pswanson   (502) staff       (20)      139 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4144 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/client.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1146 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/errors.py
--rw-r--r--   0 pswanson   (502) staff       (20)    15354 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)    10066 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/api/utils.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.131079 dead_simple_framework-1.3.3/dead_simple_framework/cache/
--rw-r--r--   0 pswanson   (502) staff       (20)       23 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/cache/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3670 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/cache/main.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.133445 dead_simple_framework-1.3.3/dead_simple_framework/config/
--rw-r--r--   0 pswanson   (502) staff       (20)      422 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1949 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/config.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1743 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/route.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3611 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/schema.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.140115 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/
--rw-r--r--   0 pswanson   (502) staff       (20)      305 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1865 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/app_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1831 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/jwt_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2385 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     6280 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/mongodb_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4085 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/rabbitmq_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3048 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/redis_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1587 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/sentry_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)      558 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/setting.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1400 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/settings/slack_settings.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1947 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/config/task.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.152370 dead_simple_framework-1.3.3/dead_simple_framework/database/
--rw-r--r--   0 pswanson   (502) staff       (20)       91 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1756 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/fixtures.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3708 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/index.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4295 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)      568 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/database/utils.py
--rw-r--r--   0 pswanson   (502) staff       (20)      598 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/encoder.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.158166 dead_simple_framework-1.3.3/dead_simple_framework/handlers/
--rw-r--r--   0 pswanson   (502) staff       (20)      288 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1969 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/default.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4775 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/login.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3514 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/permissions.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4483 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/handlers/users.py
--rw-r--r--   0 pswanson   (502) staff       (20)       61 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/jwt.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4083 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     2685 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/router.py
--rw-r--r--   0 pswanson   (502) staff       (20)     4511 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/slack.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.159889 dead_simple_framework-1.3.3/dead_simple_framework/tasks/
--rw-r--r--   0 pswanson   (502) staff       (20)       30 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/__init__.py
--rw-r--r--   0 pswanson   (502) staff       (20)    12468 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/main.py
--rw-r--r--   0 pswanson   (502) staff       (20)     3454 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/task.py
--rw-r--r--   0 pswanson   (502) staff       (20)     1306 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework/tasks/utils.py
-drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-23 02:51:27.126947 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/
--rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/PKG-INFO
--rw-r--r--   0 pswanson   (502) staff       (20)     1984 2023-04-23 02:51:27.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/SOURCES.txt
--rw-r--r--   0 pswanson   (502) staff       (20)        1 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/dependency_links.txt
--rw-r--r--   0 pswanson   (502) staff       (20)      146 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/requires.txt
--rw-r--r--   0 pswanson   (502) staff       (20)       22 2023-04-23 02:51:26.000000 dead_simple_framework-1.3.3/dead_simple_framework.egg-info/top_level.txt
--rw-r--r--   0 pswanson   (502) staff       (20)       38 2023-04-23 02:51:27.164532 dead_simple_framework-1.3.3/setup.cfg
--rw-r--r--   0 pswanson   (502) staff       (20)      824 2023-04-23 02:49:25.000000 dead_simple_framework-1.3.3/setup.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.329054 dead_simple_framework-1.3.4/
+-rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-25 09:40:15.328605 dead_simple_framework-1.3.4/PKG-INFO
+-rw-r--r--   0 pswanson   (502) staff       (20)     4847 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/README.md
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.295276 dead_simple_framework-1.3.4/dead_simple_framework/
+-rw-r--r--   0 pswanson   (502) staff       (20)      433 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/__init__.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.300883 dead_simple_framework-1.3.4/dead_simple_framework/api/
+-rw-r--r--   0 pswanson   (502) staff       (20)      139 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/api/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4144 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/api/client.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1146 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/api/errors.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    15354 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/api/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    10066 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/api/utils.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.302379 dead_simple_framework-1.3.4/dead_simple_framework/cache/
+-rw-r--r--   0 pswanson   (502) staff       (20)       23 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/cache/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3670 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/cache/main.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.310631 dead_simple_framework-1.3.4/dead_simple_framework/config/
+-rw-r--r--   0 pswanson   (502) staff       (20)      422 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1949 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/config.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1743 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/route.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3611 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/schema.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.318545 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/
+-rw-r--r--   0 pswanson   (502) staff       (20)      305 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2509 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/app_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1831 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/jwt_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2385 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     6280 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/mongodb_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4085 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/rabbitmq_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3048 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/redis_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1587 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/sentry_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      558 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/setting.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1400 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/settings/slack_settings.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1947 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/config/task.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.321544 dead_simple_framework-1.3.4/dead_simple_framework/database/
+-rw-r--r--   0 pswanson   (502) staff       (20)       91 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/database/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1756 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/database/fixtures.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3708 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/database/index.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4295 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/database/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      568 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/database/utils.py
+-rw-r--r--   0 pswanson   (502) staff       (20)      598 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/encoder.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.325862 dead_simple_framework-1.3.4/dead_simple_framework/handlers/
+-rw-r--r--   0 pswanson   (502) staff       (20)      288 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/handlers/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1969 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/handlers/default.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4775 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/handlers/login.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3514 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/handlers/permissions.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4483 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/handlers/users.py
+-rw-r--r--   0 pswanson   (502) staff       (20)       61 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/jwt.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4068 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     2685 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/router.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     4511 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/slack.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.327952 dead_simple_framework-1.3.4/dead_simple_framework/tasks/
+-rw-r--r--   0 pswanson   (502) staff       (20)       30 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/tasks/__init__.py
+-rw-r--r--   0 pswanson   (502) staff       (20)    12468 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/tasks/main.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     3454 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/tasks/task.py
+-rw-r--r--   0 pswanson   (502) staff       (20)     1306 2023-04-25 09:40:14.000000 dead_simple_framework-1.3.4/dead_simple_framework/tasks/utils.py
+drwxr-xr-x   0 pswanson   (502) staff       (20)        0 2023-04-25 09:40:15.298030 dead_simple_framework-1.3.4/dead_simple_framework.egg-info/
+-rw-r--r--   0 pswanson   (502) staff       (20)     5206 2023-04-25 09:40:15.000000 dead_simple_framework-1.3.4/dead_simple_framework.egg-info/PKG-INFO
+-rw-r--r--   0 pswanson   (502) staff       (20)     1984 2023-04-25 09:40:15.000000 dead_simple_framework-1.3.4/dead_simple_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)        1 2023-04-25 09:40:15.000000 dead_simple_framework-1.3.4/dead_simple_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)      146 2023-04-25 09:40:15.000000 dead_simple_framework-1.3.4/dead_simple_framework.egg-info/requires.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)       22 2023-04-25 09:40:15.000000 dead_simple_framework-1.3.4/dead_simple_framework.egg-info/top_level.txt
+-rw-r--r--   0 pswanson   (502) staff       (20)       38 2023-04-25 09:40:15.329221 dead_simple_framework-1.3.4/setup.cfg
+-rw-r--r--   0 pswanson   (502) staff       (20)      824 2023-04-25 09:37:52.000000 dead_simple_framework-1.3.4/setup.py
```

### Comparing `dead_simple_framework-1.3.3/PKG-INFO` & `dead_simple_framework-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead_simple_framework
-Version: 1.3.3
+Version: 1.3.4
 Summary: RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations
 Home-page: https://github.com/Topazoo/dead_simple_framework
 Author: Peter Swanson
 Author-email: pswanson@ucdavis.edu
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `dead_simple_framework-1.3.3/README.md` & `dead_simple_framework-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/api/client.py` & `dead_simple_framework-1.3.4/dead_simple_framework/api/client.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/api/errors.py` & `dead_simple_framework-1.3.4/dead_simple_framework/api/errors.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/api/main.py` & `dead_simple_framework-1.3.4/dead_simple_framework/api/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/api/utils.py` & `dead_simple_framework-1.3.4/dead_simple_framework/api/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/cache/main.py` & `dead_simple_framework-1.3.4/dead_simple_framework/cache/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/config.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/config.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/route.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/route.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/schema.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/schema.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/app_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/app_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 # Interface class
 from .setting import Setting
 
 # Utilities
 import os
 
+
+def get_list_from_env(key:str, default:str=None):
+    result = os.environ.get(key, default)
+    if result and ',' in result:
+        return result.split('')
+    elif result:
+        return [result]
+    
+    return result
+
+
 class App_Settings(Setting):
     ''' Used to specify and validate application settings '''
 
     CONFIG_TYPE = 'app_settings'
 
     # App Config
     APP_ENV = os.environ.get('APP_ENV', 'development')
     APP_ENABLE_CORS = os.environ.get('APP_ENABLE_CORS', 'False').capitalize() == 'True'
     APP_HOST = os.environ.get('APP_HOST', '0.0.0.0')
     APP_PORT = int(os.environ.get('APP_PORT', '5000'))
 
     APP_API_CLIENT_HEADERS = {"User-Agent": "Mozilla/5.0"}
 
     APP_LOG_CONFIG = os.environ.get('APP_LOG_CONFIG', 'True').capitalize() == 'True'
+    APP_CORS_ENABLED_PATHS = get_list_from_env('APP_CORS_ENABLED_PATHS', '/api/*')
     APP_DEBUG_MODE = True
 
-    def __init__(self, app_env:str=None, app_enable_cors:bool=None, app_host:str=None, app_port:int=None, app_api_client_headers:dict=None, app_log_config:bool=None):
+    def __init__(self, app_env:str=None, app_enable_cors:bool=None, app_host:str=None, app_port:int=None, app_api_client_headers:dict=None, app_log_config:bool=None, app_cors_enabled_paths:list=None):
 
         if app_env: App_Settings.APP_ENV = app_env
         os.environ['FLASK_ENV'] = App_Settings.APP_ENV
 
         if app_enable_cors != None: App_Settings.APP_ENABLE_CORS = app_enable_cors
         if app_host: App_Settings.APP_HOST = app_host
         if app_port: App_Settings.APP_PORT = app_port
         if app_api_client_headers: App_Settings.APP_API_CLIENT_HEADERS = app_api_client_headers
 
         if app_log_config: App_Settings.APP_LOG_CONFIG = app_log_config
+        if app_cors_enabled_paths: App_Settings.APP_CORS_ENABLED_PATHS = app_cors_enabled_paths
         
         App_Settings.APP_DEBUG_MODE = True if App_Settings.APP_ENV in ['dev', 'development', 'uat'] else False
         os.environ['FLASK_DEBUG'] = '1' if App_Settings.APP_DEBUG_MODE else '0'
 
 
     @staticmethod
     def get_log_data():
         ''' Returns a list of the settings to log to console '''
 
         return [
             'CORS enabled for application' if App_Settings.APP_ENABLE_CORS else 'CORS disabled for application. Set `APP_ENABLE_CORS` to True in environment to enable it',
+            f'CORS enabled for paths: {App_Settings.APP_CORS_ENABLED_PATHS}' if App_Settings.APP_ENABLE_CORS else 'CORS disabled for application. Set `APP_ENABLE_CORS` to True in environment to enable it',
             f'Default API client headers are {App_Settings.APP_API_CLIENT_HEADERS}'
-        ]
+        ]
```

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/jwt_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/jwt_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/main.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/mongodb_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/mongodb_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/rabbitmq_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/rabbitmq_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/redis_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/redis_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/sentry_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/sentry_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/setting.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/setting.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/settings/slack_settings.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/settings/slack_settings.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/config/task.py` & `dead_simple_framework-1.3.4/dead_simple_framework/config/task.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/database/fixtures.py` & `dead_simple_framework-1.3.4/dead_simple_framework/database/fixtures.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/database/index.py` & `dead_simple_framework-1.3.4/dead_simple_framework/database/index.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/database/main.py` & `dead_simple_framework-1.3.4/dead_simple_framework/database/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/database/utils.py` & `dead_simple_framework-1.3.4/dead_simple_framework/database/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/encoder.py` & `dead_simple_framework-1.3.4/dead_simple_framework/encoder.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/handlers/default.py` & `dead_simple_framework-1.3.4/dead_simple_framework/handlers/default.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/handlers/login.py` & `dead_simple_framework-1.3.4/dead_simple_framework/handlers/login.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/handlers/permissions.py` & `dead_simple_framework-1.3.4/dead_simple_framework/handlers/permissions.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/handlers/users.py` & `dead_simple_framework-1.3.4/dead_simple_framework/handlers/users.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/main.py` & `dead_simple_framework-1.3.4/dead_simple_framework/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,16 +76,15 @@
 
         # Register all HTTP routes that should be available based on the application config
         Router.register_routes(self.app, config['routes'])
         
         # Initialize inherited asynchronous task management ability
         super().__init__(dynamic_tasks=config.get('tasks'))
 
-        # # TODO - Dynamic Resources
-        if Settings.APP_ENABLE_CORS: CORS(self.app, resources=r'/api/*', supports_credentials=True)
+        if Settings.APP_ENABLE_CORS: CORS(self.app, resources=Settings.APP_CORS_ENABLED_PATHS, supports_credentials=True)
 
         Application._app = self
 
         self.app.before_first_request(lambda: Database.register_indices(self.indices))
         self.app.before_first_request(lambda: Database.register_fixtures(Fixtures(config.get('fixtures'))))
```

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/router.py` & `dead_simple_framework-1.3.4/dead_simple_framework/router.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/slack.py` & `dead_simple_framework-1.3.4/dead_simple_framework/slack.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/tasks/main.py` & `dead_simple_framework-1.3.4/dead_simple_framework/tasks/main.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/tasks/task.py` & `dead_simple_framework-1.3.4/dead_simple_framework/tasks/task.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework/tasks/utils.py` & `dead_simple_framework-1.3.4/dead_simple_framework/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework.egg-info/PKG-INFO` & `dead_simple_framework-1.3.4/dead_simple_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead-simple-framework
-Version: 1.3.3
+Version: 1.3.4
 Summary: RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations
 Home-page: https://github.com/Topazoo/dead_simple_framework
 Author: Peter Swanson
 Author-email: pswanson@ucdavis.edu
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `dead_simple_framework-1.3.3/dead_simple_framework.egg-info/SOURCES.txt` & `dead_simple_framework-1.3.4/dead_simple_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dead_simple_framework-1.3.3/setup.py` & `dead_simple_framework-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setuptools.setup(
     author="Peter Swanson",
     author_email="pswanson@ucdavis.edu",
     name='dead_simple_framework',
     license="MIT",
     description='RESTful Flask framework with builtin MongoDB, Redis, Celery, Sentry and Slack integrations',
-    version='v1.3.3',
+    version='v1.3.4',
     long_description=README,
     url='https://github.com/Topazoo/dead_simple_framework',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['flask', 'pymongo', 'celery', 'flask-cors', 'requests', 'redis', 'eventlet', 'pyOpenSSL', 'Flask-JWT-Extended', 'passlib', 'jsonschema', 'sentry-sdk[flask]', 'slack-sdk', 'Flask-PyMongo'],
     long_description_content_type='text/markdown',
     classifiers=[]
```

