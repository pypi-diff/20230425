# Comparing `tmp/watchmen_data_kernel-16.5.0.tar.gz` & `tmp/watchmen_data_kernel-16.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_data_kernel-16.5.0.tar", max compression
+gzip compressed data, was "watchmen_data_kernel-16.5.1.tar", max compression
```

## Comparing `watchmen_data_kernel-16.5.0.tar` & `watchmen_data_kernel-16.5.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1061 2023-04-06 09:13:10.380010 watchmen_data_kernel-16.5.0/LICENSE
--rw-r--r--   0        0        0     1207 2023-04-06 09:13:10.380010 watchmen_data_kernel-16.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 09:13:10.380010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/__init__.py
--rw-r--r--   0        0        0      187 2023-04-06 09:13:10.380010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/__init__.py
--rw-r--r--   0        0        0     2808 2023-04-06 09:13:10.380010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/cache_manager.py
--rw-r--r--   0        0        0     5679 2023-04-06 09:13:10.380010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/cache_service.py
--rw-r--r--   0        0        0     1555 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/data_source_cache.py
--rw-r--r--   0        0        0     1048 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/external_writer_cache.py
--rw-r--r--   0        0        0     1097 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/internal_cache.py
--rw-r--r--   0        0        0     1442 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/key_store_cache.py
--rw-r--r--   0        0        0     1709 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py
--rw-r--r--   0        0        0     2595 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/pipeline_cache.py
--rw-r--r--   0        0        0      861 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/tenant_cache.py
--rw-r--r--   0        0        0     2811 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/topic_cache.py
--rw-r--r--   0        0        0      463 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/common/__init__.py
--rw-r--r--   0        0        0       44 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/common/exception.py
--rw-r--r--   0        0        0     3594 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/common/settings.py
--rw-r--r--   0        0        0      399 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/__init__.py
--rw-r--r--   0        0        0     1840 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/aes_encryptor.py
--rw-r--r--   0        0        0     4349 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/center_masker.py
--rw-r--r--   0        0        0     2642 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/date_masker.py
--rw-r--r--   0        0        0     1475 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/encryptor.py
--rw-r--r--   0        0        0     2936 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/encryptor_registry.py
--rw-r--r--   0        0        0     1607 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/last_masker.py
--rw-r--r--   0        0        0      776 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/mail_masker.py
--rw-r--r--   0        0        0      807 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/md5_encryptor.py
--rw-r--r--   0        0        0      968 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/sha256_encryptor.py
--rw-r--r--   0        0        0      340 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/external_writer/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py
--rw-r--r--   0        0        0     2006 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/external_writer/external_writer_registry.py
--rw-r--r--   0        0        0      285 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1410 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/data_source_service.py
--rw-r--r--   0        0        0     1993 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/external_writer_service.py
--rw-r--r--   0        0        0     1091 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/key_store_service.py
--rw-r--r--   0        0        0     2479 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/pipeline_service.py
--rw-r--r--   0        0        0     1343 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/tenant_service.py
--rw-r--r--   0        0        0     3683 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/topic_service.py
--rw-r--r--   0        0        0      162 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/__init__.py
--rw-r--r--   0        0        0     1017 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/service_helper.py
--rw-r--r--   0        0        0     1535 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/storage_helper.py
--rw-r--r--   0        0        0     3078 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/topic_structure_helper.py
--rw-r--r--   0        0        0      319 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/__init__.py
--rw-r--r--   0        0        0     6963 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/data_entity_helper.py
--rw-r--r--   0        0        0    15863 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/data_service.py
--rw-r--r--   0        0        0     1560 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/factor_column_mapper.py
--rw-r--r--   0        0        0     4634 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/raw_data_service.py
--rw-r--r--   0        0        0     3146 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/regular_data_service.py
--rw-r--r--   0        0        0     2207 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/shaper.py
--rw-r--r--   0        0        0     3610 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/topic_storage.py
--rw-r--r--   0        0        0      639 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/__init__.py
--rw-r--r--   0        0        0      248 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/ask_action_defined_as.py
--rw-r--r--   0        0        0    36597 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py
--rw-r--r--   0        0        0    57812 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py
--rw-r--r--   0        0        0      250 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/time_utils.py
--rw-r--r--   0        0        0      941 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/topic_utils.py
--rw-r--r--   0        0        0     7540 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/utils.py
--rw-r--r--   0        0        0     3074 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/variables.py
--rw-r--r--   0        0        0      145 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/system/__init__.py
--rw-r--r--   0        0        0     1818 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/system/change_log_helper.py
--rw-r--r--   0        0        0     8102 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/system/operation_helper.py
--rw-r--r--   0        0        0       79 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/__init__.py
--rw-r--r--   0        0        0     2628 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py
--rw-r--r--   0        0        0     3235 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/date_time_factor.py
--rw-r--r--   0        0        0     2462 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/default_value_factor.py
--rw-r--r--   0        0        0     5245 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/encrypt_factor.py
--rw-r--r--   0        0        0      911 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/flatten_factor.py
--rw-r--r--   0        0        0     3656 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/topic_schema.py
--rw-r--r--   0        0        0     6189 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/utils.py
--rw-r--r--   0        0        0      113 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/utils/__init__.py
--rw-r--r--   0        0        0     2749 2023-04-06 09:13:10.384010 watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/utils/variable_helper.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 watchmen_data_kernel-16.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/LICENSE
+-rw-r--r--   0        0        0     1207 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/__init__.py
+-rw-r--r--   0        0        0     2808 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/cache_manager.py
+-rw-r--r--   0        0        0     5679 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/cache_service.py
+-rw-r--r--   0        0        0     1555 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/data_source_cache.py
+-rw-r--r--   0        0        0     1048 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/external_writer_cache.py
+-rw-r--r--   0        0        0     1097 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/internal_cache.py
+-rw-r--r--   0        0        0     1442 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/key_store_cache.py
+-rw-r--r--   0        0        0     1709 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py
+-rw-r--r--   0        0        0     2595 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/pipeline_cache.py
+-rw-r--r--   0        0        0      861 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/tenant_cache.py
+-rw-r--r--   0        0        0     2811 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/topic_cache.py
+-rw-r--r--   0        0        0      463 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/common/__init__.py
+-rw-r--r--   0        0        0       44 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/common/exception.py
+-rw-r--r--   0        0        0     3594 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/common/settings.py
+-rw-r--r--   0        0        0      399 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/__init__.py
+-rw-r--r--   0        0        0     1840 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/aes_encryptor.py
+-rw-r--r--   0        0        0     4349 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/center_masker.py
+-rw-r--r--   0        0        0     2642 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/date_masker.py
+-rw-r--r--   0        0        0     1475 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/encryptor.py
+-rw-r--r--   0        0        0     2936 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/encryptor_registry.py
+-rw-r--r--   0        0        0     1607 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/last_masker.py
+-rw-r--r--   0        0        0      776 2023-04-25 10:52:45.972219 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/mail_masker.py
+-rw-r--r--   0        0        0      807 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/md5_encryptor.py
+-rw-r--r--   0        0        0      968 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/sha256_encryptor.py
+-rw-r--r--   0        0        0      340 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/external_writer/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py
+-rw-r--r--   0        0        0     2006 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/external_writer/external_writer_registry.py
+-rw-r--r--   0        0        0      285 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1410 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/data_source_service.py
+-rw-r--r--   0        0        0     1993 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/external_writer_service.py
+-rw-r--r--   0        0        0     1091 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/key_store_service.py
+-rw-r--r--   0        0        0     2479 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/pipeline_service.py
+-rw-r--r--   0        0        0     1343 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/tenant_service.py
+-rw-r--r--   0        0        0     3683 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/topic_service.py
+-rw-r--r--   0        0        0      162 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/__init__.py
+-rw-r--r--   0        0        0     1017 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/service_helper.py
+-rw-r--r--   0        0        0     1535 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/storage_helper.py
+-rw-r--r--   0        0        0     3078 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/topic_structure_helper.py
+-rw-r--r--   0        0        0      319 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     6963 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/data_entity_helper.py
+-rw-r--r--   0        0        0    15863 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/data_service.py
+-rw-r--r--   0        0        0     1560 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/factor_column_mapper.py
+-rw-r--r--   0        0        0     4634 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/raw_data_service.py
+-rw-r--r--   0        0        0     3146 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/regular_data_service.py
+-rw-r--r--   0        0        0     2207 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/shaper.py
+-rw-r--r--   0        0        0     3610 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/topic_storage.py
+-rw-r--r--   0        0        0      639 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/ask_action_defined_as.py
+-rw-r--r--   0        0        0    36597 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py
+-rw-r--r--   0        0        0    57849 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py
+-rw-r--r--   0        0        0      250 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/time_utils.py
+-rw-r--r--   0        0        0      941 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/topic_utils.py
+-rw-r--r--   0        0        0     7540 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/utils.py
+-rw-r--r--   0        0        0     3074 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/variables.py
+-rw-r--r--   0        0        0      145 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/system/__init__.py
+-rw-r--r--   0        0        0     1818 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/system/change_log_helper.py
+-rw-r--r--   0        0        0     8102 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/system/operation_helper.py
+-rw-r--r--   0        0        0       79 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/__init__.py
+-rw-r--r--   0        0        0     2628 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py
+-rw-r--r--   0        0        0     3235 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/date_time_factor.py
+-rw-r--r--   0        0        0     2462 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/default_value_factor.py
+-rw-r--r--   0        0        0     5245 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/encrypt_factor.py
+-rw-r--r--   0        0        0      911 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/flatten_factor.py
+-rw-r--r--   0        0        0     3656 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/topic_schema.py
+-rw-r--r--   0        0        0     6189 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/utils.py
+-rw-r--r--   0        0        0      113 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/utils/__init__.py
+-rw-r--r--   0        0        0     2749 2023-04-25 10:52:45.976220 watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/utils/variable_helper.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 watchmen_data_kernel-16.5.1/PKG-INFO
```

### Comparing `watchmen_data_kernel-16.5.0/LICENSE` & `watchmen_data_kernel-16.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/pyproject.toml` & `watchmen_data_kernel-16.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-data-kernel"
-version = "16.5.0"
+version = "16.5.1"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_data_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cacheout = "^0.13.1"
 pycryptodome = "^3.14.1"
-watchmen-meta = "16.5.0"
-watchmen-storage-mysql = { version = "16.5.0", optional = true }
-watchmen-storage-oracle = { version = "16.5.0", optional = true }
-watchmen-storage-mongodb = { version = "16.5.0", optional = true }
-watchmen-storage-mssql = { version = "16.5.0", optional = true }
-watchmen-storage-postgresql = { version = "16.5.0", optional = true }
-watchmen-storage-oss = { version = "16.5.0", optional = true }
-watchmen-storage-s3 = { version = "16.5.0", optional = true }
+watchmen-meta = "16.5.1"
+watchmen-storage-mysql = { version = "16.5.1", optional = true }
+watchmen-storage-oracle = { version = "16.5.1", optional = true }
+watchmen-storage-mongodb = { version = "16.5.1", optional = true }
+watchmen-storage-mssql = { version = "16.5.1", optional = true }
+watchmen-storage-postgresql = { version = "16.5.1", optional = true }
+watchmen-storage-oss = { version = "16.5.1", optional = true }
+watchmen-storage-s3 = { version = "16.5.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/cache_manager.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/cache_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/data_source_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/data_source_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/external_writer_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/external_writer_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/internal_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/internal_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/key_store_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/key_store_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/pipeline_by_topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/pipeline_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/pipeline_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/tenant_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/tenant_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/cache/topic_cache.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/cache/topic_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/common/settings.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/aes_encryptor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/aes_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/center_masker.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/center_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/date_masker.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/date_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/encryptor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/encryptor_registry.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/encryptor_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/last_masker.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/last_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/mail_masker.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/mail_masker.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/md5_encryptor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/md5_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/encryption/sha256_encryptor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/encryption/sha256_encryptor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/external_writer/external_writer_builder_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/external_writer/external_writer_registry.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/external_writer/external_writer_registry.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/data_source_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/data_source_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/external_writer_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/external_writer_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/key_store_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/key_store_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/pipeline_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/tenant_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/tenant_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/meta/topic_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/meta/topic_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/service_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/service_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/storage_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/storage_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/service/topic_structure_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/service/topic_structure_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/data_entity_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/data_entity_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/data_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/factor_column_mapper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/factor_column_mapper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/raw_data_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/raw_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/regular_data_service.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/regular_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/shaper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/shaper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage/topic_storage.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage/topic_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/__init__.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/ask_from_memory.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/ask_from_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,77 +522,77 @@
 	prefix = variable.text
 	has_prefix = len(prefix) != 0
 	variable_name = variable.variable
 	if variable_name == VariablePredefineFunctions.NEXT_SEQ.value:
 		# next sequence
 		return \
 			create_snowflake_generator(prefix), \
-			[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
+				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
 	elif variable_name == VariablePredefineFunctions.NOW.value:
 		# now
 		if has_prefix:
 			value = f'{prefix}{get_current_time_in_seconds().strftime("%Y-%m-%d %H:%M:%S")}'
 			return lambda variables, principal_service: value, [PossibleParameterType.STRING]
 		else:
 			return lambda variables, principal_service: get_current_time_in_seconds(), [PossibleParameterType.DATETIME]
 	elif variable_name.startswith(VariablePredefineFunctions.YEAR_DIFF.value):
 		# year diff
 		return \
 			create_date_diff(
 				prefix, variable_name,
 				VariablePredefineFunctions.YEAR_DIFF, available_schemas, allow_in_memory_variables), \
-			[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
+				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
 	elif variable_name.startswith(VariablePredefineFunctions.MONTH_DIFF.value):
 		# month diff
 		return \
 			create_date_diff(
 				prefix, variable_name,
 				VariablePredefineFunctions.MONTH_DIFF, available_schemas, allow_in_memory_variables), \
-			[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
+				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
 	elif variable_name.startswith(VariablePredefineFunctions.DAY_DIFF.value):
 		# day diff
 		return \
 			create_date_diff(
 				prefix, variable_name,
 				VariablePredefineFunctions.DAY_DIFF, available_schemas, allow_in_memory_variables), \
-			[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
+				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
 	elif variable_name.startswith(VariablePredefineFunctions.MOVE_DATE.value):
 		# move date
 		return \
 			create_move_date(
 				prefix, variable_name, available_schemas, allow_in_memory_variables), \
-			[PossibleParameterType.STRING] if has_prefix else [
-				PossibleParameterType.DATE, PossibleParameterType.DATETIME, PossibleParameterType.TIME]
+				[PossibleParameterType.STRING] if has_prefix else [
+					PossibleParameterType.DATE, PossibleParameterType.DATETIME, PossibleParameterType.TIME]
 	elif variable_name.startswith(VariablePredefineFunctions.DATE_FORMAT.value):
 		# date format
 		return \
 			create_date_format(prefix, variable_name, available_schemas, allow_in_memory_variables), \
-			[PossibleParameterType.STRING]
+				[PossibleParameterType.STRING]
 	elif variable_name.endswith(VariablePredefineFunctions.LENGTH.value):
 		# char length
 		return \
 			create_char_length(prefix, variable_name, available_schemas, allow_in_memory_variables), \
-			[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
+				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.NUMBER]
 
 	if allow_in_memory_variables:
 		if variable_name.startswith(VariablePredefineFunctions.FROM_PREVIOUS_TRIGGER_DATA.value):
 			if variable_name == VariablePredefineFunctions.FROM_PREVIOUS_TRIGGER_DATA.value:
 				raise DataKernelException(
 					f'Previous trigger data is a dict, cannot be used for storage. '
 					f'Current constant segment is [{prefix}{{{variable_name}}}].')
 			length = len(VariablePredefineFunctions.FROM_PREVIOUS_TRIGGER_DATA.value)
 			if len(variable_name) < length + 2 or variable_name[length:length + 1] != '.':
 				raise DataKernelException(f'Constant[{variable_name}] is not supported.')
 			return \
 				create_from_previous_trigger_data(prefix, variable_name[length + 1:]), \
-				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.ANY_VALUE]
+					[PossibleParameterType.STRING if has_prefix else PossibleParameterType.ANY_VALUE]
 		else:
 			return \
 				create_get_from_variables_with_prefix(prefix, variable_name), \
-				[PossibleParameterType.STRING if has_prefix else PossibleParameterType.ANY_VALUE]
+					[PossibleParameterType.STRING if has_prefix else PossibleParameterType.ANY_VALUE]
 	else:
 		# recover to original string
 		return create_static_str(f'{prefix}{{{variable_name}}}'), [PossibleParameterType.STRING]
 
 
 def create_ask_constant_value(
 		variables: List[MightAVariable], available_schemas: List[TopicSchema], allow_in_memory_variables: bool
@@ -1017,15 +1017,15 @@
 
 def parse_conditional_parameter_for_storage(
 		parameter: Parameter, available_schemas: List[TopicSchema],
 		principal_service: PrincipalService, allow_in_memory_variables: bool
 ) -> Tuple[ParsedStorageCondition, ParsedStorageParameter]:
 	return \
 		parse_condition_for_storage(parameter.on, available_schemas, principal_service, allow_in_memory_variables), \
-		parse_parameter_for_storage(parameter, available_schemas, principal_service, allow_in_memory_variables)
+			parse_parameter_for_storage(parameter, available_schemas, principal_service, allow_in_memory_variables)
 
 
 class ParsedStorageMappingFactor:
 	def __init__(
 			self, schema: TopicSchema, mapping_factor: MappingFactor, accumulate_mode: Optional[AccumulateMode],
 			principal_service: PrincipalService):
 		self.mappingFactor = mapping_factor
@@ -1063,24 +1063,24 @@
 
 	def get_aggregate_assist_avg_count(self, data: Dict[str, Any]) -> int:
 		assist = self.get_aggregate_assist_column(data, True)
 		value = assist.get(f'{self.factor.name}.avg_count')
 		parsed, decimal_value = is_decimal(value)
 		return decimal_value if parsed else 0
 
-	def get_original_value(self, original_data: Optional[Dict[str, Any]]) -> int:
+	def get_original_value(self, original_data: Optional[Dict[str, Any]]) -> Decimal:
 		"""
 		return 0 when not found or cannot be parsed to decimal
 		"""
 		value = original_data.get(self.factor.name)
 		parsed, decimal_value = is_decimal(value)
 		if parsed:
-			return int(decimal_value)
+			return decimal_value
 		else:
-			return 0
+			return Decimal('0')
 
 	def compute_current_value(self, variables: PipelineVariables, principal_service: PrincipalService) -> Decimal:
 		value = self.parsedParameter.value(variables, principal_service)
 		parsed, decimal_value = is_decimal(value)
 		decimal_value = 0 if not parsed else decimal_value
 		return decimal_value
 
@@ -1090,15 +1090,15 @@
 		decimal_value = 0 if not parsed else decimal_value
 		return decimal_value
 
 	def compute_previous_and_current_value(
 			self, variables: PipelineVariables, principal_service: PrincipalService) -> Tuple[Decimal, Decimal]:
 		return \
 			self.compute_previous_value(variables, principal_service), \
-			self.compute_current_value(variables, principal_service)
+				self.compute_current_value(variables, principal_service)
 
 	def run(
 			self, data: Dict[str, Any], original_data: Optional[Dict[str, Any]], variables: PipelineVariables,
 			principal_service: PrincipalService
 	) -> Tuple[str, Any]:
 		if self.arithmetic == AggregateArithmetic.SUM:
 			if original_data is None:
@@ -1197,18 +1197,18 @@
 					raise DataKernelException(
 						'There is no existing aggregated data, therefore reverse count cannot be performed here.')
 				else:
 					# count always be 1
 					value = 1
 			elif self.accumulateMode == AccumulateMode.CUMULATE:
 				# using force cumulating explicitly, ignore previous data anyway, always add 1
-				value = self.get_original_value(original_data) + 1
+				value = int(self.get_original_value(original_data)) + 1
 			elif variables.has_previous_trigger_data():
 				# has previous data, it used to be triggered
-				value = self.get_original_value(original_data)
+				value = int(self.get_original_value(original_data))
 				if self.accumulateMode == AccumulateMode.REVERSE:
 					# reverse the last accumulating, subtract 1
 					if value <= 0:
 						raise DataKernelException('Count <= 0, therefore reverse count cannot be performed here.')
 					else:
 						value = value - 1
 				else:
@@ -1217,15 +1217,15 @@
 					value = 1 if value == 0 else value
 			elif self.accumulateMode == AccumulateMode.REVERSE:
 				# no previous data, reverse cannot be performed
 				raise DataKernelException(
 					'There is no previous trigger data, therefore reverse count cannot be performed here.')
 			else:
 				# no previous data, count + 1
-				value = self.get_original_value(original_data) + 1
+				value = int(self.get_original_value(original_data)) + 1
 		else:
 			value = self.parsedParameter.value(variables, principal_service)
 			# value for mapping is computed in memory
 			# parse factor value to applicable type
 			value = cast_value_for_factor(value, self.factor) if value is not None else None
 		return self.factor.name, value
```

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/topic_utils.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/utils.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/storage_bridge/variables.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/storage_bridge/variables.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/system/change_log_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/system/change_log_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/system/operation_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/system/operation_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/aid_hierarchy.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/date_time_factor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/date_time_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/default_value_factor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/default_value_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/encrypt_factor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/encrypt_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/flatten_factor.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/flatten_factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/topic_schema.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/topic_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/topic_schema/utils.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/topic_schema/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/src/watchmen_data_kernel/utils/variable_helper.py` & `watchmen_data_kernel-16.5.1/src/watchmen_data_kernel/utils/variable_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_data_kernel-16.5.0/PKG-INFO` & `watchmen_data_kernel-16.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-data-kernel
-Version: 16.5.0
+Version: 16.5.1
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: cacheout (>=0.13.1,<0.14.0)
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
-Requires-Dist: watchmen-meta (==16.5.0)
-Requires-Dist: watchmen-storage-mongodb (==16.5.0) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.0) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.0) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.0) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.0) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.0) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.0) ; extra == "s3"
+Requires-Dist: watchmen-meta (==16.5.1)
+Requires-Dist: watchmen-storage-mongodb (==16.5.1) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.1) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.1) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.1) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.1) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.1) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.1) ; extra == "s3"
```

