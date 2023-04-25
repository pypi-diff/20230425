# Comparing `tmp/thrivve_core-0.1.0.tar.gz` & `tmp/thrivve_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-jld7nv4b/thrivve_core-0.1.0.tar", last modified: Tue Apr 18 15:49:23 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-4dxlm56d/thrivve_core-0.1.1.tar", last modified: Tue Apr 25 11:39:10 2023, max compression
```

## Comparing `thrivve_core-0.1.0.tar` & `thrivve_core-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12204 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-18 15:49:08.000000 thrivve_core-0.1.0/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-18 15:49:23.000000 thrivve_core-0.1.0/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4133 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2655 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12351 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-25 11:39:01.000000 thrivve_core-0.1.1/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2124 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 11:39:10.000000 thrivve_core-0.1.1/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.1.0/PKG-INFO` & `thrivve_core-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.1.0
+Version: 0.1.1
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.1.0/setup.py` & `thrivve_core-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.1.0",
+    version="0.1.1",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.1.0/thrivve_core/__init__.py` & `thrivve_core-0.1.1/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.1.1/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.1.1/thrivve_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.1.1/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.1.1/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.1.1/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/base.py` & `thrivve_core-0.1.1/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.1.1/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.1.1/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.1.1/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.1.1/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.1.1/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.1.1/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.1.1/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/auth.py` & `thrivve_core-0.1.1/thrivve_core/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/config.py` & `thrivve_core-0.1.1/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.1.1/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.1.1/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/enums.py` & `thrivve_core-0.1.1/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.1.1/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.1.1/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/filters.py` & `thrivve_core-0.1.1/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.1.1/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.1.1/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.1.1/thrivve_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/log_config.py` & `thrivve_core-0.1.1/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.1.1/thrivve_core/helpers/micro_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,29 +131,34 @@
             if isinstance(data, list):
                 for row in data:
                     self.column_values.add(get_obj_value(row, self.lookup_key))
             else:
                 self.column_values.add(get_obj_value(data, self.lookup_key))
 
         if not len(self.column_values):
+            self.column_values = []
             return self
             # raise AppMicroFetcherError('Lookup key {} not found'.format(self.lookup_key))
 
         self.column_values = list(filter(None, self.column_values))
         self.column_values = self.column_values[0] if len(self.column_values) == 1 else self.column_values
 
         if self.compair_operator not in ('=', 'IN'):
             raise AppMicroFetcherError('Only == currently supported')
 
         self.compair_operator = 'IN' if isinstance(self.column_values, list) else self.compair_operator
 
-        self.table_name = against[0]
-        self.column_name = against[1]
+        if len(against) != 2:
+            self.column_name = against[0]
+        else:
+            self.table_name = against[0]
+            self.column_name = against[1]
+
+            self.fields.append(self.column_name)
 
-        self.fields.append(self.column_name)
         return self
 
     def fetch(self):
         if self.column_values or self.module_name or self.query_type == QueryTypes.SEARCH.value:
             return self._call_api()
         else:
             return self.base_data
@@ -219,15 +224,15 @@
                 custom_text = json.loads(response.text).get('message')
             except json.decoder.JSONDecodeError:
                 pass
             raise AppFetchServiceDataError(custom_text)
 
         result = response.json()
 
-        if self.base_data:
+        if self.base_data is not None:
             return self._map_base(result)
 
         return result
 
     def _get_global_config(self, key, default_value):
         if hasattr(self, 'global_configs') and isinstance(self.global_configs, dict):
             if self.global_configs.get(key) is None:
```

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/notification_center.py` & `thrivve_core-0.1.1/thrivve_core/helpers/notification_center.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/search_function.py` & `thrivve_core-0.1.1/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/service_config.py` & `thrivve_core-0.1.1/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/sql.py` & `thrivve_core-0.1.1/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/time.py` & `thrivve_core-0.1.1/thrivve_core/helpers/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 DATABASE_DATE_TIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 DATABASE_TIME_FORMAT = "%H:%M:%S"
 
 
 DATE_FORMAT = "%Y-%m-%d"
 TIME_FORMAT = "%H:%M:%S"
 DATETIME_FORMAT = DATE_FORMAT + " " + TIME_FORMAT
+DATETIME_FORMAT_SCHEMA = "%Y-%m-%d %H:%M"
 
 def get_time_zone():
     time_zone = "UTC"
     if request:
         if request.headers.get("country_code"):
             time_zone = dict(sa="Asia/Riyadh", ps="Asia/Hebron").get(
                 request.headers.get("country_code"), "UTC"
```

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/topics.py` & `thrivve_core-0.1.1/thrivve_core/helpers/topics.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.1.1/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.1.1/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.0/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.1.1/thrivve_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.1.0/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.1.1/thrivve_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

