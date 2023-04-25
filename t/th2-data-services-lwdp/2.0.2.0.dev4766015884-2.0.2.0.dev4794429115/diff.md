# Comparing `tmp/th2_data_services_lwdp-2.0.2.0.dev4766015884.tar.gz` & `tmp/th2_data_services_lwdp-2.0.2.0.dev4794429115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4766015884.tar", last modified: Fri Apr 21 14:43:47 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4794429115.tar", last modified: Tue Apr 25 06:38:29 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884.tar` & `th2_data_services_lwdp-2.0.2.0.dev4794429115.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-21 14:43:26.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    38821 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-04-21 14:39:54.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-21 14:43:47.000000 th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-25 06:38:08.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38821 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-04-25 06:35:44.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 06:38:29.000000 th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.0.2.0.dev4766015884
+Version: 2.0.2.0.dev4794429115
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/README.md` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/setup.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from .stub_builder import BrokenEvent, BrokenMessage
 from .message_response_format import ResponseFormat
 from .streams import Stream, Streams
 from .page import Page
 
 from th2_data_services.config import options as _o
 
 from th2_data_services.data_source.lwdp.resolver import (
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,36 @@
     http_event_struct,
     http_message_struct,
     EventStruct,
     MessageStruct,
 )
 
 
+class BrokenEvent:
+    def __str__(self):
+        return "<BrokenEvent>"
+
+    def __repr__(self):
+        return "<BrokenEvent>"
+
+    def __eq__(self, other):
+        return other == BrokenEvent
+
+
+class BrokenMessage:
+    def __str__(self):
+        return "<BrokenMessage>"
+
+    def __repr__(self):
+        return "<BrokenMessage>"
+
+    def __eq__(self, other):
+        return other == BrokenMessage
+
+
 class EventStubBuilder(IEventStub):
     def __init__(self, event_struct: EventStruct):
         """Event stub builder.
 
         Args:
             event_struct: Event struct class.
         """
@@ -38,21 +60,21 @@
         """Event stub template.
 
         Returns:
             (dict) Event stub template.
         """
         return {
             self.event_fields.ATTACHED_MESSAGES_IDS: [],
-            self.event_fields.BATCH_ID: "Broken_Event",
+            self.event_fields.BATCH_ID: BrokenEvent(),
             self.event_fields.END_TIMESTAMP: {"nano": 0, "epochSecond": 0},
             self.event_fields.START_TIMESTAMP: {"nano": 0, "epochSecond": 0},
             self.event_fields.EVENT_ID: self.REQUIRED_FIELD,
-            self.event_fields.NAME: "Broken_Event",
-            self.event_fields.EVENT_TYPE: "Broken_Event",
-            self.event_fields.PARENT_EVENT_ID: "Broken_Event",
+            self.event_fields.NAME: BrokenEvent(),
+            self.event_fields.EVENT_TYPE: BrokenEvent(),
+            self.event_fields.PARENT_EVENT_ID: BrokenEvent(),
             self.event_fields.STATUS: None,
             self.event_fields.IS_BATCHED: None,
         }
 
 
 class MessageStubBuilder(IMessageStub):
     def __init__(self, message_struct: MessageStruct):
@@ -69,16 +91,16 @@
         """Message stub template.
 
         Returns:
             (dict) Message stub template.
         """
         return {
             self.message_fields.DIRECTION: None,
-            self.message_fields.SESSION_ID: "Broken_Message",
-            self.message_fields.MESSAGE_TYPE: "Broken_Message",
+            self.message_fields.SESSION_ID: BrokenMessage(),
+            self.message_fields.MESSAGE_TYPE: BrokenMessage(),
             self.message_fields.TIMESTAMP: {"nano": 0, "epochSecond": 0},
             self.message_fields.BODY: [],
             self.message_fields.BODY_BASE64: [],
             self.message_fields.MESSAGE_ID: self.REQUIRED_FIELD,
             self.message_fields.ATTACHED_EVENT_IDS: [],
         }
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.0.2.0.dev4766015884
+Version: 2.0.2.0.dev4794429115
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4766015884/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.0.2.0.dev4794429115/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

