# Comparing `tmp/tap-pipedrive-1.1.8.tar.gz` & `tmp/tap-pipedrive-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-pipedrive-1.1.8.tar", last modified: Thu Mar  9 14:39:59 2023, max compression
+gzip compressed data, was "dist/tap-pipedrive-1.2.0.tar", last modified: Tue Apr 25 13:06:09 2023, max compression
```

## Comparing `tap-pipedrive-1.1.8.tar` & `tap-pipedrive-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.833769 tap-pipedrive-1.1.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      322 2023-03-09 14:39:59.833769 tap-pipedrive-1.1.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1536 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-09 14:39:59.833769 tap-pipedrive-1.1.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      817 2023-03-09 14:38:15.000000 tap-pipedrive-1.1.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.829769 tap-pipedrive-1.1.8/tap_pipedrive/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      696 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      988 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.829769 tap-pipedrive-1.1.8/tap_pipedrive/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      678 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/activity_types.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/currency.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-03-06 18:56:00.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/deal_products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/dealflow.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      683 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/filters.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/pipelines.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.829769 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.829769 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2238 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/activities.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2022-06-07 13:12:50.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/deals.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-03-06 18:56:00.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/notes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3402 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3740 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/persons.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/products.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1876 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/files.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1405 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      756 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/schemas/stages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6582 2023-03-07 16:21:27.000000 tap-pipedrive-1.1.8/tap_pipedrive/stream.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.829769 tap-pipedrive-1.1.8/tap_pipedrive/streams/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      298 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/activity_types.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/currencies.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      411 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/deal_products.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/dealflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      278 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/filters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      193 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/notes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/pipelines.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.833769 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.833769 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3590 2023-01-17 20:20:40.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/activities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2022-06-07 13:12:50.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/deals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/notes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/organizations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1377 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/persons.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/products.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/files.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-01-17 20:20:40.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/users.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      275 2021-06-28 21:06:42.000000 tap-pipedrive-1.1.8/tap_pipedrive/streams/stages.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16772 2023-03-09 14:38:15.000000 tap-pipedrive-1.1.8/tap_pipedrive/tap.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-09 14:39:59.829769 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      322 2023-03-09 14:39:59.000000 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1936 2023-03-09 14:39:59.000000 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-09 14:39:59.000000 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-03-09 14:39:59.000000 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-03-09 14:39:59.000000 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-03-09 14:39:59.000000 tap-pipedrive-1.1.8/tap_pipedrive.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      696 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/deal_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      411 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/deal_products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      193 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/notes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      278 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/filters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      275 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/stages.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/files.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/users.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      521 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      587 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/notes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/organizations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1520 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/deals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1377 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/persons.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3590 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/activities.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/currencies.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      298 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/activity_types.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/dealflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/streams/pipelines.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      988 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6582 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/stream.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      756 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/stages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_fields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/dealflow.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      683 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/filters.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 13:06:09.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3740 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/persons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2238 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/activities.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/notes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/deals.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3402 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1876 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/files.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1405 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      678 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/activity_types.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/pipelines.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/currency.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/tap_pipedrive/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16806 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/tap_pipedrive/tap.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      817 2023-04-25 13:04:36.000000 tap-pipedrive-1.2.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1536 2023-04-19 07:20:50.000000 tap-pipedrive-1.2.0/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-pipedrive-1.1.8/LICENSE` & `tap-pipedrive-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/README.md` & `tap-pipedrive-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/setup.py` & `tap-pipedrive-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name="tap-pipedrive",
-      version="1.1.8",
+      version="1.2.0",
       description="Singer.io tap for extracting data from the Pipedrive API",
       author="Stitch",
       author_email="dev@stitchdata.com",
       url="http://singer.io",
       classifiers=["Programming Language :: Python :: 3 :: Only"],
       py_modules=["tap_pipedrive"],
       install_requires=[
```

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/cli.py` & `tap-pipedrive-1.2.0/tap_pipedrive/cli.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/exceptions.py` & `tap-pipedrive-1.2.0/tap_pipedrive/exceptions.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/activity_types.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/activity_types.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/deal_products.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/deal_products.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/dealflow.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/dealflow.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/filters.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/filters.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/pipelines.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/pipelines.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/activities.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/activities.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/deals.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/deals.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/notes.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/notes.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/organizations.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/persons.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/persons.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/dynamic_typing/products.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/dynamic_typing/products.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/files.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/files.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/recents/users.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/recents/users.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/schemas/stages.json` & `tap-pipedrive-1.2.0/tap_pipedrive/schemas/stages.json`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/stream.py` & `tap-pipedrive-1.2.0/tap_pipedrive/stream.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/__init__.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from .recents.dynamic_typing.activities import RecentActivitiesStream
 from .recents.dynamic_typing.deals import RecentDealsStream
 from .recents.dynamic_typing.organizations import RecentOrganizationsStream
 from .recents.dynamic_typing.persons import RecentPersonsStream
 from .recents.dynamic_typing.products import RecentProductsStream
 from .dealflow import DealStageChangeStream
 from .deal_products import DealsProductsStream
+from .deal_fields import DealFields
 
 
 __all__ = ['CurrenciesStream', 'ActivityTypesStream', 'FiltersStream', 'StagesStream', 'PipelinesStream',
            'RecentUsersStream', 'RecentFilesStream',
            'RecentNotesStream', 'RecentActivitiesStream', 'RecentDealsStream', 'RecentOrganizationsStream',
-           'RecentPersonsStream', 'RecentProductsStream', 'DealStageChangeStream', 'DealsProductsStream'
+           'RecentPersonsStream', 'RecentProductsStream', 'DealStageChangeStream', 'DealsProductsStream',
+           'DealFields'
            ]
```

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/dealflow.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/dealflow.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/__init__.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/__init__.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/activities.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/activities.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/deals.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/deals.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/notes.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/notes.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/organizations.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/organizations.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/persons.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/persons.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/dynamic_typing/products.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/dynamic_typing/products.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/streams/recents/users.py` & `tap-pipedrive-1.2.0/tap_pipedrive/streams/recents/users.py`

 * *Files identical despite different names*

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive/tap.py` & `tap-pipedrive-1.2.0/tap_pipedrive/tap.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .config import BASE_URL, CONFIG_DEFAULTS
 from .exceptions import (PipedriveError, PipedriveNotFoundError, PipedriveBadRequestError, PipedriveUnauthorizedError, PipedrivePaymentRequiredError, 
                         PipedriveForbiddenError, PipedriveGoneError, PipedriveUnsupportedMediaError, PipedriveUnprocessableEntityError, PipedriveTooManyRequestsError, 
                         PipedriveTooManyRequestsInSecondError,PipedriveInternalServiceError, PipedriveNotImplementedError, PipedriveServiceUnavailableError)
 from .streams import (CurrenciesStream, ActivityTypesStream, FiltersStream, StagesStream, PipelinesStream,
                       RecentNotesStream, RecentUsersStream, RecentActivitiesStream, RecentDealsStream,
                       RecentFilesStream, RecentOrganizationsStream, RecentPersonsStream, RecentProductsStream,
-                      DealStageChangeStream, DealsProductsStream)
+                      DealStageChangeStream, DealsProductsStream, DealFields)
 
 
 logger = singer.get_logger()
 
 # timeout request after 300 seconds
 REQUEST_TIMEOUT = 300
 
@@ -112,15 +112,16 @@
         RecentActivitiesStream(),
         RecentDealsStream(),
         RecentFilesStream(),
         RecentOrganizationsStream(),
         RecentPersonsStream(),
         RecentProductsStream(),
         DealStageChangeStream(),
-        DealsProductsStream()
+        DealsProductsStream(),
+        DealFields()
     ]
 
     def __init__(self, config, state):
         self.config = self.get_default_config()
         self.config.update(config)
         self.config['start_date'] = pendulum.parse(self.config['start_date'])
         self.state = state
```

### Comparing `tap-pipedrive-1.1.8/tap_pipedrive.egg-info/SOURCES.txt` & `tap-pipedrive-1.2.0/tap_pipedrive.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 tap_pipedrive.egg-info/SOURCES.txt
 tap_pipedrive.egg-info/dependency_links.txt
 tap_pipedrive.egg-info/entry_points.txt
 tap_pipedrive.egg-info/requires.txt
 tap_pipedrive.egg-info/top_level.txt
 tap_pipedrive/schemas/activity_types.json
 tap_pipedrive/schemas/currency.json
+tap_pipedrive/schemas/deal_fields.json
 tap_pipedrive/schemas/deal_products.json
 tap_pipedrive/schemas/dealflow.json
 tap_pipedrive/schemas/filters.json
 tap_pipedrive/schemas/pipelines.json
 tap_pipedrive/schemas/stages.json
 tap_pipedrive/schemas/recents/files.json
 tap_pipedrive/schemas/recents/users.json
@@ -28,14 +29,15 @@
 tap_pipedrive/schemas/recents/dynamic_typing/notes.json
 tap_pipedrive/schemas/recents/dynamic_typing/organizations.json
 tap_pipedrive/schemas/recents/dynamic_typing/persons.json
 tap_pipedrive/schemas/recents/dynamic_typing/products.json
 tap_pipedrive/streams/__init__.py
 tap_pipedrive/streams/activity_types.py
 tap_pipedrive/streams/currencies.py
+tap_pipedrive/streams/deal_fields.py
 tap_pipedrive/streams/deal_products.py
 tap_pipedrive/streams/dealflow.py
 tap_pipedrive/streams/filters.py
 tap_pipedrive/streams/notes.py
 tap_pipedrive/streams/pipelines.py
 tap_pipedrive/streams/stages.py
 tap_pipedrive/streams/recents/__init__.py
```

