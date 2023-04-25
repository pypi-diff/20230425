# Comparing `tmp/openmsistream-1.3.4.tar.gz` & `tmp/openmsistream-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmsistream-1.3.4.tar", last modified: Fri Apr 21 18:52:34 2023, max compression
+gzip compressed data, was "openmsistream-1.4.0.tar", last modified: Mon Apr 24 23:55:54 2023, max compression
```

## Comparing `openmsistream-1.3.4.tar` & `openmsistream-1.4.0.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.396101 openmsistream-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-21 18:52:28.000000 openmsistream-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 18:52:28.000000 openmsistream-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-21 18:52:34.396101 openmsistream-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-21 18:52:28.000000 openmsistream-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.388101 openmsistream-1.3.4/openmsistream/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.388101 openmsistream-1.3.4/openmsistream/data_file_io/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.388101 openmsistream-1.3.4/openmsistream/data_file_io/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_download_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27293 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_upload_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/data_file_io/actor/file_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/file_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17858 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/data_file_io/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/data_file_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/data_file_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/download_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/reproducer_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/entity/upload_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/data_file_io/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/kafka_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/local_broker_test.config
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/prod.config
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test.config
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/consumer_and_producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/controlled_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/controlled_message_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/openmsistream_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/openmsistream_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/producible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/kafka_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/metadata_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/metadata_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/metadata_extraction/metadata_json_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/metadata_extraction/metadata_json_reproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.392101 openmsistream-1.3.4/openmsistream/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/s3_buckets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/s3_buckets/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/s3_buckets/s3_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/s3_buckets/s3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/s3_buckets/s3_transfer_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.396101 openmsistream-1.3.4/openmsistream/services/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.396101 openmsistream-1.3.4/openmsistream/services/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/examples/runnable_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/examples/script_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/install_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/linux_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/manage_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/service_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/services/windows_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.396101 openmsistream-1.3.4/openmsistream/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/controlled_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/controlled_process_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/controlled_process_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/dataclass_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/exception_tracking_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/has_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/has_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/provision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-21 18:52:28.000000 openmsistream-1.3.4/openmsistream/utilities/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:52:34.388101 openmsistream-1.3.4/openmsistream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-21 18:52:34.000000 openmsistream-1.3.4/openmsistream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-21 18:52:34.000000 openmsistream-1.3.4/openmsistream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:52:34.000000 openmsistream-1.3.4/openmsistream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-21 18:52:34.000000 openmsistream-1.3.4/openmsistream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-21 18:52:34.000000 openmsistream-1.3.4/openmsistream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 18:52:34.000000 openmsistream-1.3.4/openmsistream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 18:52:34.396101 openmsistream-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-21 18:52:28.000000 openmsistream-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-24 23:55:47.000000 openmsistream-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 23:55:47.000000 openmsistream-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-24 23:55:54.826432 openmsistream-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-24 23:55:47.000000 openmsistream-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.818432 openmsistream-1.4.0/openmsistream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_download_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_upload_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/download_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/reproducer_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/kafka_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/prod.config
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17730 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/producible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/metadata_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/metadata_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_reproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/s3_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/s3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/services/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/examples/runnable_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/examples/script_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/install_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/linux_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/manage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22468 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/service_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/windows_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21362 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/controlled_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/controlled_process_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/controlled_process_single_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22465 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/dataclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/exception_tracking_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/has_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/has_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/provision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/runnable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.818432 openmsistream-1.4.0/openmsistream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 23:55:47.000000 openmsistream-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 23:55:54.826432 openmsistream-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-24 23:55:47.000000 openmsistream-1.4.0/setup.py
```

### Comparing `openmsistream-1.3.4/LICENSE` & `openmsistream-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/PKG-INFO` & `openmsistream-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.3.4.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.4.0.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
@@ -18,15 +18,15 @@
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 
-[![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![GitHub Release Date](https://img.shields.io/github/release-date/openmsi/openmsistream) ![GitHub last commit](https://img.shields.io/github/last-commit/openmsi/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
+[![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 
 Applications for laboratory, analysis, and computational materials data streaming using [Apache Kafka](https://kafka.apache.org/)
 
 Available on PyPI at https://pypi.org/project/openmsistream and GitHub at https://github.com/openmsi/openmsistream 
 
 Official documentation at https://openmsistream.readthedocs.io/en/latest/
```

### Comparing `openmsistream-1.3.4/README.md` & `openmsistream-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <div align="center"> OpenMSIStream </div>
-#### <div align="center">***v1.3.4***</div>
+#### <div align="center">***v1.4.0***</div>
 
 #### <div align="center">Maggie Eminizer<sup>1</sup>, Sam Tabrisky<sup>2,3,4</sup>, Amir Sharifzadeh<sup>1</sup>, Christopher DiMarco<sup>4</sup>, Jacob M. Diamond<sup>4,6</sup>, K.T. Ramesh<sup>4</sup>, Todd C. Hufnagel<sup>4,5,6</sup>, Tyrel M. McQueen<sup>4,5,7,8</sup>, David Elbert<sup>1,4</sup></div>
 
  <div align="center"><sup>1</sup> Institute for Data Intensive Engineering and Science (IDIES), The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>2</sup> Department of Biology, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>3</sup> Department of Computer Science, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>4</sup> Hopkins Extreme Materials Institute (HEMI), The Johns Hopkins University, Baltimore, MD, USA </div>
@@ -12,15 +12,15 @@
  <div align="center"><sup>7</sup> Department of Chemistry, The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>8</sup> Institute for Quantum Matter (IQM), William H. Miller III Department of Physics and Astronomy, The Johns Hopkins University, Baltimore, MD, USA </div>
 
  <br>
  <div align="center"><img src="docs/source/images/openmsistream_logo.png" width="350" /></div>
  <br>
 
-[![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![GitHub Release Date](https://img.shields.io/github/release-date/openmsi/openmsistream) ![GitHub last commit](https://img.shields.io/github/last-commit/openmsi/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
+[![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 
 Applications for laboratory, analysis, and computational materials data streaming using [Apache Kafka](https://kafka.apache.org/)
 
 Available on PyPI at https://pypi.org/project/openmsistream and GitHub at https://github.com/openmsi/openmsistream 
 
 Official documentation at https://openmsistream.readthedocs.io/en/latest/
```

### Comparing `openmsistream-1.3.4/openmsistream/__init__.py` & `openmsistream-1.4.0/openmsistream/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 """OpenMSIStream library for simplified data streaming using Apache Kafka"""
 
-#imports
+# imports
 import os
 from .data_file_io.entity.upload_data_file import UploadDataFile
 from .data_file_io.actor.data_file_upload_directory import DataFileUploadDirectory
 from .data_file_io.actor.data_file_download_directory import DataFileDownloadDirectory
 from .data_file_io.actor.data_file_stream_processor import DataFileStreamProcessor
 from .data_file_io.actor.data_file_stream_reproducer import DataFileStreamReproducer
 from .s3_buckets.s3_transfer_stream_processor import S3TransferStreamProcessor
 
 __all__ = [
-    'UploadDataFile',
-    'DataFileUploadDirectory',
-    'DataFileDownloadDirectory',
-    'DataFileStreamProcessor',
-    'DataFileStreamReproducer',
-    'S3TransferStreamProcessor',
+    "UploadDataFile",
+    "DataFileUploadDirectory",
+    "DataFileDownloadDirectory",
+    "DataFileStreamProcessor",
+    "DataFileStreamReproducer",
+    "S3TransferStreamProcessor",
 ]
 
-#If running on Windows, try to pre-load the librdkafka.dll file
-if os.name=='nt' :
-    try :
+# If running on Windows, try to pre-load the librdkafka.dll file
+if os.name == "nt":
+    try:
         import confluent_kafka
-    except Exception :
+    except Exception:
         import traceback
+
         reason = None
         import sys, pathlib
-        dll_dir = pathlib.Path(sys.executable).parent/'Lib'/'site-packages'/'confluent_kafka.libs'
-        if not dll_dir.is_dir() :
-            reason = f'expected DLL directory {dll_dir} does not exist!'
+
+        dll_dir = (
+            pathlib.Path(sys.executable).parent
+            / "Lib"
+            / "site-packages"
+            / "confluent_kafka.libs"
+        )
+        if not dll_dir.is_dir():
+            reason = f"expected DLL directory {dll_dir} does not exist!"
         from ctypes import CDLL
+
         fps = []
-        for fp in dll_dir.glob('*.dll') :
-            if fp.name.startswith('librdkafka') :
+        for fp in dll_dir.glob("*.dll"):
+            if fp.name.startswith("librdkafka"):
                 fps.append(fp)
                 CDLL(str(fp))
-        if len(fps)<1 :
-            reason = f'{dll_dir} does not contain any librdkafka DLL files to preload!'
-        if reason is not None :
-            print(f'WARNING: Failed to preload librdkafka DLLs. Reason: {reason}')
-        try :
+        if len(fps) < 1:
+            reason = f"{dll_dir} does not contain any librdkafka DLL files to preload!"
+        if reason is not None:
+            print(f"WARNING: Failed to preload librdkafka DLLs. Reason: {reason}")
+        try:
             import confluent_kafka
-        except Exception as e :
-            errmsg = 'ERROR: Preloading librdkafka DLLs ('
-            errmsg+=', '.join([str(_) for _ in fps])
-            errmsg = f'{errmsg}) did not allow confluent_kafka to be imported! Exception (will be re-raised): '
-            errmsg+= f'{traceback.format_exc()}'
+        except Exception as e:
+            errmsg = "ERROR: Preloading librdkafka DLLs ("
+            errmsg += ", ".join([str(_) for _ in fps])
+            errmsg += (
+                f"{errmsg}) did not allow confluent_kafka to be imported! "
+                f"Exception (will be re-raised): {traceback.format_exc()}"
+            )
             print(errmsg)
             raise e
-    _ = confluent_kafka.Producer #appease pyflakes
+    _ = confluent_kafka.Producer  # appease pyflakes
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/__init__.py` & `openmsistream-1.4.0/openmsistream/data_file_io/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-"""Most classes in this directory are imported from the main module, but there are some other utility classes here"""
+"""
+Most classes in this directory are imported from the main module,
+but there are some other utility classes here
+"""
 
 from .entity.data_file import DataFile
-from .entity.download_data_file import DownloadDataFile, DownloadDataFileToDisk, DownloadDataFileToMemory
+from .entity.download_data_file import (
+    DownloadDataFile,
+    DownloadDataFileToDisk,
+    DownloadDataFileToMemory,
+)
 from .entity.data_file_directory import DataFileDirectory
 from .entity.reproducer_message import ReproducerMessage
 
 __all__ = [
-    'DataFile',
-    'DownloadDataFile',
-    'DownloadDataFileToDisk',
-    'DownloadDataFileToMemory',
-    'DataFileDirectory',
-    'ReproducerMessage',
+    "DataFile",
+    "DownloadDataFile",
+    "DownloadDataFileToDisk",
+    "DownloadDataFileToMemory",
+    "DataFileDirectory",
+    "ReproducerMessage",
 ]
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_chunk_handlers.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,189 @@
 """Anything that receives DataFileChunk messages from a topic and does something with them"""
 
-#imports
+# imports
 import warnings
 from abc import ABC, abstractmethod
 from threading import Lock
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto import KafkaCryptoMessage
 from ...utilities import LogOwner
 from ...kafka_wrapper.controlled_message_processor import ControlledMessageProcessor
 from ...kafka_wrapper.controlled_message_reproducer import ControlledMessageReproducer
 from ..config import DATA_FILE_HANDLING_CONST
 from ..entity.data_file_chunk import DataFileChunk
 from ..entity.download_data_file import DownloadDataFile
 
-class DataFileChunkHandler(LogOwner,ABC) :
+
+class DataFileChunkHandler(LogOwner, ABC):
     """
     A base class to perform some handling of DataFileChunk objects read from a topic.
     """
 
+    #################### CONSTANTS ####################
+
+    # Up to this many filepaths will be held onto after they've been processed
+    N_RECENT_FILES = 50
+
     #################### PROPERTIES ####################
 
     @property
-    def other_datafile_kwargs(self) :
+    def other_datafile_kwargs(self):
         """
         Overload this in child classes to define additional keyword arguments
         that should go to the specific datafile constructor
         """
         return {}
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,*args,datafile_type,**kwargs) :
+    def __init__(self, *args, datafile_type, **kwargs):
         """
         datafile_type = the type of datafile that the consumed messages will be used to create
             (must be a subclass of DownloadDataFile)
         """
-        super().__init__(*args,**kwargs)
+        super().__init__(*args, **kwargs)
         self.datafile_type = datafile_type
-        if not issubclass(self.datafile_type,DownloadDataFile) :
-            errmsg = 'ERROR: DataFileChunkProcessor requires a datafile_type that is a subclass of '
-            errmsg+= f'DownloadDataFile but {self.datafile_type} was given!'
+        if not issubclass(self.datafile_type, DownloadDataFile):
+            errmsg = (
+                "ERROR: DataFileChunkProcessor requires a datafile_type that is a subclass"
+                f" of DownloadDataFile but {self.datafile_type} was given!"
+            )
             raise ValueError(errmsg)
         self.files_in_progress_by_path = {}
         self.locks_by_fp = {}
-        self.completely_processed_filepaths = []
+        self.recent_processed_filepaths = []
+        self.n_processed_files = 0
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
     @abstractmethod
     def _process_message(self, lock, msg, rootdir_to_set):
         """
-        Make sure message values are of the expected DataFileChunk type with no root directory set, and then
-        add the chunk to the data file object. If the file is in progress this function returns True.
-        Otherwise the code from DownloadDataFile.add_chunk will be returned.
+        Make sure message values are of the expected DataFileChunk type with no root directory set,
+        and then add the chunk to the data file object. If the file is in progress this function
+        returns True. Otherwise the code from DownloadDataFile.add_chunk will be returned.
 
-        If instead the message was encrypted and could not be successfully decrypted, this will return
-        the raw Message object with KafkaCryptoMessages as its key and/or value
+        If instead the message was encrypted and could not be successfully decrypted, this will
+        return the raw Message object with KafkaCryptoMessages as its key and/or value
 
         lock = the Thread Lock object to use when processing the file this message comes from
         msg = the actual message object from a call to consumer.poll
         rootdir_to_set = root directory for the new DataFileChunk
 
         Child classes should call self._process_message() before doing anything else with
         the message to perform these checks
         """
         # If the message has KafkaCryptoMessages as its key and/or value, then decryption failed.
         # Return the message object instead of a code.
-        if ( hasattr(msg,'key') and hasattr(msg,'value') and
-             (isinstance(msg.key,KafkaCryptoMessage) or isinstance(msg.value,KafkaCryptoMessage)) ) :
+        if (
+            hasattr(msg, "key")
+            and hasattr(msg, "value")
+            and (
+                isinstance(msg.key, KafkaCryptoMessage)
+                or isinstance(msg.value, KafkaCryptoMessage)
+            )
+        ):
             return msg
-        #get the DataFileChunk from the message value
-        try :
-            dfc = msg.value() #from a regular Kafka Consumer
-        except TypeError :
-            dfc = msg.value #from KafkaCrypto
-        #make sure the chunk is of the right type
-        if not isinstance(dfc,DataFileChunk) :
-            errmsg = f'ERROR: expected DataFileChunk messages but received a message of type {type(dfc)}!'
-            self.logger.error(errmsg,exc_type=ValueError)
-        #make sure the chunk doesn't already have a rootdir set
-        if dfc.rootdir is not None :
-            warnmsg = f'WARNING: message with key {dfc.message_key} has rootdir={dfc.rootdir} '
-            warnmsg+= '(should be None as it was just consumed)! Will ignore this message and continue.'
+        # get the DataFileChunk from the message value
+        try:
+            dfc = msg.value()  # from a regular Kafka Consumer
+        except TypeError:
+            dfc = msg.value  # from KafkaCrypto
+        # make sure the chunk is of the right type
+        if not isinstance(dfc, DataFileChunk):
+            errmsg = f"ERROR: expected DataFileChunk messages but received a {type(dfc)} message!"
+            self.logger.error(errmsg, exc_type=ValueError)
+        # make sure the chunk doesn't already have a rootdir set
+        if dfc.rootdir is not None:
+            warnmsg = (
+                f"WARNING: message with key {dfc.message_key} has rootdir={dfc.rootdir} "
+                "(should be None as it was just consumed)! "
+                "Will ignore this message and continue."
+            )
             self.logger.warning(warnmsg)
-        #set the chunk's root directory
+        # set the chunk's root directory
         dfc.rootdir = rootdir_to_set
-        #add the chunk's data to the file that's being reconstructed
-        with lock :
-            if dfc.relative_filepath not in self.files_in_progress_by_path :
-                self.files_in_progress_by_path[dfc.relative_filepath] = self.datafile_type(dfc.filepath,
-                                                                                           logger=self.logger,
-                                                                                           **self.other_datafile_kwargs)
+        # add the chunk's data to the file that's being reconstructed
+        with lock:
+            if dfc.relative_filepath not in self.files_in_progress_by_path:
+                new_datafile = self.datafile_type(
+                    dfc.filepath,
+                    logger=self.logger,
+                    **self.other_datafile_kwargs,
+                )
+                self.files_in_progress_by_path[dfc.relative_filepath] = new_datafile
                 self.locks_by_fp[dfc.relative_filepath] = Lock()
-        retval = self.files_in_progress_by_path[dfc.relative_filepath].add_chunk(dfc,
-                                                                                self.locks_by_fp[dfc.relative_filepath])
-        #If the file is just in progress, return True
-        if retval in (DATA_FILE_HANDLING_CONST.FILE_IN_PROGRESS,
-                            DATA_FILE_HANDLING_CONST.CHUNK_ALREADY_WRITTEN_CODE) :
+        retval = self.files_in_progress_by_path[dfc.relative_filepath].add_chunk(
+            dfc,
+            self.locks_by_fp[dfc.relative_filepath],
+        )
+        # If the file is just in progress, return True
+        if retval in (
+            DATA_FILE_HANDLING_CONST.FILE_IN_PROGRESS,
+            DATA_FILE_HANDLING_CONST.CHUNK_ALREADY_WRITTEN_CODE,
+        ):
             return True
-        #otherwise just return the code from add_chunk
+        # otherwise just return the code from add_chunk
         return retval
 
-class DataFileChunkProcessor(DataFileChunkHandler,ControlledMessageProcessor) :
+
+class DataFileChunkProcessor(DataFileChunkHandler, ControlledMessageProcessor):
     """
     Combine template code in DataFileChunkHandler with specifics of processing messages
     """
 
     @property
-    def progress_msg(self) :
+    def progress_msg(self):
         """
         A string message describing the files that have had some chunks read
         """
-        progress_msg = 'The following files have been recognized so far:\n'
-        for datafile in self.files_in_progress_by_path.values() :
-            progress_msg+=f'\t{datafile.relative_filepath} (in progress)\n'
-        for fp in self.completely_processed_filepaths :
-            progress_msg+=f'\t{fp} (completed)\n'
+        progress_msg = (
+            f"Files recognized so far (up to {self.N_RECENT_FILES} most recent "
+            "completed files shown):\n\t"
+        )
+        progress_msg += "\n\t".join(
+            [
+                f"{df.relative_filepath} (in progress)"
+                for df in self.files_in_progress_by_path.values()
+            ]
+        )
+        if len(self.files_in_progress_by_path) > 0:
+            progress_msg += "\n\t"
+        progress_msg += "\n\t".join(
+            [f"{fp} (completed)" for fp in self.recent_processed_filepaths]
+        )
         return progress_msg
 
-class DataFileChunkReproducer(DataFileChunkHandler,ControlledMessageReproducer) :
+
+class DataFileChunkReproducer(DataFileChunkHandler, ControlledMessageReproducer):
     """
     Combine template code in DataFileChunkHandler with processing messages from one topic
     and producing others to a different topic
     """
 
     @property
-    def progress_msg(self) :
+    def progress_msg(self):
         """
         A string message describing the files that have had some chunks read
         """
-        progress_msg = 'The following files have been recognized so far:\n'
-        for datafile in self.files_in_progress_by_path.values() :
-            if datafile.relative_filepath not in self.completely_processed_filepaths :
-                progress_msg+=f'\t{datafile.relative_filepath} (in progress)\n'
-        for fp in self.completely_processed_filepaths :
-            if fp not in self.results_produced_filepaths :
-                progress_msg+=f'\t{fp} (fully read from topic)\n'
-        for fp in self.results_produced_filepaths :
-            progress_msg+=f'\t{fp} (processing results produced)\n'
+        progress_msg = (
+            f"Files recognized so far (up to {self.N_RECENT_FILES} most recent "
+            "completed files shown):\n\t"
+        )
+        progress_msg = "The following files have been recognized so far:\n"
+        for datafile in self.files_in_progress_by_path.values():
+            if datafile.relative_filepath not in self.recent_processed_filepaths:
+                progress_msg += f"\t{datafile.relative_filepath} (in progress)\n"
+        for fp in self.recent_processed_filepaths:
+            if fp not in self.recent_results_produced:
+                progress_msg += f"\t{fp} (fully read from topic)\n"
+        for fp in self.recent_results_produced:
+            progress_msg += f"\t{fp} (processing results produced)\n"
         return progress_msg
 
-    def __init__(self,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
-        self.results_produced_filepaths = []
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.recent_results_produced = []
+        self.n_results_produced_files = 0
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_download_directory.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_download_directory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,180 +1,259 @@
 """
 Write DataFileChunks directly to disk as they are consumed from topics.
 Preserve subdirectory structure if applicable
 """
 
-#imports
+# imports
 import datetime, warnings
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto.message import KafkaCryptoMessage
 from ...utilities import Runnable
 from ..config import DATA_FILE_HANDLING_CONST, RUN_OPT_CONST
 from ..utilities import get_encrypted_message_key_and_value_filenames
 from .. import DataFileDirectory, DownloadDataFileToDisk
 from .data_file_chunk_handlers import DataFileChunkProcessor
 
-class DataFileDownloadDirectory(DataFileDirectory,DataFileChunkProcessor,Runnable) :
+
+class DataFileDownloadDirectory(DataFileDirectory, DataFileChunkProcessor, Runnable):
     """
     Class representing a directory into which files are being reconstructed.
 
     :param dirpath: Path to the directory where reconstructed files should be saved
     :type dirpath: :class:`pathlib.Path`
-    :param config_path: Path to the config file to use in defining the Broker connection and Consumers
+    :param config_path: Path to the config file to use in defining the Broker connection
+        and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
     :param datafile_type: the type of data file that recognized files should be reconstructed as
         (must be a subclass of :class:`~.data_file_io.DownloadDataFileToDisk`)
     :type datafile_type: :class:`~.data_file_io.DownloadDataFileToDisk`, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
         :class:`~.data_file_io.DownloadDataFileToDisk`
     """
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,dirpath,config_path,topic_name,datafile_type=DownloadDataFileToDisk,**kwargs) :
+    def __init__(
+        self,
+        dirpath,
+        config_path,
+        topic_name,
+        datafile_type=DownloadDataFileToDisk,
+        **kwargs,
+    ):
         """
-        datafile_type = the type of datafile that the consumed messages should be assumed to represent
+        datafile_type = the type of datafile that the consumed messages are from
         In this class datafile_type should be something that extends DownloadDataFileToDisk
         """
-        super().__init__(dirpath,config_path,topic_name,datafile_type=datafile_type,**kwargs)
-        if not issubclass(self.datafile_type,DownloadDataFileToDisk) :
-            errmsg = 'ERROR: DataFileDownloadDirectory requires a datafile_type that is a subclass of '
-            errmsg+= f'DownloadDataFileToDisk but {self.datafile_type} was given!'
-            self.logger.error(errmsg,exc_type=ValueError)
-        self.__encrypted_messages_subdir = self.dirpath/'ENCRYPTED_MESSAGES'
+        super().__init__(
+            dirpath, config_path, topic_name, datafile_type=datafile_type, **kwargs
+        )
+        if not issubclass(self.datafile_type, DownloadDataFileToDisk):
+            errmsg = (
+                "ERROR: DataFileDownloadDirectory requires a datafile_type that is a "
+                f"subclass of DownloadDataFileToDisk but {self.datafile_type} was given!"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        self.__encrypted_messages_subdir = self.dirpath / "ENCRYPTED_MESSAGES"
 
-    def reconstruct(self) :
+    def reconstruct(self):
         """
-        Consumes messages and writes their data to disk using several parallel threads to reconstruct the files
-        to which they correspond. Runs until the user inputs a command to shut it down.
+        Consumes messages and writes their data to disk using several parallel threads
+        to reconstruct the files to which they correspond.
+        Runs until the user inputs a command to shut it down.
 
         :return: the total number of messages consumed
         :rtype: int
         :return: the total number of message processed (written to disk)
         :rtype: int
-        :return: the number of files whose reconstruction was completed during the run
+        :return: the total number of completely reconstructed files
         :rtype: int
+        :return: paths of up to 50 most recently reconstructed files
+        :rtype: list
         """
-        msg = f'Will reconstruct files from messages in the {self.topic_name} topic using {self.n_threads} '
-        msg+= f'thread{"s" if self.n_threads!=1 else ""}'
+        msg = (
+            f"Will reconstruct files from messages in the {self.topic_name} topic using "
+            f'{self.n_threads} thread{"s" if self.n_threads!=1 else ""}'
+        )
         self.logger.info(msg)
         self.run()
-        return self.n_msgs_read, self.n_msgs_processed, self.completely_processed_filepaths
+        return (
+            self.n_msgs_read,
+            self.n_msgs_processed,
+            self.n_processed_files,
+            self.recent_processed_filepaths,
+        )
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
     def _process_message(self, lock, msg, rootdir_to_set=None):
-        retval = super()._process_message(lock,msg,self.dirpath if rootdir_to_set is None else rootdir_to_set)
-        #if the message was returned because it couldn't be decrypted, write it to the encrypted messages directory
-        if ( hasattr(retval,'key') and hasattr(retval,'value') and
-             (isinstance(retval.key,KafkaCryptoMessage) or isinstance(retval.value,KafkaCryptoMessage)) ) :
-            if not self.__encrypted_messages_subdir.is_dir() :
+        retval = super()._process_message(
+            lock, msg, self.dirpath if rootdir_to_set is None else rootdir_to_set
+        )
+        # if the message was returned because it couldn't be decrypted,
+        # write it to the encrypted messages directory
+        if (
+            hasattr(retval, "key")
+            and hasattr(retval, "value")
+            and (
+                isinstance(retval.key, KafkaCryptoMessage)
+                or isinstance(retval.value, KafkaCryptoMessage)
+            )
+        ):
+            if not self.__encrypted_messages_subdir.is_dir():
                 self.__encrypted_messages_subdir.mkdir(parents=True)
-            key_fn, value_fn = get_encrypted_message_key_and_value_filenames(retval,self.topic_name)
-            key_fp = self.__encrypted_messages_subdir/key_fn
-            value_fp = self.__encrypted_messages_subdir/value_fn
-            warnmsg = 'WARNING: encountered a message that failed to be decrypted. Key bytes will be written to '
-            warnmsg+= f'{key_fp.relative_to(self.dirpath)} and value bytes will be written to '
-            warnmsg+= f'{value_fp.relative_to(self.dirpath)}'
+            key_fn, value_fn = get_encrypted_message_key_and_value_filenames(
+                retval, self.topic_name
+            )
+            key_fp = self.__encrypted_messages_subdir / key_fn
+            value_fp = self.__encrypted_messages_subdir / value_fn
+            warnmsg = (
+                "WARNING: encountered a message that failed to be decrypted. Key bytes "
+                f"will be written to {key_fp.relative_to(self.dirpath)} and value bytes "
+                f"will be written to {value_fp.relative_to(self.dirpath)}"
+            )
             self.logger.warning(warnmsg)
-            with open(key_fp,'wb') as fp :
+            with open(key_fp, "wb") as fp:
                 fp.write(bytes(retval.key))
-            with open(value_fp,'wb') as fp :
+            with open(value_fp, "wb") as fp:
                 fp.write(bytes(retval.value))
-            return False #because the message wasn't processed successfully
-        if retval is True :
+            return False  # because the message wasn't processed successfully
+        if retval is True:
             return retval
-        #get the DataFileChunk from the message value
-        try :
-            dfc = msg.value() #from a regular Kafka Consumer
-        except TypeError :
-            dfc = msg.value #from KafkaCrypto
-        #If the file was successfully reconstructed, return True
-        if retval==DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE :
-            self.logger.debug(f'File {dfc.relative_filepath} successfully reconstructed from stream')
-            self.completely_processed_filepaths.append(dfc.relative_filepath)
-            with lock :
+        # get the DataFileChunk from the message value
+        try:
+            dfc = msg.value()  # from a regular Kafka Consumer
+        except TypeError:
+            dfc = msg.value  # from KafkaCrypto
+        # If the file was successfully reconstructed, return True
+        if retval == DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE:
+            self.logger.debug(
+                f"File {dfc.relative_filepath} successfully reconstructed from stream"
+            )
+            with lock:
+                self.recent_processed_filepaths.append(dfc.relative_filepath)
+                while len(self.recent_processed_filepaths) > self.N_RECENT_FILES:
+                    _ = self.recent_processed_filepaths.pop(0)
+                self.n_processed_files += 1
                 del self.files_in_progress_by_path[dfc.relative_filepath]
                 del self.locks_by_fp[dfc.relative_filepath]
             return True
-        #If the file hash was mismatched after reconstruction, return False
-        if retval==DATA_FILE_HANDLING_CONST.FILE_HASH_MISMATCH_CODE :
-            warnmsg = f'WARNING: hashes for file {dfc.relative_filepath} not matched after reconstruction! '
-            warnmsg+= 'All data have been written to disk, but not as they were uploaded.'
+        # If the file hash was mismatched after reconstruction, return False
+        if retval == DATA_FILE_HANDLING_CONST.FILE_HASH_MISMATCH_CODE:
+            warnmsg = (
+                f"WARNING: hashes for file {dfc.relative_filepath} not matched after "
+                "reconstruction! All data have been written to disk, but not as they "
+                "were uploaded."
+            )
             self.logger.warning(warnmsg)
-            with lock :
+            with lock:
                 del self.files_in_progress_by_path[dfc.relative_filepath]
                 del self.locks_by_fp[dfc.relative_filepath]
             return False
-        #if this is reached the return code was unrecognized
-        self.logger.error(f'ERROR: unrecognized add_chunk return value ({retval})!',exc_type=NotImplementedError)
+        # if this is reached the return code was unrecognized
+        self.logger.error(
+            f"ERROR: unrecognized add_chunk return value ({retval})!",
+            exc_type=NotImplementedError,
+        )
         return False
 
-    def _on_check(self) :
-        msg = f'{self.n_msgs_read} messages read, {self.n_msgs_processed} messages processed, '
-        msg+= f'{len(self.completely_processed_filepaths)} files completely reconstructed so far'
+    def _on_check(self):
+        msg = (
+            f"{self.n_msgs_read} messages read, {self.n_msgs_processed} messages "
+            f"processed, {self.n_processed_files} files completely reconstructed so far"
+        )
         self.logger.info(msg)
-        if len(self.files_in_progress_by_path)>0 or len(self.completely_processed_filepaths)>0 :
+        if (
+            len(self.files_in_progress_by_path) > 0
+            or len(self.recent_processed_filepaths) > 0
+        ):
             self.logger.debug(self.progress_msg)
 
     #################### CLASS METHODS ####################
 
     @classmethod
-    def get_command_line_arguments(cls) :
-        superargs,superkwargs = super().get_command_line_arguments()
-        args = [*superargs,'output_dir','config','topic_name','update_seconds','consumer_group_id']
-        kwargs = {**superkwargs,'n_threads':RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
-        return args,kwargs
+    def get_command_line_arguments(cls):
+        superargs, superkwargs = super().get_command_line_arguments()
+        args = [
+            *superargs,
+            "output_dir",
+            "config",
+            "topic_name",
+            "update_seconds",
+            "consumer_group_id",
+        ]
+        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
+        return args, kwargs
 
     @classmethod
-    def run_from_command_line(cls,args=None) :
+    def run_from_command_line(cls, args=None):
         """
         Run a :class:`~DataFileDownloadDirectory` directly from the command line
 
         Calls :func:`~reconstruct` on a :class:`~DataFileDownloadDirectory` defined by
         command line (or given) arguments
 
-        :param args: the list of arguments to send to the parser instead of getting them from sys.argv
+        :param args: the list of arguments to send to the parser instead of getting them
+            from sys.argv
         :type args: list, optional
         """
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
-        #make the download directory
-        reconstructor_directory = cls(args.output_dir,args.config,args.topic_name,
-                                      n_threads=args.n_threads,
-                                      consumer_group_id=args.consumer_group_id,
-                                      update_secs=args.update_seconds,
-                                      streamlevel=args.logger_stream_level,filelevel=args.logger_file_level,
-                                     )
-        #start the reconstructor running
+        # make the download directory
+        reconstructor_directory = cls(
+            args.output_dir,
+            args.config,
+            args.topic_name,
+            n_threads=args.n_threads,
+            consumer_group_id=args.consumer_group_id,
+            update_secs=args.update_seconds,
+            streamlevel=args.logger_stream_level,
+            filelevel=args.logger_file_level,
+        )
+        # start the reconstructor running
         run_start = datetime.datetime.now()
-        reconstructor_directory.logger.info(f'Listening for files to reconstruct in {args.output_dir}')
-        n_read,n_processed,complete_filepaths = reconstructor_directory.reconstruct()
+        reconstructor_directory.logger.info(
+            f"Listening for files to reconstruct in {args.output_dir}"
+        )
+        (
+            n_read,
+            n_processed,
+            n_complete_files,
+            complete_filepaths,
+        ) = reconstructor_directory.reconstruct()
         reconstructor_directory.close()
         run_stop = datetime.datetime.now()
-        #shut down when that function returns
-        reconstructor_directory.logger.info(f'File reconstructor writing to {args.output_dir} shut down')
-        msg = f'{n_read} total messages were consumed'
-        if len(complete_filepaths)>0 :
-            msg+=f', {n_processed} messages were successfully processed,'
-            msg+=f' and the following {len(complete_filepaths)} file'
-            msg+=' was' if len(complete_filepaths)==1 else 's were'
-            msg+=' successfully reconstructed'
-        else :
-            msg+=f' and {n_processed} messages were successfully processed'
-        msg+=f' from {run_start} to {run_stop}'
-        for fn in complete_filepaths :
-            msg+=f'\n\t{fn}'
+        # shut down when that function returns
+        reconstructor_directory.logger.info(
+            f"File reconstructor writing to {args.output_dir} shut down"
+        )
+        msg = f"{n_read} total messages were consumed"
+        if len(complete_filepaths) > 0:
+            msg += (
+                f", {n_processed} messages were successfully processed, and "
+                f'{n_complete_files} file{" was" if n_complete_files==1 else "s were"} '
+                "successfully reconstructed"
+            )
+        else:
+            msg += f" and {n_processed} messages were successfully processed"
+        msg += (
+            f" from {run_start} to {run_stop}\n"
+            f"Most recent completed files (up to {cls.N_RECENT_FILES}):"
+        )
+        msg += "\n\t".join(complete_filepaths)
         reconstructor_directory.logger.info(msg)
 
-def main(args=None) :
+
+def main(args=None):
     """
     Main method to run from command line
     """
     DataFileDownloadDirectory.run_from_command_line(args)
 
-if __name__=='__main__' :
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_stream_handler.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,122 +1,158 @@
-"""Base class for consuming file chunks into memory and then triggering some action when whole files are available"""
+"""
+    Base class for consuming file chunks into memory and then triggering some action 
+    when whole files are available
+"""
 
-#imports
+# imports
 import pathlib, warnings
 from abc import ABC
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto.message import KafkaCryptoMessage
 from ...utilities.misc import populated_kwargs
 from ...utilities import Runnable
 from ..config import DATA_FILE_HANDLING_CONST
 from ..utilities import get_encrypted_message_timestamp_string
 from ..entity.download_data_file import DownloadDataFileToMemory
 from .data_file_chunk_handlers import DataFileChunkHandler
 
-class DataFileStreamHandler(DataFileChunkHandler,Runnable,ABC) :
+
+class DataFileStreamHandler(DataFileChunkHandler, Runnable, ABC):
     """
-    Generic base class for consuming file chunks into memory and then doing something once entire files are available
+    Generic base class for consuming file chunks into memory and then doing something
+    once entire files are available
     """
 
-    def __init__(self,*args,output_dir=None,datafile_type=DownloadDataFileToMemory,**kwargs) :
+    def __init__(
+        self, *args, output_dir=None, datafile_type=DownloadDataFileToMemory, **kwargs
+    ):
         """
         Constructor method
         """
-        #make sure the directory for the output is set
-        self._output_dir = self._get_auto_output_dir() if output_dir is None else output_dir
-        if not self._output_dir.is_dir() :
+        # make sure the directory for the output is set
+        self._output_dir = (
+            self._get_auto_output_dir() if output_dir is None else output_dir
+        )
+        if not self._output_dir.is_dir():
             self._output_dir.mkdir(parents=True)
-        kwargs = populated_kwargs(kwargs,{'logger_file':self._output_dir})
-        super().__init__(*args,datafile_type=datafile_type,**kwargs)
-        self.logger.info(f'Log files and output will be in {self._output_dir}')
-        if not issubclass(datafile_type,DownloadDataFileToMemory) :
-            errmsg = f'ERROR: {self.__class__.__name__} requires a datafile_type that is a subclass of '
-            errmsg+= f'DownloadDataFileToMemory but {datafile_type} was given!'
-            self.logger.error(errmsg,exc_type=ValueError)
-        self.file_registry = None # needs to be set in subclasses
+        kwargs = populated_kwargs(kwargs, {"logger_file": self._output_dir})
+        super().__init__(*args, datafile_type=datafile_type, **kwargs)
+        self.logger.info(f"Log files and output will be in {self._output_dir}")
+        if not issubclass(datafile_type, DownloadDataFileToMemory):
+            errmsg = (
+                f"ERROR: {self.__class__.__name__} requires a datafile_type that is a "
+                f"subclass of DownloadDataFileToMemory but {datafile_type} was given!"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        self.file_registry = None  # needs to be set in subclasses
 
-    def _process_message(self,lock,msg,rootdir_to_set=None):
+    def _process_message(self, lock, msg, rootdir_to_set=None):
         """
         Parent class message processing function to check for:
             undecryptable messages (returns False)
             files where reconstruction is just in progress (returns True)
             files with mismatched hashes (returns False)
         Child classes should call super()._process_message() and check the return value
         to find successfully-reconstructed files for further handling.
         """
-        retval = super()._process_message(lock, msg, self._output_dir if rootdir_to_set is None else rootdir_to_set)
-        #if the message was returned because it couldn't be decrypted, write it to the encrypted messages directory
-        if ( hasattr(retval,'key') and hasattr(retval,'value') and
-             (isinstance(retval.key,KafkaCryptoMessage) or isinstance(retval.value,KafkaCryptoMessage)) ) :
+        retval = super()._process_message(
+            lock, msg, self._output_dir if rootdir_to_set is None else rootdir_to_set
+        )
+        # if the message was returned because it couldn't be decrypted,
+        # write it to the encrypted messages directory
+        if (
+            hasattr(retval, "key")
+            and hasattr(retval, "value")
+            and (
+                isinstance(retval.key, KafkaCryptoMessage)
+                or isinstance(retval.value, KafkaCryptoMessage)
+            )
+        ):
             self._undecryptable_message_callback(retval)
             return False
-        #get the DataFileChunk from the message value
-        try :
-            dfc = msg.value() #from a regular Kafka Consumer
-        except TypeError :
-            dfc = msg.value #from KafkaCrypto
-        #if the file is just in progress
-        if retval is True :
-            with lock :
+        # get the DataFileChunk from the message value
+        try:
+            dfc = msg.value()  # from a regular Kafka Consumer
+        except TypeError:
+            dfc = msg.value  # from KafkaCrypto
+        # if the file is just in progress
+        if retval is True:
+            with lock:
                 self.file_registry.register_file_in_progress(dfc)
             return retval
-        #if the file hashes didn't match, invoke the callback and return False
-        if retval==DATA_FILE_HANDLING_CONST.FILE_HASH_MISMATCH_CODE :
-            warnmsg = f'WARNING: hashes for file {dfc.filename} not matched after being fully read! '
-            warnmsg+= 'The messages for this file will need to be consumed again if the file is to be processed! '
-            warnmsg+= 'Please rerun with the same consumer ID to try again.'
+        # if the file hashes didn't match, invoke the callback and return False
+        if retval == DATA_FILE_HANDLING_CONST.FILE_HASH_MISMATCH_CODE:
+            warnmsg = (
+                f"WARNING: hashes for file {dfc.filename} not matched after being read! "
+                "The messages for this file will need to be consumed again if the file "
+                "is to be processed! Please rerun with the same consumer ID to try again."
+            )
             self.logger.warning(warnmsg)
-            with lock :
+            with lock:
                 self.file_registry.register_file_mismatched_hash(dfc)
-            self._mismatched_hash_callback(self.files_in_progress_by_path[dfc.filepath],lock)
-            with lock :
+            self._mismatched_hash_callback(
+                self.files_in_progress_by_path[dfc.filepath], lock
+            )
+            with lock:
                 del self.files_in_progress_by_path[dfc.relative_filepath]
                 del self.locks_by_fp[dfc.relative_filepath]
             return False
-        if retval!=DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE :
-            self.logger.error(f'ERROR: unrecognized add_chunk return value: {retval}',exc_type=NotImplementedError)
+        if retval != DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE:
+            self.logger.error(
+                f"ERROR: unrecognized add_chunk return value: {retval}",
+                exc_type=NotImplementedError,
+            )
             return False
         return retval
 
-    def _undecryptable_message_callback(self,msg) :
+    def _undecryptable_message_callback(self, msg):
         """
         This function is called when a message that could not be decrypted is found.
-        If this function is called it is likely that the file the chunk is coming from won't be able to be processed.
+        If this function is called it is likely that the file the chunk is coming from
+        won't be able to be processed.
 
         In the base class, this logs a warning.
 
-        :param msg: the :class:`kafkacrypto.Message` object with undecrypted :class:`kafkacrypto.KafkaCryptoMessages`
-            for its key and/or value
+        :param msg: the :class:`kafkacrypto.Message` object with undecrypted
+            :class:`kafkacrypto.KafkaCryptoMessage`s for its key and/or value
         :type msg: :class:`kafkacrypto.Message`
         """
         timestamp_string = get_encrypted_message_timestamp_string(msg)
-        warnmsg = f'WARNING: encountered a message that failed to be decrypted (timestamp = {timestamp_string}). '
-        warnmsg+= 'This message will be skipped, and the file it came from cannot be processed from the stream '
-        warnmsg+= 'until it is decryptable. Please rerun with a new Consumer ID to consume these messages again.'
+        warnmsg = (
+            "WARNING: encountered a message that failed to be decrypted (timestamp = "
+            f"{timestamp_string}). This message will be skipped, and the file it came "
+            "from cannot be processed from the stream until it is decryptable. Please "
+            "rerun with a new Consumer ID to consume these messages again."
+        )
         self.logger.warning(warnmsg)
 
-    def _mismatched_hash_callback(self,datafile,lock) :
+    def _mismatched_hash_callback(self, datafile, lock):
         """
-        Called when a file reconstructed in memory doesn't match the hash of its contents originally on disk,
-        providing an opportunity for fallback/backup processing in the case of failure.
+        Called when a file reconstructed in memory doesn't match the hash of its contents
+        originally on disk, providing an opportunity for fallback/backup processing
+        in the case of failure.
 
         Does nothing in the base class.
 
         :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object that has received
             all of its messages from the topic
         :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
-        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one instance
-            of :func:`~_mismatched_hash_callback` is running at once
+        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one
+            instance of :func:`~_mismatched_hash_callback` is running at once
         :type lock: :class:`threading.Lock`
         """
 
     @classmethod
-    def _get_auto_output_dir(cls) :
-        return pathlib.Path()/f'{cls.__name__}_output'
+    def _get_auto_output_dir(cls):
+        return pathlib.Path() / f"{cls.__name__}_output"
 
     @classmethod
     def get_command_line_arguments(cls):
         superargs, superkwargs = super().get_command_line_arguments()
-        args = [*superargs,'config','consumer_group_id','update_seconds']
-        kwargs = {**superkwargs,'optional_output_dir': cls._get_auto_output_dir(),}
+        args = [*superargs, "config", "consumer_group_id", "update_seconds"]
+        kwargs = {
+            **superkwargs,
+            "optional_output_dir": cls._get_auto_output_dir(),
+        }
         return args, kwargs
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_stream_processor.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,218 +1,265 @@
 """A DataFileStreamHandler that triggers some arbitrary local code when full files are available"""
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 from ...utilities.misc import populated_kwargs
 from ..config import RUN_OPT_CONST, DATA_FILE_HANDLING_CONST
 from .data_file_chunk_handlers import DataFileChunkProcessor
 from .data_file_stream_handler import DataFileStreamHandler
 from .file_registry.stream_handler_registries import StreamProcessorRegistry
 
-class DataFileStreamProcessor(DataFileStreamHandler,DataFileChunkProcessor,ABC) :
+
+class DataFileStreamProcessor(DataFileStreamHandler, DataFileChunkProcessor, ABC):
     """
-    A class to consume :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` messages into memory
-    and perform some operation(s) when entire files are available.
+    A class to consume :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` messages
+    into memory and perform some operation(s) when entire files are available.
     This is a base class that cannot be instantiated on its own.
 
-    :param config_path: Path to the config file to use in defining the Broker connection and Consumers
+    :param config_path: Path to the config file to use in defining the Broker connection
+        and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
-    :param output_dir: Path to the directory where the log and csv registry files should be kept (if None a default
-        will be created in the current directory)
+    :param output_dir: Path to the directory where the log and csv registry files should be kept
+        (if None a default will be created in the current directory)
     :type output_dir: :class:`pathlib.Path`, optional
     :param datafile_type: the type of data file that recognized files should be reconstructed as
         (must be a subclass of :class:`~.data_file_io.DownloadDataFileToMemory`)
     :type datafile_type: :class:`~.data_file_io.DownloadDataFileToMemory`, optional
     :param n_threads: the number of threads/consumers to run
     :type n_threads: int, optional
     :param consumer_group_id: the group ID under which each consumer should be created
     :type consumer_group_id: str, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
         :class:`~.data_file_io.DownloadDataFileToMemory`
     """
 
-    LOG_SUBDIR_NAME = 'LOGS'
+    LOG_SUBDIR_NAME = "LOGS"
 
-    def __init__(self,config_file,topic_name,output_dir=None,**kwargs) :
+    def __init__(self, config_file, topic_name, output_dir=None, **kwargs):
         """
         Constructor method
         """
-        #set the output directory
-        self._output_dir = self._get_auto_output_dir() if output_dir is None else output_dir
-        #create a subdirectory for the logs
-        self.__logs_subdir = self._output_dir/self.LOG_SUBDIR_NAME
-        if not self.__logs_subdir.is_dir() :
+        # set the output directory
+        self._output_dir = (
+            self._get_auto_output_dir() if output_dir is None else output_dir
+        )
+        # create a subdirectory for the logs
+        self.__logs_subdir = self._output_dir / self.LOG_SUBDIR_NAME
+        if not self.__logs_subdir.is_dir():
             self.__logs_subdir.mkdir(parents=True)
-        #put the log file in the subdirectory
-        kwargs = populated_kwargs(kwargs,{'output_dir':self._output_dir,'logger_file':self.__logs_subdir})
-        super().__init__(config_file,topic_name,**kwargs)
+        # put the log file in the subdirectory
+        kwargs = populated_kwargs(
+            kwargs, {"output_dir": self._output_dir, "logger_file": self.__logs_subdir}
+        )
+        super().__init__(config_file, topic_name, **kwargs)
 
-    def process_files_as_read(self) :
+    def process_files_as_read(self):
         """
         Consumes messages and stores their data in memory.
-        Uses several parallel threads to consume message and calls :func:`~_process_downloaded_data_file`
-        for fully read files. Runs until the user inputs a command to shut it down.
+        Uses several parallel threads to consume message and calls
+        :func:`~_process_downloaded_data_file` for fully read files.
+        Runs until the user inputs a command to shut it down.
 
         :return: the total number of messages consumed
         :rtype: int
         :return: the total number of messages processed (registered in memory)
         :rtype: int
-        :return: the paths of files successfully processed during the run
+        :return: the number of files successfully processed during the run
+        :rtype: int
+        :return: the paths of up to 50 most recent files successfully processed during the run
         :rtype: List
         """
-        #startup message
-        msg = f'Will process files from messages in the {self.topic_name} topic using {self.n_threads} '
-        msg+= f'thread{"s" if self.n_threads>1 else ""}'
+        # startup message
+        msg = (
+            f"Will process files from messages in the {self.topic_name} topic using "
+            f'{self.n_threads} thread{"s" if self.n_threads>1 else ""}'
+        )
         self.logger.info(msg)
-        #set up the stream processor registry
-        self.file_registry = StreamProcessorRegistry(dirpath=self.__logs_subdir,
-                                                      topic_name=self.topic_name,
-                                                      consumer_group_id=self.consumer_group_id,
-                                                      logger=self.logger)
-        #if there are files that need to be re-processed, set the variables to re-read messages from those files
-        if self.file_registry.rerun_file_key_regex is not None :
-            msg = f'Consumer{"s" if self.n_threads>1 else ""} will start from the beginning of the topic to '
-            msg+= f're-read messages for {self.file_registry.n_files_to_rerun} previously-failed '
-            msg+= f'file{"s" if self.file_registry.n_files_to_rerun>1 else ""}'
+        # set up the stream processor registry
+        self.file_registry = StreamProcessorRegistry(
+            dirpath=self.__logs_subdir,
+            topic_name=self.topic_name,
+            consumer_group_id=self.consumer_group_id,
+            logger=self.logger,
+        )
+        # if there are files that need to be re-processed,
+        # set the variables to re-read messages from those files
+        if self.file_registry.rerun_file_key_regex is not None:
+            msg = (
+                f'Consumer{"s" if self.n_threads>1 else ""} will start from the beginning '
+                f"of the topic to re-read messages for {self.file_registry.n_files_to_rerun} "
+                f'previously-failed file{"s" if self.file_registry.n_files_to_rerun>1 else ""}'
+            )
             self.logger.info(msg)
-            self.restart_at_beginning=True
-            self.message_key_regex=self.file_registry.rerun_file_key_regex
-        #call the run loop
+            self.restart_at_beginning = True
+            self.message_key_regex = self.file_registry.rerun_file_key_regex
+        # call the run loop
         self.run()
-        #return the results of the processing
-        return self.n_msgs_read, self.n_msgs_processed, self.completely_processed_filepaths
+        # return the results of the processing
+        return (
+            self.n_msgs_read,
+            self.n_msgs_processed,
+            self.n_processed_files,
+            self.recent_processed_filepaths,
+        )
 
-    def _process_message(self,lock,msg,rootdir_to_set=None):
+    def _process_message(self, lock, msg, rootdir_to_set=None):
         """
-        Process a single message to add it to a file being held in memory until all messages are received.
+        Process a single message to add it to a file being held in memory until all messages
+        are received.
 
-        If the message failed to be decrypted, this method calls :func:`~_undecryptable_message_callback` and returns.
+        If the message failed to be decrypted, this method calls
+        :func:`~_undecryptable_message_callback` and returns.
 
-        If the message is the first one consumed for a particular file, or any message other than the last one needed,
-        it registers the file as 'in_progress' in the .csv file.
+        If the message is the first one consumed for a particular file, or any message other
+        than the last one needed, it registers the file as 'in_progress' in the .csv file.
 
-        If the message is the last message needed for a file and its contents match the original hash
-        of the file on disk, this method calls :func:`~_process_downloaded_data_file`.
+        If the message is the last message needed for a file and its contents match the
+        original hash of the file on disk, this method calls
+        :func:`~_process_downloaded_data_file`.
 
-        If the call to :func:`~_process_downloaded_data_file` returns None (success), this method moves the file to the
-        'successfully processed' .csv file, and returns.
+        If the call to :func:`~_process_downloaded_data_file` returns None (success),
+        this method moves the file to the 'successfully processed' .csv file, and returns.
 
-        If the call to :func:`~_process_downloaded_data_file` returns an Exception, this method calls
-        :func:`~_failed_processing_callback`, registers the file as 'failed' in the .csv file, and returns.
+        If the call to :func:`~_process_downloaded_data_file` returns an Exception,
+        this method calls :func:`~_failed_processing_callback`, registers the file as
+        'failed' in the .csv file, and returns.
 
-        If the message is the last one needed but the contents are somehow different than the original file on disk,
-        this method calls :func:`~_mismatched_hash_callback`, registers the file as 'mismatched_hash' in the .csv file,
-        and returns.
+        If the message is the last one needed but the contents are somehow different than
+        the original file on disk, this method calls :func:`~_mismatched_hash_callback`,
+        registers the file as 'mismatched_hash' in the .csv file, and returns.
 
-        :param lock: Acquiring this :class:`threading.Lock` object ensures that only one instance
-            of :func:`~_process_message` is running at once
+        :param lock: Acquiring this :class:`threading.Lock` object ensures that only one
+            instance of :func:`~_process_message` is running at once
         :type lock: :class:`threading.Lock`
-        :param msg: The received :class:`confluent_kafka.KafkaMessage` object, or an undecrypted KafkaCrypto message
+        :param msg: The received :class:`confluent_kafka.KafkaMessage` object,
+            or an undecrypted KafkaCrypto message
         :type msg: :class:`confluent_kafka.KafkaMessage` or :class:`kafkacrypto.Message`
-        :param rootdir_to_set: Path to a directory that should be set as the "root" for reconstructed data files
-            (default is the output directory)
+        :param rootdir_to_set: Path to a directory that should be set as the "root"
+            for reconstructed data files (default is the output directory)
         :type rootdir_to_set: :class:`pathlib.Path`
 
-        :return: True if processing the message was successful (file in progress or successfully processed),
-            False otherwise
+        :return: True if processing the message was successful
+            (file in progress or successfully processed), False otherwise
         :rtype: bool
         """
-        retval = super()._process_message(lock,msg,self._output_dir if rootdir_to_set is None else rootdir_to_set)
-        #if the file was in progress or had a mismatched hash, return True or False, respectively
-        if retval in (True,False) :
+        retval = super()._process_message(
+            lock, msg, self._output_dir if rootdir_to_set is None else rootdir_to_set
+        )
+        # if the file was in progress or had a mismatched hash, return True or False, respectively
+        if retval in (True, False):
             return retval
-        #get the DataFileChunk from the message value
-        try :
-            dfc = msg.value() #from a regular Kafka Consumer
-        except TypeError :
-            dfc = msg.value #from KafkaCrypto
-        #if the file has had all of its messages read successfully, send it to the processing function
-        if retval==DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE :
-            self.logger.debug(f'Processing {dfc.relative_filepath}...')
+        # get the DataFileChunk from the message value
+        try:
+            dfc = msg.value()  # from a regular Kafka Consumer
+        except TypeError:
+            dfc = msg.value  # from KafkaCrypto
+        # if the file has had all of its messages read successfully,
+        # send it to the processing function
+        if retval == DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE:
+            self.logger.debug(f"Processing {dfc.relative_filepath}...")
             processing_retval = self._process_downloaded_data_file(
-                                    self.files_in_progress_by_path[dfc.relative_filepath],
-                                    lock
-                                )
+                self.files_in_progress_by_path[dfc.relative_filepath], lock
+            )
             to_return = None
-            #if it was able to be processed
-            if processing_retval is None :
-                self.logger.debug(f'Fully-read file {dfc.relative_filepath} successfully processed')
+            # if it was able to be processed
+            if processing_retval is None:
+                self.logger.debug(
+                    f"Fully-read file {dfc.relative_filepath} successfully processed"
+                )
                 self.file_registry.register_file_successfully_processed(dfc)
-                with lock :
-                    self.completely_processed_filepaths.append(dfc.relative_filepath)
+                with lock:
+                    self.recent_processed_filepaths.append(dfc.relative_filepath)
+                    while len(self.recent_processed_filepaths) > self.N_RECENT_FILES:
+                        self.recent_processed_filepaths.pop(0)
+                    self.n_processed_files += 1
                 to_return = True
-            #warn if it wasn't processed correctly and invoke the callback
-            else :
-                if isinstance(processing_retval,Exception) :
-                    warnmsg = f'WARNING: Fully-read file {dfc.relative_filepath} was not able to be processed. '
-                    warnmsg+= 'The traceback of the Exception thrown during processing will be logged below, but not '
-                    warnmsg+= 're-raised. The messages for this file will need to be consumed again if the file is to '
-                    warnmsg+= 'be processed! Please rerun with the same consumer ID to try again.'
-                    self.logger.warning(warnmsg,exc_info=processing_retval)
-                else :
-                    warnmsg = f'Unrecognized return value from _process_downloaded_data_file: {processing_retval}'
+            # warn if it wasn't processed correctly and invoke the callback
+            else:
+                if isinstance(processing_retval, Exception):
+                    warnmsg = (
+                        f"WARNING: Fully-read file {dfc.relative_filepath} was not able "
+                        "to be processed. The traceback of the Exception thrown during "
+                        "processing will be logged below, but not re-raised. "
+                        "The messages for this file will need to be consumed again if "
+                        "the file is to be processed! Please rerun with the same "
+                        "consumer ID to try again."
+                    )
+                    self.logger.warning(warnmsg, exc_info=processing_retval)
+                else:
+                    warnmsg = (
+                        "Unrecognized return value from _process_downloaded_data_file: "
+                        f"{processing_retval}"
+                    )
                     self.logger.warning(warnmsg)
                 self.file_registry.register_file_processing_failed(dfc)
-                self._failed_processing_callback(self.files_in_progress_by_path[dfc.relative_filepath],lock)
+                self._failed_processing_callback(
+                    self.files_in_progress_by_path[dfc.relative_filepath], lock
+                )
                 to_return = False
-            #stop tracking the file
-            with lock :
+            # stop tracking the file
+            with lock:
                 del self.files_in_progress_by_path[dfc.relative_filepath]
                 del self.locks_by_fp[dfc.relative_filepath]
             return to_return
-        #otherwise the file is just in progress
+        # otherwise the file is just in progress
         return True
 
     @abstractmethod
-    def _process_downloaded_data_file(self,datafile,lock) :
+    def _process_downloaded_data_file(self, datafile, lock):
         """
-        Perform some arbitrary operation(s) on a given data file that has been fully read from the stream.
-        Can optionally lock other threads using the given lock.
+        Perform some arbitrary operation(s) on a given data file that has been fully read
+        from the stream. Can optionally lock other threads using the given lock.
 
         Not implemented in the base class.
 
-        :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object that has received
-            all of its messages from the topic
+        :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object that
+            has received all of its messages from the topic
         :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
-        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one instance
-            of :func:`~_process_downloaded_data_file` is running at once
+        :param lock: Acquiring this :class:`threading.Lock` object would ensure that
+            only one instance of :func:`~_process_downloaded_data_file` is running at once
         :type lock: :class:`threading.Lock`
 
         :return: None if processing was successful, an Exception otherwise
         """
         raise NotImplementedError
 
-    def _failed_processing_callback(self,datafile,lock) :
+    def _failed_processing_callback(self, datafile, lock):
         """
         Called when :func:`~_process_downloaded_data_file` returns an Exception,
         providing an opportunity for fallback/backup processing in the case of failure.
 
         Does nothing in the base class.
 
-        :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object that has received
-            all of its messages from the topic
+        :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object
+            that has received all of its messages from the topic
         :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
-        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one instance
-            of :func:`~_failed_processing_callback` is running at once
+        :param lock: Acquiring this :class:`threading.Lock` object would ensure that
+            only one instance of :func:`~_failed_processing_callback` is running at once
         :type lock: :class:`threading.Lock`
         """
 
-    def _on_check(self) :
-        msg = f'{self.n_msgs_read} messages read, {self.n_msgs_processed} messages processed, '
-        msg+= f'{len(self.completely_processed_filepaths)} files completely processed so far'
+    def _on_check(self):
+        msg = (
+            f"{self.n_msgs_read} messages read, {self.n_msgs_processed} messages "
+            f"processed, {self.n_processed_files} files completely processed so far"
+        )
         self.logger.info(msg)
-        if len(self.files_in_progress_by_path)>0 or len(self.completely_processed_filepaths)>0 :
+        if (
+            len(self.files_in_progress_by_path) > 0
+            or len(self.recent_processed_filepaths) > 0
+        ):
             self.logger.debug(self.progress_msg)
 
     def _on_shutdown(self):
         super()._on_shutdown()
         self.file_registry.consolidate_succeeded_files()
 
     @classmethod
     def get_command_line_arguments(cls):
-        superargs,superkwargs = super().get_command_line_arguments()
-        args = [*superargs,'topic_name']
-        kwargs = {**superkwargs,'n_threads': RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
+        superargs, superkwargs = super().get_command_line_arguments()
+        args = [*superargs, "topic_name"]
+        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
         return args, kwargs
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_stream_reproducer.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,292 +1,373 @@
 """
 A stream handler that triggers a function to compute a message on file completion.
 Produces the computed message to a different topic.
 """
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 from ..config import DATA_FILE_HANDLING_CONST
 from .data_file_chunk_handlers import DataFileChunkReproducer
 from .data_file_stream_handler import DataFileStreamHandler
 from .file_registry.stream_handler_registries import StreamReproducerRegistry
 
-class DataFileStreamReproducer(DataFileStreamHandler,DataFileChunkReproducer,ABC) :
+
+class DataFileStreamReproducer(DataFileStreamHandler, DataFileChunkReproducer, ABC):
     """
-    A class to consume :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` messages into memory,
-    compute some processing result when entire files are available, and produce that result to a different topic.
+    A class to consume :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` messages
+    into memory, compute some processing result when entire files are available,
+    and produce that result to a different topic.
 
     This is a base class that cannot be instantiated on its own.
 
-    :param config_path: Path to the config file to use in defining the Broker connection, Consumers, and Producers
+    :param config_path: Path to the config file to use in defining the Broker connection,
+        Consumers, and Producers
     :type config_path: :class:`pathlib.Path`
     :param consumer_topic_name: Name of the topic to which the Consumers should be subscribed
     :type consumer_topic_name: str
-    :param producer_topic_name: Name of the topic to which the Producer should produce the processing results
+    :param producer_topic_name: Name of the topic to which the Producer should produce
+        the processing results
     :type producer_topic_name: str
-    :param output_dir: Path to the directory where the log and csv registry files should be kept (if None a default
-        will be created in the current directory)
+    :param output_dir: Path to the directory where the log and csv registry files should be kept
+        (if None a default will be created in the current directory)
     :type output_dir: :class:`pathlib.Path`, optional
     :param datafile_type: the type of data file that recognized files should be reconstructed as
         (must be a subclass of :class:`~.data_file_io.DownloadDataFileToMemory`)
     :type datafile_type: :class:`~.data_file_io.DownloadDataFileToMemory`, optional
-    :param n_producer_threads: the number of producers to run. The total number of producer/consumer threads
-        started is `max(n_consumer_threads,n_producer_threads)`.
+    :param n_producer_threads: the number of producers to run. The total number of
+        producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_producer_threads: int, optional
-    :param n_consumer_threads: the number of consumers to run. The total number of producer/consumer threads
-        started is `max(n_consumer_threads,n_producer_threads)`.
+    :param n_consumer_threads: the number of consumers to run. The total number of
+        producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_consumer_threads: int, optional
     :param consumer_group_id: the group ID under which each consumer should be created
     :type consumer_group_id: str, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
         :class:`~.data_file_io.DownloadDataFileToMemory`
     """
 
-    def __init__(self,config_file,consumer_topic_name,producer_topic_name,**kwargs) :
+    def __init__(self, config_file, consumer_topic_name, producer_topic_name, **kwargs):
         """
         Constructor method signature duplicated above to display in Sphinx docs
         """
-        super().__init__(config_file,consumer_topic_name,producer_topic_name,**kwargs)
+        super().__init__(config_file, consumer_topic_name, producer_topic_name, **kwargs)
 
-    def produce_processing_results_for_files_as_read(self) :
+    def produce_processing_results_for_files_as_read(self):
         """
         Consumes messages in several parallel threads and stores their data in memory. Calls
         :func:`~_get_processing_result_message_for_file` for fully-read files to get their
         processing result messages. Produces processing result messages in several parallel
         threads as they're generated. Runs until the user inputs a command to shut it down.
 
         :return: the total number of messages consumed
         :rtype: int
         :return: the total number of messages processed (registered in memory)
         :rtype: int
-        :return: the paths of files successfully reconstructed from the Consumer topic during the run
-        :rtype: list
-        :return: the paths of files whose processing results were successfully produced to the Producer topic
-            during the run
+        :return: the number of files reconstructed from the topic
+        :rtype: int
+        :return: the number of files whose processing results were successfully produced
+            to the Producer topic
+        :rtype: int
+        :return: the paths of up to 50 most recent files whose processing results were
+            successfully produced to the Producer topic during the run
         :rtype: list
         """
-        #startup message
-        msg = f'Will process files from messages in the {self.consumer_topic_name} topic using '
-        msg+= f'{self.n_consumer_threads} thread{"s" if self.n_consumer_threads>1 else ""} and produce their '
-        msg+= f'processing results to the {self.producer_topic_name} topic using {self.n_producer_threads} '
-        msg+= f'thread{"s" if self.n_producer_threads>1 else ""}'
+        # startup message
+        msg = (
+            f"Will process files from messages in the {self.consumer_topic_name} topic "
+            f"using {self.n_consumer_threads} thread"
+            f'{"s" if self.n_consumer_threads>1 else ""} and produce their '
+            f"processing results to the {self.producer_topic_name} topic using "
+            f'{self.n_producer_threads} thread{"s" if self.n_producer_threads>1 else ""}'
+        )
         self.logger.info(msg)
-        #set up the stream reproducer registry
-        self.file_registry = StreamReproducerRegistry(dirpath=self._output_dir,
-                                                       consumer_topic_name=self.consumer_topic_name,
-                                                       consumer_group_id=self.consumer_group_id,
-                                                       producer_topic_name=self.producer_topic_name,
-                                                       logger=self.logger)
-        #if there are files that need to be re-processed, set the variables to re-read messages from those files
-        if self.file_registry.rerun_file_key_regex is not None :
-            msg = f'Consumer{"s" if self.n_consumer_threads>1 else ""} will start from the beginning of the topic to '
-            msg+= f're-read messages for {self.file_registry.n_files_to_rerun} previously-failed '
-            msg+= f'file{"s" if self.file_registry.n_files_to_rerun>1 else ""}'
+        # set up the stream reproducer registry
+        self.file_registry = StreamReproducerRegistry(
+            dirpath=self._output_dir,
+            consumer_topic_name=self.consumer_topic_name,
+            consumer_group_id=self.consumer_group_id,
+            producer_topic_name=self.producer_topic_name,
+            logger=self.logger,
+        )
+        # if there are files that need to be re-processed,
+        # set the variables to re-read messages from those files
+        if self.file_registry.rerun_file_key_regex is not None:
+            msg = (
+                f'Consumer{"s" if self.n_consumer_threads>1 else ""} will start from '
+                "the beginning of the topic to re-read messages for "
+                f"{self.file_registry.n_files_to_rerun} previously-failed "
+                f'file{"s" if self.file_registry.n_files_to_rerun>1 else ""}'
+            )
             self.logger.info(msg)
-            self.restart_at_beginning=True
-            self.message_key_regex=self.file_registry.rerun_file_key_regex
-        #create the arguments for each _run_worker thread
+            self.restart_at_beginning = True
+            self.message_key_regex = self.file_registry.rerun_file_key_regex
+        # create the arguments for each _run_worker thread
         run_worker_args_per_thread = []
-        for ti in range(self.n_threads) :
-            run_worker_args_per_thread.append([ti<self.n_consumer_threads,ti<self.n_producer_threads])
-        run_worker_kwargs_per_thread = {'produce_from_queue_kwargs':{'callback':self.producer_callback,'print_every':1}}
-        #call the run loop
-        self.run(args_per_thread=run_worker_args_per_thread,kwargs_per_thread=run_worker_kwargs_per_thread)
-        #return the results of the processing
-        return ( self.n_msgs_read, self.n_msgs_processed,
-                 self.completely_processed_filepaths, self.results_produced_filepaths )
-
-    def producer_callback(self,err,msg,prodid,filename,rel_filepath,n_total_chunks) :
-        """
-        A reference to this method is given as the callback for each call to :func:`confluent_kafka.Producer.produce`.
-        It is called for every message upon acknowledgement by the broker, and it uses the file registries in the
-        LOGS subdirectory to keep the information about what has and hasn't been uploaded current with what has
-        been received by the broker.
-
-        Messages associated with an error from the broker will be recomputed and added back to the queue
-        to be produced again, logging an error and registering the file as failed if the message can't be
-        computed from the datafile.
+        for ti in range(self.n_threads):
+            run_worker_args_per_thread.append(
+                [ti < self.n_consumer_threads, ti < self.n_producer_threads]
+            )
+        run_worker_kwargs_per_thread = {
+            "produce_from_queue_kwargs": {
+                "callback": self.producer_callback,
+                "print_every": 1,
+            }
+        }
+        # call the run loop
+        self.run(
+            args_per_thread=run_worker_args_per_thread,
+            kwargs_per_thread=run_worker_kwargs_per_thread,
+        )
+        # return the results of the processing
+        return (
+            self.n_msgs_read,
+            self.n_msgs_processed,
+            self.n_processed_files,
+            self.recent_processed_filepaths,
+            self.n_results_produced_files,
+            self.recent_results_produced,
+        )
+
+    def producer_callback(self, err, msg, prodid, filename, rel_filepath, n_total_chunks):
+        """
+        A reference to this method is given as the callback for each call to
+        :func:`confluent_kafka.Producer.produce`. It is called for every message
+        upon acknowledgement by the broker, and it uses the file registries in the LOGS
+        subdirectory to keep the information about what has and hasn't been uploaded
+        current with what has been received by the broker.
+
+        Messages associated with an error from the broker will be recomputed and added
+        back to the queue to be produced again, logging an error and registering the file
+        as failed if the message can't be computed from the datafile.
 
-        Messages that are successfully produced will move their associated data files to the "results_produced"
-        csv file.
+        Messages that are successfully produced will move their associated data files
+        to the "results_produced" csv file.
 
         :param err: The error object for the message
         :type err: :class:`confluent_kafka.KafkaError`
         :param msg: The message object
         :type msg: :class:`confluent_kafka.Message`
-        :param prodid: The ID of the producer that produced the message (hex(id(producer)) in memory)
+        :param prodid: The ID of the producer that produced the message
+            (hex(id(producer)) in memory)
         :type prodid: str
         :param filename: The name of the file that was used to create this processing result message
         :type filename: str
-        :param rel_filepath: The path to the file that was used to create this processing result message,
-            relative to the :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`'s root directory
+        :param rel_filepath: The path to the file that was used to create this
+            processing result message, relative to the
+            :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`'s root directory
         :type rel_filepath: :class:`pathlib.Path`
-        :param n_total_chunks: The total number of chunks in the file used to create this processing result message
+        :param n_total_chunks: The total number of chunks in the file used to create this
+            processing result message
         :type n_total_chunks: int
         """
         # If no error occured, increment the counter for the number of messages produced
-        if err is None and msg.error() is None :
-            with self.lock :
-                self.n_msgs_produced+=1
+        if err is None and msg.error() is None:
+            with self.lock:
+                self.n_msgs_produced += 1
         # If any error occured, log a warning and re-enqueue the message to be produced again
-        if err is None and msg.error() is not None :
+        if err is None and msg.error() is not None:
             err = msg.error()
-        if err is not None :
-            self.file_registry.register_file_result_production_failed(filename,rel_filepath,n_total_chunks)
-            if err.fatal() :
-                warnmsg =f'WARNING: fatally failed to deliver processing result message for {rel_filepath}. '
-                warnmsg+=f'This message will be re-enqueued. Error reason: {err.str()}'
-            elif not err.retriable() :
-                warnmsg =f'WARNING: Failed to deliver processing result message for {rel_filepath} and cannot retry. '
-                warnmsg+= f'This message will be re-enqueued. Error reason: {err.str()}'
+        if err is not None:
+            self.file_registry.register_file_result_production_failed(
+                filename, rel_filepath, n_total_chunks
+            )
+            if err.fatal():
+                warnmsg = (
+                    "WARNING: fatally failed to deliver processing result message for "
+                    f"{rel_filepath}. This message will be re-enqueued. "
+                    f"Error reason: {err.str()}"
+                )
+            elif not err.retriable():
+                warnmsg = (
+                    "WARNING: Failed to deliver processing result message for "
+                    f"{rel_filepath} and cannot retry. This message will be re-enqueued. "
+                    "Error reason: {err.str()}"
+                )
             self.logger.warning(warnmsg)
             datafile = self.files_in_progress_by_path[rel_filepath]
-            new_msg = self._get_processing_result_message_for_file(datafile,self.lock)
-            if new_msg is not None :
+            new_msg = self._get_processing_result_message_for_file(datafile, self.lock)
+            if new_msg is not None:
                 self.producer_message_queue.put(new_msg)
-            else :
-                self._failed_computing_processing_result(datafile,self.lock)
-        # Otherwise, register the associated file as having its processing result successfully produced
-        else :
-            with self.lock :
-                self.file_registry.register_file_results_produced(filename,rel_filepath,n_total_chunks,prodid)
-                self.results_produced_filepaths.append(rel_filepath)
-                #stop tracking the file
+            else:
+                self._failed_computing_processing_result(datafile, self.lock)
+        # Otherwise, register the associated file as having its processing result produced
+        else:
+            with self.lock:
+                self.file_registry.register_file_results_produced(
+                    filename, rel_filepath, n_total_chunks, prodid
+                )
+                self.recent_results_produced.append(rel_filepath)
+                while len(self.recent_results_produced) > self.N_RECENT_FILES:
+                    _ = self.recent_results_produced.pop(0)
+                self.n_results_produced_files += 1
+                # stop tracking the file
                 del self.files_in_progress_by_path[rel_filepath]
                 del self.locks_by_fp[rel_filepath]
-            infomsg = f'Processing result message for {rel_filepath} has been received by the broker for '
-            infomsg+= f'the {self.producer_topic_name} topic'
-            self.logger.debug(infomsg)
-
-    def _process_message(self,lock,msg,rootdir_to_set=None):
-        """
-        Process a single message to add it to a file being held in memory until all messages are received.
-
-        If the message failed to be decrypted, this method calls :func:`~_undecryptable_message_callback` and returns.
-
-        If the message is the first one consumed for a particular file, or any message other than the last one needed,
-        it registers the file as 'in_progress' in the .csv file.
-
-        If the message is the last message needed for a file and its contents match the original hash
-        of the file on disk, this method calls :func:`~_get_processing_result_message_for_file` and enqueues
-        the result to be produced. The file is moved to the 'results_produced' .csv file when the produced
-        message is acknowledged by the broker through :func:`~producer_callback`.
-
-        If the call to :func:`~_get_processing_result_message_for_file` returns None, this method calls
-        :func:`~_failed_computing_processing_result` and returns.
-
-        If the message is the last one needed but the contents are somehow different than the original file on disk,
-        this method calls :func:`~_mismatched_hash_callback`, registers the file as 'mismatched_hash' in the .csv file,
-        and returns.
+            debugmsg = (
+                f"Processing result message for {rel_filepath} has been received by "
+                f"the broker for the {self.producer_topic_name} topic"
+            )
+            self.logger.debug(debugmsg)
+
+    def _process_message(self, lock, msg, rootdir_to_set=None):
+        """
+        Process a single message to add it to a file being held in memory
+        until all messages are received.
+
+        If the message failed to be decrypted, this method calls
+        :func:`~_undecryptable_message_callback` and returns.
+
+        If the message is the first one consumed for a particular file, or any message other
+        than the last one needed, it registers the file as 'in_progress' in the .csv file.
+
+        If the message is the last message needed for a file and its contents match the
+        original hash of the file on disk, this method calls
+        :func:`~_get_processing_result_message_for_file` and enqueues the result to be produced.
+        The file is moved to the 'results_produced' .csv file when the produced message
+        is acknowledged by the broker through :func:`~producer_callback`.
+
+        If the call to :func:`~_get_processing_result_message_for_file` returns None,
+        this method calls :func:`~_failed_computing_processing_result` and returns.
+
+        If the message is the last one needed but the contents are somehow different than the
+        original file on disk, this method calls :func:`~_mismatched_hash_callback`,
+        registers the file as 'mismatched_hash' in the .csv file, and returns.
 
         :param lock: Acquiring this :class:`threading.Lock` object ensures that only one instance
             of :func:`~_process_message` is running at once
         :type lock: :class:`threading.Lock`
-        :param msg: The received :class:`confluent_kafka.KafkaMessage` object, or an undecrypted KafkaCrypto message
+        :param msg: The received :class:`confluent_kafka.KafkaMessage` object,
+            or an undecrypted KafkaCrypto message
         :type msg: :class:`confluent_kafka.KafkaMessage` or :class:`kafkacrypto.Message`
-        :param rootdir_to_set: Path to a directory that should be set as the "root" for reconstructed data files
-            (default is the output directory)
+        :param rootdir_to_set: Path to a directory that should be set as the "root"
+            for reconstructed data files (default is the output directory)
         :type rootdir_to_set: :class:`pathlib.Path`
 
-        :return: True if processing the message was successful (file in progress or message enqueue to be produced),
-            False otherwise
+        :return: True if processing the message was successful (file in progress or
+            message enqueued to be produced), False otherwise
         :rtype: bool
         """
-        retval = super()._process_message(lock,msg,self._output_dir if rootdir_to_set is None else rootdir_to_set)
-        #if the file was in progress or had a mismatched hash, return True or False, respectively
-        if retval in (True,False) :
+        retval = super()._process_message(
+            lock, msg, self._output_dir if rootdir_to_set is None else rootdir_to_set
+        )
+        # if the file was in progress or had a mismatched hash, return True or False, respectively
+        if retval in (True, False):
             return retval
-        #get the DataFileChunk from the message value
-        try :
-            dfc = msg.value() #from a regular Kafka Consumer
-        except TypeError :
-            dfc = msg.value #from KafkaCrypto
-        #if the file has had all of its messages read successfully, try to enqueue its processing result to produce
-        if retval==DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE :
-            with lock :
-                self.completely_processed_filepaths.append(dfc.relative_filepath)
-            self.logger.debug(f'Getting message to produce for {dfc.relative_filepath}...')
+        # get the DataFileChunk from the message value
+        try:
+            dfc = msg.value()  # from a regular Kafka Consumer
+        except TypeError:
+            dfc = msg.value  # from KafkaCrypto
+        # if the file has had all of its messages read successfully,
+        # try to enqueue its processing result to produce
+        if retval == DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE:
+            with lock:
+                self.recent_processed_filepaths.append(dfc.relative_filepath)
+                while len(self.recent_processed_filepaths) > self.N_RECENT_FILES:
+                    _ = self.recent_processed_filepaths.pop(0)
+                self.n_processed_files += 1
+            self.logger.debug(
+                f"Getting message to produce for {dfc.relative_filepath}..."
+            )
             new_msg = self._get_processing_result_message_for_file(
-                        self.files_in_progress_by_path[dfc.relative_filepath],
-                        lock
-                    )
-            if new_msg is not None :
+                self.files_in_progress_by_path[dfc.relative_filepath], lock
+            )
+            if new_msg is not None:
                 self.producer_message_queue.put(new_msg)
                 return True
-            self._failed_computing_processing_result(self.files_in_progress_by_path[dfc.relative_filepath],self.lock)
+            self._failed_computing_processing_result(
+                self.files_in_progress_by_path[dfc.relative_filepath], self.lock
+            )
             return False
-        #otherwise the file is just in progress
+        # otherwise the file is just in progress
         return True
 
     @abstractmethod
-    def _get_processing_result_message_for_file(self,datafile,lock) :
+    def _get_processing_result_message_for_file(self, datafile, lock):
         """
         Given a relative :class:`~.data_file_io.DownloadDataFileToMemory`, compute and return a
         :class:`~.data_file_io.ReproducerMessage` object that should be produced as the processing
         result for the file.
 
-        This function should log an error and return None if the processing result fails to be computed.
+        This function should log an error and return None if the processing result
+        fails to be computed.
 
         Not implemented in the base class.
 
         :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object that has received
             all of its messages from the topic
         :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
-        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one instance
-            of :func:`~_get_processing_result_message_for_file` is running at once
+        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one
+            instance of :func:`~_get_processing_result_message_for_file` is running at once
         :type lock: :class:`threading.Lock`
 
         :return: message object to be produced
             (or None if computing it failed for any reason)
         :rtype: :class:`~.kafka_wrapper.Producible`
         """
         raise NotImplementedError
 
-    def _failed_computing_processing_result(self,datafile,lock) :
+    def _failed_computing_processing_result(self, datafile, lock):
         """
-        This function is called when :func:`_get_processing_result_message_for_file` returns None because a
-        processing result message could not be computed. It registers the original data file read from the
-        topic as 'failed' in the .csv file so that that file will have its messages re-consumed if the
-        program is restarted reading from the same topic with the same Consumer group ID. It then logs a
-        warning and stops tracking the file.
+        This function is called when :func:`_get_processing_result_message_for_file` returns None
+        because a processing result message could not be computed. It registers the original data
+        file read from the topic as 'failed' in the .csv file so that that file will have its
+        messages re-consumed if the program is restarted reading from the same topic with the
+        same Consumer group ID. It then logs a warning and stops tracking the file.
 
-        :param datafile: The datafile that should have been used to compute a processing result message
+        :param datafile: The datafile that should have been used to compute a
+            processing result message
         :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
-        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one instance
-            of :func:`~_get_processing_result_message_for_file` is running at once
+        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only
+            one instance of :func:`~_get_processing_result_message_for_file` is running at once
         :type lock: :class:`threading.Lock`
         """
-        #register the file in the registry as computing result failed
-        with lock :
-            self.file_registry.register_file_computing_result_failed(datafile.filename,
-                                                                      datafile.filepath.relative_to(self._output_dir),
-                                                                      datafile.n_total_chunks)
-        #log the warning
-        warnmsg = f'WARNING: Failed to compute the message to produce from {datafile.filepath}. Messages for this file '
-        warnmsg+= 'will need to be re-consumed to try again. Check logs above for specific error messages.'
+        # register the file in the registry as computing result failed
+        with lock:
+            self.file_registry.register_file_computing_result_failed(
+                datafile.filename,
+                datafile.filepath.relative_to(self._output_dir),
+                datafile.n_total_chunks,
+            )
+        # log the warning
+        warnmsg = (
+            f"WARNING: Failed to compute the message to produce from {datafile.filepath}. "
+            "Messages for this file will need to be re-consumed to try again. "
+            "Check logs above for specific error messages."
+        )
         self.logger.warning(warnmsg)
-        #stop tracking the file
-        with self.lock :
+        # stop tracking the file
+        with self.lock:
             del self.files_in_progress_by_path[datafile.relative_filepath]
             del self.locks_by_fp[datafile.relative_filepath]
 
-    def _on_check(self) :
-        msg = f'{self.n_msgs_read} messages read, {self.n_msgs_processed} messages processed, '
-        msg+= f'{len(self.completely_processed_filepaths)} files completely reconstructed, and '
-        msg+= f'{len(self.results_produced_filepaths)} processing result messages produced so far'
+    def _on_check(self):
+        msg = (
+            f"{self.n_msgs_read} messages read, {self.n_msgs_processed} messages processed, "
+            f"{self.n_processed_files} files completely reconstructed, and "
+            f"{self.n_results_produced_files} processing result messages produced so far"
+        )
         self.logger.info(msg)
-        if ( len(self.files_in_progress_by_path)>0 or
-             len(self.completely_processed_filepaths)>0 or
-             len(self.results_produced_filepaths)>0 ) :
+        if (
+            len(self.files_in_progress_by_path) > 0
+            or len(self.recent_processed_filepaths) > 0
+            or len(self.recent_results_produced) > 0
+        ):
             self.logger.debug(self.progress_msg)
 
     def _on_shutdown(self):
         super()._on_shutdown()
         self.file_registry.consolidate_succeeded_files()
 
     @classmethod
     def get_command_line_arguments(cls):
-        superargs,superkwargs = super().get_command_line_arguments()
-        args = [*superargs,'consumer_topic_name','producer_topic_name','n_consumer_threads','n_producer_threads']
+        superargs, superkwargs = super().get_command_line_arguments()
+        args = [
+            *superargs,
+            "consumer_topic_name",
+            "producer_topic_name",
+            "n_consumer_threads",
+            "n_producer_threads",
+        ]
         kwargs = {**superkwargs}
         return args, kwargs
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/data_file_upload_directory.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_upload_directory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,534 +1,729 @@
-"""A directory holding files that may or may not be marked for uploading. Updates when new files are added."""
+"""
+A directory holding files that may or may not be marked for uploading.
+Updates when new files are added.
+"""
 
-#imports
-import pathlib, datetime, time
+# imports
+import datetime, time
 from threading import Lock
 from queue import Queue
+from watchdog.observers import Observer
 from ...kafka_wrapper import ProducerGroup
 from ...utilities import Runnable, ControlledProcessSingleThread
 from ...utilities.misc import populated_kwargs
 from ...utilities.exception_tracking_thread import ExceptionTrackingThread
 from ..config import RUN_OPT_CONST
 from .. import DataFileDirectory
 from .file_registry.producer_file_registry import ProducerFileRegistry
 from ..entity.upload_data_file import UploadDataFile
+from ..entity.upload_directory_event_handler import UploadDirectoryEventHandler
 
-class DataFileUploadDirectory(DataFileDirectory,ControlledProcessSingleThread,ProducerGroup,Runnable) :
+
+class DataFileUploadDirectory(
+    DataFileDirectory, ControlledProcessSingleThread, ProducerGroup, Runnable
+):
     """
     Class representing a directory being watched for new files to be added.
     Files added to the directory are broken into chunks and uploaded as messages to a Kafka topic.
 
     :param dirpath: Path to the directory that should be watched for new files
     :type dirpath: :class:`pathlib.Path`
-    :param config_path: Path to the config file to use in defining the Broker connection and Producers
+    :param config_path: Path to the config file to use in defining the Broker connection
+        and Producers
     :type config_path: :class:`pathlib.Path`
     :param upload_regex: only files matching this regular expression will be uploaded
     :type upload_regex: :func:`re.compile`, optional
     :param datafile_type: the type of data file that recognized files should be uploaded as
         (must be a subclass of :class:`~UploadDataFile`)
     :type datafile_type: :class:`~UploadDataFile`, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of :class:`~UploadDataFile`
     """
 
     #################### CONSTANTS ####################
 
-    MIN_WAIT_TIME = 0.005 # starting point for how long to wait between pinging the directory looking for new files
-    MAX_WAIT_TIME = 60 # never wait more than a minute to check again for new files
-    LOG_SUBDIR_NAME = 'LOGS'
+    # starting point for how long to wait between pinging the directory looking for new files
+    MIN_WAIT_TIME = 0.005
+    # never wait more than a minute to check again for new files
+    MAX_WAIT_TIME = 60
+    # amount of time to wait for watchdog to pull events from the queue
+    WATCHDOG_OBSERVER_TIMEOUT = 0.1
+    # the max number of files to report status messages for
+    N_STATUS_MESSAGE_FILES = 50
+    # name of the logging subdirectory
+    LOG_SUBDIR_NAME = "LOGS"
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,dirpath,config_path,upload_regex=RUN_OPT_CONST.DEFAULT_UPLOAD_REGEX,
-                    datafile_type=UploadDataFile,**kwargs) :
+    def __init__(
+        self,
+        dirpath,
+        config_path,
+        upload_regex=RUN_OPT_CONST.DEFAULT_UPLOAD_REGEX,
+        datafile_type=UploadDataFile,
+        **kwargs,
+    ):
         """
         Constructor method
         """
-        #create a subdirectory for the logs
-        self.__logs_subdir = dirpath/self.LOG_SUBDIR_NAME
-        if not self.__logs_subdir.is_dir() :
+        # create a subdirectory for the logs
+        self.__logs_subdir = dirpath / self.LOG_SUBDIR_NAME
+        if not self.__logs_subdir.is_dir():
             self.__logs_subdir.mkdir(parents=True)
-        #put the log file in the subdirectory
-        kwargs = populated_kwargs(kwargs,{'logger_file':self.__logs_subdir})
-        super().__init__(dirpath,config_path,**kwargs)
-        if not issubclass(datafile_type,UploadDataFile) :
-            errmsg = 'ERROR: DataFileUploadDirectory requires a datafile_type that is a subclass of '
-            errmsg+= f'UploadDataFile but {datafile_type} was given!'
-            self.logger.error(errmsg,exc_type=ValueError)
-        self.__upload_regex = upload_regex
+        # put the log file in the subdirectory
+        kwargs = populated_kwargs(kwargs, {"logger_file": self.__logs_subdir})
+        super().__init__(dirpath, config_path, **kwargs)
+        if not issubclass(datafile_type, UploadDataFile):
+            errmsg = (
+                "ERROR: DataFileUploadDirectory requires a datafile_type that is a "
+                f"subclass of UploadDataFile but {datafile_type} was given!"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
         self.__datafile_type = datafile_type
         self.__wait_time = self.MIN_WAIT_TIME
         self.__lock = Lock()
+        self.__observer = Observer(timeout=self.WATCHDOG_OBSERVER_TIMEOUT)
+        self.__event_handler = UploadDirectoryEventHandler(
+            upload_regex=upload_regex,
+            logs_subdir=self.__logs_subdir,
+            logger=self.logger,
+        )
+        self.__active_files_by_path = {}
+        self.__status_message_files = {}
         self.__topic_name = None
         self.__chunk_size = None
         self.__file_registry = None
         self.__upload_queue = None
         self.__producers = []
         self.__upload_threads = []
 
-    def upload_files_as_added(self,topic_name,
-                              n_threads=RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
-                              chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
-                              max_queue_size=RUN_OPT_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
-                              upload_existing=False) :
+    def upload_files_as_added(
+        self,
+        topic_name,
+        n_threads=RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
+        chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
+        max_queue_size=RUN_OPT_CONST.DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES,
+        upload_existing=False,
+    ):
         """
         Watch for new files to be added to the directory.
         Chunk and produce newly added files as messages to a Kafka topic.
 
         :param topic_name: Name of the topic to produce messages to
         :type topic_name: str
         :param n_threads: The number of threads to use to produce from the shared queue
         :type n_threads: int, optional
         :param chunk_size: The size of each file chunk in bytes
         :type chunk_size: int, optional
         :param max_queue_size: The maximum size in MB of the internal upload queue
             (this is distinct from the librdkafka buffering queue)
         :type max_queue_size: int, optional
-        :param upload_existing: True if any files that already exist in the directory should be uploaded. If False
-            (the default) then only files added to the directory after startup will be enqueued to the producer
+        :param upload_existing: True if any files that already exist in the directory
+            should be uploaded. If False (the default) then only files added to the
+            directory after startup will be enqueued to the producer
         :type upload_existing: bool, optional
         """
-        #set the topic name and chunk size
+        # set the topic name and chunk size
         self.__topic_name = topic_name
         self.__chunk_size = chunk_size
-        #start up a file registry in the watched directory
-        self.__file_registry = ProducerFileRegistry(dirpath=self.__logs_subdir,topic_name=topic_name,logger=self.logger)
-        #if we're only going to upload new files, exclude what's already in the directory
-        if not upload_existing :
-            self.__find_new_files(to_upload=False)
-        #add or modify datafiles to upload based on the contents of the file registry
-        self.__startup_from_file_registry()
-        #start the upload queue and thread
-        msg = 'Will upload '
-        if not upload_existing :
-            msg+='new files added to '
-        else :
-            msg+='files in '
-        msg+=f'{self.dirpath} to the {topic_name} topic using {n_threads} threads'
+        msg = (
+            f'Will upload {"files in" if upload_existing else "new files added to"}'
+            f"{self.dirpath} to the {self.__topic_name} topic as "
+            f"{self.__chunk_size}-byte chunks using {n_threads} threads"
+        )
         self.logger.info(msg)
-        n_max_queue_items = int((1000000*max_queue_size)/self.__chunk_size)
+        # start up a file registry in the watched directory
+        self.__file_registry = ProducerFileRegistry(
+            dirpath=self.__logs_subdir, topic_name=topic_name, logger=self.logger
+        )
+        # start the upload queue
+        n_max_queue_items = int((1000000 * max_queue_size) / self.__chunk_size)
         self.__upload_queue = Queue(n_max_queue_items)
-        #start the producers and upload threads
-        for _ in range(n_threads) :
+        # start the producers and upload threads
+        for _ in range(n_threads):
             self.__producers.append(self.get_new_producer())
-            thread = ExceptionTrackingThread(target=self.__producers[-1].produce_from_queue_looped,
-                                             args=(self.__upload_queue,self.__topic_name),
-                                             kwargs={'callback': self.producer_callback},
-                    )
+            thread = ExceptionTrackingThread(
+                target=self.__producers[-1].produce_from_queue_looped,
+                args=(self.__upload_queue, self.__topic_name),
+                kwargs={"callback": self.producer_callback},
+            )
             thread.start()
             self.__upload_threads.append(thread)
-        #loop until the user inputs a command to stop
+        # if we're going to upload files that are already in the directory, scrape it now
+        if upload_existing:
+            self.__scrape_dir_for_files()
+        # add or modify datafiles to upload based on the contents of the file registry
+        self.__startup_from_file_registry()
+        # schedule and start the observer
+        self.__observer.schedule(self.__event_handler, self.dirpath, recursive=True)
+        self.__observer.start()
+        # loop until the user inputs a command to stop
         self.run()
-        #return a list of filepaths that have been uploaded
-        return [fp for fp,datafile in self.data_files_by_path.items() if datafile.fully_produced]
-
-    def producer_callback(self,err,msg,prodid,filename,filepath,n_total_chunks,chunk_i) :
-        """
-        A reference to this method is given as the callback for each call to :func:`confluent_kafka.Producer.produce`.
-        It is called for every message upon acknowledgement by the broker, and it uses the file registries in the
-        LOGS subdirectory to keep the information about what has and hasn't been uploaded current with what has
-        been received by the broker.
+        # return a list of relative filepaths that have been uploaded
+        to_return = []
+        for rel_filepath in self.__file_registry.get_completed_filepaths():
+            to_return.append(rel_filepath)
+        return to_return
+
+    def producer_callback(
+        self, err, msg, prodid, filename, filepath, n_total_chunks, chunk_i
+    ):
+        """
+        A reference to this method is given as the callback for each call to
+        :func:`confluent_kafka.Producer.produce`. It is called for every message
+        upon acknowledgement by the broker, and it uses the file registries in the LOGS
+        subdirectory to keep the information about what has and hasn't been uploaded
+        current with what has been received by the broker.
 
-        If the message is the final one to be acknowledged from its corresponding :class:`~UploadDataFile`,
-        the :class:`~UploadDataFile` is registered as "fully produced".
+        If the message is the final one to be acknowledged from its corresponding
+        :class:`~UploadDataFile`, the :class:`~UploadDataFile` is registered as "fully produced".
 
         :param err: The error object for the message
         :type err: :class:`confluent_kafka.KafkaError`
         :param msg: The message object
         :type msg: :class:`confluent_kafka.Message`
-        :param prodid: The ID of the producer that produced the message (hex(id(producer)) in memory)
+        :param prodid: The ID of the producer that produced the message
+            (hex(id(producer)) in memory)
         :type prodid: str
         :param filename: The name of the file the message is coming from
         :type filename: str
         :param filepath: The full path to the file the message is coming from
         :type filepath: :class:`pathlib.Path`
         :param n_total_chunks: The total number of chunks in the file this message came from
         :type n_total_chunks: int
         :param chunk_i: The index of the message's file chunk in the full list for the file
         :type chunk_i: int
         """
         # If any error occured, re-enqueue the message's file chunk
-        if err is None and msg.error() is not None :
+        if err is None and msg.error() is not None:
             err = msg.error()
-        if err is not None :
-            if err.fatal() :
-                warnmsg =f'WARNING: Producer with ID {prodid} fatally failed to deliver message for chunk '
-                warnmsg+=f'{chunk_i} of {filepath}. This message will be re-enqeued. Error reason: {err.str()}'
-            elif not err.retriable() :
-                warnmsg =f'WARNING: Producer with ID {prodid} failed to deliver message for chunk {chunk_i} of '
-                warnmsg+= f'{filepath} and cannot retry. This message will be re-enqueued. Error reason: {err.str()}'
+        if err is not None:
+            warnmsg = (
+                f'WARNING: Producer with ID {prodid} {"fatally" if err.fatal() else ""} '
+                f"failed to deliver message for chunk {chunk_i} of {filepath}"
+                f'{" and cannot retry" if not err.retriable() else ""}. '
+                f"This message will be re-enqeued. Error reason: {err.str()}"
+            )
             self.logger.warning(warnmsg)
-            self.__add_chunks_for_filepath(filepath,[chunk_i])
+            with self.__lock:
+                self.__add_chunks_for_filepath(filepath, [chunk_i])
         # Otherwise, register the chunk as successfully sent to the broker
-        else :
+        else:
             rel_filepath = filepath.relative_to(self.dirpath)
-            fully_produced = self.__file_registry.register_chunk(filename,rel_filepath,n_total_chunks,chunk_i,prodid)
-            #If the file has now been fully produced to the topic, set the variable for the file and log a line
-            if fully_produced :
-                with self.__lock :
-                    self.data_files_by_path[filepath].fully_enqueued = False
-                    self.data_files_by_path[filepath].fully_produced = True
-                debugmsg = f'{filepath.relative_to(self.dirpath)} has been fully produced to the '
-                debugmsg+= f'"{self.__topic_name}" topic as '
-                if n_total_chunks==1 :
-                    debugmsg+=f'{n_total_chunks} message'
-                else :
-                    debugmsg+=f'a set of {n_total_chunks} messages'
+            fully_produced = self.__file_registry.register_chunk(
+                filename, rel_filepath, n_total_chunks, chunk_i, prodid
+            )
+            # If the file has now been fully produced to the topic,
+            # set the variable for the file and log a line
+            if fully_produced:
+                with self.__lock:
+                    self.__active_files_by_path[filepath].fully_enqueued = False
+                    self.__active_files_by_path[filepath].fully_produced = True
+                    self.__forget_inactive_files()
+                debugmsg = (
+                    f'{rel_filepath} has been fully produced to the "{self.__topic_name}"'
+                    f' topic as {n_total_chunks} message{"s" if n_total_chunks!=1 else ""}'
+                )
                 self.logger.debug(debugmsg)
 
-    def filepath_should_be_uploaded(self,filepath) :
+    def filepath_should_be_uploaded(self, filepath):
         """
         Returns True if a given filepath should be uploaded (if it matches the upload regex)
 
         :param filepath: A candidate upload filepath
         :type filepath: :class:`pathlib.Path`
 
         :return: True if the filepath is an existing file outside of the LOGS directory
-            whose name matches the upload regex, False otherwise
+            whose path matches the upload regex, False otherwise
         :rtype: bool
 
         :raises TypeError: if `filepath` isn't a :class:`pathlib.Path` object
         """
-        if not isinstance(filepath,pathlib.PurePath) :
-            errmsg = f'ERROR: {filepath} passed to filepath_should_be_uploaded is not a Path!'
-            self.logger.error(errmsg,exc_type=TypeError)
-        if not filepath.is_file() :
-            return False
-        if self.__logs_subdir in filepath.parents :
-            return False
-        if self.__upload_regex.match(filepath.name) :
-            return True
-        return False
+        return self.__event_handler.filepath_matched(filepath)
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def _run_iteration(self) :
-        #check for new files in the directory if we haven't already found some to run
-        if not self.have_file_to_upload :
-            # wait here with some slight backoff so that the watched directory isn't just constantly pinged
+    def _run_iteration(self):
+        """
+        If there are any files currently uploading, finish uploading them.
+        If not, consult the watchdog event handler to get new active files.
+        On iterations where nothing is being actively uploaded, poll the producers
+        and increase the timeout for getting event handler updates exponentially
+        if nothing is happening.
+        """
+        # pull any new files from the event handler and poll the producers
+        if not self.have_file_to_upload:
+            # wait here so that this loop isn't constantly consuming CPU if nothing
+            # is happening
             time.sleep(self.__wait_time)
-            self.__find_new_files()
+            self.__pull_from_handler()
             n_new_callbacks = 0
-            for producer in self.__producers :
+            for producer in self.__producers:
                 new_callbacks = producer.poll(0)
-                if new_callbacks is not None :
-                    n_new_callbacks+=new_callbacks
-                if n_new_callbacks>0 :
-                    break
-            if (not self.have_file_to_upload) and (n_new_callbacks==0) :
-                if self.__wait_time<self.MAX_WAIT_TIME :
-                    self.__wait_time*=1.1
-            else :
+                if new_callbacks is not None:
+                    n_new_callbacks += new_callbacks
+            if (not self.have_file_to_upload) and (n_new_callbacks == 0):
+                if self.__wait_time < self.MAX_WAIT_TIME:
+                    self.__wait_time *= 1.05
+            else:
                 self.__wait_time = self.MIN_WAIT_TIME
             return
-        #find the first file that's running and add some of its chunks to the upload queue
-        for datafile in self.data_files_by_path.values() :
-            if datafile.upload_in_progress or datafile.waiting_to_upload :
-                datafile.enqueue_chunks_for_upload(self.__upload_queue,
-                                                    n_threads=len(self.__upload_threads),
-                                                    chunk_size=self.__chunk_size)
-        #check for new files again
-        self.__find_new_files()
-        #restart any crashed threads
+        # find the first file that's running and add some of its chunks to the upload queue
+        for datafile in self.__active_files_by_path.values():
+            if datafile.upload_in_progress or datafile.waiting_to_upload:
+                datafile.enqueue_chunks_for_upload(
+                    self.__upload_queue,
+                    n_threads=len(self.__upload_threads),
+                    chunk_size=self.__chunk_size,
+                )
+                break
+        # restart any crashed threads
         self.__restart_crashed_threads()
 
-    def _on_check(self) :
-        #poll the producers
-        for producer in self.__producers :
+    def _on_check(self):
+        # poll the producers
+        for producer in self.__producers:
             producer.poll(0)
-        #log progress so far
+        # forget inactive files
+        with self.__lock:
+            self.__forget_inactive_files()
+        # log progress so far
         self.logger.info(self.status_msg)
         self.logger.debug(self.progress_msg)
-        #reset the wait time
+        # reset the wait time
         self.__wait_time = self.MIN_WAIT_TIME
 
-    def _on_shutdown(self) :
-        self.logger.info('Will quit after all currently enqueued files are done being transferred.')
+    def _on_shutdown(self):
+        self.logger.info(
+            "Will quit after all currently enqueued files are done being transferred."
+        )
         self.logger.debug(self.progress_msg)
-        #add the remainder of any files currently in progress
-        if self.n_partially_done_files>0 :
-            msg='Will finish queueing the following files before flushing the producer and quitting:\n\t'
-            msg+='\n\t'.join([str(_) for _ in self.partially_done_file_paths])
-            self.logger.debug(msg)
-        while self.n_partially_done_files>0 :
-            for datafile in self.data_files_by_path.values() :
-                if datafile.upload_in_progress :
-                    datafile.enqueue_chunks_for_upload(self.__upload_queue,
-                                                        n_threads=len(self.__upload_threads),
-                                                        chunk_size=self.__chunk_size)
+        # shut down the watchdog observer
+        self.__observer.stop()
+        self.__observer.join()
+        # add the remainder of any files currently in progress
+        if self.n_partially_done_files > 0:
+            msg = "Will finish queueing the following files:\n\t" "\n\t".join(
+                [str(_) for _ in self.partially_done_file_paths]
+            )
+            self.logger.info(msg)
+        while self.n_partially_done_files > 0:
+            for datafile in self.__active_files_by_path.values():
+                if datafile.upload_in_progress:
+                    datafile.enqueue_chunks_for_upload(
+                        self.__upload_queue,
+                        n_threads=len(self.__upload_threads),
+                        chunk_size=self.__chunk_size,
+                    )
                     break
-        #stop the uploading threads by adding "None"s to their queues and joining them
-        for thread in self.__upload_threads :
+        # stop the uploading threads by adding "None"s to their queues and joining them
+        for thread in self.__upload_threads:
             self.__upload_queue.put(None)
-        for thread in self.__upload_threads :
+        for thread in self.__upload_threads:
             thread.join()
-        self.logger.info('Waiting for all enqueued messages to be delivered (this may take a moment)....')
-        for producer in self.__producers :
-            producer.flush(timeout=-1) #don't move on until all enqueued messages have been sent/received
+        self.logger.info(
+            "Waiting for all enqueued messages to be delivered (this may take a moment)"
+        )
+        for producer in self.__producers:
+            # don't move on until all enqueued messages have been sent/received
+            producer.flush(timeout=-1)
             producer.close()
         self.close()
         self.__file_registry.consolidate_completed_files()
 
-    def __find_new_files(self,to_upload=True) :
+    def __add_active_datafile_for_path(self, filepath):
         """
-        Search the directory for any unrecognized files and add them to _data_files_by_path
+        Create a new datafile with the given path and add it to the dictionaries of
+        active datafiles and datafiles to report for status messages
 
-        to_upload = if False, new files found will NOT be marked for uploading
-                    (default is new files are expected to be uploaded)
+        filepath = the path to the file that should be added
         """
-        #This is in a try/except in case a file is moved or a subdirectory is renamed while this method is running
-        #it'll just return and try again if so
-        try :
-            for filepath in self.dirpath.rglob('*') :
+        new_datafile = self.__datafile_type(
+            filepath,
+            to_upload=True,
+            rootdir=self.dirpath,
+            logger=self.logger,
+            **self.other_datafile_kwargs,
+        )
+        self.__active_files_by_path[filepath] = new_datafile
+        n_keys_to_remove = (
+            len(self.__status_message_files) + 1 - self.N_STATUS_MESSAGE_FILES
+        )
+        if n_keys_to_remove > 0:
+            keys_to_remove = list(self.__status_message_files.keys())[:n_keys_to_remove]
+            for key in keys_to_remove:
+                _ = self.__status_message_files.pop(key)
+        self.__status_message_files[filepath] = new_datafile
+
+    def __scrape_dir_for_files(self, retries_left=10):
+        """
+        Search the directory for any unrecognized files and add them as active datafiles
+
+        retries_left = how many attempts should be made to retry if an error is encountered
+        """
+        # This is in a try/except in case a file is moved or a subdirectory is renamed
+        # while this method is running: it'll retry up to ten times
+        try:
+            for filepath in self.dirpath.rglob("*"):
                 filepath = filepath.resolve()
-                if (filepath not in self.data_files_by_path) and self.filepath_should_be_uploaded(filepath) :
-                    #wait until the file is actually available
+                if (
+                    filepath not in self.__active_files_by_path
+                ) and self.filepath_should_be_uploaded(filepath):
+                    # wait until the file is actually available
                     file_ready = False
-                    while not file_ready :
-                        try :
-                            with open(filepath) as _ :
+                    while not file_ready:
+                        try:
+                            with open(filepath) as _:
                                 file_ready = True
-                        except PermissionError :
+                        except PermissionError:
                             time.sleep(0.05)
-                    self.data_files_by_path[filepath]=self.__datafile_type(filepath,
-                                                                           to_upload=to_upload,
-                                                                           rootdir=self.dirpath,
-                                                                           logger=self.logger,
-                                                                           **self.other_datafile_kwargs)
-        except FileNotFoundError :
-            return
+                    self.__add_active_datafile_for_path(filepath)
+        except FileNotFoundError as exc:
+            if retries_left > 0:
+                self.__scrape_dir_for_files(retries_left=retries_left - 1)
+            warnmsg = (
+                f"WARNING: exhausted retries finding new files in {self.dirpath}. "
+                "Check log messages below for the error encountered."
+            )
+            self.logger.warning(warnmsg, exc_info=exc)
+
+    def __pull_from_handler(self):
+        """
+        Call the watchdog EventHandler to get paths to files that should be uploaded
+        """
+        to_kick_back = set()
+        # get all the new files for which events have occurred
+        for handler_file in self.__event_handler.get_new_files():
+            new_filepath = handler_file.filepath
+            # if the file isn't active yet, add it and move on
+            if new_filepath not in self.__active_files_by_path:
+                with self.__lock:
+                    self.__add_active_datafile_for_path(new_filepath)
+                continue
+            # otherwise, if the file is already active in the directory
+            updated_at = handler_file.last_updated
+            extant_datafile = self.__active_files_by_path[new_filepath]
+            # if it wasn't going to be uploaded, set it to upload
+            if not extant_datafile.to_upload:
+                extant_datafile.to_upload = True
+            # if it's been fully produced, remove and replace it with the new version
+            elif extant_datafile.fully_produced:
+                with self.__lock:
+                    self.__forget_inactive_files()
+                    self.__add_active_datafile_for_path(new_filepath)
+            # if it's been fully enqueued, or is being uploaded, send it back
+            elif extant_datafile.fully_enqueued or extant_datafile.upload_in_progress:
+                to_kick_back.add(handler_file)
+            # if it's been waiting to upload
+            elif extant_datafile.waiting_to_upload:
+                # if it has been chunked before its updated time, send it back
+                # otherwise nothing needs to happen
+                if (
+                    extant_datafile.chunked_at_timestamp
+                    and extant_datafile.chunked_at_timestamp < updated_at
+                ):
+                    to_kick_back.add(handler_file)
+            else:
+                warnmsg = (
+                    "WARNING: unknown status for active upload file! Will reset file to "
+                    f"produce again (status message = {extant_datafile.upload_status_message})"
+                )
+                self.logger.warning(warnmsg)
+                with self.__lock:
+                    self.__forget_inactive_files()
+                    self.__add_active_datafile_for_path(new_filepath)
+        # send back any files that will need to be handled later
+        for handler_file in to_kick_back:
+            self.__event_handler.kick_back(handler_file)
+
+    def __forget_inactive_files(self):
+        """
+        Read through the dictionary of active files and remove any
+        that won't be uploaded or that have been fully produced
+        """
+        keys_to_remove = []
+        for key, datafile in self.__active_files_by_path.items():
+            if (not datafile.to_upload) or datafile.fully_produced:
+                keys_to_remove.append(key)
+        for key in keys_to_remove:
+            _ = self.__active_files_by_path.pop(key)
 
-    def __startup_from_file_registry(self) :
+    def __startup_from_file_registry(self):
         """
         Look through the file registry to find and prepare to enqueue any files
         that were in progress the last time the code was shut down and ignore
-        any files that have previously been fuly uploaded
+        any files that have previously been fully uploaded
         """
-        #make sure any files listed as "in progress" have their remaining chunks enqueued
+        # make sure any files listed as "in progress" have their remaining chunks enqueued
         n_files_to_resume = 0
         n_chunks_resumed = 0
-        for rel_filepath,chunks in self.__file_registry.get_incomplete_filepaths_and_chunks() :
-            debugmsg = f'Found {rel_filepath} in progress from a previous run. Re-enqueuing {len(chunks)} chunks.'
+        for (
+            rel_filepath,
+            chunks,
+        ) in self.__file_registry.get_incomplete_filepaths_and_chunks():
+            debugmsg = (
+                f"Found {rel_filepath} in progress from a previous run. "
+                f"Re-enqueuing {len(chunks)} chunks."
+            )
             self.logger.debug(debugmsg)
-            self.__add_chunks_for_filepath(self.dirpath/rel_filepath,chunks)
-            n_files_to_resume+=1
-            n_chunks_resumed+=len(chunks)
-        if n_files_to_resume>0 :
-            infomsg = f'Found {n_files_to_resume} file'
-            if n_files_to_resume!=1 :
-                infomsg+='s'
-            infomsg+= f' in progress from a previous run. Will re-enqueue {n_chunks_resumed} total chunk'
-            if n_chunks_resumed!=1 :
-                infomsg+='s'
+            self.__add_chunks_for_filepath(self.dirpath / rel_filepath, chunks)
+            n_files_to_resume += 1
+            n_chunks_resumed += len(chunks)
+        if n_files_to_resume > 0:
+            infomsg = (
+                f'Found {n_files_to_resume} file{"s" if n_files_to_resume!=1 else ""}'
+                f" in progress from a previous run. Will re-enqueue {n_chunks_resumed} "
+                f'total chunk{"s" if n_chunks_resumed!=1 else ""}'
+            )
             self.logger.info(infomsg)
-        #make sure any files listed as "completed" will not be uploaded again
-        n_files_already_uploaded = 0
-        for rel_filepath in self.__file_registry.get_completed_filepaths() :
-            filepath = self.dirpath/rel_filepath
-            if filepath in self.data_files_by_path :
-                if self.data_files_by_path[filepath].to_upload :
-                    msg = f'Found {filepath} listed as fully uploaded during a previous run. Will not produce it again.'
-                    self.logger.debug(msg)
-                self.data_files_by_path[filepath].to_upload=False
-            elif filepath.is_file() :
-                msg = f'Found {filepath} listed as fully uploaded during a previous run. Will not produce it again.'
-                self.logger.debug(msg)
-                self.data_files_by_path[filepath]=self.__datafile_type(filepath,
-                                                                       to_upload=False,
-                                                                       rootdir=self.dirpath,
-                                                                       logger=self.logger,
-                                                                       **self.other_datafile_kwargs)
-            n_files_already_uploaded+=1
-        if n_files_already_uploaded>0 :
-            infomsg = f'Found {n_files_already_uploaded} file'
-            if n_files_already_uploaded!=1 :
-                infomsg+='s'
-            infomsg+=' fully uploaded during a previous run that will not be produced again.'
+        # make sure any files listed as "completed" will not be uploaded again
+        n_prev_uploaded = 0
+        for rel_filepath in self.__file_registry.get_completed_filepaths():
+            filepath = self.dirpath / rel_filepath
+            debugmsg = (
+                f"Found {filepath} listed as fully uploaded during a previous run. "
+                "Will not produce it again."
+            )
+            if filepath in self.__active_files_by_path:
+                if self.__active_files_by_path[filepath].to_upload:
+                    self.logger.debug(debugmsg)
+                self.__active_files_by_path[filepath].to_upload = False
+            elif filepath.is_file():
+                self.logger.debug(debugmsg)
+            n_prev_uploaded += 1
+        if n_prev_uploaded > 0:
+            infomsg = (
+                f'Found {n_prev_uploaded} file{"s" if n_prev_uploaded!=1 else ""} '
+                "fully uploaded during a previous run that will not be produced again."
+            )
             self.logger.info(infomsg)
+        # forget any files that are now set to inactive
+        self.__forget_inactive_files()
 
-    def __add_chunks_for_filepath(self,filepath,chunks) :
+    def __add_chunks_for_filepath(self, filepath, chunks):
         """
         Add the given chunks to the list of chunks to upload for a given file
-        Creates the file if it doesn't already exist in the dictionary of recognized files
+        Creates the file if it doesn't already exist in the dictionary of active files
         """
-        if filepath in self.data_files_by_path :
-            self.data_files_by_path[filepath].to_upload=True
-        else :
-            self.data_files_by_path[filepath]=self.__datafile_type(filepath,
-                                                                    to_upload=True,
-                                                                    rootdir=self.dirpath,
-                                                                    logger=self.logger,
-                                                                    **self.other_datafile_kwargs)
-        self.data_files_by_path[filepath].add_chunks_to_upload(chunks,chunk_size=self.__chunk_size)
-
-    def __restart_crashed_threads(self) :
-        """
-        Iterate over the upload threads and restart any that crashed, logging the exception they threw
-        """
-        for ti,upload_thread in enumerate(self.__upload_threads) :
-            if upload_thread.caught_exception is not None :
-                #log the error
-                warnmsg = 'WARNING: an upload thread raised an Exception, which will be logged as an error below '
-                warnmsg = 'but not re-raised. The Producer and upload thread that raised the error will be restarted.'
-                self.logger.warning(warnmsg,exc_info=upload_thread.caught_exception)
-                #try to join the thread
-                try :
+        if filepath in self.__active_files_by_path:
+            self.__active_files_by_path[filepath].to_upload = True
+        else:
+            self.__add_active_datafile_for_path(filepath)
+        self.__active_files_by_path[filepath].add_chunks_to_upload(
+            chunks,
+            chunk_size=self.__chunk_size,
+        )
+
+    def __restart_crashed_threads(self):
+        """
+        Iterate over the upload threads and restart any that crashed,
+        logging the exception they threw
+        """
+        for ti, upload_thread in enumerate(self.__upload_threads):
+            if upload_thread.caught_exception is not None:
+                # log the error
+                warnmsg = (
+                    "WARNING: an upload thread raised an Exception, which will be logged "
+                    "as an error below but not re-raised. The Producer and upload thread "
+                    "that raised the error will be restarted."
+                )
+                self.logger.warning(warnmsg, exc_info=upload_thread.caught_exception)
+                # try to join the thread
+                try:
                     upload_thread.join()
-                except Exception :
+                except Exception:
                     pass
-                finally :
+                finally:
                     self.__upload_threads[ti] = None
                     self.__producers[ti] = None
-                #recreate the producer and restart the thread
+                # recreate the producer and restart the thread
                 self.__producers[ti] = self.get_new_producer()
-                thread = ExceptionTrackingThread(target=self.__producers[ti].produce_from_queue_looped,
-                                                 args=(self.__upload_queue,self.__topic_name),
-                                                 kwargs={'callback': self.producer_callback},
-                            )
+                thread = ExceptionTrackingThread(
+                    target=self.__producers[ti].produce_from_queue_looped,
+                    args=(self.__upload_queue, self.__topic_name),
+                    kwargs={"callback": self.producer_callback},
+                )
                 thread.start()
                 self.__upload_threads[ti] = thread
 
     #################### CLASS METHODS ####################
 
     @classmethod
-    def get_command_line_arguments(cls) :
-        superargs,superkwargs = super().get_command_line_arguments()
-        args = [*superargs,'upload_dir','config','topic_name','upload_regex',
-                'chunk_size','queue_max_size','update_seconds','upload_existing']
-        kwargs = {**superkwargs,'n_threads':RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS}
+    def get_command_line_arguments(cls):
+        superargs, superkwargs = super().get_command_line_arguments()
+        args = [
+            *superargs,
+            "upload_dir",
+            "config",
+            "topic_name",
+            "upload_regex",
+            "chunk_size",
+            "queue_max_size",
+            "update_seconds",
+            "upload_existing",
+        ]
+        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS}
         return args, kwargs
 
     @classmethod
-    def run_from_command_line(cls,args=None) :
+    def run_from_command_line(cls, args=None):
         """
         Run a :class:`~DataFileUploadDirectory` directly from the command line
 
-        Calls :func:`~upload_files_as_added` on a :class:`~DataFileUploadDirectory` defined by
-        command line (or given) arguments
+        Calls :func:`~upload_files_as_added` on a :class:`~DataFileUploadDirectory`
+        defined by command line (or given) arguments
 
-        :param args: the list of arguments to send to the parser instead of getting them from sys.argv
+        :param args: the list of arguments to send to the parser
         :type args: List
         """
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
-        #make the DataFileDirectory for the specified directory
-        upload_file_directory = cls(args.upload_dir,args.config,
-                                    upload_regex=args.upload_regex,update_secs=args.update_seconds,
-                                    streamlevel=args.logger_stream_level,filelevel=args.logger_file_level)
-        #listen for new files in the directory and run uploads as they come in until the process is shut down
+        # make the DataFileDirectory for the specified directory
+        upload_file_directory = cls(
+            args.upload_dir,
+            args.config,
+            upload_regex=args.upload_regex,
+            update_secs=args.update_seconds,
+            streamlevel=args.logger_stream_level,
+            filelevel=args.logger_file_level,
+        )
+        # listen for new files in the directory and run uploads until shut down
         run_start = datetime.datetime.now()
-        if not args.upload_existing :
-            upload_file_directory.logger.info(f'Listening for files to be added to {args.upload_dir}...')
-        else :
-            upload_file_directory.logger.info(f'Uploading files in/added to {args.upload_dir}...')
-        uploaded_filepaths = upload_file_directory.upload_files_as_added(args.topic_name,
-                                                                         n_threads=args.n_threads,
-                                                                         chunk_size=args.chunk_size,
-                                                                         max_queue_size=args.queue_max_size,
-                                                                         upload_existing=args.upload_existing)
+        if not args.upload_existing:
+            upload_file_directory.logger.info(
+                f"Listening for files to be added to {args.upload_dir}..."
+            )
+        else:
+            upload_file_directory.logger.info(
+                f"Uploading files in/added to {args.upload_dir}..."
+            )
+        uploaded_filepaths = upload_file_directory.upload_files_as_added(
+            args.topic_name,
+            n_threads=args.n_threads,
+            chunk_size=args.chunk_size,
+            max_queue_size=args.queue_max_size,
+            upload_existing=args.upload_existing,
+        )
         run_stop = datetime.datetime.now()
-        upload_file_directory.logger.info(f'Done listening to {args.upload_dir} for files to upload')
-        if len(uploaded_filepaths)>0 :
-            final_msg = f'The following {len(uploaded_filepaths)} file'
-            if len(uploaded_filepaths)==1 :
-                final_msg+=' was'
-            else :
-                final_msg+='s were'
-            final_msg+=f' uploaded between {run_start} and {run_stop}:\n'
-            for fp in uploaded_filepaths :
-                final_msg+=f'\t{fp.relative_to(args.upload_dir)}\n'
-        else :
-            final_msg=f'No files were uploaded between {run_start} and {run_stop}'
+        upload_file_directory.logger.info(
+            f"Done listening to {args.upload_dir} for files to upload"
+        )
+        if len(uploaded_filepaths) > 0:
+            final_msg = (
+                f"The following {len(uploaded_filepaths)} file"
+                f'{" was" if len(uploaded_filepaths)==1 else "s were"}'
+                f" uploaded between {run_start} and {run_stop}:\n\t"
+            )
+            final_msg += "\n\t".join([str(ufp) for ufp in uploaded_filepaths])
+        else:
+            final_msg = f"No files were uploaded between {run_start} and {run_stop}"
         upload_file_directory.logger.info(final_msg)
 
     #################### PROPERTIES ####################
 
     @property
-    def other_datafile_kwargs(self) :
+    def other_datafile_kwargs(self):
         """
-        Overload this property to send extra keyword arguments to the :class:`~UploadDataFile` constructor
-        for each recognized file (useful if using a custom `datafile_type`)
+        Overload this property to send extra keyword arguments to the
+        :class:`~UploadDataFile` constructor for each recognized file
+        (useful if using a custom `datafile_type`)
         """
         return {}
+
     @property
-    def status_msg(self) :
+    def status_msg(self):
         """
-        A message stating the number of files currently at each stage of progress
+        A message stating the number of files currently at each stage of progress,
+        up to the maximum number of files
         """
-        self.__find_new_files()
+        self.__forget_inactive_files()
         n_wont_be_uploaded = 0
         n_waiting_to_upload = 0
         n_upload_in_progress = 0
         n_fully_enqueued = 0
         n_fully_produced = 0
-        for datafile in self.data_files_by_path.values() :
-            if not datafile.to_upload :
-                n_wont_be_uploaded+=1
-            elif datafile.waiting_to_upload :
-                n_waiting_to_upload+=1
-            elif datafile.upload_in_progress :
-                n_upload_in_progress+=1
-            elif datafile.fully_enqueued :
-                n_fully_enqueued+=1
-            elif datafile.fully_produced :
-                n_fully_produced+=1
-        status_message = f'{len(self.data_files_by_path)} files found in {self.dirpath}'
-        if len(self.data_files_by_path)>0 :
-            status_message+=' ('
-            if n_wont_be_uploaded>0 :
-                status_message+=f'{n_wont_be_uploaded} will not be uploaded, '
-            if n_waiting_to_upload>0 :
-                status_message+=f'{n_waiting_to_upload} waiting to upload, '
-            if n_upload_in_progress>0 :
-                status_message+=f'{n_upload_in_progress} with upload in progress, '
-            if n_fully_enqueued>0 :
-                status_message+=f'{n_fully_enqueued} enqueued to be produced, '
-            if n_fully_produced>0 :
-                status_message+=f'{n_fully_produced} fully produced, '
-            status_message=f'{status_message[:-2]})'
+        for datafile in self.__status_message_files.values():
+            if not datafile.to_upload:
+                n_wont_be_uploaded += 1
+            elif datafile.waiting_to_upload:
+                n_waiting_to_upload += 1
+            elif datafile.upload_in_progress:
+                n_upload_in_progress += 1
+            elif datafile.fully_enqueued:
+                n_fully_enqueued += 1
+            elif datafile.fully_produced:
+                n_fully_produced += 1
+        if len(self.__status_message_files) > 0:
+            status_message = (
+                f"Of the {len(self.__status_message_files)} most recent files "
+                f"found in {self.dirpath}, "
+            )
+            ns_msgs = [
+                (n_wont_be_uploaded, "will not be uploaded"),
+                (n_waiting_to_upload, "are waiting to upload"),
+                (n_upload_in_progress, "have uploads in progress"),
+                (n_fully_enqueued, "are enqueued to be produced"),
+                (n_fully_produced, "are fully produced"),
+            ]
+            for nvar, msg in ns_msgs:
+                if nvar > 0:
+                    status_message += f"{nvar} {msg}, "
+            status_message = f"{status_message[:-2]}"
+        else:
+            status_message = f"No files to be uploaded found yet in {self.dirpath}"
         return status_message
+
     @property
-    def progress_msg(self) :
+    def progress_msg(self):
         """
         A message describing the files that are currently recognized as part of the directory
         """
-        self.__find_new_files()
-        if len(self.data_files_by_path)>0 :
-            progress_msg = 'The following files have been recognized so far:\n'
-            for datafile in self.data_files_by_path.values() :
-                if not datafile.to_upload :
-                    continue
-                progress_msg+=f'\t{datafile.upload_status_msg}\n'
-        else :
-            progress_msg = f'No files found yet in {self.dirpath}'
-        return progress_msg
+        self.__forget_inactive_files()
+        if len(self.__status_message_files) > 0:
+            msg = (
+                "The following files have been recognized so far "
+                f"(up to {self.N_STATUS_MESSAGE_FILES} most recent):\n\t"
+            )
+            msg += "\n\t".join(
+                [df.upload_status_msg for df in self.__status_message_files.values()]
+            )
+        else:
+            msg = f"No files to be uploaded found yet in {self.dirpath}"
+        return msg
+
     @property
-    def have_file_to_upload(self) :
+    def have_file_to_upload(self):
         """
         True if there are any files waiting to be uploaded or in progress
         """
-        for datafile in self.data_files_by_path.values() :
-            if datafile.upload_in_progress or datafile.waiting_to_upload :
+        for datafile in self.__active_files_by_path.values():
+            if datafile.upload_in_progress or datafile.waiting_to_upload:
                 return True
         return False
+
     @property
-    def partially_done_file_paths(self) :
+    def partially_done_file_paths(self):
         """
         A list of filepaths whose uploads are currently in progress
         """
-        return [fp for fp,df in self.data_files_by_path.items() if df.upload_in_progress]
+        return [
+            fp for fp, df in self.__active_files_by_path.items() if df.upload_in_progress
+        ]
+
     @property
-    def n_partially_done_files(self) :
+    def n_partially_done_files(self):
         """
         The number of files currently in the process of being uploaded
         """
         return len(self.partially_done_file_paths)
 
-def main(args=None) :
+
+def main(args=None):
     """
     Main method to run from command line
     """
     DataFileUploadDirectory.run_from_command_line(args)
 
-if __name__=='__main__' :
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,248 +1,327 @@
 """
 Code for managing the two csv files listing files that are
 in the process of being produced/have been fully produced
 """
 
-#imports
+# imports
 import pathlib, datetime
 from typing import Set
 from dataclasses import dataclass
-from ....utilities import DataclassTableReadOnly, DataclassTableAppendOnly, DataclassTable, LogOwner
+from ....utilities import (
+    DataclassTableReadOnly,
+    DataclassTableAppendOnly,
+    DataclassTable,
+    LogOwner,
+)
+
 
 @dataclass
-class RegistryLineInProgress :
+class RegistryLineInProgress:
     """
     A line in the table listing files in progress
     """
-    filename : str
-    rel_filepath : pathlib.Path
-    n_chunks : int
-    n_chunks_delivered : int
-    n_chunks_to_send : int
-    started : datetime.datetime
-    chunks_delivered : Set[int]
-    chunks_to_send : Set[int]
+
+    filename: str
+    rel_filepath: pathlib.Path
+    n_chunks: int
+    n_chunks_delivered: int
+    n_chunks_to_send: int
+    started: datetime.datetime
+    chunks_delivered: Set[int]
+    chunks_to_send: Set[int]
+
 
 @dataclass
-class RegistryLineCompleted :
+class RegistryLineCompleted:
     """
     A line in the table listing completed files
     """
-    filename : str
-    rel_filepath : pathlib.Path
-    n_chunks : int
-    started : datetime.datetime
-    completed : datetime.datetime
 
-class ProducerFileRegistry(LogOwner) :
+    filename: str
+    rel_filepath: pathlib.Path
+    n_chunks: int
+    started: datetime.datetime
+    completed: datetime.datetime
+
+
+class ProducerFileRegistry(LogOwner):
     """
     A class to manage two atomic csv files listing which portions
     of which files have been uploaded to a particular topic
     """
 
-    def __init__(self,dirpath,topic_name,*args,max_completed_lines_per_file=1000,**kwargs) :
+    def __init__(
+        self, dirpath, topic_name, *args, max_completed_lines_per_file=1000, **kwargs
+    ):
         """
         dirpath    = path to the directory that should contain the csv file
         topic_name = the name of the topic that will be produced to (used in the filename)
         """
-        super().__init__(*args,**kwargs)
-        #A table to list the files currently in progress
-        in_prog_filepath = dirpath / f'upload_to_{topic_name}_in_progress.csv'
-        self.__in_prog = DataclassTable(dataclass_type=RegistryLineInProgress,filepath=in_prog_filepath,
-                                        logger=self.logger)
-        #Pattern for the "completed" .csv file names
-        self.completed_filepath_pattern = dirpath / f'uploaded_to_{topic_name}.csv'
-        #keep track of the maximum number of lines per "completed" file
+        super().__init__(*args, **kwargs)
+        # A table to list the files currently in progress
+        in_prog_filepath = dirpath / f"upload_to_{topic_name}_in_progress.csv"
+        self.__in_prog = DataclassTable(
+            dataclass_type=RegistryLineInProgress,
+            filepath=in_prog_filepath,
+            logger=self.logger,
+        )
+        # Pattern for the "completed" .csv file names
+        self.completed_filepath_pattern = dirpath / f"uploaded_to_{topic_name}.csv"
+        # keep track of the maximum number of lines per "completed" file
         self.max_completed_lines_per_file = max_completed_lines_per_file
-        #Make a dictionary to hold tables of any newly received "completed" entries
+        # Make a dictionary to hold tables of any newly received "completed" entries
         self.__completed_tables_by_path = {}
-        #Consolidate existing "completed" csv files into one
+        # Consolidate existing "completed" csv files into one
         self.consolidate_completed_files()
 
-    def __del__(self) :
+    def __del__(self):
         self.consolidate_completed_files()
 
-    def consolidate_completed_files(self) :
+    def consolidate_completed_files(self):
         """
-        Search the directory holding the files for all "completed" file entries and write them into a single file
+        Search the directory holding the files for all "completed" file entries
+        and write them into a single file
         """
-        #add any lines from files in the directory to the one consolidated file at the expected path
-        globpattern = f'{self.completed_filepath_pattern.stem}*{self.completed_filepath_pattern.suffix}'
+        # add any lines from files in the directory to the one consolidated file
+        stem = self.completed_filepath_pattern.stem
+        suffix = self.completed_filepath_pattern.suffix
+        globpattern = f"{stem}*{suffix}"
         consolidated_file = None
-        for fp in self.completed_filepath_pattern.parent.glob(globpattern) :
-            if fp==self.completed_filepath_pattern :
+        for fp in self.completed_filepath_pattern.parent.glob(globpattern):
+            if fp == self.completed_filepath_pattern:
                 continue
-            if fp in self.__completed_tables_by_path :
+            if fp in self.__completed_tables_by_path:
                 self.__completed_tables_by_path[fp].dump_to_file()
-            file_to_add = DataclassTableReadOnly(dataclass_type=RegistryLineCompleted,filepath=fp,logger=self.logger)
-            if consolidated_file is None :
-                consolidated_file = DataclassTableAppendOnly(dataclass_type=RegistryLineCompleted,
-                                                             filepath=self.completed_filepath_pattern,
-                                                             logger=self.logger)
+            file_to_add = DataclassTableReadOnly(
+                dataclass_type=RegistryLineCompleted, filepath=fp, logger=self.logger
+            )
+            if consolidated_file is None:
+                consolidated_file = DataclassTableAppendOnly(
+                    dataclass_type=RegistryLineCompleted,
+                    filepath=self.completed_filepath_pattern,
+                    logger=self.logger,
+                )
             consolidated_file.add_entries(file_to_add.objects)
-        if consolidated_file is None :
+        if consolidated_file is None:
             return
-        #dump out the consolidated file
+        # dump out the consolidated file
         consolidated_file.dump_to_file()
-        #make sure that all the lines from the individual files have been successfully copied
-        all_lines = (DataclassTableReadOnly(dataclass_type=RegistryLineCompleted,
-                                            filepath=self.completed_filepath_pattern,logger=self.logger)).lines
-        for fp in self.completed_filepath_pattern.parent.glob(globpattern) :
-            if fp==self.completed_filepath_pattern :
+        # make sure that all the lines from the individual files have been successfully copied
+        all_lines = (
+            DataclassTableReadOnly(
+                dataclass_type=RegistryLineCompleted,
+                filepath=self.completed_filepath_pattern,
+                logger=self.logger,
+            )
+        ).lines
+        for fp in self.completed_filepath_pattern.parent.glob(globpattern):
+            if fp == self.completed_filepath_pattern:
                 continue
-            added_file = DataclassTableReadOnly(dataclass_type=RegistryLineCompleted,filepath=fp,logger=self.logger)
-            for entry_line in added_file.lines :
-                if entry_line not in all_lines :
-                    errmsg = f'ERROR: failed to consolidate individual files into {self.completed_filepath_pattern}. '
-                    errmsg+= 'Individual files will be retained and should be manually concatenated. '
-                    errmsg+= 'Duplicate entries may be present.'
-                    raise RuntimeError(errmsg)
-            if fp in self.__completed_tables_by_path :
+            added_file = DataclassTableReadOnly(
+                dataclass_type=RegistryLineCompleted, filepath=fp, logger=self.logger
+            )
+            for entry_line in added_file.lines:
+                if entry_line not in all_lines:
+                    warnmsg = (
+                        "WARNING: failed to consolidate individual files into "
+                        f"{self.completed_filepath_pattern}. Individual files will be "
+                        "retained and should be manually concatenated. "
+                        "Duplicate entries may be present."
+                    )
+                    self.logger.warning(warnmsg)
+            if fp in self.__completed_tables_by_path:
                 self.__completed_tables_by_path.pop(fp)
             fp.unlink()
 
-    def get_incomplete_filepaths_and_chunks(self) :
+    def get_incomplete_filepaths_and_chunks(self):
         """
-        Generate tuples of (rel_filepath, chunks to upload) for each file that has not yet been completely uploaded
+        Generate tuples of (rel_filepath, chunks to upload) for each file
+        that has not yet been completely uploaded
         """
-        for obj_address in self.__in_prog.obj_addresses :
-            attr_dict = self.__in_prog.get_entry_attrs(obj_address,'rel_filepath','chunks_to_send')
-            if len(attr_dict['chunks_to_send'])>0 :
-                yield attr_dict['rel_filepath'],attr_dict['chunks_to_send']
+        for obj_address in self.__in_prog.obj_addresses:
+            attr_dict = self.__in_prog.get_entry_attrs(
+                obj_address, "rel_filepath", "chunks_to_send"
+            )
+            if len(attr_dict["chunks_to_send"]) > 0:
+                yield attr_dict["rel_filepath"], attr_dict["chunks_to_send"]
 
-    def get_completed_filepaths(self) :
+    def get_completed_filepaths(self):
         """
         Generate relative filepaths for each file that has been completely uploaded
         """
         self.consolidate_completed_files()
-        completed = DataclassTableReadOnly(dataclass_type=RegistryLineCompleted,
-                                           filepath=self.completed_filepath_pattern,logger=self.logger)
-        for obj_address in completed.obj_addresses :
-            yield completed.get_entry_attrs(obj_address,'rel_filepath')
+        completed = DataclassTableReadOnly(
+            dataclass_type=RegistryLineCompleted,
+            filepath=self.completed_filepath_pattern,
+            logger=self.logger,
+        )
+        seen = set()
+        for obj_address in completed.obj_addresses:
+            rel_filepath = completed.get_entry_attrs(obj_address, "rel_filepath")
+            if rel_filepath not in seen:
+                seen.add(rel_filepath)
+                yield rel_filepath
 
-    def register_chunk(self,filename,rel_filepath,n_total_chunks,chunk_i,prodid) :
+    def register_chunk(self, filename, rel_filepath, n_total_chunks, chunk_i, prodid):
         """
         Register a chunk as having been successfully produced by a particular producer
         Returns True if all chunks for the file have been produced
         """
-        #acquire the lock so no other threads can change the in progress file
+        # acquire the lock so no other threads can change the in progress file
         self.__in_prog.lock.acquire()
-        #get a dictionary of the existing object addresses keyed by their filepaths
-        existing_obj_addresses = self.__in_prog.obj_addresses_by_key_attr('rel_filepath')
-        #if the file is already recognized as in progress
-        if rel_filepath in existing_obj_addresses :
-            return self.__register_chunk_of_existing_file(filename,rel_filepath,n_total_chunks,chunk_i,prodid)
-        #otherwise it's a new file to list somewhere
-        return self.__register_chunk_for_new_file(filename,rel_filepath,n_total_chunks,chunk_i,prodid)
-
-    def __register_chunk_of_existing_file(self,filename,rel_filepath,n_total_chunks,chunk_i,prodid) :
+        # get a dictionary of the existing object addresses keyed by their filepaths
+        existing_obj_addresses = self.__in_prog.obj_addresses_by_key_attr("rel_filepath")
+        # if the file is already recognized as in progress
+        if rel_filepath in existing_obj_addresses:
+            return self.__register_chunk_of_existing_file(
+                filename, rel_filepath, n_total_chunks, chunk_i, prodid
+            )
+        # otherwise it's a new file to list somewhere
+        return self.__register_chunk_for_new_file(
+            filename, rel_filepath, n_total_chunks, chunk_i, prodid
+        )
+
+    def __register_chunk_of_existing_file(
+        self, filename, rel_filepath, n_total_chunks, chunk_i, prodid
+    ):
         """
         Register a chunk that belongs to an existing file.
         Returns True if all chunks for the file have been received by the broker.
         """
-        #get a dictionary of the existing object addresses keyed by their filepaths
-        existing_obj_addresses = self.__in_prog.obj_addresses_by_key_attr('rel_filepath')
-        #make sure there's only one object with this filepath
-        if len(existing_obj_addresses[rel_filepath])!=1 :
-            errmsg = f'ERROR: found {len(existing_obj_addresses[rel_filepath])} files in the producer registry '
-            errmsg+= f'for filepath {rel_filepath}'
+        # get a dictionary of the existing object addresses keyed by their filepaths
+        existing_obj_addresses = self.__in_prog.obj_addresses_by_key_attr("rel_filepath")
+        # make sure there's only one object with this filepath
+        if len(existing_obj_addresses[rel_filepath]) != 1:
+            errmsg = (
+                f"ERROR: found {len(existing_obj_addresses[rel_filepath])} files in the "
+                f"producer registry for filepath {rel_filepath}"
+            )
             self.__in_prog.lock.release()
-            self.logger.error(errmsg,exc_type=RuntimeError)
+            self.logger.error(errmsg, exc_type=RuntimeError)
         existing_addr = existing_obj_addresses[rel_filepath][0]
-        #make sure the total numbers of chunks match
-        existing_n_chunks = self.__in_prog.get_entry_attrs(existing_addr,'n_chunks')
-        if existing_n_chunks!=n_total_chunks :
-            errmsg = f'ERROR: {rel_filepath} in {self.__class__.__name__} is listed as having '
-            errmsg+= f'{existing_n_chunks} total chunks, but the producer callback for this file '
-            errmsg+= f'lists {n_total_chunks} chunks! Did the chunk size change?'
+        # make sure the total numbers of chunks match
+        existing_n_chunks = self.__in_prog.get_entry_attrs(existing_addr, "n_chunks")
+        if existing_n_chunks != n_total_chunks:
+            errmsg = (
+                f"ERROR: {rel_filepath} in {self.__class__.__name__} is listed as having "
+                f"{existing_n_chunks} total chunks, but the producer callback for this "
+                f"file lists {n_total_chunks} chunks! Did the chunk size change?"
+            )
             self.__in_prog.lock.release()
-            self.logger.error(errmsg,exc_type=RuntimeError)
-        #get its current state
-        attrs = self.__in_prog.get_entry_attrs(existing_addr,'chunks_delivered','chunks_to_send')
-        #if the chunk is already registered, just return
-        if chunk_i in attrs['chunks_delivered'] :
+            self.logger.error(errmsg, exc_type=RuntimeError)
+        # get its current state
+        attrs = self.__in_prog.get_entry_attrs(
+            existing_addr, "chunks_delivered", "chunks_to_send"
+        )
+        # if the chunk is already registered, just return
+        if chunk_i in attrs["chunks_delivered"]:
             self.__in_prog.lock.release()
             return False
-        #otherwise add/remove it from the sets
-        attrs['chunks_delivered'].add(chunk_i)
-        try :
-            attrs['chunks_to_send'].remove(chunk_i)
-        except KeyError :
+        # otherwise add/remove it from the sets
+        attrs["chunks_delivered"].add(chunk_i)
+        try:
+            attrs["chunks_to_send"].remove(chunk_i)
+        except KeyError:
             pass
-        #reset the attributes for the object
+        # reset the attributes for the object
         new_attrs = {
-            'n_chunks_delivered':len(attrs['chunks_delivered']),
-            'n_chunks_to_send':len(attrs['chunks_to_send']),
-            'chunks_delivered':attrs['chunks_delivered'],
-            'chunks_to_send':attrs['chunks_to_send'],
-            }
-        self.__in_prog.set_entry_attrs(existing_addr,**new_attrs)
+            "n_chunks_delivered": len(attrs["chunks_delivered"]),
+            "n_chunks_to_send": len(attrs["chunks_to_send"]),
+            "chunks_delivered": attrs["chunks_delivered"],
+            "chunks_to_send": attrs["chunks_to_send"],
+        }
+        self.__in_prog.set_entry_attrs(existing_addr, **new_attrs)
         # if there are no more chunks to send and all chunks have been delivered,
         # move this file from "in progress" to "completed" and force-dump the files
-        if ( self.__in_prog.get_entry_attrs(existing_addr,'n_chunks_delivered')==n_total_chunks and
-                self.__in_prog.get_entry_attrs(existing_addr,'n_chunks_to_send')==0 ) :
-            started = self.__in_prog.get_entry_attrs(existing_addr,'started')
-            completed_entry = RegistryLineCompleted(filename,rel_filepath,n_total_chunks,
-                                                    started,datetime.datetime.now())
-            self.__add_completed_entry(completed_entry,prodid)
+        if (
+            self.__in_prog.get_entry_attrs(existing_addr, "n_chunks_delivered")
+            == n_total_chunks
+            and self.__in_prog.get_entry_attrs(existing_addr, "n_chunks_to_send") == 0
+        ):
+            started = self.__in_prog.get_entry_attrs(existing_addr, "started")
+            completed_entry = RegistryLineCompleted(
+                filename, rel_filepath, n_total_chunks, started, datetime.datetime.now()
+            )
+            self.__add_completed_entry(completed_entry, prodid)
             self.__in_prog.remove_entries(existing_addr)
             self.__in_prog.dump_to_file()
             self.__in_prog.lock.release()
             return True
         self.__in_prog.lock.release()
         return False
 
-    def __register_chunk_for_new_file(self,filename,rel_filepath,n_total_chunks,chunk_i,prodid) :
+    def __register_chunk_for_new_file(
+        self, filename, rel_filepath, n_total_chunks, chunk_i, prodid
+    ):
         """
         Register the first chunk for a file.
         Returns True if the file only had one chunk.
         """
         to_deliver = set([])
-        for ichunk in range(1,n_total_chunks+1) :
-            if ichunk!=chunk_i :
+        for ichunk in range(1, n_total_chunks + 1):
+            if ichunk != chunk_i:
                 to_deliver.add(ichunk)
-        #if there are other chunks to deliver, register it to "in_progress"
-        if len(to_deliver)>0 :
-            in_prog_entry = RegistryLineInProgress(filename,rel_filepath,n_total_chunks,
-                                                    1,n_total_chunks-1,datetime.datetime.now(),
-                                                    set([chunk_i]),to_deliver)
+        # if there are other chunks to deliver, register it to "in_progress"
+        if len(to_deliver) > 0:
+            in_prog_entry = RegistryLineInProgress(
+                filename,
+                rel_filepath,
+                n_total_chunks,
+                1,
+                n_total_chunks - 1,
+                datetime.datetime.now(),
+                set([chunk_i]),
+                to_deliver,
+            )
             self.__in_prog.add_entries(in_prog_entry)
             self.__in_prog.dump_to_file()
             self.__in_prog.lock.release()
             return False
-        #otherwise register it as a completed file
+        # otherwise register it as a completed file
         self.__in_prog.lock.release()
-        completed_entry = RegistryLineCompleted(filename,rel_filepath,n_total_chunks,
-                                                datetime.datetime.now(),datetime.datetime.now())
-        self.__add_completed_entry(completed_entry,prodid)
+        completed_entry = RegistryLineCompleted(
+            filename,
+            rel_filepath,
+            n_total_chunks,
+            datetime.datetime.now(),
+            datetime.datetime.now(),
+        )
+        self.__add_completed_entry(completed_entry, prodid)
         return True
 
-    def __add_completed_entry(self,completed_entry,prodid) :
+    def __add_completed_entry(self, completed_entry, prodid):
         """
-        Add a given entry from a given produced as "completed", possibly juggling the files around
-        if they're getting too large
+        Add a given entry from a given produced as "completed", possibly juggling
+        the files around if they're getting too large
         """
-        #create the path to the table file that should be added to
-        prod_name = f'{self.completed_filepath_pattern.stem}_p{prodid}{self.completed_filepath_pattern.suffix}'
+        # create the path to the table file that should be added to
+        stem = self.completed_filepath_pattern.stem
+        suffix = self.completed_filepath_pattern.suffix
+        prod_name = f"{stem}_p{prodid}{suffix}"
         table_path = self.completed_filepath_pattern.with_name(prod_name)
         create_new_table_at_path = False
-        #if the table already exists
-        if table_path in self.__completed_tables_by_path :
-            #if the table has the max # of entries or more entries already
-            if self.__completed_tables_by_path[table_path].n_entries>=self.max_completed_lines_per_file :
-                #dump it out to its file
+        # if the table already exists
+        if table_path in self.__completed_tables_by_path:
+            # if the table has the max # of entries or more entries already
+            if (
+                self.__completed_tables_by_path[table_path].n_entries
+                >= self.max_completed_lines_per_file
+            ):
+                # dump it out to its file
                 self.__completed_tables_by_path[table_path].dump_to_file()
-                #rename the dumped file with a timestamp
-                timestamp = str(datetime.datetime.now().timestamp()).replace('.','_')
-                new_path = table_path.with_name(f'{table_path.stem}_{timestamp}{table_path.suffix}')
+                # rename the dumped file with a timestamp
+                timestamp = str(datetime.datetime.now().timestamp()).replace(".", "_")
+                new_path = table_path.with_name(
+                    f"{table_path.stem}_{timestamp}{table_path.suffix}"
+                )
                 table_path.rename(new_path)
-                #reset the table associated with the filepath for this producer
+                # reset the table associated with the filepath for this producer
                 create_new_table_at_path = True
-        else :
+        else:
             create_new_table_at_path = True
-        if create_new_table_at_path :
-            self.__completed_tables_by_path[table_path] = DataclassTableAppendOnly(RegistryLineCompleted,
-                                                                                   filepath=table_path,
-                                                                                   logger=self.logger)
+        if create_new_table_at_path:
+            self.__completed_tables_by_path[table_path] = DataclassTableAppendOnly(
+                RegistryLineCompleted, filepath=table_path, logger=self.logger
+            )
         self.__completed_tables_by_path[table_path].add_entries(completed_entry)
         self.__completed_tables_by_path[table_path].dump_to_file()
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py` & `openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,338 +1,444 @@
 """
 Code for managing the two .csv files listing files that are
 being reconstructed from the topic and files that have been fully handled
 """
 
-#imports
+# imports
 import pathlib, datetime, re, threading
 from abc import ABC
 from dataclasses import dataclass
-from ....utilities import DataclassTableReadOnly, DataclassTableAppendOnly, DataclassTable, LogOwner
+from ....utilities import (
+    DataclassTableReadOnly,
+    DataclassTableAppendOnly,
+    DataclassTable,
+    LogOwner,
+)
 from ...utilities import get_message_prepend
 
+
 @dataclass
-class StreamHandlerRegistryLineInProgress :
+class StreamHandlerRegistryLineInProgress:
     """
     A line in the table listing files in progress
     """
-    filename : str #the name of the file
-    rel_filepath : pathlib.Path #the path to the file, relative to its root directory
-    status : str #the status of the file, either "in_progress", "failed", or "mismatched_hash"
-    n_chunks : int #the total number of chunks in the file
-    first_message : datetime.datetime #timestamp of when the first message for the file was consumed
-    most_recent_message : datetime.datetime #timestamp of when the most recent chunk from the file was consumed
+
+    filename: str
+    rel_filepath: pathlib.Path
+    status: str
+    n_chunks: int
+    first_message: datetime.datetime
+    most_recent_message: datetime.datetime
+
 
 @dataclass
-class StreamHandlerRegistryLineSucceeded :
+class StreamHandlerRegistryLineSucceeded:
     """
     A line in the table listing files that have been successfully handled
     """
-    filename : str #the name of the file
-    rel_filepath : pathlib.Path #the path to the file, relative to its root directory
-    n_chunks : int #the total number of chunks in the file
-    first_message : datetime.datetime #timestamp of when the most recent chunk from the file was consumed
-    processed_at : datetime.datetime #timestamp of when the file was processed
 
-class StreamHandlerRegistry(LogOwner,ABC) :
+    filename: str
+    rel_filepath: pathlib.Path
+    n_chunks: int
+    first_message: datetime.datetime
+    processed_at: datetime.datetime
+
+
+class StreamHandlerRegistry(LogOwner, ABC):
     """
     A general base class to keep track of the status of files read during stream handling
     """
 
-    IN_PROGRESS = 'in_progress'
-    MISMATCHED_HASH = 'mismatched_hash'
+    IN_PROGRESS = "in_progress"
+    MISMATCHED_HASH = "mismatched_hash"
 
     @property
-    def in_progress_table(self) :
+    def in_progress_table(self):
         """
         A read-only version of the table listing files in progress
         """
         return self._in_progress_table.as_read_only()
 
     @property
-    def succeeded_table(self) :
+    def succeeded_table(self):
         """
         A read-only version of the table listing files that have been successfully handled
         """
         self.consolidate_succeeded_files()
-        return DataclassTableReadOnly(StreamHandlerRegistryLineSucceeded,
-                                      filepath=self.succeeded_filepath,logger=self.logger)
+        return DataclassTableReadOnly(
+            StreamHandlerRegistryLineSucceeded,
+            filepath=self.succeeded_filepath,
+            logger=self.logger,
+        )
 
     @property
-    def filepaths_to_rerun(self) :
+    def filepaths_to_rerun(self):
         """
         A list of all the filepaths that have not yet been successfully processed
         """
         to_rerun = []
-        for addr in self._in_progress_table.obj_addresses :
-            to_rerun.append(self._in_progress_table.get_entry_attrs(addr,'rel_filepath'))
+        for addr in self._in_progress_table.obj_addresses:
+            to_rerun.append(self._in_progress_table.get_entry_attrs(addr, "rel_filepath"))
         return to_rerun
 
     @property
-    def rerun_file_key_regex(self) :
+    def rerun_file_key_regex(self):
         """
         Regex matching keys for messages from files that need to be rerun
         """
-        if self.n_files_to_rerun<=0 :
+        if self.n_files_to_rerun <= 0:
             return None
-        regex_str = r'^('
-        for fp in self.filepaths_to_rerun :
-            if fp!=fp.name :
-                subdir_str = str(fp.parent.as_posix())
-            else :
-                subdir_str = None
-            regex_str+=f'{get_message_prepend(subdir_str,fp.name)}|'
-        regex_str=f'{regex_str[:-1]})_.*$'
+        regex_str = r"^("
+        for fp in self.filepaths_to_rerun:
+            subdir_str = str(fp.parent.as_posix()) if fp != fp.name else None
+            regex_str += f"{get_message_prepend(subdir_str,fp.name)}|"
+        regex_str = f"{regex_str[:-1]})_.*$"
         return re.compile(regex_str)
 
     @property
-    def n_files_to_rerun(self) :
+    def n_files_to_rerun(self):
         """
         The number of files in the registry that are marked as "in_progress"
         """
         return len(self.filepaths_to_rerun)
 
-    def __init__(self,in_progress_filepath,succeeded_filepath,*args,max_succeeded_lines_per_file=1000,**kwargs) :
-        """
-        in_progress_filepath = path to the file that should hold the "in_progress" datatable
-        succeeded_filepath = path to the file that should hole the "succeeded" datatable
-        """
-        super().__init__(*args,**kwargs)
-        self._in_progress_table = DataclassTable(dataclass_type=StreamHandlerRegistryLineInProgress,
-                                                  filepath=in_progress_filepath,logger=self.logger)
+    def __init__(
+        self,
+        in_progress_filepath,
+        succeeded_filepath,
+        *args,
+        max_succeeded_lines_per_file=1000,
+        **kwargs,
+    ):
+        """
+        in_progress_filepath = path to the file with the "in_progress" datatable
+        succeeded_filepath = path to the file with the "succeeded" datatable
+        """
+        super().__init__(*args, **kwargs)
+        self._in_progress_table = DataclassTable(
+            dataclass_type=StreamHandlerRegistryLineInProgress,
+            filepath=in_progress_filepath,
+            logger=self.logger,
+        )
         self.succeeded_filepath = succeeded_filepath
         self.max_succeeded_lines_per_file = max_succeeded_lines_per_file
         self.__succeeded_tables_by_id = {}
         self.consolidate_succeeded_files()
 
-    def register_file_in_progress(self,dfc) :
+    def register_file_in_progress(self, dfc):
         """
         Add/update a line in the table showing that a file is in progress
         """
-        self._add_or_modify_in_progress_entry(dfc,self.IN_PROGRESS)
+        self._add_or_modify_in_progress_entry(dfc, self.IN_PROGRESS)
 
-    def register_file_mismatched_hash(self,dfc) :
+    def register_file_mismatched_hash(self, dfc):
         """
-        Add/update a line in the table to show that a consumed file was mismatched with its original content hash
+        Add/update a line in the table to show that a consumed file
+        was mismatched with its original content hash
         """
-        self._add_or_modify_in_progress_entry(dfc,self.MISMATCHED_HASH)
+        self._add_or_modify_in_progress_entry(dfc, self.MISMATCHED_HASH)
 
-    def consolidate_succeeded_files(self) :
+    def consolidate_succeeded_files(self):
         """
-        Search the directory holding the files for all "completed" file entries and write them into a single file
+        Search the directory holding the files for all "completed" file entries
+        and write them into a single file
         """
-        #add any lines from files in the directory to the one consolidated file at the expected path
-        globpattern = f'{self.succeeded_filepath.stem}*{self.succeeded_filepath.suffix}'
+        # add any lines from files in the directory to the one consolidated file
+        globpattern = f"{self.succeeded_filepath.stem}*{self.succeeded_filepath.suffix}"
         consolidated_file = None
-        for fp in self.succeeded_filepath.parent.glob(globpattern) :
-            if fp==self.succeeded_filepath :
+        for fp in self.succeeded_filepath.parent.glob(globpattern):
+            if fp == self.succeeded_filepath:
                 continue
-            for table in self.__succeeded_tables_by_id.values() :
-                if fp==table.filepath :
+            for table in self.__succeeded_tables_by_id.values():
+                if fp == table.filepath:
                     table.dump_to_file()
-            file_to_add = DataclassTableReadOnly(dataclass_type=StreamHandlerRegistryLineSucceeded,
-                                                 filepath=fp,logger=self.logger)
-            if consolidated_file is None :
-                consolidated_file = DataclassTableAppendOnly(dataclass_type=StreamHandlerRegistryLineSucceeded,
-                                                             filepath=self.succeeded_filepath,
-                                                             logger=self.logger)
+            file_to_add = DataclassTableReadOnly(
+                dataclass_type=StreamHandlerRegistryLineSucceeded,
+                filepath=fp,
+                logger=self.logger,
+            )
+            if consolidated_file is None:
+                consolidated_file = DataclassTableAppendOnly(
+                    dataclass_type=StreamHandlerRegistryLineSucceeded,
+                    filepath=self.succeeded_filepath,
+                    logger=self.logger,
+                )
             consolidated_file.add_entries(file_to_add.objects)
-        if consolidated_file is None :
+        if consolidated_file is None:
             return
-        #dump out the consolidated file
+        # dump out the consolidated file
         consolidated_file.dump_to_file()
-        #make sure that all the lines from the individual files have been successfully copied
-        all_lines = (DataclassTableReadOnly(dataclass_type=StreamHandlerRegistryLineSucceeded,
-                                            filepath=self.succeeded_filepath,logger=self.logger)).lines
-        for fp in self.succeeded_filepath.parent.glob(globpattern) :
-            if fp==self.succeeded_filepath :
+        # make sure that all the lines from the individual files have been copied
+        all_lines = (
+            DataclassTableReadOnly(
+                dataclass_type=StreamHandlerRegistryLineSucceeded,
+                filepath=self.succeeded_filepath,
+                logger=self.logger,
+            )
+        ).lines
+        for fp in self.succeeded_filepath.parent.glob(globpattern):
+            if fp == self.succeeded_filepath:
                 continue
-            added_file = DataclassTableReadOnly(dataclass_type=StreamHandlerRegistryLineSucceeded,
-                                                filepath=fp,logger=self.logger)
-            for entry_line in added_file.lines :
-                if entry_line not in all_lines :
-                    errmsg = f'ERROR: failed to consolidate individual files into {self.succeeded_filepath}. '
-                    errmsg+= 'Individual files will be retained and should be manually concatenated. '
-                    errmsg+= 'Duplicate entries may be present.'
-                    raise RuntimeError(errmsg)
-            to_pop = [table_id for table_id,table in self.__succeeded_tables_by_id.items() if fp==table.filepath]
-            for table_id in to_pop :
+            added_file = DataclassTableReadOnly(
+                dataclass_type=StreamHandlerRegistryLineSucceeded,
+                filepath=fp,
+                logger=self.logger,
+            )
+            for entry_line in added_file.lines:
+                if entry_line not in all_lines:
+                    warnmsg = (
+                        "WARNING: failed to consolidate individual files into "
+                        f"{self.succeeded_filepath}. Individual files will be retained "
+                        "and should be manually concatenated. "
+                        "Duplicate entries may be present."
+                    )
+                    self.logger.warning(warnmsg)
+            to_pop = [
+                table_id
+                for table_id, table in self.__succeeded_tables_by_id.items()
+                if fp == table.filepath
+            ]
+            for table_id in to_pop:
                 self.__succeeded_tables_by_id.pop(table_id)
             fp.unlink()
 
-    def _add_or_modify_in_progress_entry(self,dfc,new_status) :
-        with self._in_progress_table.lock :
-            existing_entry_addr = self._get_in_progress_address_for_rel_filepath(dfc.relative_filepath)
-            if existing_entry_addr is None :
-                new_entry = StreamHandlerRegistryLineInProgress(dfc.filename,
-                                                                dfc.relative_filepath,
-                                                                new_status,
-                                                                dfc.n_total_chunks,
-                                                                datetime.datetime.now(),
-                                                                datetime.datetime.now())
+    def _add_or_modify_in_progress_entry(self, dfc, new_status):
+        with self._in_progress_table.lock:
+            existing_entry_addr = self._get_in_progress_address_for_rel_filepath(
+                dfc.relative_filepath
+            )
+            if existing_entry_addr is None:
+                new_entry = StreamHandlerRegistryLineInProgress(
+                    dfc.filename,
+                    dfc.relative_filepath,
+                    new_status,
+                    dfc.n_total_chunks,
+                    datetime.datetime.now(),
+                    datetime.datetime.now(),
+                )
                 self._in_progress_table.add_entries(new_entry)
                 self._in_progress_table.dump_to_file()
-            else :
-                self._in_progress_table.set_entry_attrs(existing_entry_addr,
-                                                        status=new_status,
-                                                        most_recent_message=datetime.datetime.now())
-
-    def _get_in_progress_address_for_rel_filepath(self,rel_filepath) :
-        existing_obj_addresses = self._in_progress_table.obj_addresses_by_key_attr('rel_filepath')
-        if rel_filepath not in existing_obj_addresses :
+            else:
+                self._in_progress_table.set_entry_attrs(
+                    existing_entry_addr,
+                    status=new_status,
+                    most_recent_message=datetime.datetime.now(),
+                )
+
+    def _get_in_progress_address_for_rel_filepath(self, rel_filepath):
+        existing_obj_addresses = self._in_progress_table.obj_addresses_by_key_attr(
+            "rel_filepath"
+        )
+        if rel_filepath not in existing_obj_addresses:
             return None
-        if len(existing_obj_addresses[rel_filepath])!=1 :
-            errmsg = f'ERROR: found more than one {self.__class__.__name__} entry for relative filepath '
-            errmsg+= f'{rel_filepath} in file at {self._in_progress_table.filepath}'
-            self.logger.error(errmsg,exc_type=ValueError)
+        if len(existing_obj_addresses[rel_filepath]) != 1:
+            errmsg = (
+                f"ERROR: found more than one {self.__class__.__name__} entry for "
+                f"relative filepath {rel_filepath} in file "
+                f"at {self._in_progress_table.filepath}"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
         return existing_obj_addresses[rel_filepath][0]
 
-    def _add_to_succeeded_table(self,new_entry,thread_identifier=None) :
-        if thread_identifier is None :
-            thread_identifier = f't{threading.get_ident()}'
-        if thread_identifier in self.__succeeded_tables_by_id :
-            if self.__succeeded_tables_by_id[thread_identifier].n_entries>=self.max_succeeded_lines_per_file :
+    def _add_to_succeeded_table(self, new_entry, thread_identifier=None):
+        if thread_identifier is None:
+            thread_identifier = f"t{threading.get_ident()}"
+        if thread_identifier in self.__succeeded_tables_by_id:
+            if (
+                self.__succeeded_tables_by_id[thread_identifier].n_entries
+                >= self.max_succeeded_lines_per_file
+            ):
                 old_fp = self.__succeeded_tables_by_id[thread_identifier].filepath
-                timestamp = str(datetime.datetime.now().timestamp()).replace('.','_')
-                new_fp = old_fp.with_name(f'{old_fp.stem}_{timestamp}{old_fp.suffix}')
+                timestamp = str(datetime.datetime.now().timestamp()).replace(".", "_")
+                new_fp = old_fp.with_name(f"{old_fp.stem}_{timestamp}{old_fp.suffix}")
                 old_fp.rename(new_fp)
-                new_table = DataclassTableAppendOnly(StreamHandlerRegistryLineSucceeded,
-                                                     filepath=old_fp,logger=self.logger)
+                new_table = DataclassTableAppendOnly(
+                    StreamHandlerRegistryLineSucceeded,
+                    filepath=old_fp,
+                    logger=self.logger,
+                )
                 self.__succeeded_tables_by_id[thread_identifier] = new_table
-        else :
-            new_name = f'{self.succeeded_filepath.stem}_{thread_identifier}{self.succeeded_filepath.suffix}'
+        else:
+            stem = self.succeeded_filepath.stem
+            suffix = self.succeeded_filepath.suffix
+            new_name = f"{stem}_{thread_identifier}{suffix}"
             new_fp = self.succeeded_filepath.with_name(new_name)
-            new_table = DataclassTableAppendOnly(StreamHandlerRegistryLineSucceeded,
-                                                 filepath=new_fp,logger=self.logger)
+            new_table = DataclassTableAppendOnly(
+                StreamHandlerRegistryLineSucceeded, filepath=new_fp, logger=self.logger
+            )
             self.__succeeded_tables_by_id[thread_identifier] = new_table
         self.__succeeded_tables_by_id[thread_identifier].add_entries(new_entry)
         self.__succeeded_tables_by_id[thread_identifier].dump_to_file()
 
-class StreamProcessorRegistry(StreamHandlerRegistry) :
+
+class StreamProcessorRegistry(StreamHandlerRegistry):
     """
     A class to keep track of the status of files read during stream processing
     """
 
-    FAILED = 'failed'
+    FAILED = "failed"
 
-    def __init__(self,dirpath,topic_name,consumer_group_id,*args,**kwargs) :
+    def __init__(self, dirpath, topic_name, consumer_group_id, *args, **kwargs):
         """
         dirpath    = path to the directory that should contain the csv files
-        topic_name = the name of the topic that will be produced to (used in the filenames)
+        topic_name = the name of the topic that will be produced to
         """
-        in_progress_filepath = dirpath / f'consuming_from_{topic_name}_in_progress_by_{consumer_group_id}.csv'
-        succeeded_filepath = dirpath / f'processed_from_{topic_name}_by_{consumer_group_id}.csv'
-        super().__init__(in_progress_filepath,succeeded_filepath,*args,**kwargs)
+        in_progress_filepath = (
+            dirpath
+            / f"consuming_from_{topic_name}_in_progress_by_{consumer_group_id}.csv"
+        )
+        succeeded_filepath = (
+            dirpath / f"processed_from_{topic_name}_by_{consumer_group_id}.csv"
+        )
+        super().__init__(in_progress_filepath, succeeded_filepath, *args, **kwargs)
 
-    def register_file_successfully_processed(self,dfc) :
+    def register_file_successfully_processed(self, dfc):
         """
         Add/update a line in the table to show that a file has successfully been processed
         """
         self._in_progress_table.lock.acquire()
-        existing_entry_addr = self._get_in_progress_address_for_rel_filepath(dfc.relative_filepath)
-        if existing_entry_addr is not None :
+        existing_entry_addr = self._get_in_progress_address_for_rel_filepath(
+            dfc.relative_filepath
+        )
+        if existing_entry_addr is not None:
             attrs = self._in_progress_table.get_entry_attrs(existing_entry_addr)
             self._in_progress_table.lock.release()
-            new_entry = StreamHandlerRegistryLineSucceeded(attrs['filename'],
-                                                           attrs['rel_filepath'],
-                                                           attrs['n_chunks'],
-                                                           attrs['first_message'],
-                                                           datetime.datetime.now())
-        else :
+            new_entry = StreamHandlerRegistryLineSucceeded(
+                attrs["filename"],
+                attrs["rel_filepath"],
+                attrs["n_chunks"],
+                attrs["first_message"],
+                datetime.datetime.now(),
+            )
+        else:
             self._in_progress_table.lock.release()
-            new_entry = StreamHandlerRegistryLineSucceeded(dfc.filename,
-                                                           dfc.relative_filepath,
-                                                           dfc.n_total_chunks,
-                                                           datetime.datetime.now(),
-                                                           datetime.datetime.now())
+            new_entry = StreamHandlerRegistryLineSucceeded(
+                dfc.filename,
+                dfc.relative_filepath,
+                dfc.n_total_chunks,
+                datetime.datetime.now(),
+                datetime.datetime.now(),
+            )
         self._add_to_succeeded_table(new_entry)
-        if existing_entry_addr is not None :
-            try :
+        if existing_entry_addr is not None:
+            try:
                 self._in_progress_table.remove_entries(existing_entry_addr)
                 self._in_progress_table.dump_to_file()
-            except ValueError :
+            except ValueError:
                 pass
 
-    def register_file_processing_failed(self,dfc) :
+    def register_file_processing_failed(self, dfc):
         """
         Add/update a line in the table to show that a file has failed to be processed
         """
-        self._add_or_modify_in_progress_entry(dfc,self.FAILED)
+        self._add_or_modify_in_progress_entry(dfc, self.FAILED)
+
 
-class StreamReproducerRegistry(StreamHandlerRegistry) :
+class StreamReproducerRegistry(StreamHandlerRegistry):
     """
-    A class to keep track of the status of files read from one topic with associated information
-    created and re-produced to a different topic
+    A class to keep track of the status of files read from one topic with associated
+    information created and re-produced to a different topic
     """
 
-    PRODUCING_MESSAGE_FAILED = 'producing_message_failed'
-    COMPUTING_RESULT_FAILED = 'computing_result_message_failed'
+    PRODUCING_MESSAGE_FAILED = "producing_message_failed"
+    COMPUTING_RESULT_FAILED = "computing_result_message_failed"
 
-    def __init__(self,dirpath,consumer_topic_name,producer_topic_name,consumer_group_id,*args,**kwargs) :
+    def __init__(
+        self,
+        dirpath,
+        consumer_topic_name,
+        producer_topic_name,
+        consumer_group_id,
+        *args,
+        **kwargs,
+    ):
         """
         dirpath    = path to the directory that should contain the csv file
         topic_name = the name of the topic that will be produced to (used in the filename)
         """
-        in_progress_filepath = dirpath / f'consuming_from_{consumer_topic_name}_in_progress_by_{consumer_group_id}.csv'
-        succeeded_filepath = dirpath / f'results_produced_to_{producer_topic_name}.csv'
-        super().__init__(in_progress_filepath,succeeded_filepath,*args,**kwargs)
-
-    def register_file_results_produced(self,filename,rel_filepath,n_total_chunks,prodid) :
+        in_progress_filepath = (
+            dirpath
+            / f"consuming_from_{consumer_topic_name}_in_progress_by_{consumer_group_id}.csv"
+        )
+        succeeded_filepath = dirpath / f"results_produced_to_{producer_topic_name}.csv"
+        super().__init__(in_progress_filepath, succeeded_filepath, *args, **kwargs)
+
+    def register_file_results_produced(
+        self, filename, rel_filepath, n_total_chunks, prodid
+    ):
         """
         Add/update a line in the table to show that a file has successfully been processed
         """
         self._in_progress_table.lock.acquire()
         existing_entry_addr = self._get_in_progress_address_for_rel_filepath(rel_filepath)
-        if existing_entry_addr is not None :
+        if existing_entry_addr is not None:
             attrs = self._in_progress_table.get_entry_attrs(existing_entry_addr)
             self._in_progress_table.lock.release()
-            new_entry = StreamHandlerRegistryLineSucceeded(attrs['filename'],
-                                                           attrs['rel_filepath'],
-                                                           attrs['n_chunks'],
-                                                           attrs['first_message'],
-                                                           datetime.datetime.now())
-        else :
+            new_entry = StreamHandlerRegistryLineSucceeded(
+                attrs["filename"],
+                attrs["rel_filepath"],
+                attrs["n_chunks"],
+                attrs["first_message"],
+                datetime.datetime.now(),
+            )
+        else:
             self._in_progress_table.lock.release()
-            new_entry = StreamHandlerRegistryLineSucceeded(filename,
-                                                           rel_filepath,
-                                                           n_total_chunks,
-                                                           datetime.datetime.now(),
-                                                           datetime.datetime.now())
-        self._add_to_succeeded_table(new_entry,f'p{prodid}')
-        if existing_entry_addr is not None :
-            try :
+            new_entry = StreamHandlerRegistryLineSucceeded(
+                filename,
+                rel_filepath,
+                n_total_chunks,
+                datetime.datetime.now(),
+                datetime.datetime.now(),
+            )
+        self._add_to_succeeded_table(new_entry, f"p{prodid}")
+        if existing_entry_addr is not None:
+            try:
                 self._in_progress_table.remove_entries(existing_entry_addr)
                 self._in_progress_table.dump_to_file()
-            except ValueError :
+            except ValueError:
                 pass
 
-    def register_file_computing_result_failed(self,filename,rel_filepath,n_total_chunks) :
+    def register_file_computing_result_failed(
+        self, filename, rel_filepath, n_total_chunks
+    ):
         """
         Update a line in the table to show that a file failed to have its processing result computed
         """
-        self._add_or_modify_in_progress_entry_without_chunk(filename,rel_filepath,n_total_chunks,
-                                                            self.COMPUTING_RESULT_FAILED)
-
-    def register_file_result_production_failed(self,filename,rel_filepath,n_total_chunks) :
-        """
-        Update a line in the table to show that the call to Producer.produce() for a message computed
-        from a file returned an error
-        """
-        self._add_or_modify_in_progress_entry_without_chunk(filename,rel_filepath,n_total_chunks,
-                                                            self.PRODUCING_MESSAGE_FAILED)
-
-    def _add_or_modify_in_progress_entry_without_chunk(self,filename,rel_filepath,n_total_chunks,new_status) :
-        with self._in_progress_table.lock :
-            existing_entry_addr = self._get_in_progress_address_for_rel_filepath(rel_filepath)
-            if existing_entry_addr is None :
-                new_entry = StreamHandlerRegistryLineInProgress(filename,
-                                                                rel_filepath,
-                                                                new_status,
-                                                                n_total_chunks,
-                                                                datetime.datetime.now(),
-                                                                datetime.datetime.now())
+        self._add_or_modify_in_progress_entry_without_chunk(
+            filename, rel_filepath, n_total_chunks, self.COMPUTING_RESULT_FAILED
+        )
+
+    def register_file_result_production_failed(
+        self, filename, rel_filepath, n_total_chunks
+    ):
+        """
+        Update a line in the table to show that the call to Producer.produce()
+         for a message computed from a file returned an error
+        """
+        self._add_or_modify_in_progress_entry_without_chunk(
+            filename, rel_filepath, n_total_chunks, self.PRODUCING_MESSAGE_FAILED
+        )
+
+    def _add_or_modify_in_progress_entry_without_chunk(
+        self, filename, rel_filepath, n_total_chunks, new_status
+    ):
+        with self._in_progress_table.lock:
+            existing_entry_addr = self._get_in_progress_address_for_rel_filepath(
+                rel_filepath
+            )
+            if existing_entry_addr is None:
+                new_entry = StreamHandlerRegistryLineInProgress(
+                    filename,
+                    rel_filepath,
+                    new_status,
+                    n_total_chunks,
+                    datetime.datetime.now(),
+                    datetime.datetime.now(),
+                )
                 self._in_progress_table.add_entries(new_entry)
                 self._in_progress_table.dump_to_file()
-            else :
-                self._in_progress_table.set_entry_attrs(existing_entry_addr,
-                                                        status=new_status,
-                                                        most_recent_message=datetime.datetime.now())
+            else:
+                self._in_progress_table.set_entry_attrs(
+                    existing_entry_addr,
+                    status=new_status,
+                    most_recent_message=datetime.datetime.now(),
+                )
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/config.py` & `openmsistream-1.4.0/openmsistream/data_file_io/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 """Constants used for internally processing file chunks and for some default parameter values"""
 
-#imports
+# imports
 import re
 
-class DataFileHandlingConstants :
+
+class DataFileHandlingConstants:
     """
     Constants for internally handling DataFileChunks
     """
 
-    CHUNK_ALREADY_WRITTEN_CODE = 10 # code indicating that a particular chunk has already been written
-    FILE_HASH_MISMATCH_CODE = -1 # code indicating that a file's hashes didn't match
-    FILE_SUCCESSFULLY_RECONSTRUCTED_CODE = 3 # code indicating that a file was successfully fully reconstructed
-    FILE_IN_PROGRESS = 2 # code indicating that a file is in the process of being reconstructed
+    CHUNK_ALREADY_WRITTEN_CODE = 10
+    FILE_HASH_MISMATCH_CODE = -1
+    FILE_SUCCESSFULLY_RECONSTRUCTED_CODE = 3
+    FILE_IN_PROGRESS = 2
+
 
-DATA_FILE_HANDLING_CONST=DataFileHandlingConstants()
+DATA_FILE_HANDLING_CONST = DataFileHandlingConstants()
 
-class RunOptionConstants :
+
+class RunOptionConstants:
     """
     Some default command line options/function kwargs
     """
 
-    DEFAULT_CONFIG_FILE = 'test' # name of the config file that will be used by default
-    DEFAULT_TOPIC_NAME = 'test' # name of the topic to produce to by default
-    PRODUCTION_CONFIG_FILE = 'prod' # name of the config file used in "real" production
-    N_DEFAULT_UPLOAD_THREADS = 2 # default number of threads to use when uploading a file
-    N_DEFAULT_DOWNLOAD_THREADS = 2 # default number of threads to use when downloading chunks of a file
-
-    #matches everything except something starting with a '.' or ending in '.log'
-    DEFAULT_UPLOAD_REGEX = re.compile(r'^((?!(\.|.*.log))).*$')
+    # name of the config file that will be used by default
+    DEFAULT_CONFIG_FILE = "test"
+    # name of the topic to produce to by default
+    DEFAULT_TOPIC_NAME = "test"
+    # name of the config file used in "real" production
+    PRODUCTION_CONFIG_FILE = "prod"
+    # default number of threads to use when uploading a file
+    N_DEFAULT_UPLOAD_THREADS = 2
+    # default number of threads to use when downloading chunks of a file
+    N_DEFAULT_DOWNLOAD_THREADS = 2
+
+    # matches everything except something starting with a '.' or ending in '.log'
+    DEFAULT_UPLOAD_REGEX = re.compile(r"^((?!(\.|.*.log))).*$")
+
+    # default size in bytes of each file upload chunk
+    DEFAULT_CHUNK_SIZE = 524288
+    # default maximum size (in MB) of the internal upload Queue
+    DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES = 500
 
-    DEFAULT_CHUNK_SIZE = 524288 # default size in bytes of each file upload chunk
-    DEFAULT_MAX_UPLOAD_QUEUE_MEGABYTES = 500 # default maximum size (in MB) of the internal upload Queue
 
 RUN_OPT_CONST = RunOptionConstants()
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/entity/data_file.py` & `openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """A single data file"""
 
-#imports
+# imports
 from ...utilities import LogOwner
 from ...utilities.misc import populated_kwargs
 
-class DataFile(LogOwner) :
+
+class DataFile(LogOwner):
     """
     Base class for representing a single data file
 
     :param filepath: the path to the file
     :type filepath: :class:`pathlib.Path`
     """
 
-    def __init__(self,filepath,*args,**kwargs) :
+    def __init__(self, filepath, *args, **kwargs):
         self.filepath = filepath
         self.filename = self.filepath.name
-        kwargs = populated_kwargs(kwargs,{'logger_file':self.filepath.parent})
-        super().__init__(*args,**kwargs)
+        kwargs = populated_kwargs(kwargs, {"logger_file": self.filepath.parent})
+        super().__init__(*args, **kwargs)
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/entity/data_file_chunk.py` & `openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_chunk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,232 +1,261 @@
 """A single chunk of a DataFile. Can be produced to a topic or consumed from one."""
 
-#imports
+# imports
 import pathlib
 from hashlib import sha512
 from ...utilities.logging import Logger
 from ...kafka_wrapper.producible import Producible
 from ..utilities import get_message_prepend
 
-class DataFileChunk(Producible) :
+
+class DataFileChunk(Producible):
     """
-    Class representing a single chunk of an uploaded or downloaded file. DataFileChunk objects are
-    automatically serialized/deserialized when they are produced/consumed to topics using OpenMSIStream.
+    Class representing a single chunk of an uploaded or downloaded file.
+    DataFileChunk objects are automatically serialized/deserialized when they are
+    produced/consumed to topics using OpenMSIStream.
 
-    :param filepath: path to this chunk's file (fully resolved if being produced, may be relative if it was consumed)
+    :param filepath: path to this chunk's file (fully resolved if being produced,
+        may be relative if it was consumed)
     :type filepath: :class:`pathlib.Path`
     :param filename: the name of the file
     :type filename: str
     :param file_hash: hash of this chunk's entire file data
     :type file_hash: str
     :param chunk_hash: hash of this chunk's data
     :type chunk_hash: str
     :param chunk_offset_read: offset (in bytes) of this chunk within the original file
     :type chunk_offset_read: int
-    :param chunk_offset_write: offset (in bytes) of this chunk within the reconstructed file (may be different than
-        chunk_offset_read due to excluding some bytes in uploading)
+    :param chunk_offset_write: offset (in bytes) of this chunk within the reconstructed file
+        (may be different than chunk_offset_read due to excluding some bytes in uploading)
     :type chunk_offset_write: int
     :param chunk_size: size of this chunk (in bytes)
     :type chunk_size: int
     :param chunk_i: index of this chunk within the larger file
     :type chunk_i: int
     :param n_total_chunks: the total number of chunks to expect from the original file
     :type n_total_chunks: int
-    :param rootdir: path to the "root" directory; anything beyond in the filepath is considered a subdirectory
-        (can also be set later)
+    :param rootdir: path to the "root" directory; anything beyond in the filepath is considered
+        a subdirectory (can also be set later)
     :type rootdir: :class:`pathlib.Path`, optional
-    :param filename_append: string to append to the stem of the filename when the file is reconstructed
+    :param filename_append: string to append to the stem of the filename when the file
+        is reconstructed
     :type filename_append: str, optional
-    :param data: the actual binary data of this chunk of the file (can be set later if this chunk is being produced
-        and not consumed)
+    :param data: the actual binary data of this chunk of the file (can be set later
+        if this chunk is being produced and not consumed)
     :type data: bytes, optional
     """
 
     #################### PROPERTIES ####################
 
     @property
-    def filepath(self) :
+    def filepath(self):
         """
         The path to the file
         """
         return self.__filepath
 
     @property
-    def relative_filepath(self) :
+    def relative_filepath(self):
         """
         The path to the file, relative to its root directory (if it has one)
         """
         return self.__relative_filepath
 
     @property
-    def rootdir(self) :
+    def rootdir(self):
         """
         The path to the file's root directory (already set if chunk is to be produced,
         but must be set later if chunk is a consumed message)
         """
         return self.__rootdir
 
     @rootdir.setter
-    def rootdir(self,rootdir) :
+    def rootdir(self, rootdir):
         """
         Also resets the overall filepath (used in consuming messages for files in subdirectories)
         """
-        self.__rootdir=rootdir
-        if rootdir is not None :
-            try :
+        self.__rootdir = rootdir
+        if rootdir is not None:
+            try:
                 self.__filepath = self.__filepath.relative_to(self.__rootdir)
-            except ValueError :
+            except ValueError:
                 pass
             self.__filepath = self.__rootdir / self.__filepath
             self.__relative_filepath = self.__filepath.relative_to(self.__rootdir)
 
     @property
-    def subdir_str(self) :
+    def subdir_str(self):
         """
         A string representation of the path to the file, relative to its root directory
         """
-        if self.__rootdir is None :
+        if self.__rootdir is None:
             parentdir_as_posix = self.__filepath.parent.as_posix()
-            if parentdir_as_posix=='.' :
-                return ''
+            if parentdir_as_posix == ".":
+                return ""
             return parentdir_as_posix
         relpath = self.__filepath.parent.relative_to(self.__rootdir)
-        if relpath==pathlib.Path() :
-            return ''
+        if relpath == pathlib.Path():
+            return ""
         return relpath.as_posix()
 
     @property
-    def msg_key(self) :
+    def msg_key(self):
         """
         string representing the key of the message this chunk will be produced as
         """
-        key_pp = get_message_prepend(self.subdir_str,self.filename)
-        return f'{key_pp}_{self.chunk_i}_of_{self.n_total_chunks}'
+        key_pp = get_message_prepend(self.subdir_str, self.filename)
+        return f"{key_pp}_{self.chunk_i}_of_{self.n_total_chunks}"
 
     @property
-    def msg_value(self) :
+    def msg_value(self):
         """
         value of the message this chunk will be produced as (just the object itself, since a
         :class:`DataFileChunkSerializer` is used)
         """
         return self
 
     @property
     def callback_kwargs(self):
         """
-        keyword arguments that should be sent to the producer callback function when the chunk is produced
+        keyword arguments that should be sent to the producer callback function
+        when the chunk is produced
         """
         return {
-            'filepath' : self.__filepath,
-            'filename' : self.filename,
-            'n_total_chunks' : self.n_total_chunks,
-            'chunk_i' : self.chunk_i,
-            }
-
+            "filepath": self.__filepath,
+            "filename": self.filename,
+            "n_total_chunks": self.n_total_chunks,
+            "chunk_i": self.chunk_i,
+        }
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,filepath,filename,file_hash,chunk_hash,chunk_offset_read,chunk_offset_write,chunk_size,chunk_i,
-                 n_total_chunks,rootdir=None,filename_append='',data=None) :
+    def __init__(
+        self,
+        filepath,
+        filename,
+        file_hash,
+        chunk_hash,
+        chunk_offset_read,
+        chunk_offset_write,
+        chunk_size,
+        chunk_i,
+        n_total_chunks,
+        rootdir=None,
+        filename_append="",
+        data=None,
+    ):
         self.__filepath = filepath
         self.filename = filename
         self.file_hash = file_hash
         self.chunk_hash = chunk_hash
         self.chunk_offset_read = chunk_offset_read
         self.chunk_offset_write = chunk_offset_write
         self.chunk_size = chunk_size
         self.chunk_i = chunk_i
         self.n_total_chunks = n_total_chunks
         self.__rootdir = rootdir
-        if self.__rootdir is not None :
+        if self.__rootdir is not None:
             self.__relative_filepath = self.__filepath.relative_to(self.__rootdir)
-        else :
+        else:
             self.__relative_filepath = self.__filepath
         self.filename_append = filename_append
         self.data = data
 
-    def __eq__(self,other) :
-        if not isinstance(other,DataFileChunk) :
+    def __eq__(self, other):
+        if not isinstance(other, DataFileChunk):
             return NotImplemented
-        #compare everything but the filepath
+        # compare everything but the filepath
         retval = self.filename == other.filename
         retval = retval and self.file_hash == other.file_hash
         retval = retval and self.chunk_hash == other.chunk_hash
         retval = retval and self.chunk_offset_write == other.chunk_offset_write
         retval = retval and self.chunk_size == other.chunk_size
         retval = retval and self.chunk_i == other.chunk_i
         retval = retval and self.n_total_chunks == other.n_total_chunks
         retval = retval and self.subdir_str == other.subdir_str
         retval = retval and self.filename_append == other.filename_append
         retval = retval and self.data == other.data
         return retval
 
-    def __str__(self) :
-        string_rep = 'DataFileChunk('
-        string_rep+=f'filename: {self.filename}, '
-        string_rep+=f'file_hash: {self.file_hash}, '
-        string_rep+=f'chunk_hash: {self.chunk_hash}, '
-        string_rep+=f'chunk_offset_read: {self.chunk_offset_read}, '
-        string_rep+=f'chunk_offset_write: {self.chunk_offset_write}, '
-        string_rep+=f'chunk_size: {self.chunk_size}, '
-        string_rep+=f'chunk_i: {self.chunk_i}, '
-        string_rep+=f'n_total_chunks: {self.n_total_chunks}, '
-        string_rep+=f'subdir_str: {self.subdir_str}, '
-        string_rep+=f'filename_append: {self.filename_append}, '
-        #string_rep+=f'data: {self.data}, '
-        string_rep+=')'
+    def __str__(self):
+        string_rep = (
+            "DataFileChunk("
+            f"filename: {self.filename}, "
+            f"file_hash: {self.file_hash}, "
+            f"chunk_hash: {self.chunk_hash}, "
+            f"chunk_offset_read: {self.chunk_offset_read}, "
+            f"chunk_offset_write: {self.chunk_offset_write}, "
+            f"chunk_size: {self.chunk_size}, "
+            f"chunk_i: {self.chunk_i}, "
+            f"n_total_chunks: {self.n_total_chunks}, "
+            f"subdir_str: {self.subdir_str}, "
+            f"filename_append: {self.filename_append})"  # , '
+            # f'data: {self.data})'
+        )
         return string_rep
 
-    def __hash__(self) :
+    def __hash__(self):
         return super().__hash__()
 
     def get_log_msg(self, print_every=None):
         """
         If the chunk's index mod ``print_every`` is 0, or if the chunk is the last one for the file,
         returns a message to log. Otherwise returns None.
 
         :param print_every: number of chunks that should be skipped between logging messages
         :type print_every: int, optional
 
         :return: message to log stating which chunk from which file is being uploaded
         :rtype: str, or None
         """
-        if (print_every and (self.chunk_i-1)%print_every==0) or self.chunk_i==self.n_total_chunks :
-            return f'uploading {self.filename} chunk {self.chunk_i} (out of {self.n_total_chunks})'
+        if (
+            print_every and (self.chunk_i - 1) % print_every == 0
+        ) or self.chunk_i == self.n_total_chunks:
+            return f"uploading {self.filename} chunk {self.chunk_i} (out of {self.n_total_chunks})"
         return None
 
-    def populate_with_file_data(self,logger=None) :
+    def populate_with_file_data(self, logger=None):
         """
-        Populate this chunk with the actual data from the file. Called only when this chunk is being produced.
+        Populate this chunk with the actual data from the file.
+        Called only when this chunk is being produced.
 
-        :param logger: a logger object to use to log errors that may arise in populating the file chunk
+        :param logger: a logger object to use to log errors that may arise
+            in populating the file chunk
         :type logger: :class:`~.utilities.Logger`, optional
 
         :raises FileNotFoundError: if the file doesn't exist on disk at ``self.filepath``
         :raises ValueError: if the data read from the file is not of the expected size,
             or if its hash is not matched to what was originally calculated.
         """
-        #create a new logger if one isn't given
-        if logger is None :
+        # create a new logger if one isn't given
+        if logger is None:
             logger = Logger(self.__class__.__name__)
-        #make sure the file exists
-        if not self.filepath.is_file() :
-            logger.error(f'ERROR: file {self.filepath} does not exist!',exc_type=FileNotFoundError)
-        #get the data from the file
+        # make sure the file exists
+        if not self.filepath.is_file():
+            logger.error(
+                f"ERROR: file {self.filepath} does not exist!", exc_type=FileNotFoundError
+            )
+        # get the data from the file
         with open(self.filepath, "rb") as fp:
             fp.seek(self.chunk_offset_read)
             data = fp.read(self.chunk_size)
-        #make sure it's of the expected size
+        # make sure it's of the expected size
         if len(data) != self.chunk_size:
-            msg = f'ERROR: chunk {self.chunk_hash} size {len(data)} != expected size {self.chunk_size} in file '
-            msg+= f'{self.filepath}, offset {self.chunk_offset_read}'
-            logger.error(msg,exc_type=ValueError)
-        #check that its hash matches what was found at the time of putting it in the queue
+            msg = (
+                f"ERROR: chunk {self.chunk_hash} size {len(data)} != expected size "
+                f"{self.chunk_size} in file {self.filepath}, "
+                f"offset {self.chunk_offset_read}"
+            )
+            logger.error(msg, exc_type=ValueError)
+        # check that its hash matches what was found at the time of putting it in the queue
         check_chunk_hash = sha512()
         check_chunk_hash.update(data)
         check_chunk_hash = check_chunk_hash.digest()
         if self.chunk_hash != check_chunk_hash:
-            msg = f'ERROR: chunk hash {check_chunk_hash} != expected hash {self.chunk_hash} in file {self.filepath}, '
-            msg+= f'offset {self.chunk_offset_read}'
-            logger.error(msg,exc_type=ValueError)
-        #set the chunk's data value
+            msg = (
+                f"ERROR: chunk hash {check_chunk_hash} != expected hash {self.chunk_hash} "
+                f"in file {self.filepath}, offset {self.chunk_offset_read}"
+            )
+            logger.error(msg, exc_type=ValueError)
+        # set the chunk's data value
         self.data = data
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/entity/download_data_file.py` & `openmsistream-1.4.0/openmsistream/data_file_io/entity/download_data_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,256 +1,279 @@
 """Various types of DataFiles that have been read back from messages in a topic"""
 
-#imports
+# imports
 import pathlib, os
 from hashlib import sha512
 from contextlib import nullcontext
 from abc import ABC, abstractmethod
 from ..config import DATA_FILE_HANDLING_CONST
 from .data_file import DataFile
 
-class DownloadDataFile(DataFile,ABC) :
+
+class DownloadDataFile(DataFile, ABC):
     """
     Class to represent a data file that will be read as messages from a topic
 
     :param filepath: Path to the file
     :type filepath: :class:`pathlib.Path`
     """
 
     #################### PROPERTIES AND STATIC METHODS ####################
 
     @staticmethod
-    def get_full_filepath(dfc) :
+    def get_full_filepath(dfc):
         """
         Return the full filepath of a downloaded file given one of its DataFileChunks
 
         :param dfc: One of the DataFileChunk objects contributing to the file
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
 
         :return: the full path to the file
         :rtype: :class:`pathlib.Path`
         """
-        if dfc.filename_append=='' :
+        if dfc.filename_append == "":
             return dfc.filepath
-        return dfc.filepath.with_name(dfc.filepath.stem+dfc.filename_append+dfc.filepath.suffix)
+        return dfc.filepath.with_name(
+            dfc.filepath.stem + dfc.filename_append + dfc.filepath.suffix
+        )
 
     @property
     @abstractmethod
-    def check_file_hash(self) :
+    def check_file_hash(self):
         """
         The hash of the data in the file after it was read. Not implemented in the base class.
         """
         raise NotImplementedError
 
     @property
-    def relative_filepath(self) :
+    def relative_filepath(self):
         """
         The path to the file, relative to its root directory
         """
-        if self.subdir_str=='' :
+        if self.subdir_str == "":
             return pathlib.Path(self.filename)
-        return pathlib.Path(self.subdir_str+'/'+self.filename)
+        return pathlib.Path(self.subdir_str + "/" + self.filename)
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,filepath,*args,**kwargs) :
-        super().__init__(filepath,*args,**kwargs)
-        #start an empty set of this file's downloaded offsets
+    def __init__(self, filepath, *args, **kwargs):
+        super().__init__(filepath, *args, **kwargs)
+        # start an empty set of this file's downloaded offsets
         self._chunk_offsets_downloaded = []
         self.full_filepath = None
         self.subdir_str = None
         self.n_total_chunks = None
 
-    def add_chunk(self,dfc,thread_lock=nullcontext()) :
+    def add_chunk(self, dfc, thread_lock=nullcontext()):
         """
         Process a chunk that's been read from a topic.
         Returns a number of codes based on what effect adding the chunk had.
 
         This function calls :func:`~_on_add_chunk`,
         with the :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` as the argument.
 
         :param dfc: the DataFileChunk object whose data should be added
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
-        :param thread_lock: the lock object to acquire/release so that race conditions don't affect reconstruction
-                            of the files (only needed if running this function asynchronously)
+        :param thread_lock: the lock object to acquire/release so that race conditions
+            don't affect reconstruction of the files
+            (only needed if running this function asynchronously)
         :type thread_lock: :class:`threading.Lock`, optional
 
-        :return: an internal code indicating whether the chunk: was successfully added to a file in progress,
-            was already received, was the last chunk needed and the file is successfully reconstructed according
-            to its hash or the post-reconstruction has is mismatched to the hash of the file contents originally
-            read from disk.
+        :return: an internal code indicating whether the chunk: was successfully added to
+            a file in progress, was already received, was the last chunk needed and
+            the file is successfully reconstructed according to its hash or the
+            post-reconstruction hash is mismatched to the hash of the file contents
+            originally read from disk.
         :rtype: int
         """
-        #if this chunk's offset has already been written to disk, return the "already written" code
-        with thread_lock :
+        # if this chunk's offset has already been written to disk, return the "already written" code
+        with thread_lock:
             already_written = dfc.chunk_offset_write in self._chunk_offsets_downloaded
-        if already_written :
+        if already_written:
             return DATA_FILE_HANDLING_CONST.CHUNK_ALREADY_WRITTEN_CODE
-        #the filepath of this DownloadDataFile and of the given DataFileChunk must match
-        if dfc.filepath!=self.filepath :
-            errmsg = f'ERROR: filepath mismatch between data file chunk with {dfc.filepath} and '
-            errmsg+= f'data file with {self.filepath}'
-            self.logger.error(errmsg,exc_type=ValueError)
-        #modify the filepath to include any append to the name
+        # the filepath of this DownloadDataFile and of the given DataFileChunk must match
+        if dfc.filepath != self.filepath:
+            errmsg = (
+                f"ERROR: filepath mismatch between data file chunk with {dfc.filepath} "
+                f"and data file with {self.filepath}"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        # modify the filepath to include any append to the name
         full_filepath = self.__class__.get_full_filepath(dfc)
-        if self.full_filepath is None :
+        if self.full_filepath is None:
             self.full_filepath = full_filepath
             self.filename = self.full_filepath.name
-        elif self.full_filepath!=full_filepath :
-            errmsg = f'ERROR: filepath for data file chunk {dfc.chunk_i}/{dfc.n_total_chunks} with offset '
-            errmsg+= f'{dfc.chunk_offset_write} is {full_filepath} but the file being reconstructed is '
-            errmsg+= f'expected to have filepath {self.full_filepath}'
-            self.logger.error(errmsg,exc_type=ValueError)
-        #add the subdirectory string to this file
-        if self.subdir_str is None :
+        elif self.full_filepath != full_filepath:
+            errmsg = (
+                f"ERROR: filepath for data file chunk {dfc.chunk_i}/{dfc.n_total_chunks} "
+                f"with offset {dfc.chunk_offset_write} is {full_filepath} but the file "
+                f"being reconstructed is expected to have filepath {self.full_filepath}"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        # add the subdirectory string to this file
+        if self.subdir_str is None:
             self.subdir_str = dfc.subdir_str
-        elif self.subdir_str!=dfc.subdir_str :
-            errmsg = f"Mismatched subdirectory strings! From file = {self.subdir_str}, from chunk = {dfc.subdir_str}"
-            self.logger.error(errmsg,exc_type=ValueError)
-        #set or check the total number of chunks expected
-        if self.n_total_chunks is None :
-            with thread_lock :
+        elif self.subdir_str != dfc.subdir_str:
+            errmsg = (
+                f"Mismatched subdirectory strings! From file = {self.subdir_str}, "
+                f"from chunk = {dfc.subdir_str}"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        # set or check the total number of chunks expected
+        if self.n_total_chunks is None:
+            with thread_lock:
                 self.n_total_chunks = dfc.n_total_chunks
-        elif self.n_total_chunks!=dfc.n_total_chunks :
-            errmsg = f'ERROR: {self.__class__.__name__} with filepath {self.full_filepath} is expecting '
-            errmsg+= f'{self.n_total_chunks} chunks but found a chunk from a split with '
-            errmsg+= f'{dfc.n_total_chunks} total chunks.'
-            self.logger.error(errmsg,exc_type=ValueError)
-        #acquire the thread lock to make sure this process is the only one dealing with this particular file
-        with thread_lock :
-            #call the function to actually add the chunk
+        elif self.n_total_chunks != dfc.n_total_chunks:
+            errmsg = (
+                f"ERROR: {self.__class__.__name__} with filepath {self.full_filepath} "
+                f"is expecting {self.n_total_chunks} chunks but found a chunk from a split "
+                f"with {dfc.n_total_chunks} total chunks."
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        with thread_lock:
+            # call the function to actually add the chunk
             self._on_add_chunk(dfc)
-            #add the offset of the added chunk to the set of reconstructed file chunks
+            # add the offset of the added chunk to the set of reconstructed file chunks
             self._chunk_offsets_downloaded.append(dfc.chunk_offset_write)
-            last_chunk = len(self._chunk_offsets_downloaded)==dfc.n_total_chunks
-        #if this chunk was the last that needed to be added, check the hashes
-        if last_chunk :
-            if self.check_file_hash!=dfc.file_hash :
+            last_chunk = len(self._chunk_offsets_downloaded) == dfc.n_total_chunks
+        # if this chunk was the last that needed to be added, check the hashes
+        if last_chunk:
+            if self.check_file_hash != dfc.file_hash:
                 return DATA_FILE_HANDLING_CONST.FILE_HASH_MISMATCH_CODE
             return DATA_FILE_HANDLING_CONST.FILE_SUCCESSFULLY_RECONSTRUCTED_CODE
         return DATA_FILE_HANDLING_CONST.FILE_IN_PROGRESS
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
     @abstractmethod
-    def _on_add_chunk(self,dfc) :
+    def _on_add_chunk(self, dfc):
         """
         A function to actually process a new chunk being added to the file.
-        This function is executed while a thread lock is acquired so it will never run asynchronously.
-        Also any DataFileChunks passed to this function are guaranteed to have unique offsets.
+        This function is executed while a thread lock is acquired so it will never
+        run asynchronously. Also any DataFileChunks passed to this function are
+        guaranteed to have unique offsets.
 
         Not implemented in the base class.
 
         :param dfc: the DataFileChunk object whose data should be added
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
         """
         raise NotImplementedError
 
-class DownloadDataFileToDisk(DownloadDataFile) :
+
+class DownloadDataFileToDisk(DownloadDataFile):
     """
-    Class to represent a data file that will be reconstructed on disk using messages read from a topic
+    Class to represent a data file that will be reconstructed on disk
+    using messages read from a topic
 
     :param filepath: Path to the file
     :type filepath: :class:`pathlib.Path`
     """
 
     #################### PROPERTIES ####################
 
     @property
-    def check_file_hash(self) :
+    def check_file_hash(self):
         """
         Hash of the file contents as read from its current location on disk
         """
         check_file_hash = sha512()
-        with open(self.full_filepath,'rb') as fp :
+        with open(self.full_filepath, "rb") as fp:
             data = fp.read()
         check_file_hash.update(data)
         return check_file_hash.digest()
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,filepath,*args,**kwargs) :
-        super().__init__(filepath,*args,**kwargs)
-        #create the parent directory of the file if it doesn't exist yet (in case the file is in a new subdirectory)
-        if not self.filepath.parent.is_dir() :
+    def __init__(self, filepath, *args, **kwargs):
+        super().__init__(filepath, *args, **kwargs)
+        # create the parent directory of the file if it doesn't exist yet
+        if not self.filepath.parent.is_dir():
             self.filepath.parent.mkdir(parents=True)
 
-    def _on_add_chunk(self,dfc) :
+    def _on_add_chunk(self, dfc):
         """
         Add the data from a given file chunk to this file on disk
 
         :param dfc: the DataFileChunk object whose data should be added
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
         """
-        mode = 'r+b' if self.full_filepath.is_file() else 'w+b'
-        with open(self.full_filepath,mode) as fp :
+        mode = "r+b" if self.full_filepath.is_file() else "w+b"
+        with open(self.full_filepath, mode) as fp:
             fp.seek(dfc.chunk_offset_write)
             fp.write(dfc.data)
             fp.flush()
             os.fsync(fp.fileno())
             fp.close()
 
-class DownloadDataFileToMemory(DownloadDataFile) :
+
+class DownloadDataFileToMemory(DownloadDataFile):
     """
-    Class to represent a data file that will be held in memory and populated by the contents of messages from a topic
+    Class to represent a data file that will be held in memory
+    and populated by the contents of messages from a topic
 
     :param filepath: Path to the file
     :type filepath: :class:`pathlib.Path`
     """
 
     #################### PROPERTIES ####################
 
     @property
-    def bytestring(self) :
+    def bytestring(self):
         """
-        The bytestring of the file contents (like calling file_pointer.read() for a file opened in "rb" mode).
-        Call bytestring.decode() to convert this to a text string.
+        The bytestring of the file contents (like calling file_pointer.read() for a file
+        opened in "rb" mode). Call bytestring.decode() to convert this to a text string.
         """
-        if self.__bytestring is None :
+        if self.__bytestring is None:
             self.__create_bytestring()
         return self.__bytestring
 
     @bytestring.setter
-    def bytestring(self,new_bytestring) :
-        if self.__bytestring is not None :
-            warnmsg = f'WARNING: resetting a non-None bytestring for {self.__class__.__name__} '
-            warnmsg+= f'with path {self.filepath}'
+    def bytestring(self, new_bytestring):
+        if self.__bytestring is not None:
+            warnmsg = (
+                f"WARNING: resetting a non-None bytestring for {self.__class__.__name__} "
+                f"with path {self.filepath}"
+            )
             self.logger.warning(warnmsg)
         self.__bytestring = new_bytestring
 
     @property
-    def check_file_hash(self) :
+    def check_file_hash(self):
         """
         The hash of the file contents determined from the bytestring of the file stored in memory
         """
         check_file_hash = sha512()
         check_file_hash.update(self.bytestring)
         return check_file_hash.digest()
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,filepath,*args,**kwargs) :
-        super().__init__(filepath,*args,**kwargs)
-        #start a dictionary of the file data by their offsets
+    def __init__(self, filepath, *args, **kwargs):
+        super().__init__(filepath, *args, **kwargs)
+        # start a dictionary of the file data by their offsets
         self.__chunk_data_by_offset = {}
-        #placeholder for the eventual full data bytestring
+        # placeholder for the eventual full data bytestring
         self.__bytestring = None
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def _on_add_chunk(self,dfc) :
+    def _on_add_chunk(self, dfc):
         """
         Add the data from a given file chunk to the dictionary of data by offset
 
         :param dfc: the DataFileChunk object whose data should be added
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
         """
         self.__chunk_data_by_offset[dfc.chunk_offset_write] = dfc.data
 
-    def __create_bytestring(self) :
+    def __create_bytestring(self):
         """
-        Makes all of the data held in the dictionary into a single bytestring ordered by offset of each chunk
+        Makes all of the data held in the dictionary into a single bytestring
         """
-        bytestring = b''
-        for data in [self.__chunk_data_by_offset[offset] for offset in sorted(self.__chunk_data_by_offset.keys())] :
-            bytestring+=data
+        bytestring = b""
+        for data in [
+            self.__chunk_data_by_offset[offset]
+            for offset in sorted(self.__chunk_data_by_offset.keys())
+        ]:
+            bytestring += data
         self.__bytestring = bytestring
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/entity/reproducer_message.py` & `openmsistream-1.4.0/openmsistream/data_file_io/entity/reproducer_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """Base class for messages computed from reconstructed data files and produced to new topics"""
 
-#imports
+# imports
 from abc import ABC
 from ...kafka_wrapper.producible import Producible
 from ..utilities import get_message_prepend
 
-class ReproducerMessage(Producible,ABC) :
+
+class ReproducerMessage(Producible, ABC):
     """
     Abstract base class for messages that are computed from data files and produced to a new topic
 
     :param datafile: The DataFile object used to compute this message
     :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
     """
 
     @property
-    def msg_key(self) :
+    def msg_key(self):
         """
         The automatically defined key for these messages is a string version of the path
         to the original file with "_processing_result" appended
         """
-        key_pp = get_message_prepend(self.__datafile.subdir_str,self.__datafile.filename)
-        return f'{key_pp}_processing_result'
+        key_pp = get_message_prepend(self.__datafile.subdir_str, self.__datafile.filename)
+        return f"{key_pp}_processing_result"
 
     @property
-    def callback_kwargs(self) :
+    def callback_kwargs(self):
         """
-        The callback kwargs defined for these messages are the original datafile name, its relative filepath,
-        and the total number of chunks into which the file was broken.
+        The callback kwargs defined for these messages are the original datafile name,
+        its relative filepath, and the total number of chunks into which the file was broken.
         """
-        return {'filename':self.__datafile.filename,
-                'rel_filepath':self.__datafile.relative_filepath,
-                'n_total_chunks':self.__datafile.n_total_chunks}
+        return {
+            "filename": self.__datafile.filename,
+            "rel_filepath": self.__datafile.relative_filepath,
+            "n_total_chunks": self.__datafile.n_total_chunks,
+        }
 
-    def get_log_msg(self,print_every=None) :
+    def get_log_msg(self, print_every=None):
         """
-        Prints a message saying that the processing result from [filepath] is being produced, if print_every is defined
+        Prints a message saying that the processing result from [filepath] is being produced,
+        if print_every is defined
         """
-        if print_every :
-            return f'Producing processing result from {self.__datafile.filepath}'
+        if print_every:
+            return f"Producing processing result from {self.__datafile.filepath}"
         return None
 
-    def __init__(self,datafile,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
+    def __init__(self, datafile, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.__datafile = datafile
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/entity/upload_data_file.py` & `openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_data_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,365 +1,451 @@
 """A DataFile that will be broken into chunks and uploaded to a topic"""
 
-#imports
-import time
+# imports
+import time, datetime
 from threading import Thread
 from queue import Queue
 from hashlib import sha512
 from ...utilities import Runnable
 from ...kafka_wrapper import ProducerGroup
 from ..config import RUN_OPT_CONST
 from .. import DataFile
 from .data_file_chunk import DataFileChunk
 
-class UploadDataFile(DataFile,Runnable) :
+
+class UploadDataFile(DataFile, Runnable):
     """
     Class to represent a data file whose messages will be uploaded to a topic
 
     Used as part of a :class:`~.DataFileUploadDirectory`, but can also be run standalone
     to upload a single file.
 
     :param filepath: The path to the file on disk
     :type filepath: :class:`pathlib.Path`
-    :param to_upload: True (default) if the file should be uploaded. Used to set the existing files as
-        "already uploaded" when running a :class:`~.DataFileUploadDirectory`.
+    :param to_upload: True (default) if the file should be uploaded. Used to set the existing files
+        as "already uploaded" when running a :class:`~.DataFileUploadDirectory`.
     :type to_upload: bool, optional
-    :param rootdir: path to the "root" directory that this file is in. Anything in the path beyond it
-        will be added to the DataFileChunk so that it will be reconstructed inside a subdirectory
+    :param rootdir: path to the "root" directory that this file is in. Anything in the path
+        beyond it will be added to the DataFileChunk so that it will be reconstructed
+        inside a subdirectory
     :type rootdir: None or :class:`pathlib.Path`, optional
-    :param filename_append: a string that should be appended to the end of the filename stem to distinguish the file
-        that's produced from its original file on disk
+    :param filename_append: a string that should be appended to the end of the filename stem
+        to distinguish the file that's produced from its original file on disk
     :type filename_append: None or str, optional
     """
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,filepath,to_upload=True,rootdir=None,filename_append=None,**kwargs) :
+    def __init__(
+        self, filepath, to_upload=True, rootdir=None, filename_append=None, **kwargs
+    ):
         """
         Constructor method
         """
-        super().__init__(filepath,**kwargs)
+        super().__init__(filepath, **kwargs)
         self.__to_upload = to_upload
-        if rootdir is None :
-            self.rootdir = self.filepath.parent
-        else :
-            self.rootdir = rootdir
-        self.__filename_append = filename_append if filename_append is not None else ''
+        self.rootdir = self.filepath.parent if rootdir is None else rootdir
+        self.__filename_append = filename_append if filename_append is not None else ""
         self.__fully_enqueued = False
         self.__fully_produced = False
         self.chunks_to_upload = []
         self.__n_total_chunks = 0
         self.__chunk_infos = None
         self.__file_hash = None
+        self.__chunked_at_timestamp = None
 
-    def upload_whole_file(self,config_path,topic_name,
-                          n_threads=RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
-                          chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE) :
+    def upload_whole_file(
+        self,
+        config_path,
+        topic_name,
+        n_threads=RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS,
+        chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
+    ):
         """
         Chunk and upload an entire file on disk to a broker's topic.
 
-        :param config_path: Path to the config file to use in defining the Broker connection and Producers
+        :param config_path: Path to the config file to use in defining the Broker connection
+            and Producers
         :type config_path: :class:`pathlib.Path`
         :param topic_name: Name of the topic to which the file's messages should be produced
         :type topic_name: str
         :param n_threads: The number of threads/Producers to run at once during uploading
         :type n_threads: int, optional
         :param chunk_size: The size of the file chunk in each message in bytes
         :type chunk_size: int, optional
         """
-        startup_msg = f"Uploading entire file {self.filepath} to {topic_name} in {chunk_size} byte chunks "
-        startup_msg+=f"using {n_threads} threads...."
+        startup_msg = (
+            f"Uploading {self.filepath} to {topic_name} in {chunk_size}-byte chunks "
+            f"using {n_threads} threads...."
+        )
         self.logger.info(startup_msg)
-        #add all the chunks to the upload queue
+        # add all the chunks to the upload queue
         upload_queue = Queue()
-        self.enqueue_chunks_for_upload(upload_queue,chunk_size=chunk_size)
-        #add "None" to the queue for each thread as the final values
-        for _ in range(n_threads) :
+        self.enqueue_chunks_for_upload(upload_queue, chunk_size=chunk_size)
+        # add "None" to the queue for each thread as the final values
+        for _ in range(n_threads):
             upload_queue.put(None)
-        #produce all the messages in the queue using multiple threads
-        producer_group = ProducerGroup(config_path,logger=self.logger)
+        # produce all the messages in the queue using multiple threads
+        producer_group = ProducerGroup(config_path, logger=self.logger)
         producers = []
         upload_threads = []
-        for _ in range(n_threads) :
+        for _ in range(n_threads):
             producers.append(producer_group.get_new_producer())
-            thread = Thread(target=producers[-1].produce_from_queue_looped, args=(upload_queue,topic_name))
+            thread = Thread(
+                target=producers[-1].produce_from_queue_looped,
+                args=(upload_queue, topic_name),
+            )
             thread.start()
             upload_threads.append(thread)
-        #join the threads
-        for u_t in upload_threads :
+        # join the threads
+        for u_t in upload_threads:
             u_t.join()
-        self.logger.info('Waiting for all enqueued messages to be delivered (this may take a moment)....')
-        for producer in producers :
-            producer.flush(timeout=-1) #don't leave the function until all messages have been sent/received
+        self.logger.info(
+            "Waiting for all enqueued messages to be delivered (this may take a moment)...."
+        )
+        for producer in producers:
+            producer.flush(
+                timeout=-1
+            )  # don't leave the function until all messages have been sent/received
             producer.close()
         producer_group.close()
-        self.logger.info(f'Done uploading {self.filepath}')
+        self.logger.info(f"Done uploading {self.filepath}")
 
-    def add_chunks_to_upload(self,chunks_to_add=None,chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE) :
+    def add_chunks_to_upload(
+        self, chunks_to_add=None, chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE
+    ):
         """
         Add chunks from this file to the internal list of chunks to upload,
         possibly with some selection defined by :attr:`~select_bytes`
 
-        :param chunks_to_add: a list of chunk indices to add to the list to be uploaded (Default=None adds all chunks)
+        :param chunks_to_add: a list of chunk indices to add to the list to be uploaded
+            (Default=None adds all chunks)
         :type chunks_to_add: None or list[int], optional
         :param chunk_size: The size of the file chunk in each message in bytes
         :type chunk_size: int, optional
         """
-        if self.__chunk_infos is None :
-            try :
+        if self.__chunk_infos is None:
+            try:
                 self._build_list_of_file_chunks(chunk_size)
-            except Exception as exc :
-                fp = self.filepath.relative_to(self.rootdir) if self.rootdir is not None else self.filepath
-                errmsg = f'ERROR: was not able to break {fp} into chunks for uploading. '
-                errmsg+= 'Check log lines below for details on what went wrong. File will not be uploaded.'
-                self.logger.error(errmsg,exc_info=exc)
+            except Exception as exc:
+                fp = (
+                    self.filepath.relative_to(self.rootdir)
+                    if self.rootdir is not None
+                    else self.filepath
+                )
+                errmsg = (
+                    f"ERROR: was not able to break {fp} into chunks for uploading. "
+                    "Check log lines below for details. File will not be uploaded."
+                )
+                self.logger.error(errmsg, exc_info=exc)
                 self.__to_upload = False
                 return
-        #add the chunks to the final list as DataFileChunk objects
-        for ichunk,chunk in enumerate(self.__chunk_infos,start=1) :
-            if chunks_to_add is None or ichunk in chunks_to_add :
-                self.chunks_to_upload.append(DataFileChunk(self.filepath,self.filename,self.__file_hash,
-                                                            chunk[0],chunk[1],chunk[2],chunk[3],ichunk,
-                                                            self.__n_total_chunks,
-                                                            rootdir=self.rootdir,
-                                                            filename_append=self.__filename_append))
-        if len(self.chunks_to_upload)>0 and self.__fully_enqueued :
+        # add the chunks to the final list as DataFileChunk objects
+        for ichunk, chunk in enumerate(self.__chunk_infos, start=1):
+            if chunks_to_add is None or ichunk in chunks_to_add:
+                self.chunks_to_upload.append(
+                    DataFileChunk(
+                        self.filepath,
+                        self.filename,
+                        self.__file_hash,
+                        chunk[0],
+                        chunk[1],
+                        chunk[2],
+                        chunk[3],
+                        ichunk,
+                        self.__n_total_chunks,
+                        rootdir=self.rootdir,
+                        filename_append=self.__filename_append,
+                    )
+                )
+        if len(self.chunks_to_upload) > 0 and self.__fully_enqueued:
             self.__fully_enqueued = False
 
-    def enqueue_chunks_for_upload(self,queue,n_threads=None,chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
-                                   queue_full_timeout=0.001) :
+    def enqueue_chunks_for_upload(
+        self,
+        queue,
+        n_threads=None,
+        chunk_size=RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
+        queue_full_timeout=0.001,
+    ):
         """
         Add some chunks of this file from the internal list to a given upload queue
-        (the internal list will be created if :func:`~add_chunks_to_upload` hasn't already been called).
+        (the internal list will be created if :func:`~add_chunks_to_upload`
+        hasn't already been called).
 
         When the entire internal list of file chunks has been added to the queue,
         the file will be marked as fully enqueued.
 
         If the given queue is full, this function will wait a bit and then return.
 
         :param queue: the Queue to which chunks should be added
         :type queue: :class:`queue.Queue`
-        :param n_threads: the number of threads running during uploading; at most 5*this number of chunks will be
-            added per call to this method. If this argument isn't given, every chunk in the internal list will be added.
+        :param n_threads: the number of threads running during uploading; at most 5*this
+            number of chunks will be added per call to this method. If this argument
+            isn't given, every chunk in the internal list will be added.
         :type n_threads: None or int, optional
         :param chunk_size: The size of the file chunk in each message in bytes
         :type chunk_size: int, optional
         :param queue_full_timeout: amount of time to wait before returning if the queue is full
             and new messages can't be added
         :type queue_full_timeout: float, optional
         """
-        if self.__fully_enqueued :
-            warnmsg = f'WARNING: enqueue_chunks_for_upload called for fully enqueued file {self.filepath}, '
-            warnmsg+= 'nothing else will be added.'
+        if self.__fully_enqueued:
+            warnmsg = (
+                "WARNING: enqueue_chunks_for_upload called for fully enqueued file "
+                f"{self.filepath}, nothing else will be added."
+            )
             self.logger.warning(warnmsg)
             return
-        if queue.full() :
+        if queue.full():
             time.sleep(queue_full_timeout)
             return
-        if len(self.chunks_to_upload)==0 :
+        if len(self.chunks_to_upload) == 0:
             self.add_chunks_to_upload(chunk_size=chunk_size)
-        if n_threads is not None :
-            n_chunks_to_add = 5*n_threads
-        else :
+        if n_threads is not None:
+            n_chunks_to_add = 5 * n_threads
+        else:
             n_chunks_to_add = len(self.chunks_to_upload)
         ichunk = 0
-        while len(self.chunks_to_upload)>0 and ichunk<n_chunks_to_add :
-            while queue.full() :
+        while len(self.chunks_to_upload) > 0 and ichunk < n_chunks_to_add:
+            while queue.full():
                 time.sleep(queue_full_timeout)
             queue.put(self.chunks_to_upload.pop(0))
-            ichunk+=1
-        if len(self.chunks_to_upload)==0 :
+            ichunk += 1
+        if len(self.chunks_to_upload) == 0:
             self.__fully_enqueued = True
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def _build_list_of_file_chunks(self,chunk_size) :
+    def _build_list_of_file_chunks(self, chunk_size):
         """
         Build the list of DataFileChunks for this file
 
         chunk_size = the size of each chunk in bytes
         """
-        #first make sure the choices of select_bytes are valid if necessary
-        #and sort them by their start byte to keep the file hash in order
-        if self.select_bytes :
-            if not isinstance(self.select_bytes,list) :
-                errmsg=f'ERROR: select_bytes={self.select_bytes} but is expected to be a list!'
-                self.logger.error(errmsg,exc_type=ValueError)
-            for sbt in self.select_bytes :
-                if (not isinstance(sbt,tuple)) or len(sbt)!=2 :
-                    errmsg = f'ERROR: found {sbt} in select_bytes but all elements are expected to be two-entry tuples!'
-                    self.logger.error(errmsg,exc_type=ValueError)
-                elif sbt[0]>=sbt[1] :
-                    errmsg = f'ERROR: found {sbt} in select_bytes but start byte cannot be >= stop byte!'
-                    self.logger.error(errmsg,exc_type=ValueError)
-            sorted_select_bytes = sorted(self.select_bytes,key=lambda x: x[0])
-        #start a hash for the file and the lists of chunks
+        # first make sure the choices of select_bytes are valid if necessary
+        # and sort them by their start byte to keep the file hash in order
+        if self.select_bytes:
+            if not isinstance(self.select_bytes, list):
+                errmsg = f"ERROR: select_bytes={self.select_bytes} but is expected to be a list!"
+                self.logger.error(errmsg, exc_type=ValueError)
+            for sbt in self.select_bytes:
+                if (not isinstance(sbt, tuple)) or len(sbt) != 2:
+                    errmsg = (
+                        f"ERROR: found {sbt} in select_bytes but all elements are "
+                        "expected to be two-entry tuples!"
+                    )
+                    self.logger.error(errmsg, exc_type=ValueError)
+                elif sbt[0] >= sbt[1]:
+                    errmsg = (
+                        f"ERROR: found {sbt} in select_bytes but "
+                        "start byte cannot be >= stop byte!"
+                    )
+                    self.logger.error(errmsg, exc_type=ValueError)
+            sorted_select_bytes = sorted(self.select_bytes, key=lambda x: x[0])
+        # start a hash for the file and the lists of chunks
         file_hash = sha512()
         chunks = []
-        isb = 0 #index for the current sorted_select_bytes entry if necessary
-        #read the binary data in the file as chunks of the given size, adding each chunk to the list
-        with open(self.filepath,'rb') as fp :
+        isb = 0  # index for the current sorted_select_bytes entry if necessary
+        # read the binary data in the file as chunks of the given size, adding each to the list
+        with open(self.filepath, "rb") as fp:
             chunk_offset = 0
             file_offset = 0 if (not self.select_bytes) else sorted_select_bytes[isb][0]
             n_bytes_to_read = chunk_size
-            if self.select_bytes :
-                n_bytes_to_read = min(chunk_size,sorted_select_bytes[isb][1]-file_offset)
+            if self.select_bytes:
+                n_bytes_to_read = min(
+                    chunk_size, sorted_select_bytes[isb][1] - file_offset
+                )
             chunk = fp.read(n_bytes_to_read)
-            while len(chunk) > 0 :
+            while len(chunk) > 0:
                 file_hash.update(chunk)
                 chunk_hash = sha512()
                 chunk_hash.update(chunk)
                 chunk_hash = chunk_hash.digest()
                 chunk_length = len(chunk)
-                chunks.append([chunk_hash,file_offset,chunk_offset,chunk_length])
+                chunks.append([chunk_hash, file_offset, chunk_offset, chunk_length])
                 chunk_offset += chunk_length
                 file_offset += chunk_length
-                if self.select_bytes and file_offset==sorted_select_bytes[isb][1] :
-                    isb+=1
-                    if isb>(len(sorted_select_bytes)-1) :
+                if self.select_bytes and file_offset == sorted_select_bytes[isb][1]:
+                    isb += 1
+                    if isb > (len(sorted_select_bytes) - 1):
                         break
-                    file_offset=sorted_select_bytes[isb][0]
+                    file_offset = sorted_select_bytes[isb][0]
                 n_bytes_to_read = chunk_size
-                if self.select_bytes :
-                    n_bytes_to_read = min(chunk_size,sorted_select_bytes[isb][1]-file_offset)
+                if self.select_bytes:
+                    n_bytes_to_read = min(
+                        chunk_size, sorted_select_bytes[isb][1] - file_offset
+                    )
                 fp.seek(file_offset)
                 chunk = fp.read(n_bytes_to_read)
         file_hash = file_hash.digest()
-        self.logger.debug(f'File {self.filepath} has a total of {len(chunks)} chunks')
-        #set the hash for the file
+        self.__chunked_at_timestamp = datetime.datetime.now()
+        self.logger.debug(f"File {self.filepath} has a total of {len(chunks)} chunks")
+        # set the hash for the file
         self.__file_hash = file_hash
-        #set the total number of chunks for this file
+        # set the total number of chunks for this file
         self.__n_total_chunks = len(chunks)
-        #build the list of all of the chunk infos for the file
+        # build the list of all of the chunk infos for the file
         self.__chunk_infos = []
-        for chunk in chunks :
+        for chunk in chunks:
             self.__chunk_infos.append(chunk)
 
     #################### CLASS METHODS ####################
 
     @classmethod
-    def get_command_line_arguments(cls) :
-        superargs,superkwargs = super().get_command_line_arguments()
-        args = [*superargs,'filepath','config','topic_name','chunk_size']
-        kwargs = {**superkwargs,'n_threads':RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS}
-        return args,kwargs
+    def get_command_line_arguments(cls):
+        superargs, superkwargs = super().get_command_line_arguments()
+        args = [*superargs, "filepath", "config", "topic_name", "chunk_size"]
+        kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_UPLOAD_THREADS}
+        return args, kwargs
 
     @classmethod
-    def run_from_command_line(cls,args=None) :
+    def run_from_command_line(cls, args=None):
         """
         Run an :class:`~UploadDataFile` directly from the command line
 
-        Calls :func:`~upload_whole_file` on an :class:`~.UploadDataFile` defined by command line (or given) arguments
+        Calls :func:`~upload_whole_file` on an :class:`~.UploadDataFile` defined by
+        command line (or given) arguments
 
-        :param args: the list of arguments to send to the parser instead of getting them from sys.argv
+        :param args: the list of arguments to send to the parser instead of getting them
+            from sys.argv
         :type args: list
         """
-        #make the argument parser
+        # make the argument parser
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
-        #make the DataFile for the single specified file
-        upload_file = cls(args.filepath,streamlevel=args.logger_stream_level,filelevel=args.logger_file_level)
-        #chunk and upload the file
-        upload_file.upload_whole_file(args.config,args.topic_name,
-                                      n_threads=args.n_threads,
-                                      chunk_size=args.chunk_size)
+        # make the DataFile for the single specified file
+        upload_file = cls(
+            args.filepath,
+            streamlevel=args.logger_stream_level,
+            filelevel=args.logger_file_level,
+        )
+        # chunk and upload the file
+        upload_file.upload_whole_file(
+            args.config,
+            args.topic_name,
+            n_threads=args.n_threads,
+            chunk_size=args.chunk_size,
+        )
 
     #################### PROPERTIES ####################
 
     @property
-    def select_bytes(self) :
+    def select_bytes(self):
         """
-        In child classes, this property can be a list of tuples of (start_byte,stop_byte) in the file
-        that will be the only ranges of bytes added when creating the list of chunks.
+        In child classes, this property can be a list of tuples of (start_byte,stop_byte)
+        in the file that will be the only ranges of bytes added when creating the list of chunks.
         The empty list in the base class will cause all bytes of the file to be uploaded.
         """
         return []
+
     @property
     def to_upload(self):
         """
         whether or not this file will be considered when uploading some group of data files
         """
         return self.__to_upload
+
     @to_upload.setter
-    def to_upload(self,to_upload) :
-        if to_upload and (not self.__to_upload) :
-            self.logger.debug(f'Setting {self.filepath} to be uploaded')
-        elif (not to_upload) and self.__to_upload :
-            self.logger.debug(f'Setting {self.filepath} to NOT be uploaded')
+    def to_upload(self, to_upload):
+        if to_upload and (not self.__to_upload):
+            self.logger.debug(f"Setting {self.filepath} to be uploaded")
+        elif (not to_upload) and self.__to_upload:
+            self.logger.debug(f"Setting {self.filepath} to NOT be uploaded")
         self.__to_upload = to_upload
+
     @property
-    def fully_enqueued(self) :
+    def fully_enqueued(self):
         """
         True if this file has had all of its chunks added to an upload queue
         """
         return self.__fully_enqueued
+
     @fully_enqueued.setter
-    def fully_enqueued(self,fully_enqueued) :
+    def fully_enqueued(self, fully_enqueued):
         self.__fully_enqueued = fully_enqueued
+
     @property
-    def fully_produced(self) :
+    def fully_produced(self):
         """
         True if this file has had all of its chunks successfully sent to the broker
         (only used when run as part of a :class:`~.DataFileUploadDirectory`)
         """
         return self.__fully_produced
+
     @fully_produced.setter
-    def fully_produced(self,fp) :
+    def fully_produced(self, fp):
         self.__fully_produced = fp
+
     @property
-    def waiting_to_upload(self) :
+    def waiting_to_upload(self):
         """
         True if this file is waiting for its upload to begin
         """
-        if (not self.__to_upload) or self.__fully_enqueued or self.__fully_produced :
+        if (not self.__to_upload) or self.__fully_enqueued or self.__fully_produced:
             return False
-        if len(self.chunks_to_upload)>0 :
+        if len(self.chunks_to_upload) > 0:
             return False
         return True
+
     @property
-    def upload_in_progress(self) :
+    def upload_in_progress(self):
         """
         True if this file is in the process of being enqueued to be uploaded
         """
-        if (not self.__to_upload) or self.__fully_enqueued or self.__fully_produced :
+        if (not self.__to_upload) or self.__fully_enqueued or self.__fully_produced:
             return False
-        if len(self.chunks_to_upload)==0 :
+        if len(self.chunks_to_upload) == 0:
             return False
         return True
+
     @property
-    def upload_status_msg(self) :
+    def upload_status_msg(self):
         """
         A message stating the file's name and status w.r.t. being enqueued to be uploaded
         """
-        if self.rootdir is None :
-            msg = f'{self.filepath} '
-        else :
-            msg = f'{self.filepath.relative_to(self.rootdir)} '
-        if not self.__to_upload :
-            msg+='(will not be uploaded)'
-        elif self.__fully_produced :
-            msg+=f'({self.__n_total_chunks} message'
-            if self.__n_total_chunks!=1 :
-                msg+='s'
-            msg+=' fully produced to broker)'
-        elif self.__fully_enqueued :
-            msg+=f'({self.__n_total_chunks} message'
-            if self.__n_total_chunks!=1 :
-                msg+='s'
-            msg+=' fully enqueued)'
-        elif self.upload_in_progress :
-            msg+=f'(in progress with {self.__n_total_chunks-len(self.chunks_to_upload)}'
-            msg+=f'/{self.__n_total_chunks} messages enqueued)'
-        elif self.waiting_to_upload :
-            msg+=f'({self.__n_total_chunks} messages waiting to be enqueued)'
-        else :
-            msg+='(status unknown)'
+        if self.rootdir is None:
+            msg = f"{self.filepath} "
+        else:
+            msg = f"{self.filepath.relative_to(self.rootdir)} "
+        if not self.__to_upload:
+            msg += "(will not be uploaded)"
+        elif self.__fully_produced:
+            msg += f"({self.__n_total_chunks} message"
+            if self.__n_total_chunks != 1:
+                msg += "s"
+            msg += " fully produced to broker)"
+        elif self.__fully_enqueued:
+            msg += f"({self.__n_total_chunks} message"
+            if self.__n_total_chunks != 1:
+                msg += "s"
+            msg += " fully enqueued)"
+        elif self.upload_in_progress:
+            msg += f"(in progress with {self.__n_total_chunks-len(self.chunks_to_upload)}"
+            msg += f"/{self.__n_total_chunks} messages enqueued)"
+        elif self.waiting_to_upload:
+            if self.__n_total_chunks == 0:
+                msg += "(all "
+            else:
+                msg += f"({self.__n_total_chunks} "
+            msg += "messages waiting to be enqueued)"
+        else:
+            msg += "(status unknown)"
         return msg
 
-def main(args=None) :
+    @property
+    def chunked_at_timestamp(self):
+        """
+        A datetime object representing a timestamp of when the list of chunks was built
+        """
+        return self.__chunked_at_timestamp
+
+
+def main(args=None):
     """
     main method to run from command line
     """
     UploadDataFile.run_from_command_line(args)
 
-if __name__=='__main__' :
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/data_file_io/utilities.py` & `openmsistream-1.4.0/openmsistream/data_file_io/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 """Various utility functions used elsewhere in this subdirectory"""
 
-#imports
+# imports
 import datetime
-from confluent_kafka import TIMESTAMP_NOT_AVAILABLE, TIMESTAMP_CREATE_TIME, TIMESTAMP_LOG_APPEND_TIME
+from confluent_kafka import (
+    TIMESTAMP_NOT_AVAILABLE,
+    TIMESTAMP_CREATE_TIME,
+    TIMESTAMP_LOG_APPEND_TIME,
+)
 
-def get_encrypted_message_timestamp_string(msg) :
+
+def get_encrypted_message_timestamp_string(msg):
     """
     Given a Message object containing still-encrypted keys and/or values,
     return a string describing the timestamp in local time.
     """
     format_string = "on_%b_%d_%Y_at_%H_%M_%S_%f"
     ts_type, timestamp = msg.timestamp
-    if ts_type==TIMESTAMP_NOT_AVAILABLE :
-        timestamp_string = f'consumed_{datetime.datetime.now().strftime(format_string)}'
-    elif ts_type in (TIMESTAMP_CREATE_TIME,TIMESTAMP_LOG_APPEND_TIME) :
-        utc_dt = datetime.datetime.fromtimestamp(timestamp/1000.,tz=datetime.timezone.utc)
+    if ts_type == TIMESTAMP_NOT_AVAILABLE:
+        timestamp_string = f"consumed_{datetime.datetime.now().strftime(format_string)}"
+    elif ts_type in (TIMESTAMP_CREATE_TIME, TIMESTAMP_LOG_APPEND_TIME):
+        utc_dt = datetime.datetime.fromtimestamp(
+            timestamp / 1000.0, tz=datetime.timezone.utc
+        )
         local_timezone = datetime.datetime.now(datetime.timezone.utc).astimezone().tzinfo
         local_dt = utc_dt.astimezone(local_timezone)
-        if ts_type==TIMESTAMP_CREATE_TIME :
-            timestamp_string = 'produced'
-        elif ts_type==TIMESTAMP_LOG_APPEND_TIME :
-            timestamp_string = 'received'
-        timestamp_string+=f'_{local_dt.strftime(format_string)}'
-    else :
-        raise ValueError(f'ERROR: Unrecognized timestamp type {ts_type}')
+        if ts_type == TIMESTAMP_CREATE_TIME:
+            timestamp_string = "produced"
+        elif ts_type == TIMESTAMP_LOG_APPEND_TIME:
+            timestamp_string = "received"
+        timestamp_string += f"_{local_dt.strftime(format_string)}"
+    else:
+        raise ValueError(f"ERROR: Unrecognized timestamp type {ts_type}")
     return timestamp_string
 
-def get_encrypted_message_key_and_value_filenames(msg,topic_name) :
+
+def get_encrypted_message_key_and_value_filenames(msg, topic_name):
     """
     Given a Message object containing still-encrypted keys and/or values and the name
     of the topic it came from, return the names of the files to which the key and
     value should have their bytes written
     """
     timestamp_string = get_encrypted_message_timestamp_string(msg)
-    fp_pp = f'encrypted_message_from_{topic_name}_{timestamp_string}'
-    return f'{fp_pp}_key.bin',f'{fp_pp}_value.bin'
+    fp_pp = f"encrypted_message_from_{topic_name}_{timestamp_string}"
+    return f"{fp_pp}_key.bin", f"{fp_pp}_value.bin"
+
 
-def get_message_prepend(subdir_str,filename) :
+def get_message_prepend(subdir_str, filename):
     """
     Return the prepend for each message key, based on the filepath
     """
-    key_pp = ''
-    if subdir_str is not None :
-        key_pp = f'{"_".join(subdir_str.split("/"))}'
-    if key_pp!='' :
-        key_pp+='_'
-    return f'{key_pp}{filename}_chunk'
+    key_pp = f'{"_".join(subdir_str.split("/"))}_' if subdir_str is not None else ""
+    return f"{key_pp}{filename}_chunk"
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_file_parser.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_file_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """
 A wrapper around ConfigFileParser to handle OpenMSIStream config files that have sections
 for connecting to brokers and running Producers and Consumers
 """
 
-#imports
+# imports
 import pathlib
-from confluent_kafka.serialization import DoubleSerializer, IntegerSerializer, StringSerializer
-from confluent_kafka.serialization import DoubleDeserializer, IntegerDeserializer, StringDeserializer
+from confluent_kafka.serialization import (
+    DoubleSerializer,
+    IntegerSerializer,
+    StringSerializer,
+)
+from confluent_kafka.serialization import (
+    DoubleDeserializer,
+    IntegerDeserializer,
+    StringDeserializer,
+)
 from ..utilities.config_file_parser import ConfigFileParser
 from ..utilities.config import RUN_CONST
 from .serialization import DataFileChunkSerializer, DataFileChunkDeserializer
 
-class KafkaConfigFileParser(ConfigFileParser) :
+
+class KafkaConfigFileParser(ConfigFileParser):
     """
     A class to parse Kafka configurations from files
     """
 
     #################### CONSTANTS ####################
 
     SERIALIZERS = [
@@ -31,119 +40,126 @@
         DoubleDeserializer,
         DataFileChunkDeserializer,
     ]
 
     #################### PROPERTIES ####################
 
     @property
-    def broker_configs(self) :
+    def broker_configs(self):
         """
         Configs for connecting to the broker
         """
-        if self.__broker_configs is None :
-            self.__broker_configs = self._get_config_dict('broker')
+        if self.__broker_configs is None:
+            self.__broker_configs = self._get_config_dict("broker")
         return self.__convert_floats(self.__broker_configs)
+
     @property
-    def producer_configs(self) :
+    def producer_configs(self):
         """
         Configs for setting up Producers
         """
-        if self.__producer_configs is None :
-            pcs = self._get_config_dict('producer')
-            self.__producer_configs = self.get_replaced_configs(pcs,'serialization')
+        if self.__producer_configs is None:
+            pcs = self._get_config_dict("producer")
+            self.__producer_configs = self.get_replaced_configs(pcs, "serialization")
         return self.__convert_floats(self.__producer_configs)
+
     @property
-    def consumer_configs(self) :
+    def consumer_configs(self):
         """
         Configs for setting up Consumers
         """
-        if self.__consumer_configs is None :
-            ccs = self._get_config_dict('consumer')
-            #if the auto.offset.reset was given as "none" then remove it from the ccs
-            if 'auto.offset.reset' in ccs and ccs['auto.offset.reset']=='none' :
-                del ccs['auto.offset.reset']
-            self.__consumer_configs = self.get_replaced_configs(ccs,'deserialization')
+        if self.__consumer_configs is None:
+            ccs = self._get_config_dict("consumer")
+            # if the auto.offset.reset was given as "none" then remove it from the ccs
+            if "auto.offset.reset" in ccs and ccs["auto.offset.reset"] == "none":
+                del ccs["auto.offset.reset"]
+            self.__consumer_configs = self.get_replaced_configs(ccs, "deserialization")
         return self.__convert_floats(self.__consumer_configs)
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.__broker_configs = None
         self.__producer_configs = None
         self.__consumer_configs = None
         self.kc_config_file_str = self.__get_kc_config_file_str()
 
     @staticmethod
-    def get_replaced_configs(configs,replacement_type) :
+    def get_replaced_configs(configs, replacement_type):
         """
         Returns a configuration dictionary with (de)serialization parameters replaced
         by instances of corresponding classes
 
         configs = the configurations dictionary to alter and return
         replacement_type = a string indicating the type of replacement that should be performed
         """
-        if replacement_type=='serialization' :
+        if replacement_type == "serialization":
             classes = KafkaConfigFileParser.SERIALIZERS
-        elif replacement_type=='deserialization' :
+        elif replacement_type == "deserialization":
             classes = KafkaConfigFileParser.DESERIALIZERS
-        else :
-            raise ValueError(f'ERROR: unrecognized replacement_type "{replacement_type}" in get_replaced_configs!')
-        for cfg_name,cfg_value in configs.items() :
-            for serdes_class in classes :
-                if cfg_value==serdes_class.__name__ :
+        else:
+            raise ValueError(f'ERROR: unrecognized replacement_type "{replacement_type}"')
+        for cfg_name, cfg_value in configs.items():
+            for serdes_class in classes:
+                if cfg_value == serdes_class.__name__:
                     configs[cfg_name] = serdes_class()
                     break
         return configs
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def __get_kc_config_file_str(self) :
+    def __get_kc_config_file_str(self):
         """
         Returns the path to the config file that KafkaCrypto needs based on the current configs.
         Return value is a string as expected by KafkaCrypto.
-        If no config file is found according to the conventions listed below, this function returns None
-        and it will be assumed that no configuration for KafkaCrypto exists
+        If no config file is found according to the conventions listed below, this function
+        returns None and it will be assumed that no configuration for KafkaCrypto exists
 
         Options are:
-        1) The regular config file has a "kafkacrypto" section with a "config_file" parameter that is the
-        path to the KafkaCrypo config file
-        2) The regular config file has a "kafkacrypto" section with a "node_id" parameter corresponding to
-        a named subdirectory in openmsistream/kafka_wrapper/config_files that was created when the node was provisioned
-        """
-        if 'kafkacrypto' in self.available_group_names :
-            kc_configs = self.get_config_dict_for_groups('kafkacrypto')
-            #option 1 above
-            if 'config_file' in kc_configs :
-                path_as_str = (kc_configs['config_file']).lstrip('file#')
-                if not pathlib.Path(path_as_str).is_file() :
-                    errmsg = f'ERROR: KafkaCrypto config file {path_as_str} '
-                    errmsg+= f'(from config file {self.filepath}) not found!'
-                    self.logger.error(errmsg,exc_type=FileNotFoundError)
+        1) The regular config file has a "kafkacrypto" section with a "config_file" parameter
+        that is the path to the KafkaCrypo config file
+        2) The regular config file has a "kafkacrypto" section with a "node_id" parameter
+        corresponding to a named subdirectory in openmsistream/kafka_wrapper/config_files
+        that was created when the node was provisioned
+        """
+        if "kafkacrypto" in self.available_group_names:
+            kc_configs = self.get_config_dict_for_groups("kafkacrypto")
+            # option 1 above
+            if "config_file" in kc_configs:
+                path_as_str = (kc_configs["config_file"]).lstrip("file#")
+                if not pathlib.Path(path_as_str).is_file():
+                    errmsg = (
+                        f"ERROR: KafkaCrypto config file {path_as_str} (from config file "
+                        f"{self.filepath}) not found!"
+                    )
+                    self.logger.error(errmsg, exc_type=FileNotFoundError)
                 return path_as_str
-            #option 2 above
-            if 'node_id' in kc_configs :
-                node_id = kc_configs['node_id']
+            # option 2 above
+            if "node_id" in kc_configs:
+                node_id = kc_configs["node_id"]
                 dirpath = RUN_CONST.CONFIG_FILE_DIR / node_id
-                filepath = dirpath / f'{node_id}.config'
-                if (not dirpath.is_dir()) or (not filepath.is_file()) :
-                    errmsg = f'ERROR: no KafkaCrypto config file found in the default location ({filepath}) '
-                    errmsg+= f'for node ID = {node_id}'
-                    self.logger.error(errmsg,exc_type=FileNotFoundError)
+                filepath = dirpath / f"{node_id}.config"
+                if (not dirpath.is_dir()) or (not filepath.is_file()):
+                    errmsg = (
+                        "ERROR: no KafkaCrypto config file found in the default location "
+                        f"({filepath}) for node ID = {node_id}"
+                    )
+                    self.logger.error(errmsg, exc_type=FileNotFoundError)
                 return str(filepath)
-        #no config file found
+        # no config file found
         return None
 
-    def __convert_floats(self,given_dict) :
+    def __convert_floats(self, given_dict):
         """
-        Return a version of the dictionary "given_dict" where any values that can be converted to floats
-        are converted to floats
+        Return a version of the dictionary "given_dict" where any values that can be
+        converted to floats are converted to floats
         (Some KafkaCrypto code assumes configs will be floats)
         """
         return_dict = {}
-        for k,v in given_dict.items() :
-            try :
+        for k, v in given_dict.items():
+            try:
                 v_as_float = float(v)
                 return_dict[k] = v_as_float
-            except Exception :
-                return_dict[k]=v
+            except Exception:
+                return_dict[k] = v
         return return_dict
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/prod.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/prod.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_encrypted.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/consumer_and_producer_group.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,101 @@
 """A set of Consumers and Producers that share share the same KafkaCrypto key-passing instance"""
 
-#imports
+# imports
 from ..utilities.logging import LogOwner
 from .consumer_group import ConsumerGroup
 from .producer_group import ProducerGroup
 
-class ConsumerAndProducerGroup(LogOwner) :
+
+class ConsumerAndProducerGroup(LogOwner):
     """
-    Class for working with a group of Consumers and Producers sharing a single :class:`kafkacrypto.KafkaCrypto` instance
+    Class for working with a group of Consumers and Producers sharing a single
+    :class:`kafkacrypto.KafkaCrypto` instance
 
-    :param config_path: Path to the config file that should be used to define Consumers/Producers in the group
+    :param config_path: Path to the config file that should be used to define
+        Consumers/Producers in the group
     :type config_path: :class:`pathlib.Path`
     :param consumer_topic_name: The name of the topic to which the Consumers should be subscribed
     :type consumer_topic_name: str
     :param consumer_group_id: The ID string that should be used for each Consumer in the group.
         "create_new" (the defaults) will create a new UID to use.
     :type consumer_group_id: str, optional
     """
 
     @property
-    def consumer_topic_name(self) :
+    def consumer_topic_name(self):
         """
         Name of the topic to which the consumers are subscribed
         """
         return self.__consumer_group.topic_name
+
     @property
-    def consumer_group_id(self) :
+    def consumer_group_id(self):
         """
         Group ID of all consumers in the group
         """
         return self.__consumer_group.consumer_group_id
 
-    def __init__(self,config_path,consumer_topic_name,*,consumer_group_id='create_new',**kwargs) :
+    def __init__(
+        self,
+        config_path,
+        consumer_topic_name,
+        *,
+        consumer_group_id="create_new",
+        **kwargs,
+    ):
         """
         Constructor method
         """
         super().__init__(**kwargs)
-        self.__consumer_group = ConsumerGroup(config_path,consumer_topic_name,
-                                              consumer_group_id=consumer_group_id,logger=self.logger)
-        self.__producer_group = ProducerGroup(config_path,kafkacrypto=self.__consumer_group.kafkacrypto,
-                                              logger=self.logger)
+        self.__consumer_group = ConsumerGroup(
+            config_path,
+            consumer_topic_name,
+            consumer_group_id=consumer_group_id,
+            logger=self.logger,
+        )
+        self.__producer_group = ProducerGroup(
+            config_path, kafkacrypto=self.__consumer_group.kafkacrypto, logger=self.logger
+        )
 
-    def get_new_subscribed_consumer(self,*,restart_at_beginning=False,**kwargs) :
+    def get_new_subscribed_consumer(self, *, restart_at_beginning=False, **kwargs):
         """
         Return a new Consumer, subscribed to the topic and with the shared group ID.
         Call this function from a child thread to get thread-independent Consumers.
 
         Note: This function just creates and subscribes the Consumer. Polling it, closing
         it, and everything else must be handled by whatever calls this function.
 
-        :param restart_at_beginning: if True, the new Consumer will start reading partitions from the earliest
-            messages available, regardless of Consumer group ID and auto.offset.reset values.
-            Useful when re-reading messages.
+        :param restart_at_beginning: if True, the new Consumer will start reading partitions
+            from the earliest messages available, regardless of Consumer group ID and
+            auto.offset.reset values. Useful when re-reading messages.
         :type restart_at_beginning: bool, optional
-        :param kwargs: other keyword arguments are passed to the :class:`~OpenMSIStreamConsumer` constructor method
-            (for example, parameters to set a key regex or how to filter messages)
+        :param kwargs: other keyword arguments are passed to the
+            :class:`~OpenMSIStreamConsumer` constructor method
         :type kwargs: dict
 
-        :return: a Consumer created using the configs set in the constructor/from `kwargs`, subscribed to the topic
+        :return: a Consumer created using the configs set in the constructor/from `kwargs`,
+            subscribed to the topic
         :rtype: :class:`~OpenMSIStreamConsumer`
         """
-        return self.__consumer_group.get_new_subscribed_consumer(restart_at_beginning=restart_at_beginning,**kwargs)
+        return self.__consumer_group.get_new_subscribed_consumer(
+            restart_at_beginning=restart_at_beginning, **kwargs
+        )
 
-    def get_new_producer(self) :
+    def get_new_producer(self):
         """
         Return a new :class:`~OpenMSIStreamProducer` object.
         Call this function from a child thread to get thread-independent Producers.
-        Note: this function just creates the Producer; closing it etc. must be handled by whatever calls this function.
+        Note: this function just creates the Producer; closing it etc. must be handled by
+        whatever calls this function.
 
         :return: a Producer created using the config set in the constructor
         :rtype: :class:`~OpenMSIStreamProducer`
         """
         return self.__producer_group.get_new_producer()
 
-    def close(self) :
+    def close(self):
         """
         Wrapper around :func:`kafkacrypto.KafkaCrypto.close`.
         """
         self.__consumer_group.close()
         self.__producer_group.close()
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/consumer_group.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,148 +1,196 @@
-"""A set of Consumers sharing a subscribed topic, group ID, and (optionally) KafkaCrypto instance for key passing"""
+"""
+A set of Consumers sharing a subscribed topic, group ID, and (optionally)
+KafkaCrypto instance for key passing
+"""
 
-#imports
+# imports
 import kafka
 from confluent_kafka.admin import AdminClient
 from confluent_kafka import TopicPartition
 from ..utilities import LogOwner
 from .utilities import reset_to_beginning_on_assign
 from .config_file_parser import KafkaConfigFileParser
 from .openmsistream_consumer import OpenMSIStreamConsumer
 
-class ConsumerGroup(LogOwner) :
+
+class ConsumerGroup(LogOwner):
     """
-    Class for working with a group of consumers sharing a single :class:`kafkacrypto.KafkaCrypto` instance
+    Class for working with a group of consumers sharing a single
+    :class:`kafkacrypto.KafkaCrypto` instance
 
     :param config_path: Path to the config file that should be used to define Consumers in the group
     :type config_path: :class:`pathlib.Path`
     :param topic_name: The name of the topic to which the Consumers should be subscribed
     :type topic_name: str
     :param consumer_group_id: The ID string that should be used for each Consumer in the group.
         "create_new" (the default) will create a new UID to use.
     :type consumer_group_id: str, optional
-    :param kafkacrypto: The :class:`~OpenMSIStreamKafkaCrypto` object that should be used to instantiate Consumers.
-        Only needed if a single specific :class:`~OpenMSIStreamKafkaCrypto` instance should be shared.
+    :param kafkacrypto: The :class:`~OpenMSIStreamKafkaCrypto` object that should be used
+        to instantiate Consumers. Only needed if a single specific
+        :class:`~OpenMSIStreamKafkaCrypto` instance should be shared.
     :type kafkacrypto: :class:`~OpenMSIStreamKafkaCrypto`, optional
-    :param kwargs: Other keyword arguments will be added to the underlying Consumer's configurations,
-        with underscores in their names replaced with dots.
+    :param kwargs: Other keyword arguments will be added to the underlying Consumer's
+        configurations, with underscores in their names replaced with dots.
     :type kwargs: dict
     """
 
     @property
-    def topic_name(self) :
+    def topic_name(self):
         """
         Name of the topic to which Consumers are subscribed
         """
         return self.__topic_name
+
     @property
-    def consumer_group_id(self) :
+    def consumer_group_id(self):
         """
         String ID of Consumers in the group
         """
         return self.__consumer_group_id
+
     @property
-    def kafkacrypto(self) :
+    def kafkacrypto(self):
         """
-        The KafkaCrypto object handling key passing and deserialization for the group of Consumers (if applicable)
+        The KafkaCrypto object handling key passing and deserialization
+        for the group of Consumers (if applicable)
         """
-        return self.__c_kwargs['kafkacrypto'] if 'kafkacrypto' in self.__c_kwargs else None
-
-    def __init__(self,config_path,topic_name,*,consumer_group_id='create_new',kafkacrypto=None,**kwargs) :
+        return (
+            self.__c_kwargs["kafkacrypto"] if "kafkacrypto" in self.__c_kwargs else None
+        )
+
+    def __init__(
+        self,
+        config_path,
+        topic_name,
+        *,
+        consumer_group_id="create_new",
+        kafkacrypto=None,
+        **kwargs,
+    ):
         """
         Constructor method
         """
         super().__init__(**kwargs)
-        self.__group_starting_offsets = self.__get_group_starting_offsets(config_path,topic_name,consumer_group_id)
+        self.__group_starting_offsets = self.__get_group_starting_offsets(
+            config_path, topic_name, consumer_group_id
+        )
         self.__topic_name = topic_name
-        self.__c_args, self.__c_kwargs = OpenMSIStreamConsumer.get_consumer_args_kwargs(config_path,
-                                                                                        group_id=consumer_group_id,
-                                                                                        logger=self.logger,
-                                                                                        kafkacrypto=kafkacrypto)
-        if len(self.__c_args)>1 and 'group.id' in self.__c_args[1] :
-            self.__consumer_group_id = self.__c_args[1]['group.id']
-        else :
+        self.__c_args, self.__c_kwargs = OpenMSIStreamConsumer.get_consumer_args_kwargs(
+            config_path,
+            group_id=consumer_group_id,
+            logger=self.logger,
+            kafkacrypto=kafkacrypto,
+        )
+        if len(self.__c_args) > 1 and "group.id" in self.__c_args[1]:
+            self.__consumer_group_id = self.__c_args[1]["group.id"]
+        else:
             self.__consumer_group_id = consumer_group_id
 
-    def get_new_subscribed_consumer(self,*,restart_at_beginning=False,**kwargs) :
+    def get_new_subscribed_consumer(self, *, restart_at_beginning=False, **kwargs):
         """
         Return a new Consumer, subscribed to the topic and with the shared group ID.
         Call this function from a child thread to get thread-independent Consumers.
 
         Note: This function just creates and subscribes the Consumer. Polling it, closing
         it, and everything else must be handled by whatever calls this function.
 
-        :param restart_at_beginning: if True, the new Consumer will start reading partitions from the earliest
-            messages available, regardless of Consumer group ID and auto.offset.reset values.
-            Useful when re-reading messages.
+        :param restart_at_beginning: if True, the new Consumer will start reading partitions
+            from the earliest messages available, regardless of Consumer group ID and
+            auto.offset.reset values. Useful when re-reading messages.
         :type restart_at_beginning: bool, optional
-        :param kwargs: other keyword arguments are passed to the :class:`~OpenMSIStreamConsumer` constructor method
-            (for example, parameters to set a key regex or how to filter messages)
+        :param kwargs: other keyword arguments are passed to the
+            :class:`~OpenMSIStreamConsumer` constructor method
         :type kwargs: dict
 
-        :return: a Consumer created using the configs set in the constructor/from `kwargs`, subscribed to the topic
+        :return: a Consumer created using the configs set in the constructor/from `kwargs`,
+            subscribed to the topic
         :rtype: :class:`~OpenMSIStreamConsumer`
         """
-        consumer = OpenMSIStreamConsumer(*self.__c_args,
-                                         **kwargs,
-                                         starting_offsets=self.__group_starting_offsets,**self.__c_kwargs)
-        if restart_at_beginning :
-            consumer.subscribe([self.__topic_name],on_assign=reset_to_beginning_on_assign)
-        else :
+        consumer = OpenMSIStreamConsumer(
+            *self.__c_args,
+            **kwargs,
+            starting_offsets=self.__group_starting_offsets,
+            **self.__c_kwargs,
+        )
+        if restart_at_beginning:
+            consumer.subscribe(
+                [self.__topic_name], on_assign=reset_to_beginning_on_assign
+            )
+        else:
             consumer.subscribe([self.__topic_name])
         return consumer
 
-    def close(self) :
+    def close(self):
         """
         Wrapper around :func:`kafkacrypto.KafkaCrypto.close`.
         """
-        try :
-            self.__c_kwargs['kafkacrypto'].close()
-        except Exception :
+        try:
+            self.__c_kwargs["kafkacrypto"].close()
+        except Exception:
             pass
-        finally :
-            self.__c_kwargs['kafkacrypto'] = None
+        finally:
+            self.__c_kwargs["kafkacrypto"] = None
 
-    def __get_group_starting_offsets(self,config_path,topic_name,consumer_group_id,n_retries=10) :
+    def __get_group_starting_offsets(
+        self, config_path, topic_name, consumer_group_id, n_retries=10
+    ):
         """
         Return a list of TopicPartitions listing the starting offsets for each partition
         in the topic for the given consumer group ID
 
-        Retries a configurable number of times if it fails at first, since there can be some lag involved
+        Retries a configurable number of times if it fails at first, since there can be
+        some lag involved
 
         Re-raises any errors encountered in getting the necessary metadata,
         returning None if that happens
         """
         caught_exc = None
-        while n_retries>0 :
+        while n_retries > 0:
             cfp = KafkaConfigFileParser(config_path)
             starting_offsets = []
-            try :
-                cluster_metadata = AdminClient(cfp.broker_configs).list_topics(topic=topic_name)
+            try:
+                cluster_metadata = AdminClient(cfp.broker_configs).list_topics(
+                    topic=topic_name
+                )
                 n_partitions = len(cluster_metadata.topics[topic_name].partitions)
-                if n_partitions<=0 :
-                    raise RuntimeError(f'ERROR: number of partitions for topic {topic_name} is {n_partitions}')
+                if n_partitions <= 0:
+                    raise RuntimeError(
+                        f"ERROR: number of partitions for topic {topic_name} is {n_partitions}"
+                    )
                 kac_kwargs = {}
-                for k,v in cfp.broker_configs.items() :
-                    if k in ('sasl.username','sasl.password') :
-                        key = k.replace('.','_plain_')
-                    else :
-                        key = k.replace('.','_')
-                    kac_kwargs[key]=v
-                parts = [kafka.TopicPartition(topic_name,p_i) for p_i in range(n_partitions)]
-                tp_offsets=kafka.KafkaAdminClient(**kac_kwargs).list_consumer_group_offsets(group_id=consumer_group_id,
-                                                                                            partitions=parts)
-                if len(tp_offsets)!=n_partitions :
-                    errmsg = f'Found {n_partitions} partitions for topic {topic_name} but got {len(tp_offsets)} '
-                    errmsg+= 'TopicPartitions listing current consumer group offsets'
+                for k, v in cfp.broker_configs.items():
+                    if k in ("sasl.username", "sasl.password"):
+                        key = k.replace(".", "_plain_")
+                    else:
+                        key = k.replace(".", "_")
+                    kac_kwargs[key] = v
+                parts = [
+                    kafka.TopicPartition(topic_name, p_i) for p_i in range(n_partitions)
+                ]
+                tp_offsets = kafka.KafkaAdminClient(
+                    **kac_kwargs
+                ).list_consumer_group_offsets(
+                    group_id=consumer_group_id, partitions=parts
+                )
+                if len(tp_offsets) != n_partitions:
+                    errmsg = (
+                        f"Found {n_partitions} partitions for topic {topic_name} but got "
+                        f"{len(tp_offsets)} TopicPartitions listing current consumer group offsets"
+                    )
                     raise RuntimeError(errmsg)
-                for t_p,offset_metadata in tp_offsets.items() :
-                    starting_offsets.append(TopicPartition(t_p.topic,t_p.partition,offset_metadata.offset))
+                for t_p, offset_metadata in tp_offsets.items():
+                    starting_offsets.append(
+                        TopicPartition(t_p.topic, t_p.partition, offset_metadata.offset)
+                    )
                 return starting_offsets
-            except Exception as exc :
+            except Exception as exc:
                 caught_exc = exc
-                n_retries-=1
-        if caught_exc :
-            errmsg = f'ERROR: encountered an exception when gathering initial "{topic_name}" topic offsets for '
-            errmsg+= f'consumer group ID "{consumer_group_id}". The error will be logged below and re-raised.'
-            self.logger.error(errmsg,exc_info=caught_exc,reraise=True)
+                n_retries -= 1
+        if caught_exc:
+            errmsg = (
+                f'ERROR: encountered an exception when gathering initial "{topic_name}" '
+                f'topic offsets for consumer group ID "{consumer_group_id}". '
+                "The error will be logged below and re-raised."
+            )
+            self.logger.error(errmsg, exc_info=caught_exc, reraise=True)
         return None
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/controlled_message_processor.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,144 @@
-"""A ConsumerGroup whose receipt of messages is governed using the ControlledProcess infrastructure"""
+"""
+A ConsumerGroup whose receipt of messages is governed using the ControlledProcess infrastructure
+"""
 
-#imports
+# imports
 import time
 from abc import ABC, abstractmethod
 from ..utilities import ControlledProcessMultiThreaded
 from .consumer_group import ConsumerGroup
 
-class ControlledMessageProcessor(ControlledProcessMultiThreaded,ConsumerGroup,ABC) :
+
+class ControlledMessageProcessor(ControlledProcessMultiThreaded, ConsumerGroup, ABC):
     """
     Combine a ControlledProcessMultiThreaded and a ConsumerGroup to create a
     single interface for reading and processing individual messages
     """
 
     CONSUMER_POLL_TIMEOUT = 0.050
-    NO_MESSAGE_WAIT = 0.005 #how long to wait if consumer.get_next_message_value returns None
+    NO_MESSAGE_WAIT = (
+        0.005  # how long to wait if consumer.get_next_message_value returns None
+    )
 
-    def __init__(self,*args,**kwargs) :
+    def __init__(self, *args, **kwargs):
         """
         Hang onto the number of messages read and processed
         """
         self.n_msgs_read = 0
         self.n_msgs_processed = 0
-        super().__init__(*args,**kwargs)
-        self.restart_at_beginning = False #set to true to reset new consumers to their earliest offsets
-        self.message_key_regex = None #set to some regex to filter messages by their keys
-        self.filter_new_messages = False #reset the regex after the consumer has filtered through previous messages
-        self.last_message = None #hold onto the last consumed message to manually commit its offset on shutdown
+        super().__init__(*args, **kwargs)
+        # set below to true to reset new consumers to their earliest offsets
+        self.restart_at_beginning = False
+        # set below to some regex to filter messages by their keys
+        self.message_key_regex = None
+        # reset the regex after the consumer has filtered through previous messages
+        self.filter_new_messages = False
+        # hold onto the last consumed message to manually commit its offset on shutdown
+        self.last_message = None
 
     def _run_worker(self):
         """
         Handle startup and shutdown of a thread-independent Consumer and
         serve individual messages to the _process_message function
         """
-        #create the Consumer for this thread
-        if self.alive :
-            consumer = self.get_new_subscribed_consumer(restart_at_beginning=self.restart_at_beginning,
-                                                        message_key_regex=self.message_key_regex,
-                                                        filter_new_messages=self.filter_new_messages)
-        if ('enable.auto.commit' not in consumer.configs.keys()) or (consumer.configs['enable.auto.commit'] is True) :
-            warnmsg = 'WARNING: enable.auto.commit has not been set to False for a Consumer that will manually commit '
-            warnmsg+= 'offsets. Missed or duplicate messages could result. You can set "enable.auto.commit"=False in '
-            warnmsg+= 'the "consumer" section of the config file to re-enable manual offset commits (recommended).'
+        # create the Consumer for this thread
+        if self.alive:
+            consumer = self.get_new_subscribed_consumer(
+                restart_at_beginning=self.restart_at_beginning,
+                message_key_regex=self.message_key_regex,
+                filter_new_messages=self.filter_new_messages,
+            )
+        if ("enable.auto.commit" not in consumer.configs.keys()) or (
+            consumer.configs["enable.auto.commit"] is True
+        ):
+            warnmsg = (
+                "WARNING: enable.auto.commit has not been set to False for a Consumer "
+                "that will manually commit offsets. Missed or duplicate messages could result. "
+                'You can set "enable.auto.commit"=False in the "consumer" section of the '
+                "config file to re-enable manual offset commits (recommended)."
+            )
             self.logger.warning(warnmsg)
-        #start the loop for while the controlled process is alive
-        while self.alive :
+        # start the loop for while the controlled process is alive
+        while self.alive:
             self.__do_alive_loop_iteration(consumer)
-        #commit the offset of the last message received
-        if (self.last_message is not None) and (not consumer.message_consumed_before(self.last_message)) :
+        # commit the offset of the last message received
+        if (self.last_message is not None) and (
+            not consumer.message_consumed_before(self.last_message)
+        ):
             self.__commit_last_message_offset(consumer)
-        #shut down the Consumer that was created once the process isn't alive anymore
+        # shut down the Consumer that was created once the process isn't alive anymore
         consumer.close()
 
     def _on_shutdown(self):
         super()._on_shutdown()
         self.close()
 
     @abstractmethod
-    def _process_message(self,lock,msg,*args,**kwargs) :
+    def _process_message(self, lock, msg, *args, **kwargs):
         """
         Process a single message read from the thread-independent Consumer
         Returns true if processing was successful, and False otherwise
 
-        lock = lock across all created child threads (use to enforce thread safety during processing)
+        lock = lock across all created child threads
         msg  = a single message that was consumed and should be processed by this function
 
         Not implemented in the base class
         """
         raise NotImplementedError
 
-    def __do_alive_loop_iteration(self,consumer) :
+    def __do_alive_loop_iteration(self, consumer):
         """
         Helper function to perform actions that happen continuously while the process is alive
         """
-        #consume a message from the topic
+        # consume a message from the topic
         msg = consumer.get_next_message(self.CONSUMER_POLL_TIMEOUT)
-        if msg is None :
-            time.sleep(self.NO_MESSAGE_WAIT) #wait just a bit to not over-tax things
+        if msg is None:
+            time.sleep(self.NO_MESSAGE_WAIT)  # wait just a bit to not over-tax things
             return
-        with self.lock :
-            self.n_msgs_read+=1
+        with self.lock:
+            self.n_msgs_read += 1
             self.last_message = msg
-        #send the message to the _process_message function
-        retval = self._process_message(self.lock,msg)
-        #count and (asynchronously) commit the message as processed (if it wasn't consumed already in the past)
-        if retval :
-            with self.lock :
-                self.n_msgs_processed+=1
-            if not consumer.message_consumed_before(msg) :
+        # send the message to the _process_message function
+        retval = self._process_message(self.lock, msg)
+        # count and (asynchronously) commit the message as processed
+        if retval:
+            with self.lock:
+                self.n_msgs_processed += 1
+            if not consumer.message_consumed_before(msg):
                 tps = consumer.commit(msg)
-                if tps is None :
+                if tps is None:
                     return
-                for t_p in tps :
-                    if t_p.error is not None :
-                        warnmsg = 'WARNING: failed to synchronously commit offset of last message received on '
-                        warnmsg+= f'"{t_p.topic}" partition {t_p.partition}. Duplicate messages may result '
-                        warnmsg+= f'when this Consumer is restarted. Error reason: {t_p.error.str()}'
+                for t_p in tps:
+                    if t_p.error is not None:
+                        warnmsg = (
+                            f"WARNING: failed to synchronously commit offset of last message "
+                            f'received on "{t_p.topic}" partition {t_p.partition}. '
+                            "Duplicate messages may result when this Consumer is restarted. "
+                            f"Error reason: {t_p.error.str()}"
+                        )
                         self.logger.warning(warnmsg)
 
-    def __commit_last_message_offset(self,consumer) :
+    def __commit_last_message_offset(self, consumer):
         """
-        Commit the offset of the last message received if it wasn't already consumed in the past (block until done)
+        Commit the offset of the last message received if it wasn't already consumed in the past
+        (block until done)
         """
-        try :
-            tps = consumer.commit(self.last_message,asynchronous=False)
-            if tps is not None :
-                for t_p in tps :
-                    if t_p.error is not None :
-                        warnmsg = 'WARNING: failed to synchronously commit offset of last message received on '
-                        warnmsg+= f'"{t_p.topic}" partition {t_p.partition}. Duplicate messages may result '
-                        warnmsg+= f'when this Consumer is restarted. Error reason: {t_p.error.str()}'
+        try:
+            tps = consumer.commit(self.last_message, asynchronous=False)
+            if tps is not None:
+                for t_p in tps:
+                    if t_p.error is not None:
+                        warnmsg = (
+                            f"WARNING: failed to synchronously commit offset of last message "
+                            f'received on "{t_p.topic}" partition {t_p.partition}. '
+                            "Duplicate messages may result when this Consumer is restarted. "
+                            "Error reason: {t_p.error.str()}"
+                        )
                         self.logger.warning(warnmsg)
-        except Exception as exc :
-            warnmsg = 'WARNING: failed to synchronously commit offset of last message received. '
-            warnmsg+= 'Duplicate messages may be read the next time this Consumer is started. '
-            warnmsg+= 'Error will be logged below but not re-raised.'
-            self.logger.warning(warnmsg,exc_info=exc)
+        except Exception as exc:
+            warnmsg = (
+                "WARNING: failed to synchronously commit offset of last message received. "
+                "Duplicate messages may be read the next time this Consumer is started. "
+                "Error will be logged below but not re-raised."
+            )
+            self.logger.warning(warnmsg, exc_info=exc)
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/controlled_message_reproducer.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,182 +1,235 @@
 """
 A ConsumerAndProducerGroup whose receipt and production of messages
 is managed using the ControlledProcessInfrastructure
 """
 
-#imports
+# imports
 import time
 from abc import ABC, abstractmethod
 from queue import Queue
 from ..utilities.config import RUN_CONST
 from ..utilities import ControlledProcessMultiThreaded
 from .consumer_and_producer_group import ConsumerAndProducerGroup
 
-class ControlledMessageReproducer(ControlledProcessMultiThreaded,ConsumerAndProducerGroup,ABC) :
+
+class ControlledMessageReproducer(
+    ControlledProcessMultiThreaded, ConsumerAndProducerGroup, ABC
+):
     """
-    An abstract base class combining and ControlledProcessMultiThreaded and a ConsumerAndProducerGroup
-    to systematically read messages and produce others.
+    An abstract base class combining and ControlledProcessMultiThreaded and a
+    ConsumerAndProducerGroup to systematically read messages and produce others.
     """
 
     CONSUMER_POLL_TIMEOUT = 0.050
     NO_MESSAGE_WAIT = 0.005
-    FLUSH_PRODUCER_EVERY = 100 #flush the producer after this many calls to produce_from_queue (could be fast)
-    PRODUCER_FLUSH_TIMEOUT = 0.050 #timeout for the intermediate calls to producer.flush
-
-    def __init__(self,config_path,consumer_topic_name,producer_topic_name,*,
-                 n_producer_threads=1,n_consumer_threads=RUN_CONST.DEFAULT_N_THREADS,**kwargs) :
+    # flush the producer after this many calls to produce_from_queue (could be fast)
+    FLUSH_PRODUCER_EVERY = 100
+    # timeout for the intermediate calls to producer.flush
+    PRODUCER_FLUSH_TIMEOUT = 0.050
+
+    def __init__(
+        self,
+        config_path,
+        consumer_topic_name,
+        producer_topic_name,
+        *,
+        n_producer_threads=1,
+        n_consumer_threads=RUN_CONST.DEFAULT_N_THREADS,
+        **kwargs,
+    ):
         """
         Hang onto the number of messages read, processed, and produced
         """
         self.n_msgs_read = 0
         self.n_msgs_processed = 0
         self.n_msgs_produced = 0
-        super().__init__(config_path,consumer_topic_name,n_threads=max(n_producer_threads,n_consumer_threads),**kwargs)
-        self.restart_at_beginning = False #set to true to reset new consumers to their earliest offsets
-        self.message_key_regex = None #set to some regex to filter messages by their keys
-        self.filter_new_messages = False #reset the regex after the consumer has filtered through previous messages
-        self.last_message = None #hold onto the last consumed message to commit its offset on shutdown
+        super().__init__(
+            config_path,
+            consumer_topic_name,
+            n_threads=max(n_producer_threads, n_consumer_threads),
+            **kwargs,
+        )
+        # set to true to reset new consumers to their earliest offsets
+        self.restart_at_beginning = False
+        # set to some regex to filter messages by their keys
+        self.message_key_regex = None
+        # reset the regex after the consumer has filtered through previous messages
+        self.filter_new_messages = False
+        # hold onto the last consumed message to commit its offset on shutdown
+        self.last_message = None
         self.producer_topic_name = producer_topic_name
         self.n_producer_threads = n_producer_threads
         self.n_consumer_threads = n_consumer_threads
         self.producer_message_queue = Queue()
 
-    def _run_worker(self,create_consumer=False,create_producer=False,
-                    produce_from_queue_args=None,produce_from_queue_kwargs=None):
+    def _run_worker(
+        self,
+        create_consumer=False,
+        create_producer=False,
+        produce_from_queue_args=None,
+        produce_from_queue_kwargs=None,
+    ):
         """
         Handle optional startup and shutdown of thread-independent Consumer and/or Producer.
         Serve individual messages to the _process_message function on the Consumer side,
         and produce messages from the shared Queue on the Producer side.
         """
-        #create the Consumer and/or Producer for this thread
-        if self.alive :
-            consumer, producer = self.__get_thread_consumer_and_producer(create_consumer,create_producer)
-        #start the loop for while the controlled process is alive
+        # create the Consumer and/or Producer for this thread
+        if self.alive:
+            consumer, producer = self.__get_thread_consumer_and_producer(
+                create_consumer, create_producer
+            )
+        # start the loop for while the controlled process is alive
         calls_since_producer_flush = 0
-        while self.alive :
-            #if this thread has a Consumer side
-            if consumer is not None :
+        while self.alive:
+            # if this thread has a Consumer side
+            if consumer is not None:
                 self.__consume_messages_while_alive(consumer)
-            #if this thread has a Producer side
-            if producer is not None :
-                calls_since_producer_flush = self.__produce_messages_while_alive(producer,
-                                                                                 produce_from_queue_args,
-                                                                                 produce_from_queue_kwargs,
-                                                                                 calls_since_producer_flush)
-        #commit the offset of the last message received if it wasn't already consumed in the past (block until done)
-        if ( (consumer is not None) and
-             (self.last_message is not None) and (not consumer.message_consumed_before(self.last_message)) ) :
+            # if this thread has a Producer side
+            if producer is not None:
+                calls_since_producer_flush = self.__produce_messages_while_alive(
+                    producer,
+                    produce_from_queue_args,
+                    produce_from_queue_kwargs,
+                    calls_since_producer_flush,
+                )
+        # synchronously commit the offset of the last message received
+        if (
+            (consumer is not None)
+            and (self.last_message is not None)
+            and (not consumer.message_consumed_before(self.last_message))
+        ):
             self.__commit_last_message_offset(consumer)
-        #shut down the Consumer/Producer that was created once the process isn't alive anymore
-        if consumer is not None :
+        # shut down the Consumer/Producer that was created once the process isn't alive anymore
+        if consumer is not None:
             consumer.close()
-        if producer is not None :
+        if producer is not None:
             producer.flush(timeout=-1)
             producer.close()
 
     def _on_shutdown(self):
         super()._on_shutdown()
         self.close()
 
     @abstractmethod
-    def _process_message(self,lock,msg,*args,**kwargs) :
+    def _process_message(self, lock, msg, *args, **kwargs):
         """
         Process a single message read from the thread-independent Consumer
         Returns true if processing was successful, and False otherwise
 
-        lock = lock across all created child threads (use to enforce thread safety during processing)
+        lock = lock across all created child threads
         msg  = a single message that was consumed and should be processed by this function
 
         Not implemented in the base class
         """
         raise NotImplementedError
 
-    def __get_thread_consumer_and_producer(self,create_consumer,create_producer) :
+    def __get_thread_consumer_and_producer(self, create_consumer, create_producer):
         """
         Return the consumer and producer to use for a specific thread
         """
-        if create_consumer :
-            consumer = self.get_new_subscribed_consumer(restart_at_beginning=self.restart_at_beginning,
-                                                        message_key_regex=self.message_key_regex,
-                                                        filter_new_messages=self.filter_new_messages)
-        else :
+        if create_consumer:
+            consumer = self.get_new_subscribed_consumer(
+                restart_at_beginning=self.restart_at_beginning,
+                message_key_regex=self.message_key_regex,
+                filter_new_messages=self.filter_new_messages,
+            )
+        else:
             consumer = None
-        if create_producer :
+        if create_producer:
             producer = self.get_new_producer()
-        else :
+        else:
             producer = None
-        if ( (consumer is not None) and
-             ( ('enable.auto.commit' not in consumer.configs.keys()) or
-               (consumer.configs['enable.auto.commit'] is True))) :
-            warnmsg = 'WARNING: enable.auto.commit has not been set to False for a Consumer that will manually commit '
-            warnmsg+= 'offsets. Missed or duplicate messages could result. You can set "enable.auto.commit"=False in '
-            warnmsg+= 'the "consumer" section of the config file to re-enable manual offset commits (recommended).'
+        if (consumer is not None) and (
+            ("enable.auto.commit" not in consumer.configs.keys())
+            or (consumer.configs["enable.auto.commit"] is True)
+        ):
+            warnmsg = (
+                "WARNING: enable.auto.commit has not been set to False for a Consumer "
+                "that will manually commit offsets. Missed or duplicate messages could result. "
+                'You can set "enable.auto.commit"=False in the "consumer" section of '
+                "the config file to re-enable manual offset commits (recommended)."
+            )
             self.logger.warning(warnmsg)
         return consumer, producer
 
-    def __consume_messages_while_alive(self,consumer) :
+    def __consume_messages_while_alive(self, consumer):
         """
         Runs continuously while the calling thread is alive to consume messages
         """
-        #consume a message from the topic
+        # consume a message from the topic
         msg = consumer.get_next_message(self.CONSUMER_POLL_TIMEOUT)
-        if msg is None :
-            time.sleep(self.NO_MESSAGE_WAIT) #wait just a bit to not over-tax things
+        if msg is None:
+            time.sleep(self.NO_MESSAGE_WAIT)  # wait just a bit to not over-tax things
             return
-        with self.lock :
-            self.n_msgs_read+=1
+        with self.lock:
+            self.n_msgs_read += 1
             self.last_message = msg
-        #send the message to the _process_message function
-        retval = self._process_message(self.lock,msg)
-        #count and (asynchronously) commit the message as processed (if not consumed already in the past)
-        if retval :
-            with self.lock :
-                self.n_msgs_processed+=1
-            if not consumer.message_consumed_before(msg) :
+        # send the message to the _process_message function
+        retval = self._process_message(self.lock, msg)
+        # count and (asynchronously) commit the message as processed
+        if retval:
+            with self.lock:
+                self.n_msgs_processed += 1
+            if not consumer.message_consumed_before(msg):
                 tps = consumer.commit(msg)
-                if tps is None :
+                if tps is None:
                     return
-                for t_p in tps :
-                    if t_p.error is not None :
-                        warnmsg = 'WARNING: failed to synchronously commit offset of last message '
-                        warnmsg+= f'received on "{t_p.topic}" partition {t_p.partition}. Duplicate '
-                        warnmsg+=  'messages may result when this Consumer is restarted. '
-                        warnmsg+= f'Error reason: {t_p.error.str()}'
+                for t_p in tps:
+                    if t_p.error is not None:
+                        warnmsg = (
+                            f"WARNING: failed to synchronously commit offset of last message "
+                            f'received on "{t_p.topic}" partition {t_p.partition}. '
+                            "Duplicate messages may result when this Consumer is restarted. "
+                            f"Error reason: {t_p.error.str()}"
+                        )
                         self.logger.warning(warnmsg)
 
-    def __produce_messages_while_alive(self,producer,pfq_args,pfq_kwargs,calls_since_flush) :
+    def __produce_messages_while_alive(
+        self, producer, pfq_args, pfq_kwargs, calls_since_flush
+    ):
         """
         Runs continuously while the calling thread is alive to produce messages
         """
-        if self.producer_message_queue.empty() :
-            time.sleep(self.NO_MESSAGE_WAIT) #wait just a bit to not overtax things
-        else :
+        if self.producer_message_queue.empty():
+            time.sleep(self.NO_MESSAGE_WAIT)  # wait just a bit to not overtax things
+        else:
             pfq_args = [] if pfq_args is None else pfq_args
             pfq_kwargs = {} if pfq_kwargs is None else pfq_kwargs
-            producer.produce_from_queue(self.producer_message_queue,self.producer_topic_name,
-                                        *pfq_args,**pfq_kwargs)
-        if calls_since_flush>=self.FLUSH_PRODUCER_EVERY :
+            producer.produce_from_queue(
+                self.producer_message_queue,
+                self.producer_topic_name,
+                *pfq_args,
+                **pfq_kwargs,
+            )
+        if calls_since_flush >= self.FLUSH_PRODUCER_EVERY:
             producer.flush(timeout=self.PRODUCER_FLUSH_TIMEOUT)
-            calls_since_flush=0
-        else :
-            calls_since_flush+=1
+            calls_since_flush = 0
+        else:
+            calls_since_flush += 1
         return calls_since_flush
 
-    def __commit_last_message_offset(self,consumer) :
+    def __commit_last_message_offset(self, consumer):
         """
         Commit the offset of the last message received while blocking
         """
-        try :
-            tps = consumer.commit(self.last_message,asynchronous=False)
-            if tps is None :
+        try:
+            tps = consumer.commit(self.last_message, asynchronous=False)
+            if tps is None:
                 return
-            for t_p in tps :
-                if t_p.error is not None :
-                    warnmsg = 'WARNING: failed to synchronously commit offset of last message received on '
-                    warnmsg+= f'"{t_p.topic}" partition {t_p.partition}. Duplicate messages may result '
-                    warnmsg+= f'when this Consumer is restarted. Error reason: {t_p.error.str()}'
+            for t_p in tps:
+                if t_p.error is not None:
+                    warnmsg = (
+                        f"WARNING: failed to synchronously commit offset of last message "
+                        f'received on "{t_p.topic}" partition {t_p.partition}. '
+                        "Duplicate messages may result when this Consumer is restarted. "
+                        f"Error reason: {t_p.error.str()}"
+                    )
                     self.logger.warning(warnmsg)
-        except Exception as exc :
-            warnmsg = 'WARNING: failed to synchronously commit offset of last message received. '
-            warnmsg+= 'Duplicate messages may be read the next time this Consumer is started. '
-            warnmsg+= 'Error will be logged below but not re-raised.'
-            self.logger.warning(warnmsg,exc_info=exc)
+        except Exception as exc:
+            warnmsg = (
+                "WARNING: failed to synchronously commit offset of last message received. "
+                "Duplicate messages may be read the next time this Consumer is started. "
+                "Error will be logged below but not re-raised."
+            )
+            self.logger.warning(warnmsg, exc_info=exc)
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/openmsistream_consumer.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,306 +1,371 @@
 """A wrapped Kafka Consumer. May consume encrypted messages."""
 
-#imports
+# imports
 import uuid, warnings, methodtools
 from confluent_kafka import DeserializingConsumer, Message
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto import KafkaConsumer
 from ..utilities import LogOwner
-from ..utilities.misc import raise_err_with_optional_logger, debug_msg_with_optional_logger
+from ..utilities.misc import (
+    raise_err_with_optional_logger,
+    debug_msg_with_optional_logger,
+)
 from .utilities import add_kwargs_to_configs, KCCommitOffsetDictKey, KCCommitOffset
 from .config_file_parser import KafkaConfigFileParser
 from .openmsistream_kafka_crypto import OpenMSIStreamKafkaCrypto
 from .serialization import CompoundDeserializer
 
-class OpenMSIStreamConsumer(LogOwner) :
+
+class OpenMSIStreamConsumer(LogOwner):
     """
     Wrapper for working with a Consumer of some type. Expects message values that are
     :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` objects by default;
-    other message value types can be accommodated by setting "value.deserializer" in the config file.
+    other message value types can be accommodated by setting "value.deserializer"
+    in the config file.
 
     :param consumer_type: The type of underlying Consumer that should be used
-    :type consumer_type: :class:`confluent_kafka.DeserializingConsumer` or :class:`kafkacrypto.KafkaConsumer`
-    :param configs: A dictionary of configuration names and parameters to use in instantiating the underlying Consumer
+    :type consumer_type: :class:`confluent_kafka.DeserializingConsumer` or
+        :class:`kafkacrypto.KafkaConsumer`
+    :param configs: A dictionary of configuration names and parameters to use in instantiating
+        the underlying Consumer
     :type configs: dict
-    :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object that should be used
-        to instantiate the Consumer. Only needed if `consumer_type` is :class:`kafkacrypto.KafkaConsumer`.
+    :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object
+        that should be used to instantiate the Consumer. Only needed if `consumer_type` is
+        :class:`kafkacrypto.KafkaConsumer`.
     :type kafkacrypto: :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto`, optional
     :param message_key_regex: A regular expression to filter messages based on their keys.
         Only messages matching this regex will be returned by :func:`~get_next_message`.
-        This parameter only has an effect if `restart_at_beginning` is true and a consumer group with the given ID
-        has previously consumed messages from the topic, or if `filter_new_messages` is True.
-        Messages with keys that are not strings will always be consumed, logging warnings if they should be filtered.
+        This parameter only has an effect if `restart_at_beginning` is true and a consumer group
+        with the given ID has previously consumed messages from the topic, or if
+        `filter_new_messages` is True. Messages with keys that are not strings will always
+        be consumed, logging warnings if they should be filtered.
     :type message_key_regex: :func:`re.compile` or None, optional
-    :param filter_new_messages: If False (the default) the `message_key_regex` will only be used to filter
-        messages from before each partition's currently committed location. Useful if you want to process only some
-        messages from earlier in the topic, but all new messages that have never been read. To filter every message read
-        instead of just previously-consumed messages, set this to True.
+    :param filter_new_messages: If False (the default) the `message_key_regex` will only be used
+        to filter messages from before each partition's currently committed location.
+        Useful if you want to process only some messages from earlier in the topic, but all new
+        messages that have never been read. To filter every message read instead of just
+        previously-consumed messages, set this to True.
     :type filter_new_messages: bool, optional
-    :param starting_offsets: A list of :class:`confluent_kafka.TopicPartition` objects listing the initial starting
-        offsets for each partition in the topic for Consumers with this group ID. If `filter_new_messages` is
-        False, messages with offsets greater than or equal to these will NOT be filtered using `message_key_regex`.
+    :param starting_offsets: A list of :class:`confluent_kafka.TopicPartition` objects listing
+        the initial starting offsets for each partition in the topic for Consumers with this
+        group ID. If `filter_new_messages` is False, messages with offsets greater than or
+        equal to these will NOT be filtered using `message_key_regex`.
     :type starting_offsets: list(:class:`confluent_kafka.TopicPartition`) or None, optional
     :param kwargs: Any extra keyword arguments are added to the configuration dict for the Consumer,
         with underscores in their names replaced by dots
     :type kwargs: dict
 
     :raises ValueError: if `consumer_type` is not :class:`confluent_kafka.DeserializingConsumer`
         or :class:`kafkacrypto.KafkaConsumer`
-    :raises ValueError: if `consumer_type` is :class:`kafkacrypto.KafkaConsumer` and `kafkacrypto` is None
+    :raises ValueError: if `consumer_type` is :class:`kafkacrypto.KafkaConsumer` and
+        `kafkacrypto` is None
     """
 
-    def __init__(self,consumer_type,configs,kafkacrypto=None,
-                 message_key_regex=None,filter_new_messages=False,starting_offsets=None,**kwargs) :
+    def __init__(
+        self,
+        consumer_type,
+        configs,
+        kafkacrypto=None,
+        message_key_regex=None,
+        filter_new_messages=False,
+        starting_offsets=None,
+        **kwargs,
+    ):
         """
         Constructor method
         """
         super().__init__(**kwargs)
-        if consumer_type==KafkaConsumer :
-            if kafkacrypto is None :
-                errmsg = 'ERROR: creating a KafkaConsumer requires holding onto its KafkaCrypto objects!'
-                self.logger.error(errmsg,exc_type=ValueError)
+        if consumer_type == KafkaConsumer:
+            if kafkacrypto is None:
+                errmsg = "ERROR: creating a KafkaConsumer requires giving its KafkaCrypto objects!"
+                self.logger.error(errmsg, exc_type=ValueError)
             self.__kafkacrypto = kafkacrypto
             self._consumer = consumer_type(**configs)
             self.__messages = []
-        elif consumer_type==DeserializingConsumer :
+        elif consumer_type == DeserializingConsumer:
             self._consumer = consumer_type(configs)
-        else :
-            errmsg=f'ERROR: Unrecognized consumer type {consumer_type} for OpenMSIStreamConsumer!'
-            self.logger.error(errmsg,exc_type=ValueError)
+        else:
+            errmsg = f"ERROR: Unrecognized consumer type {consumer_type} for OpenMSIStreamConsumer!"
+            self.logger.error(errmsg, exc_type=ValueError)
         self.configs = configs
-        self.message_key_regex=message_key_regex
-        self.filter_new_messages=filter_new_messages
-        self.__starting_offsets=starting_offsets
+        self.message_key_regex = message_key_regex
+        self.filter_new_messages = filter_new_messages
+        self.__starting_offsets = starting_offsets
 
     @staticmethod
-    def get_consumer_args_kwargs(config_file_path,logger=None,kafkacrypto=None,**kwargs) :
+    def get_consumer_args_kwargs(
+        config_file_path, logger=None, kafkacrypto=None, **kwargs
+    ):
         """
-        Return the list of arguments and dictionary or keyword arguments that should be used to instantiate
-        :class:`~OpenMSIStreamConsumer` objects based on the given config file.
+        Return the list of arguments and dictionary or keyword arguments that should be used
+        to instantiate :class:`~OpenMSIStreamConsumer` objects based on the given config file.
         Used to share a single :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` instance across
         several Consumers.
 
         :param config_file_path: Path to the config file to use in defining Consumers
         :type config_file_path: :class:`pathlib.Path`
         :param logger: The :class:`~.utilities.Logger` object to use for each of the
             :class:`~OpenMSIStreamConsumer` objects
         :type logger: :class:`~.utilities.Logger`
-        :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object that should be
-            used to instantiate Consumers. Only needed if a single specific
+        :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object
+            that should be used to instantiate Consumers. Only needed if a single specific
             :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` instance should be shared.
         :type kafkacrypto: :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto`, optional
-        :param kwargs: Any extra keyword arguments are added to the configuration dict for the Consumers,
-            with underscores in their names replaced by dots
+        :param kwargs: Any extra keyword arguments are added to the configuration dict for
+            the Consumers, with underscores in their names replaced by dots
         :type kwargs: dict
 
-        :return: ret_args, the list of arguments to create new :class:`~OpenMSIStreamConsumer` objects
-            based on the config file and arguments to this method
+        :return: ret_args, the list of arguments to create new :class:`~OpenMSIStreamConsumer`
+            objects based on the config file and arguments to this method
         :rtype: list
-        :return: ret_kwargs, the dictionary of keyword arguments to create new :class:`~OpenMSIStreamConsumer` objects
-            based on the config file and arguments to this method
+        :return: ret_kwargs, the dictionary of keyword arguments to create new
+            :class:`~OpenMSIStreamConsumer` objects based on the config file and arguments
+            to this method
         :rtype: dict
         """
-        parser = KafkaConfigFileParser(config_file_path,logger=logger)
-        ret_kwargs = {'logger':logger}
-        #get the broker and consumer configurations
-        all_configs = {**parser.broker_configs,**parser.consumer_configs}
-        all_configs = add_kwargs_to_configs(all_configs,logger,**kwargs)
-        #all_configs['debug']='broker,topic,msg'
-        #if the group.id has been set as "create_new" generate a new group ID
-        if 'group.id' in all_configs and all_configs['group.id'].lower()=='create_new' :
-            all_configs['group.id']=str(uuid.uuid1())
-        #Use a DeserializingConsumer by default
-        if kafkacrypto is None and parser.kc_config_file_str is None :
-            ret_args = [DeserializingConsumer,all_configs]
+        parser = KafkaConfigFileParser(config_file_path, logger=logger)
+        ret_kwargs = {"logger": logger}
+        # get the broker and consumer configurations
+        all_configs = {**parser.broker_configs, **parser.consumer_configs}
+        all_configs = add_kwargs_to_configs(all_configs, logger, **kwargs)
+        # all_configs['debug']='broker,topic,msg'
+        # if the group.id has been set as "create_new" generate a new group ID
+        if "group.id" in all_configs and all_configs["group.id"].lower() == "create_new":
+            all_configs["group.id"] = str(uuid.uuid1())
+        # Use a DeserializingConsumer by default
+        if kafkacrypto is None and parser.kc_config_file_str is None:
+            ret_args = [DeserializingConsumer, all_configs]
             return ret_args, ret_kwargs
-        #if "kafkacrypto" was given, or there are configs for KafkaCrypto, use a KafkaConsumer
-        if kafkacrypto is not None :
-            if not isinstance(kafkacrypto,OpenMSIStreamKafkaCrypto) :
-                errmsg = f'ERROR: kafkacrypto argument type = {type(kafkacrypto)}'
-                raise_err_with_optional_logger(logger,errmsg,TypeError)
-            debugmsg = f'Consumed messages will be decrypted using configs at {kafkacrypto.config_file_path}'
-            debug_msg_with_optional_logger(logger,debugmsg)
+        # if "kafkacrypto" was given, or there are configs for KafkaCrypto, use a KafkaConsumer
+        if kafkacrypto is not None:
+            if not isinstance(kafkacrypto, OpenMSIStreamKafkaCrypto):
+                errmsg = f"ERROR: kafkacrypto argument type = {type(kafkacrypto)}"
+                raise_err_with_optional_logger(logger, errmsg, TypeError)
+            debugmsg = (
+                f"Consumed messages will be decrypted using configs "
+                f"at {kafkacrypto.config_file_path}"
+            )
+            debug_msg_with_optional_logger(logger, debugmsg)
             k_c = kafkacrypto
-        else :
-            debugmsg = f'Consumed messages will be decrypted using configs at {parser.kc_config_file_str}'
-            debug_msg_with_optional_logger(logger,debugmsg)
-            k_c = OpenMSIStreamKafkaCrypto(parser.broker_configs,parser.kc_config_file_str)
-        if 'key.deserializer' in all_configs :
-            keydes = CompoundDeserializer(k_c.key_deserializer,all_configs.pop('key.deserializer'))
-        else :
+        else:
+            debugmsg = (
+                f"Consumed messages will be decrypted using configs "
+                f"at {parser.kc_config_file_str}"
+            )
+            debug_msg_with_optional_logger(logger, debugmsg)
+            k_c = OpenMSIStreamKafkaCrypto(
+                parser.broker_configs, parser.kc_config_file_str
+            )
+        if "key.deserializer" in all_configs:
+            keydes = CompoundDeserializer(
+                k_c.key_deserializer, all_configs.pop("key.deserializer")
+            )
+        else:
             keydes = k_c.key_deserializer
-        if 'value.deserializer' in all_configs :
-            valdes = CompoundDeserializer(k_c.value_deserializer,all_configs.pop('value.deserializer'))
-        else :
+        if "value.deserializer" in all_configs:
+            valdes = CompoundDeserializer(
+                k_c.value_deserializer, all_configs.pop("value.deserializer")
+            )
+        else:
             valdes = k_c.value_deserializer
-        all_configs['key_deserializer']=keydes
-        all_configs['value_deserializer']=valdes
-        ret_args = [KafkaConsumer,all_configs]
-        ret_kwargs['kafkacrypto']=k_c
+        all_configs["key_deserializer"] = keydes
+        all_configs["value_deserializer"] = valdes
+        ret_args = [KafkaConsumer, all_configs]
+        ret_kwargs["kafkacrypto"] = k_c
         return ret_args, ret_kwargs
 
     @classmethod
-    def from_file(cls,*args,**kwargs) :
+    def from_file(cls, *args, **kwargs):
         """
-        Wrapper around :func:`~OpenMSIStreamConsumer.get_consumer_args_kwargs` and the :class:`~OpenMSIStreamConsumer`
-        constructor to return a single :class:`~OpenMSIStreamConsumer` from a given config file/arguments.
+        Wrapper around :func:`~OpenMSIStreamConsumer.get_consumer_args_kwargs` and the
+        :class:`~OpenMSIStreamConsumer` constructor to return a single
+        :class:`~OpenMSIStreamConsumer` from a given config file/arguments.
         Arguments are the same as :func:`~OpenMSIStreamConsumer.get_consumer_args_kwargs`
 
         :returns: An :class:`~OpenMSIStreamConsumer` object based on the given config file/arguments
         :rtype: :class:`~OpenMSIStreamConsumer`
         """
-        args_to_use, kwargs_to_use = OpenMSIStreamConsumer.get_consumer_args_kwargs(*args,**kwargs)
-        return cls(*args_to_use,**kwargs_to_use)
+        args_to_use, kwargs_to_use = OpenMSIStreamConsumer.get_consumer_args_kwargs(
+            *args, **kwargs
+        )
+        return cls(*args_to_use, **kwargs_to_use)
 
-    def get_next_message(self,*poll_args,**poll_kwargs) :
+    def get_next_message(self, *poll_args, **poll_kwargs):
         """
-        Call poll() for the underlying consumer and return any successfully consumed message's value.
+        Call poll() for the underlying consumer and return any consumed message's value.
 
-        If this Consumer's `message_key_regex` is not None this method may return None even though a message
-        was consumed.
+        If this Consumer's `message_key_regex` is not None this method may return None
+        even though a message was consumed.
 
-        For the case of encrypted messages, this may return a :class:`kafkacrypto.Message` object with
-        :class:`kafkacrypto.KafkaCryptoMessages` for its key and/or value if the message fails to be
-        decrypted within a certain amount of time
+        For the case of encrypted messages, this may return a :class:`kafkacrypto.Message`
+        object with :class:`kafkacrypto.KafkaCryptoMessages` for its key and/or value
+        if the message fails to be decrypted within a certain amount of time
 
-        All arguments/keyword arguments are passed through to the underlying Consumer's poll() function.
+        All arguments/keyword arguments are passed through to the underlying Consumer's
+        poll() function.
 
         :return: a single consumed :class:`confluent_kafka.Message` object, an undecrypted
             :class:`kafkacrypto.Message` object, or None
         :rtype: :class:`confluent_kafka.Message`, :class:`kafkacrypto.Message`, or None
 
-        :raises Exception: for any error encountered in calling poll(). A special error-level message will be
-            logged, including the stack trace of the Exception.
+        :raises Exception: for any error encountered in calling poll(). A special
+            error-level message will be logged, including the stack trace of the Exception.
         """
-        #There's one version for the result of a KafkaConsumer.poll() call
-        if isinstance(self._consumer,KafkaConsumer) :
-            #check if there are any messages still waiting to be processed from a recent KafkaCrypto poll call
-            if len(self.__messages)>0 :
+        # There's one version for the result of a KafkaConsumer.poll() call
+        if isinstance(self._consumer, KafkaConsumer):
+            # check if there are any messages still waiting to be processed
+            if len(self.__messages) > 0:
                 consumed_msg = self.__messages.pop(0)
                 return self._filter_message(consumed_msg)
-            msg_dict = self._consumer.poll(*poll_args,**poll_kwargs)
-            if msg_dict=={} :
+            msg_dict = self._consumer.poll(*poll_args, **poll_kwargs)
+            if msg_dict == {}:
                 return None
-            for t_p in msg_dict.keys() :
-                for msg in msg_dict[t_p] :
+            for t_p in msg_dict.keys():
+                for msg in msg_dict[t_p]:
                     self.__messages.append(msg)
-            return self.get_next_message(*poll_args,**poll_kwargs)
-        #And another version for a regular Consumer
+            return self.get_next_message(*poll_args, **poll_kwargs)
+        # And another version for a regular Consumer
         consumed_msg = None
-        try :
-            consumed_msg = self._consumer.poll(*poll_args,**poll_kwargs)
-        except Exception as exc :
-            errmsg = 'ERROR: encountered an error in a call to consumer.poll() and this message will be '
-            errmsg+= 'skipped. Exception will be logged below and re-raised.'
-            self.logger.error(errmsg,exc_info=exc,reraise=True)
+        try:
+            consumed_msg = self._consumer.poll(*poll_args, **poll_kwargs)
+        except Exception as exc:
+            errmsg = (
+                "ERROR: encountered an error in a call to consumer.poll() and this message "
+                "will be skipped. Exception will be logged below and re-raised."
+            )
+            self.logger.error(errmsg, exc_info=exc, reraise=True)
             return None
-        if consumed_msg is not None and consumed_msg!={} :
-            if consumed_msg.error() is not None or consumed_msg.value() is None :
-                warnmsg = f'WARNING: unexpected consumed message, consumed_msg = {consumed_msg}'
-                warnmsg+= f', consumed_msg.error() = {consumed_msg.error()}, '
-                warnmsg+= f'consumed_msg.value() = {consumed_msg.value()}'
+        if consumed_msg is not None and consumed_msg != {}:
+            if consumed_msg.error() is not None or consumed_msg.value() is None:
+                warnmsg = (
+                    f"WARNING: unexpected consumed message, consumed_msg = {consumed_msg}, "
+                    f"consumed_msg.error() = {consumed_msg.error()}, "
+                    f"consumed_msg.value() = {consumed_msg.value()}"
+                )
                 self.logger.warning(warnmsg)
             return self._filter_message(consumed_msg)
         return None
 
-    def subscribe(self,*args,**kwargs) :
+    def subscribe(self, *args, **kwargs):
         """
         A wrapper around the underlying Consumer's subscribe() method
         """
-        return self._consumer.subscribe(*args,**kwargs)
+        return self._consumer.subscribe(*args, **kwargs)
 
-    def commit(self,message=None,offsets=None,asynchronous=True) :
+    def commit(self, message=None, offsets=None, asynchronous=True):
         """
         A wrapper around the underlying Consumer's commit() method.
         Exactly one of `message` and `offsets` must be given.
 
         :param message: The message whose offset should be committed
         :type message: :class:`confluent_kafka.Message` or :class:`kafkacrypto.Message`, optional
         :param offsets: The list of topic+partitions+offsets to commit
         :type offsets: list(:class:`confluent_kafka.TopicPartition`), optional
-        :param asynchronous: If True, the Consumer.commit call will return immediately and run asynchronously
-            instead of blocking
+        :param asynchronous: If True, the Consumer.commit call will return immediately and
+            run asynchronously instead of blocking
         :type asynchronous: bool
 
         :raises ValueError: if `message` and `offsets` are both given
         """
-        if (message is not None) and (not isinstance(message,Message)) :
-            try :
-                offset_dict = {KCCommitOffsetDictKey(message.topic,message.partition):KCCommitOffset(message.offset)}
-                if asynchronous :
+        if (message is not None) and (not isinstance(message, Message)):
+            try:
+                offset_dict = {
+                    KCCommitOffsetDictKey(
+                        message.topic, message.partition
+                    ): KCCommitOffset(message.offset)
+                }
+                if asynchronous:
                     return self._consumer.commit_async(offsets=offset_dict)
                 return self._consumer.commit(offsets=offset_dict)
-            except Exception :
-                warnmsg = 'WARNING: failed to commit an offset for an encrypted message. '
-                warnmsg = 'Duplicates may result if the Consumer is restarted.'
+            except Exception:
+                warnmsg = "WARNING: failed to commit an offset for an encrypted message. "
+                warnmsg = "Duplicates may result if the Consumer is restarted."
                 self.logger.warning(warnmsg)
                 return None
-        if message is None :
-            return self._consumer.commit(offsets=offsets,asynchronous=asynchronous)
-        if offsets is None :
-            return self._consumer.commit(message=message,asynchronous=asynchronous)
-        errmsg = 'ERROR: "message" and "offset" arguments are exclusive for Consumer.commit. Nothing commited.'
-        self.logger.error(errmsg,exc_type=ValueError)
+        if message is None:
+            return self._consumer.commit(offsets=offsets, asynchronous=asynchronous)
+        if offsets is None:
+            return self._consumer.commit(message=message, asynchronous=asynchronous)
+        errmsg = (
+            'ERROR: "message" and "offset" arguments are exclusive for Consumer.commit. '
+            "Nothing committed."
+        )
+        self.logger.error(errmsg, exc_type=ValueError)
         return None
 
-    def close(self,*args,**kwargs) :
+    def close(self, *args, **kwargs):
         """
-        Combined wrapper around the underlying Consumer's close() method and :func:`kafkacrypto.KafkaCrypto.close`.
+        Combined wrapper around the underlying Consumer's close() method and
+        :func:`kafkacrypto.KafkaCrypto.close`.
         """
-        self._consumer.close(*args,**kwargs)
-        try :
-            if self.__kafkacrypto :
+        self._consumer.close(*args, **kwargs)
+        try:
+            if self.__kafkacrypto:
                 self.__kafkacrypto.close()
-        except Exception :
+        except Exception:
             pass
-        finally :
+        finally:
             self.__kafkacrypto = None
 
-    def _filter_message(self,msg) :
+    def _filter_message(self, msg):
         """
         Checks a message's key against the regex and its offset against the starting offsets.
         Returns None if a message should be skipped, otherwise returns the message.
         """
-        if (self.message_key_regex is not None) and (self.filter_new_messages or self.message_consumed_before(msg)) :
-            try :
-                msg_key = msg.key() #from a regular Kafka Consumer
-            except TypeError :
-                msg_key = msg.key #from KafkaCrypto
-            if not isinstance(msg_key,str) :
-                warnmsg = f'WARNING: found a message whose key ({msg_key}) is not a string, but which should be '
-                warnmsg+= 'filtered using the key regex. This message will be consumed as though it successfully '
-                warnmsg+= 'passed the filter.'
+        if (self.message_key_regex is not None) and (
+            self.filter_new_messages or self.message_consumed_before(msg)
+        ):
+            try:
+                msg_key = msg.key()  # from a regular Kafka Consumer
+            except TypeError:
+                msg_key = msg.key  # from KafkaCrypto
+            if not isinstance(msg_key, str):
+                warnmsg = (
+                    f"WARNING: found a message whose key ({msg_key}) is not a string, "
+                    "but which should be filtered using the key regex. "
+                    "This message will be consumed as though it successfully passed the filter."
+                )
                 self.logger.warning(warnmsg)
                 return msg
-            if self.message_key_regex.match(msg_key) :
+            if self.message_key_regex.match(msg_key):
                 return msg
             return None
         return msg
 
     @methodtools.lru_cache()
-    def message_consumed_before(self,msg) :
+    def message_consumed_before(self, msg):
         """
-        Returns True if a message has an offset less than the starting offset for the topic/partition, False otherwise
+        Returns True if a message has an offset less than the starting offset
+        for the topic/partition, False otherwise
         """
-        try : #from a regular Kafka Consumer
+        try:  # from a regular Kafka Consumer
             msg_topic = msg.topic()
             msg_partition = msg.partition()
             msg_offset = msg.offset()
-        except TypeError : #from KafkaCrypto
+        except TypeError:  # from KafkaCrypto
             msg_topic = msg.topic
             msg_partition = msg.partition
             msg_offset = msg.offset
-        if not (isinstance(msg_topic,str) and isinstance(msg_partition,int) and isinstance(msg_offset,int)) :
-            errmsg =  'ERROR: failed to check whether a message has been consumed before '
-            errmsg+= f'because its topic/partition/offset are {msg_topic}/{msg_partition}/{msg_offset}!'
-            self.logger.error(errmsg,exc_type=TypeError)
+        if not (
+            isinstance(msg_topic, str)
+            and isinstance(msg_partition, int)
+            and isinstance(msg_offset, int)
+        ):
+            errmsg = (
+                "ERROR: failed to check whether a message has been consumed before "
+                f"because its topic/partition/offset are {msg_topic}/{msg_partition}/{msg_offset}!"
+            )
+            self.logger.error(errmsg, exc_type=TypeError)
         starting_offset = None
-        for tpo in self.__starting_offsets :
-            if tpo.topic==msg_topic and tpo.partition==msg_partition :
+        for tpo in self.__starting_offsets:
+            if tpo.topic == msg_topic and tpo.partition == msg_partition:
                 starting_offset = tpo.offset
-        if starting_offset is None :
-            errmsg = 'ERROR: failed to check whether a message has been consumed before '
-            errmsg+= 'because its topic/partition were not found in the list of starting offsets'
-            self.logger.error(errmsg,exc_type=ValueError)
-        return msg_offset<starting_offset
+        if starting_offset is None:
+            errmsg = (
+                "ERROR: failed to check whether a message has been consumed before "
+                "because its topic/partition were not found in the list of starting offsets"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        return msg_offset < starting_offset
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,92 @@
-"""Wrapper around the KafkaCrypto producer/consumer pair communicating with the key passing topics"""
+"""
+Wrapper around the KafkaCrypto producer/consumer pair communicating with the key passing topics
+"""
 
-#imports
+# imports
 import pathlib, uuid, warnings, logging
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto import KafkaProducer, KafkaConsumer, KafkaCrypto
 from ..utilities.misc import change_dir
 
-class OpenMSIStreamKafkaCrypto :
+
+class OpenMSIStreamKafkaCrypto:
     """
     A wrapper class to own and work with the Producers, Consumers, and other objects needed
     by KafkaCrypto to handle encrypting/decrypting messages and exchanging keys
 
-    :param broker_configs: the producer/consumer-agnostic configurations for connecting to the broker
+    :param broker_configs: the producer/consumer-agnostic configurations for connecting
+        to the broker
     :type broker_configs: dict
     :param config_file: the path to the KafkaCrypto config file for the node being used
     :type config_file: :class:`pathlib.Path`
     """
 
     @property
-    def config_file_path(self) :
+    def config_file_path(self):
         """
         The path to the KafkaCrypto config file used
         """
         return self.__config_file
+
     @property
-    def key_serializer(self) :
+    def key_serializer(self):
         """
         The crypto key serializer
         """
         return self._kc.getKeySerializer()
+
     @property
-    def key_deserializer(self) :
+    def key_deserializer(self):
         """
         The crypto key deserializer
         """
         return self._kc.getKeyDeserializer()
+
     @property
-    def value_serializer(self) :
+    def value_serializer(self):
         """
         The crypto value serializer
         """
         return self._kc.getValueSerializer()
+
     @property
-    def value_deserializer(self) :
+    def value_deserializer(self):
         """
         The crypto value deserializer
         """
         return self._kc.getValueDeserializer()
 
-    def __init__(self,broker_configs,config_file) :
+    def __init__(self, broker_configs, config_file):
         """
         Constructor method
         """
         producer_configs = broker_configs.copy()
         consumer_configs = broker_configs.copy()
-        #figure out a consumer group ID to use (KafkaCrypto Consumers need one)
-        if 'group.id' not in consumer_configs.keys() :
-            consumer_configs['group.id'] = str(uuid.uuid1())
-        with change_dir(pathlib.Path(config_file).parent) :
-            kc_logger = logging.getLogger('kafkacrypto')
+        # figure out a consumer group ID to use (KafkaCrypto Consumers need one)
+        if "group.id" not in consumer_configs.keys():
+            consumer_configs["group.id"] = str(uuid.uuid1())
+        with change_dir(pathlib.Path(config_file).parent):
+            kc_logger = logging.getLogger("kafkacrypto")
             kc_logger.setLevel(logging.ERROR)
-            #start up the producer and consumer
+            # start up the producer and consumer
             self._kcp = KafkaProducer(**producer_configs)
             self._kcc = KafkaConsumer(**consumer_configs)
-            #initialize the KafkaCrypto object
-            self._kc = KafkaCrypto(None,self._kcp,self._kcc,config_file)
+            # initialize the KafkaCrypto object
+            self._kc = KafkaCrypto(None, self._kcp, self._kcc, config_file)
             kc_logger.setLevel(logging.WARNING)
         self.__config_file = config_file
 
-    def close(self) :
+    def close(self):
         """
         Close the :class:`kafkacrypto.KafkaCrypto` object and un-set its producer/consumer
         """
-        try :
+        try:
             self._kc.close()
-        except Exception :
+        except Exception:
             pass
-        finally :
+        finally:
             self._kc = None
             self._kcp = None
             self._kcc = None
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/openmsistream_producer.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_producer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,309 +1,367 @@
 """A wrapped Kafka Producer. May produce encrypted messages."""
 
-#imports
+# imports
 import time, warnings
 from confluent_kafka import SerializingProducer
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto import KafkaProducer
 from ..utilities import LogOwner
-from ..utilities.misc import raise_err_with_optional_logger, debug_msg_with_optional_logger
+from ..utilities.misc import (
+    raise_err_with_optional_logger,
+    debug_msg_with_optional_logger,
+)
 from .utilities import add_kwargs_to_configs, default_producer_callback, make_callback
 from .producible import Producible
 from .config_file_parser import KafkaConfigFileParser
 from .openmsistream_kafka_crypto import OpenMSIStreamKafkaCrypto
 from .serialization import CompoundSerializer
 
-class OpenMSIStreamProducer(LogOwner) :
+
+class OpenMSIStreamProducer(LogOwner):
     """
     Wrapper for working with a Producer of some type. Expects message values that are
     :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk` objects by default;
-    other message value types can be accommodated by setting "value.serializer" in the config file.
+    other message value types can be accommodated by setting "value.serializer"
+    in the config file.
 
     :param producer_type: The type of underlying Producer that should be used
-    :type producer_type: :class:`confluent_kafka.SerializingProducer` or :class:`kafkacrypto.KafkaProducer`
-    :param configs: A dictionary of configuration names and parameters to use in instantiating the underlying Producer
+    :type producer_type: :class:`confluent_kafka.SerializingProducer` or
+        :class:`kafkacrypto.KafkaProducer`
+    :param configs: A dictionary of configuration names and parameters to use in instantiating
+        the underlying Producer
     :type configs: dict
-    :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object that should be used
-        to instantiate the Producer. Only needed if `producer_type` is :class:`kafkacrypto.KafkaProducer`.
+    :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object that
+        should be used to instantiate the Producer. Only needed if `producer_type` is
+        :class:`kafkacrypto.KafkaProducer`.
     :type kafkacrypto: :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto`, optional
-    :param kwargs: Any extra keyword arguments (other than "logger") are added to the configuration dict for the
-        Producer, with underscores in their names replaced by dots
+    :param kwargs: Any extra keyword arguments (other than "logger") are added to the
+        configuration dict for the Producer, with underscores in their names replaced by dots
     :type kwargs: dict
 
     :raises ValueError: if `producer_type` is not :class:`confluent_kafka.SerializingProducer`
         or :class:`kafkacrypto.KafkaProducer`
-    :raises ValueError: if `producer_type` is :class:`kafkacrypto.KafkaProducer` and `kafkacrypto` is None
+    :raises ValueError: if `producer_type` is :class:`kafkacrypto.KafkaProducer` and
+        `kafkacrypto` is None
     """
 
-    POLL_EVERY = 5 # poll the producer at least every 5 calls to produce
+    POLL_EVERY = 5  # poll the producer at least every 5 calls to produce
 
-    def __init__(self,producer_type,configs,kafkacrypto=None,**kwargs) :
+    def __init__(self, producer_type, configs, kafkacrypto=None, **kwargs):
         """
         Constructor method
         """
         super().__init__(**kwargs)
-        if producer_type==KafkaProducer :
-            if kafkacrypto is None :
-                errmsg = 'ERROR: creating a KafkaProducer requires holding onto its KafkaCrypto objects!'
-                self.logger.error(errmsg,exc_type=ValueError)
+        if producer_type == KafkaProducer:
+            if kafkacrypto is None:
+                errmsg = "ERROR: creating a KafkaProducer requires giving its KafkaCrypto objects!"
+                self.logger.error(errmsg, exc_type=ValueError)
             self.__kafkacrypto = kafkacrypto
             self._producer = producer_type(**configs)
-        elif producer_type==SerializingProducer :
+        elif producer_type == SerializingProducer:
             self._producer = producer_type(configs)
-        else :
-            errmsg=f'ERROR: Unrecognized producer type {producer_type} for OpenMSIStreamProducer!'
-            self.logger.error(errmsg,exc_type=ValueError)
+        else:
+            errmsg = f"ERROR: Unrecognized producer type {producer_type} for OpenMSIStreamProducer!"
+            self.logger.error(errmsg, exc_type=ValueError)
         # poll the producer at least every 5 calls to produce
         self.__poll_counter = 0
         # create an ID for the producer based on its location in memory
         self.producer_id = str(hex(id(self)))[2:]
 
     @staticmethod
-    def get_producer_args_kwargs(config_file_path,logger=None,kafkacrypto=None,**kwargs) :
+    def get_producer_args_kwargs(
+        config_file_path, logger=None, kafkacrypto=None, **kwargs
+    ):
         """
-        Return the list of arguments and dictionary or keyword arguments that should be used to instantiate
-        :class:`~OpenMSIStreamProducer` objects based on the given config file.
+        Return the list of arguments and dictionary or keyword arguments that should be used
+        to instantiate :class:`~OpenMSIStreamProducer` objects based on the given config file.
         Used to share a single :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` instance across
         several Producers.
 
         :param config_file_path: Path to the config file to use in defining Producers
         :type config_file_path: :class:`pathlib.Path`
         :param logger: The :class:`~.utilities.Logger` object to use for each of the
             :class:`~OpenMSIStreamProducer` objects
         :type logger: :class:`~.utilities.Logger`
         :param kafkacrypto: The :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` object that should
             be used to instantiate Producers. Only needed if a single specific
             :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto` instance should be shared.
         :type kafkacrypto: :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto`, optional
-        :param kwargs: Any extra keyword arguments are added to the configuration dict for the Producers,
-            with underscores in their names replaced by dots
+        :param kwargs: Any extra keyword arguments are added to the configuration dict for the
+            Producers, with underscores in their names replaced by dots
         :type kwargs: dict
 
-        :return: ret_args, the list of arguments to create new :class:`~OpenMSIStreamProducer` objects
-            based on the config file and arguments to this method
+        :return: ret_args, the list of arguments to create new :class:`~OpenMSIStreamProducer`
+            objects based on the config file and arguments to this method
         :rtype: list
-        :return: ret_kwargs, the dictionary of keyword arguments to create new :class:`~OpenMSIStreamProducer` objects
-            based on the config file and arguments to this method
+        :return: ret_kwargs, the dictionary of keyword arguments to create new
+            :class:`~OpenMSIStreamProducer` objects based on the config file and
+            arguments to this method
         :rtype: dict
         """
-        parser = KafkaConfigFileParser(config_file_path,logger=logger)
-        ret_kwargs = {'logger':logger}
-        #get the broker and producer configurations
-        all_configs = {**parser.broker_configs,**parser.producer_configs}
-        all_configs = add_kwargs_to_configs(all_configs,logger,**kwargs)
-        #all_configs['debug']='broker,topic,msg'
-        #use a SerializingProducer by default
-        if kafkacrypto is None and parser.kc_config_file_str is None :
-            ret_args = [SerializingProducer,all_configs]
+        parser = KafkaConfigFileParser(config_file_path, logger=logger)
+        ret_kwargs = {"logger": logger}
+        # get the broker and producer configurations
+        all_configs = {**parser.broker_configs, **parser.producer_configs}
+        all_configs = add_kwargs_to_configs(all_configs, logger, **kwargs)
+        # all_configs['debug']='broker,topic,msg'
+        # use a SerializingProducer by default
+        if kafkacrypto is None and parser.kc_config_file_str is None:
+            ret_args = [SerializingProducer, all_configs]
             return ret_args, ret_kwargs
-        #if "kafkacrypto" is given, or there are configs for KafkaCrypto, use a KafkaProducer
-        if kafkacrypto is not None :
-            if not isinstance(kafkacrypto,OpenMSIStreamKafkaCrypto) :
-                errmsg = f'ERROR: kafkacrypto argument type = {type(kafkacrypto)}'
-                raise_err_with_optional_logger(logger,errmsg,TypeError)
-            debugmsg = f'Produced messages will be encrypted using configs at {kafkacrypto.config_file_path}'
-            debug_msg_with_optional_logger(logger,debugmsg)
+        # if "kafkacrypto" is given, or there are configs for KafkaCrypto, use a KafkaProducer
+        if kafkacrypto is not None:
+            if not isinstance(kafkacrypto, OpenMSIStreamKafkaCrypto):
+                errmsg = f"ERROR: kafkacrypto argument type = {type(kafkacrypto)}"
+                raise_err_with_optional_logger(logger, errmsg, TypeError)
+            debugmsg = (
+                f"Produced messages will be encrypted using configs "
+                f"at {kafkacrypto.config_file_path}"
+            )
+            debug_msg_with_optional_logger(logger, debugmsg)
             k_c = kafkacrypto
-        else :
-            debugmsg = f'Produced messages will be encrypted using configs at {parser.kc_config_file_str}'
-            debug_msg_with_optional_logger(logger,debugmsg)
-            k_c = OpenMSIStreamKafkaCrypto(parser.broker_configs,parser.kc_config_file_str)
-        if 'key.serializer' in all_configs :
-            keyser = CompoundSerializer(all_configs.pop('key.serializer'),k_c.key_serializer)
-        else :
+        else:
+            debugmsg = (
+                f"Produced messages will be encrypted using configs "
+                f"at {parser.kc_config_file_str}"
+            )
+            debug_msg_with_optional_logger(logger, debugmsg)
+            k_c = OpenMSIStreamKafkaCrypto(
+                parser.broker_configs, parser.kc_config_file_str
+            )
+        if "key.serializer" in all_configs:
+            keyser = CompoundSerializer(
+                all_configs.pop("key.serializer"), k_c.key_serializer
+            )
+        else:
             keyser = k_c.key_serializer
-        if 'value.serializer' in all_configs :
-            valser = CompoundSerializer(all_configs.pop('value.serializer'),k_c.value_serializer)
-        else :
+        if "value.serializer" in all_configs:
+            valser = CompoundSerializer(
+                all_configs.pop("value.serializer"), k_c.value_serializer
+            )
+        else:
             valser = k_c.value_serializer
-        all_configs['key_serializer']=keyser
-        all_configs['value_serializer']=valser
-        ret_args = [KafkaProducer,all_configs]
-        ret_kwargs['kafkacrypto']=k_c
+        all_configs["key_serializer"] = keyser
+        all_configs["value_serializer"] = valser
+        ret_args = [KafkaProducer, all_configs]
+        ret_kwargs["kafkacrypto"] = k_c
         return ret_args, ret_kwargs
 
     @classmethod
-    def from_file(cls,*args,**kwargs) :
+    def from_file(cls, *args, **kwargs):
         """
-        Wrapper around :func:`~OpenMSIStreamProducer.get_producer_args_kwargs` and the :class:`~OpenMSIStreamProducer`
-        constructor to return a single :class:`~OpenMSIStreamProducer` from a given config file/arguments.
+        Wrapper around :func:`~OpenMSIStreamProducer.get_producer_args_kwargs` and the
+        :class:`~OpenMSIStreamProducer` constructor to return a single
+        :class:`~OpenMSIStreamProducer` from a given config file/arguments.
         Arguments are the same as :func:`~OpenMSIStreamProducer.get_producer_args_kwargs`
 
         :returns: An :class:`~OpenMSIStreamProducer` object based on the given config file/arguments
         :rtype: :class:`~OpenMSIStreamProducer`
         """
-        args_to_use, kwargs_to_use = OpenMSIStreamProducer.get_producer_args_kwargs(*args,**kwargs)
-        return cls(*args_to_use,**kwargs_to_use)
+        args_to_use, kwargs_to_use = OpenMSIStreamProducer.get_producer_args_kwargs(
+            *args, **kwargs
+        )
+        return cls(*args_to_use, **kwargs_to_use)
 
-    def produce_from_queue(self,queue,topic_name,**kwargs) :
+    def produce_from_queue(self, queue, topic_name, **kwargs):
         """
         Get a :class:`~.kafka_wrapper.Producible` object from a given Queue and produce it to
-        the given topic. Does nothing if the queue is empty, and does not block waiting for items from the queue.
+        the given topic. Does nothing if the queue is empty, and does not block
+        waiting for items from the queue.
 
         Meant to be run in multiple threads in parallel.
 
         :param queue: the :class:`queue.Queue` holding objects that should be produced
         :type queue: :class:`queue.Queue`
         :param topic_name: the name of the topic to produce to
         :type topic_name: str
         :param kwargs: other keyword arguments are passed to :func:`~produce_object`
         :type kwargs: dict
         """
-        if queue.empty() :
+        if queue.empty():
             return
-        #get the next object from the Queue
+        # get the next object from the Queue
         obj = queue.get_nowait()
-        if isinstance(obj,Producible) :
-            success = self.produce_object(obj,topic_name,**kwargs)
-            if not success :
-                warnmsg = f'WARNING: message with key {obj.msg_key} failed to buffer for longer than '
-                warnmsg+=  'the timeout with no new callbacks served. This message will be re-enqueued.'
+        if isinstance(obj, Producible):
+            success = self.produce_object(obj, topic_name, **kwargs)
+            if not success:
+                warnmsg = (
+                    f"WARNING: message with key {obj.msg_key} failed to buffer for longer "
+                    "than the timeout with no new callbacks served. "
+                    "This message will be re-enqueued."
+                )
                 self.logger.warning(warnmsg)
                 queue.put(obj)
-            self.__poll_counter+=1
-            if self.__poll_counter%self.POLL_EVERY==0 :
+            self.__poll_counter += 1
+            if self.__poll_counter % self.POLL_EVERY == 0:
                 _ = self.poll(0)
                 self.__poll_counter = 0
-        else :
-            warnmsg = f'WARNING: found an object of type {type(obj)} in a Producer queue that should only contain '
-            warnmsg+= 'Producible objects. This object will be skipped!'
+        else:
+            warnmsg = (
+                f"WARNING: found an object of type {type(obj)} in a Producer queue "
+                "that should only contain Producible objects. This object will be skipped!"
+            )
             self.logger.warning(warnmsg)
 
-    def produce_from_queue_looped(self,queue,topic_name,**kwargs) :
+    def produce_from_queue_looped(self, queue, topic_name, **kwargs):
         """
         Get :class:`~.kafka_wrapper.Producible` objects from a given Queue and produce
         them to the given topic. Blocks while waiting for items to appear in the queue.
         Runs until "None" is pulled from the queue.
 
         Meant to be run in multiple threads in parallel.
 
         :param queue: the :class:`queue.Queue` holding objects that should be produced
         :type queue: :class:`queue.Queue`
         :param topic_name: the name of the topic to produce to
         :type topic_name: str
         :param kwargs: other keyword arguments are passed to :func:`~produce_object`
         :type kwargs: dict
         """
-        #get the next object from the Queue
+        # get the next object from the Queue
         obj = queue.get()
-        #loop until "None" is pulled from the Queue
-        while obj is not None :
-            if isinstance(obj,Producible) :
-                success = self.produce_object(obj,topic_name,**kwargs)
-                if not success :
-                    warnmsg = f'WARNING: message with key {obj.msg_key} failed to buffer for longer than '
-                    warnmsg+=  'the timeout with no new callbacks served. This message will be re-enqueued.'
+        # loop until "None" is pulled from the Queue
+        while obj is not None:
+            if isinstance(obj, Producible):
+                success = self.produce_object(obj, topic_name, **kwargs)
+                if not success:
+                    warnmsg = (
+                        f"WARNING: message with key {obj.msg_key} failed to buffer for "
+                        "longer than the timeout with no new callbacks served. "
+                        "This message will be re-enqueued."
+                    )
                     self.logger.warning(warnmsg)
                     queue.put(obj)
-                self.__poll_counter+=1
-                if self.__poll_counter%self.POLL_EVERY==0 :
+                self.__poll_counter += 1
+                if self.__poll_counter % self.POLL_EVERY == 0:
                     _ = self.poll(0)
                     self.__poll_counter = 0
-            else :
-                warnmsg = f'WARNING: found an object of type {type(obj)} in a Producer queue that should only contain '
-                warnmsg+= 'Producible objects. This object will be skipped!'
+            else:
+                warnmsg = (
+                    f"WARNING: found an object of type {type(obj)} in a Producer queue "
+                    "that should only contain Producible objects. This object will be skipped!"
+                )
                 self.logger.warning(warnmsg)
-            #get the next object in the Queue
+            # get the next object in the Queue
             obj = queue.get()
         queue.task_done()
 
-    def produce_object(self,obj,topic_name,callback=None,print_every=1000,timeout=60,retry_sleep=5) :
+    def produce_object(
+        self, obj, topic_name, callback=None, print_every=1000, timeout=60, retry_sleep=5
+    ):
         """
         Produce a given :class:`~.kafka_wrapper.Producible` object to a given topic,
         with some handling for BufferErrors, calling poll() automatically, and using callbacks
         constructed on the fly.
 
         :param obj: the object to produce
         :type obj: :class:`~.kafka_wrapper.Producible`
         :param topic_name: the name of the topic to produce to
         :type topic_name: str
-        :param callback: a function that should be called for each message upon recognition by the broker.
-            Will be wrapped in a lambda for each call to produce().
-            Arguments to the callback function are determined by the particular type of :class:`Producible` object used
-        :type callback: producer callback function (takes at least "err" and "msg" arguments), optional
+        :param callback: a function that should be called for each message upon recognition
+            by the broker. Will be wrapped in a lambda for each call to produce().
+            Arguments to the callback function are determined by the particular type of
+            :class:`Producible` object used
+        :type callback: producer callback function (takes at least "err" and "msg" arguments),
+            optional
         :param print_every: print/log progress every (this many) messages
         :type print_every: int, optional
         :param timeout: max time (seconds) to wait for the message to be produced in the event of
             (repeated) BufferError(s)
         :type timeout: float, optional
-        :param retry_sleep: how long (seconds) to wait between produce attempts if one fails with a BufferError
+        :param retry_sleep: how long (seconds) to wait between produce attempts if one fails
+            with a BufferError
         :type retry_sleep: float, optional
 
         :return: True if the call to produce is successful, False otherwise.
         :rtype: bool
         """
-        #log a line about this message if applicable
+        # log a line about this message if applicable
         logmsg = obj.get_log_msg(print_every)
-        if logmsg is not None :
+        if logmsg is not None:
             self.logger.debug(logmsg)
-        #get the Producible's callback arguments and set the callback to use
-        if callback is None :
-            callback_to_use = make_callback(default_producer_callback,self.producer_id,logger=self.logger,
-                                            **obj.callback_kwargs)
-        else :
-            callback_to_use = make_callback(callback,self.producer_id,**obj.callback_kwargs)
-        #produce the message to the topic
-        success=False
-        total_wait_secs=0
-        while (not success) and total_wait_secs<timeout :
-            try :
-                self.produce(topic=topic_name,key=obj.msg_key,value=obj.msg_value,on_delivery=callback_to_use)
-                success=True
-            except BufferError :
+        # get the Producible's callback arguments and set the callback to use
+        if callback is None:
+            callback_to_use = make_callback(
+                default_producer_callback,
+                self.producer_id,
+                logger=self.logger,
+                **obj.callback_kwargs,
+            )
+        else:
+            callback_to_use = make_callback(
+                callback, self.producer_id, **obj.callback_kwargs
+            )
+        # produce the message to the topic
+        success = False
+        total_wait_secs = 0
+        while (not success) and total_wait_secs < timeout:
+            try:
+                self.produce(
+                    topic=topic_name,
+                    key=obj.msg_key,
+                    value=obj.msg_value,
+                    on_delivery=callback_to_use,
+                )
+                success = True
+            except BufferError:
                 n_new_callbacks = self.poll(0)
                 time.sleep(retry_sleep)
-                if n_new_callbacks is None or n_new_callbacks==0 :
-                    total_wait_secs+=retry_sleep
-                else :
+                if n_new_callbacks is None or n_new_callbacks == 0:
+                    total_wait_secs += retry_sleep
+                else:
                     total_wait_secs = 0
-            except Exception as exc :
-                errmsg = 'ERROR: failed during call to Producer.produce! Will log and re-raise Exception.'
-                self.logger.error(errmsg,exc_info=exc,reraise=True)
-        self.__poll_counter+=1
-        if self.__poll_counter%self.POLL_EVERY==0 :
+            except Exception as exc:
+                errmsg = (
+                    "ERROR: failed during call to Producer.produce! "
+                    "Will log and re-raise Exception."
+                )
+                self.logger.error(errmsg, exc_info=exc, reraise=True)
+        self.__poll_counter += 1
+        if self.__poll_counter % self.POLL_EVERY == 0:
             n_new_callbacks = self.poll(0)
             self.__poll_counter = 0
         return success
 
-    def produce(self,topic,key,value,**kwargs) :
+    def produce(self, topic, key, value, **kwargs):
         """
         Produce a message to a topic.
         Other kwargs are passed through to the underlying producer's produce() function.
 
         :param topic: the name of the topic to produce to
         :type topic: str
         :param key: the key of the message
         :type key: depends on serialization settings
         :param value: the value of the message
         :type value: depends on the serialization settings
         """
-        if isinstance(self._producer,KafkaProducer) :
-            key = self._producer.ks(topic,key)
-            value = self._producer.vs(topic,value)
-        return self._producer.produce(topic=topic,key=key,value=value,**kwargs)
+        if isinstance(self._producer, KafkaProducer):
+            key = self._producer.ks(topic, key)
+            value = self._producer.vs(topic, value)
+        return self._producer.produce(topic=topic, key=key, value=value, **kwargs)
 
-    def poll(self,*args,**kwargs) :
+    def poll(self, *args, **kwargs):
         """
         Wrapper around Producer.poll()
         """
-        return self._producer.poll(*args,**kwargs)
+        return self._producer.poll(*args, **kwargs)
 
-    def flush(self,*args,**kwargs) :
+    def flush(self, *args, **kwargs):
         """
         Wrapper around Producer.flush()
         """
-        return self._producer.flush(*args,**kwargs)
+        return self._producer.flush(*args, **kwargs)
 
-    def close(self) :
+    def close(self):
         """
         Wrapper around :func:`kafkacrypto.KafkaCrypto.close`.
         It's important to call this on shutdown if the Producer is producing encrypted messages.
         """
-        try :
-            if self.__kafkacrypto :
+        try:
+            if self.__kafkacrypto:
                 self.__kafkacrypto.close()
-        except Exception :
+        except Exception:
             pass
-        finally :
+        finally:
             self.__kafkacrypto = None
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/producer_group.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/producer_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 """A set of Producers sharing an optional KafkaCrypto instance for key passing"""
 
-#imports
+# imports
 from ..utilities import LogOwner
 from .openmsistream_producer import OpenMSIStreamProducer
 
-class ProducerGroup(LogOwner) :
+
+class ProducerGroup(LogOwner):
     """
-    Class for working with a group of producers sharing a single :class:`kafkacrypto.KafkaCrypto` instance
+    Class for working with a group of producers sharing a single
+    :class:`kafkacrypto.KafkaCrypto` instance
 
     :param config_path: Path to the config file that should be used to define Producers in the group
     :type config_path: :class:`pathlib.Path`
-    :param kafkacrypto: The :class:`~OpenMSIStreamKafkaCrypto` object that should be used to instantiate Producers.
-        Only needed if a single specific :class:`~OpenMSIStreamKafkaCrypto` instance should be shared.
+    :param kafkacrypto: The :class:`~OpenMSIStreamKafkaCrypto` object that should be used
+        to instantiate Producers. Only needed if a single specific
+        :class:`~OpenMSIStreamKafkaCrypto` instance should be shared.
     :type kafkacrypto: :class:`~OpenMSIStreamKafkaCrypto`, optional
     """
 
     @property
-    def kafkacrypto(self) :
+    def kafkacrypto(self):
         """
         The KafkaCrypto object handling key passing and serialization for encrypted messages
         """
-        return self.__p_kwargs['kafkacrypto'] if 'kafkacrypto' in self.__p_kwargs else None
+        return (
+            self.__p_kwargs["kafkacrypto"] if "kafkacrypto" in self.__p_kwargs else None
+        )
 
-    def __init__(self,config_path,kafkacrypto=None,**kwargs) :
+    def __init__(self, config_path, kafkacrypto=None, **kwargs):
         """
         Constructor method
         """
         super().__init__(**kwargs)
-        self.__p_args, self.__p_kwargs = OpenMSIStreamProducer.get_producer_args_kwargs(config_path,
-                                                                                        logger=self.logger,
-                                                                                        kafkacrypto=kafkacrypto)
+        self.__p_args, self.__p_kwargs = OpenMSIStreamProducer.get_producer_args_kwargs(
+            config_path, logger=self.logger, kafkacrypto=kafkacrypto
+        )
 
-    def get_new_producer(self) :
+    def get_new_producer(self):
         """
         Return a new :class:`~OpenMSIStreamProducer` object.
         Call this function from a child thread to get thread-independent Producers.
-        Note: this function just creates the Producer; closing it etc. must be handled by whatever calls this function.
+        Note: this function just creates the Producer; closing it etc. must be handled
+        by whatever calls this function.
 
         :return: a Producer created using the config set in the constructor
         :rtype: :class:`~OpenMSIStreamProducer`
         """
-        producer = OpenMSIStreamProducer(*self.__p_args,**self.__p_kwargs)
+        producer = OpenMSIStreamProducer(*self.__p_args, **self.__p_kwargs)
         return producer
 
-    def close(self) :
+    def close(self):
         """
         Wrapper around :func:`kafkacrypto.KafkaCrypto.close`.
         """
-        try :
-            self.__p_kwargs['kafkacrypto'].close()
-        except Exception :
+        try:
+            self.__p_kwargs["kafkacrypto"].close()
+        except Exception:
             pass
-        finally :
-            self.__p_kwargs['kafkacrypto'] = None
+        finally:
+            self.__p_kwargs["kafkacrypto"] = None
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/producible.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/producible.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """Small utility class to simplify producing messages with standardized callbacks"""
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 
-class Producible(ABC) :
+
+class Producible(ABC):
     """
     Small utility class for anything that can be Produced as a message to a topic
     """
 
     @property
     @abstractmethod
-    def msg_key(self) :
+    def msg_key(self):
         """
         The key of the object when it's represented as a message.
         This can be something that needs to be serialized still
 
         Not implemented in base class
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def msg_value(self) :
+    def msg_value(self):
         """
         The value of the object when it's represented as a message.
         This can be something that needs to be serialized still
 
         Not implemented in base class
         """
         raise NotImplementedError
 
     @property
-    def callback_kwargs(self) :
+    def callback_kwargs(self):
         """
         A dictionary of keyword arguments that should be sent to the callback function
         for Producers producing messages of this Producible
 
         Empty for the base class
         """
         return {}
 
     @abstractmethod
-    def get_log_msg(self,print_every=None) :
+    def get_log_msg(self, print_every=None):
         """
-        Given some (optional) "print_every" variable, return the string that should be logged (at debug level)
-        for this message. If "None" is returned (the default) nothing will be logged.
+        Given some (optional) "print_every" variable, return the string that should be
+        logged (at debug level) for this message.
+        If "None" is returned (the default) nothing will be logged.
         """
         return None
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/serialization.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,243 @@
 """Classes for serialization and deserialization operations"""
 
-#imports
+# imports
 import pathlib, inspect, time, warnings
 from hashlib import sha512
 import msgpack
 from confluent_kafka.error import SerializationError
 from confluent_kafka.serialization import Serializer, Deserializer
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto.message import KafkaCryptoMessage, KafkaCryptoMessageError
 from ..data_file_io.entity.data_file_chunk import DataFileChunk
 
 ####################### COMPOUND (DE)SERIALIZERS FOR STACKING MULTIPLE STEPS #######################
 
+
 class CompoundSerDes(Serializer, Deserializer):
     """
     A Serializer/Deserializer that stacks multiple Serialization/Deserialization steps
     """
 
     def __init__(self, *args):
         """
-        args = a list of (De)Serializer (or otherwise callable) objects to apply IN GIVEN ORDER to some data
+        args = a list of (De)Serializer (or otherwise callable) objects to apply
+        IN GIVEN ORDER to some data
         """
         self.__steps = list(args)
 
-    def __call__(self,data,ctx=None) :
-        if data is None :
+    def __call__(self, data, ctx=None):
+        if data is None:
             return None
-        for istep,serdes in enumerate(self.__steps,start=1) :
-            try :
+        for istep, serdes in enumerate(self.__steps, start=1):
+            try:
                 data = serdes(data)
-            except Exception as exc :
-                errmsg = f'ERROR: failed to (de)serialize at step {istep} (of {len(self.__steps)}) in CompoundSerDes! '
-                errmsg+= f'Callable = {serdes}, exception = {exc}'
+            except Exception as exc:
+                errmsg = (
+                    f"ERROR: failed to (de)serialize at step {istep} (of {len(self.__steps)}) "
+                    f"in CompoundSerDes! Callable = {serdes}, exception = {exc}"
+                )
                 raise SerializationError(errmsg)
         return data
 
+
 class CompoundSerializer(Serializer):
     """
     A Serializer that stacks multiple steps
     For use with KafkaCrypto since topic names must be passed
     """
 
     def __init__(self, *args):
         self.__steps = list(args)
 
-    def serialize(self,topic,data) :
+    def serialize(self, topic, data):
         """
         Call a chain of Serializers for a given message (may contain encryption)
         """
-        for istep,ser in enumerate(self.__steps,start=1) :
-            try :
-                if hasattr(ser,'serialize') and inspect.isroutine(ser.serialize) :
-                    data = ser.serialize(topic,data)
-                else :
-                    data = ser(data,ctx=None)
-            except Exception as exc :
-                errmsg = f'ERROR: failed to serialize at step {istep} (of {len(self.__steps)}) in '
-                errmsg+= f'{self.__class__.__name__}! Callable = {ser}, exception = {exc}'
+        for istep, ser in enumerate(self.__steps, start=1):
+            try:
+                if hasattr(ser, "serialize") and inspect.isroutine(ser.serialize):
+                    data = ser.serialize(topic, data)
+                else:
+                    data = ser(data, ctx=None)
+            except Exception as exc:
+                errmsg = (
+                    f"ERROR: failed to serialize at step {istep} (of {len(self.__steps)}) "
+                    f"in {self.__class__.__name__}! Callable = {ser}, exception = {exc}"
+                )
                 raise SerializationError(errmsg)
         return data
 
-    def __call__(self,data,ctx=None) :
-        if data is None :
+    def __call__(self, data, ctx=None):
+        if data is None:
             return None
-        raise SerializationError(f'ERROR: __call__ method not implemented for a {self.__class__.__name__}')
+        raise SerializationError(
+            f"ERROR: __call__ method not implemented for a {self.__class__.__name__}"
+        )
+
 
 class CompoundDeserializer(Deserializer):
     """
     A Deserializer that stacks multiple steps
     For use with KafkaCrypto since topic names must be passed
     """
 
-    MAX_WAIT_PER_DECRYPT = 60.0 #in seconds
+    MAX_WAIT_PER_DECRYPT = 60.0  # in seconds
 
     def __init__(self, *args):
         self.__steps = list(args)
 
-    def deserialize(self,topic,data) :
+    def deserialize(self, topic, data):
         """
         Call a chain of Deserializers for a given message (may contain decryption)
         """
-        for istep,des in enumerate(self.__steps,start=1) :
-            try :
-                data = self.__deserialize_message(des,topic,data)
-            except Exception as exc :
-                errmsg = f'ERROR: failed to deserialize at step {istep} (of {len(self.__steps)})'
-                errmsg+= f' in {self.__class__.__name__}! Callable = {des}, exception = {exc}'
+        for istep, des in enumerate(self.__steps, start=1):
+            try:
+                data = self.__deserialize_message(des, topic, data)
+            except Exception as exc:
+                errmsg = (
+                    f"ERROR: failed to deserialize at step {istep} (of {len(self.__steps)}) "
+                    f"in {self.__class__.__name__}! Callable = {des}, exception = {exc}"
+                )
                 raise SerializationError(errmsg)
         return data
 
-    def __call__(self,data,ctx=None) :
-        if data is None :
+    def __call__(self, data, ctx=None):
+        if data is None:
             return None
-        raise SerializationError(f'ERROR: __call__ method not implemented for a {self.__class__.__name__}')
+        raise SerializationError(
+            f"ERROR: __call__ method not implemented for a {self.__class__.__name__}"
+        )
 
-    def __deserialize_message(self,des,topic,data) :
+    def __deserialize_message(self, des, topic, data):
         """
         Deserialize a (possibly encrypted) message
         """
-        #deserialize a KafkaCrypto message
-        if hasattr(des,'deserialize') and inspect.isroutine(des.deserialize) :
-            data = des.deserialize(topic,data)
-            if isinstance(data,KafkaCryptoMessage) :
+        # deserialize a KafkaCrypto message
+        if hasattr(des, "deserialize") and inspect.isroutine(des.deserialize):
+            data = des.deserialize(topic, data)
+            if isinstance(data, KafkaCryptoMessage):
                 success = False
                 elapsed = 0
-                while (not success) and elapsed<self.MAX_WAIT_PER_DECRYPT :
-                    try :
+                while (not success) and elapsed < self.MAX_WAIT_PER_DECRYPT:
+                    try:
                         data = data.getMessage()
                         success = True
-                    except KafkaCryptoMessageError :
+                    except KafkaCryptoMessageError:
                         time.sleep(0.1)
-                        elapsed+=0.1
-                #if the message could not be decrypted, return the Message object itself
-                if not success :
+                        elapsed += 0.1
+                # if the message could not be decrypted, return the Message object itself
+                if not success:
                     return data
-        #if a previous step failed to deserialize a KafkaCrypto message, don't bother trying this next step
-        elif not isinstance(data,KafkaCryptoMessage) :
-            data = des(data,ctx=None)
+        # if a previous step failed to deserialize a KafkaCrypto message,
+        # don't bother trying this next step
+        elif not isinstance(data, KafkaCryptoMessage):
+            data = des(data, ctx=None)
         return data
 
 
 ####################### SERIALIZING/DESERIALIZING FILE CHUNKS #######################
 
-class DataFileChunkSerializer(Serializer) :
+
+class DataFileChunkSerializer(Serializer):
     """
     Serializes DataFileChunk objects to bytesarrays
     """
 
-    def __call__(self,file_chunk_obj,ctx=None) :
-        if file_chunk_obj is None :
+    def __call__(self, file_chunk_obj, ctx=None):
+        if file_chunk_obj is None:
             return None
-        if not isinstance(file_chunk_obj,DataFileChunk) :
-            raise SerializationError('ERROR: object passed to FileChunkSerializer is not a DataFileChunk!')
-        #pack up all the relevant bits of information into a single bytearray
-        try :
-            #get the chunk's data from the file if necessary
-            if file_chunk_obj.data is None :
+        if not isinstance(file_chunk_obj, DataFileChunk):
+            raise SerializationError(
+                "ERROR: object passed to FileChunkSerializer is not a DataFileChunk!"
+            )
+        # pack up all the relevant bits of information into a single bytearray
+        try:
+            # get the chunk's data from the file if necessary
+            if file_chunk_obj.data is None:
                 file_chunk_obj.populate_with_file_data()
-            #pack up all of the properties of the message
+            # pack up all of the properties of the message
             ordered_properties = []
             ordered_properties.append(str(file_chunk_obj.filename))
             ordered_properties.append(file_chunk_obj.file_hash)
             ordered_properties.append(file_chunk_obj.chunk_hash)
             ordered_properties.append(file_chunk_obj.chunk_offset_write)
             ordered_properties.append(file_chunk_obj.chunk_i)
             ordered_properties.append(file_chunk_obj.n_total_chunks)
             ordered_properties.append(file_chunk_obj.subdir_str)
             ordered_properties.append(file_chunk_obj.filename_append)
             ordered_properties.append(file_chunk_obj.data)
-            return msgpack.packb(ordered_properties,use_bin_type=True)
-        except Exception as exc :
-            raise SerializationError(f'ERROR: failed to serialize a DataFileChunk! Exception: {exc}')
+            return msgpack.packb(ordered_properties, use_bin_type=True)
+        except Exception as exc:
+            raise SerializationError(
+                f"ERROR: failed to serialize a DataFileChunk! Exception: {exc}"
+            )
+
 
-class DataFileChunkDeserializer(Deserializer) :
+class DataFileChunkDeserializer(Deserializer):
     """
     Deseralizes bytearrays to DataFileChunk objects
     """
 
-    def __call__(self,byte_array,ctx=None) :
-        if byte_array is None :
+    def __call__(self, byte_array, ctx=None):
+        if byte_array is None:
             return None
-        try :
-            #unpack the byte array
-            ordered_properties = msgpack.unpackb(byte_array,raw=True)
-            if len(ordered_properties)!=9 :
-                errmsg = 'ERROR: unrecognized token passed to DataFileChunkDeserializer. Expected 9 properties'
-                errmsg+= f' but found {len(ordered_properties)}'
+        try:
+            # unpack the byte array
+            ordered_properties = msgpack.unpackb(byte_array, raw=True)
+            if len(ordered_properties) != 9:
+                errmsg = (
+                    f"ERROR: unrecognized token passed to DataFileChunkDeserializer. "
+                    f"Expected 9 properties but found {len(ordered_properties)}"
+                )
                 raise ValueError(errmsg)
-            try :
+            try:
                 filename = str(ordered_properties[0].decode())
                 file_hash = ordered_properties[1]
                 chunk_hash = ordered_properties[2]
                 chunk_offset_read = None
                 chunk_offset_write = int(ordered_properties[3])
                 chunk_i = int(ordered_properties[4])
                 n_total_chunks = int(ordered_properties[5])
                 subdir_str = str(ordered_properties[6].decode())
                 filename_append = str(ordered_properties[7].decode())
                 data = ordered_properties[8]
-            except Exception as exc :
-                errmsg = f'ERROR: unrecognized value(s) when deserializing a DataFileChunk from token. Exception: {exc}'
+            except Exception as exc:
+                errmsg = (
+                    f"ERROR: unrecognized value(s) when deserializing a DataFileChunk "
+                    f"from token. Exception: {exc}"
+                )
                 raise ValueError(errmsg)
-            #make sure the hash of the chunk's data matches with what it was before
+            # make sure the hash of the chunk's data matches with what it was before
             check_chunk_hash = sha512()
             check_chunk_hash.update(data)
             check_chunk_hash = check_chunk_hash.digest()
-            if check_chunk_hash!=chunk_hash :
-                errmsg = f'ERROR: chunk hash {check_chunk_hash} != expected hash {chunk_hash} in file {filename}, '
-                errmsg+= f'offset {chunk_offset_write}'
+            if check_chunk_hash != chunk_hash:
+                errmsg = (
+                    f"ERROR: chunk hash {check_chunk_hash} != expected hash {chunk_hash} "
+                    f"in file {filename}, offset {chunk_offset_write}"
+                )
                 raise RuntimeError(errmsg)
-            #set the filepath based on the subdirectory string
-            if subdir_str=='' :
+            # set the filepath based on the subdirectory string
+            if subdir_str == "":
                 filepath = pathlib.Path(filename)
             subdir_path = pathlib.PurePosixPath(subdir_str)
-            filepath = pathlib.Path('').joinpath(*(subdir_path.parts),filename)
-            return DataFileChunk(filepath,filename,file_hash,chunk_hash,chunk_offset_read,chunk_offset_write,
-                                 len(data),chunk_i,n_total_chunks,data=data,filename_append=filename_append)
-        except Exception as exc :
-            raise SerializationError(f'ERROR: failed to deserialize a DataFileChunk! Exception: {exc}')
+            filepath = pathlib.Path("").joinpath(*(subdir_path.parts), filename)
+            return DataFileChunk(
+                filepath,
+                filename,
+                file_hash,
+                chunk_hash,
+                chunk_offset_read,
+                chunk_offset_write,
+                len(data),
+                chunk_i,
+                n_total_chunks,
+                data=data,
+                filename_append=filename_append,
+            )
+        except Exception as exc:
+            raise SerializationError(
+                f"ERROR: failed to deserialize a DataFileChunk! Exception: {exc}"
+            )
```

### Comparing `openmsistream-1.3.4/openmsistream/kafka_wrapper/utilities.py` & `openmsistream-1.4.0/openmsistream/kafka_wrapper/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,83 @@
 """Miscellaneous functions/classes used elsewhere in the Kafka wrapper"""
 
-#imports
+# imports
 import warnings
 from collections import namedtuple
 from confluent_kafka import OFFSET_BEGINNING
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto import KafkaConsumer
 
-def add_kwargs_to_configs(configs,logger,**kwargs) :
+
+def add_kwargs_to_configs(configs, logger, **kwargs):
     """
     Add any kwargs with underscores replaced with dots to a given config dictionary
     """
     new_configs = configs.copy()
-    for argname,arg in kwargs.items() :
-        config_name = argname.replace('_','.')
-        if config_name in new_configs and new_configs[config_name]!=arg :
-            if logger is not None :
-                msg = f'A new value for the "{config_name}" config has been supplied '
-                msg+=  'by a keyword argument that will overwrite a previously-set value. '
-                msg+= f'The value will be set to {arg} instead of {new_configs[config_name]}.'
+    for argname, arg in kwargs.items():
+        config_name = argname.replace("_", ".")
+        if config_name in new_configs and new_configs[config_name] != arg:
+            if logger is not None:
+                msg = (
+                    f'A new value for the "{config_name}" config has been supplied by '
+                    f"a keyword argument that will overwrite a previously-set value. "
+                    f"The value will be set to {arg} instead of {new_configs[config_name]}."
+                )
                 logger.debug(msg)
-        new_configs[config_name]=arg
+        new_configs[config_name] = arg
     return new_configs
 
-def default_producer_callback(err,msg,prodid,logger=None,**other_kwargs) :
+
+def default_producer_callback(err, msg, prodid, logger=None, **other_kwargs):
     """
-    Default callback function to use for testing whether a message has been successfully produced to the topic
+    Default callback function to use for testing whether a message has been
+    successfully produced to the topic
     """
-    if err is None and msg.error() is not None :
+    if err is None and msg.error() is not None:
         err = msg.error()
-    if err is not None: #raise an error if the message wasn't sent successfully
-        if err.fatal() :
-            logmsg =f'ERROR: Producer with ID {prodid} fatally failed to deliver message with kwargs '
-            logmsg+=f'"{other_kwargs}". MESSAGE DROPPED. Error reason: {err.str()}'
-            if logger is not None :
+    if err is not None:  # raise an error if the message wasn't sent successfully
+        if err.fatal():
+            logmsg = (
+                f"ERROR: Producer with ID {prodid} fatally failed to deliver message "
+                f'with kwargs "{other_kwargs}". MESSAGE DROPPED. Error reason: {err.str()}'
+            )
+            if logger is not None:
                 logger.error(logmsg)
-            else :
+            else:
                 raise RuntimeError(logmsg)
-        elif not err.retriable() :
-            logmsg =f'ERROR: Producer with ID {prodid} failed to deliver message with kwargs "{other_kwargs}" '
-            logmsg+= f'and cannot retry. MESSAGE DROPPED. Error reason: {err.str()}'
-            if logger is not None :
+        elif not err.retriable():
+            logmsg = (
+                f"ERROR: Producer with ID {prodid} failed to deliver message with kwargs "
+                f'"{other_kwargs}" and cannot retry. MESSAGE DROPPED. '
+                f"Error reason: {err.str()}"
+            )
+            if logger is not None:
                 logger.error(logmsg)
-            else :
+            else:
                 raise RuntimeError(logmsg)
 
-def make_callback(func,*args,**kwargs) :
+
+def make_callback(func, *args, **kwargs):
     """
     Callbacks are rendered at runtime and so regular functions used as producer callbacks
     need to be wrapped in this lambda
     """
-    return lambda err,msg : func(err,msg,*args,**kwargs)
+    return lambda err, msg: func(err, msg, *args, **kwargs)
+
+
+KCCommitOffsetDictKey = namedtuple("KCCommitOffsetDictKey", ["topic", "partition"])
+KCCommitOffset = namedtuple("KCCommitOffset", ["offset"])
 
-KCCommitOffsetDictKey = namedtuple('KCCommitOffsetDictKey',['topic','partition'])
-KCCommitOffset = namedtuple('KCCommitOffset',['offset'])
 
 def reset_to_beginning_on_assign(consumer, partitions):
     """
     Used as the "on_assign" parameter to a Consumer constructor to get each partition
     to start at its earliest message when it's assigned to a Consumer
     """
     for part in partitions:
-        part.offset=OFFSET_BEGINNING
-    if isinstance(consumer,KafkaConsumer) :
+        part.offset = OFFSET_BEGINNING
+    if isinstance(consumer, KafkaConsumer):
         consumer.assign_and_seek(partitions)
-    else :
+    else:
         consumer.assign(partitions)
```

### Comparing `openmsistream-1.3.4/openmsistream/metadata_extraction/metadata_json_message.py` & `openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """The base message type that must be produced by a MetadataJSONReproducer"""
 
-#imports
+# imports
 import json
 from ..data_file_io.entity.reproducer_message import ReproducerMessage
 
-class MetadataJSONMessage(ReproducerMessage) :
+
+class MetadataJSONMessage(ReproducerMessage):
     """
     A class to represent the json metadata from a file as a Producible
     """
 
     @property
-    def msg_value(self) :
-        if self.json_content is None :
-            raise ValueError(f'ERROR: JSON content should not be None for a {self.__class__.__name__}!')
+    def msg_value(self):
+        if self.json_content is None:
+            raise ValueError(
+                f"ERROR: JSON content should not be None for a {self.__class__.__name__}!"
+            )
         return json.dumps(self.json_content)
 
-    def __init__(self,*args,json_content=None,**kwargs) :
-        super().__init__(*args,**kwargs)
-        self.json_content=json_content
+    def __init__(self, *args, json_content=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.json_content = json_content
```

### Comparing `openmsistream-1.3.4/openmsistream/metadata_extraction/metadata_json_reproducer.py` & `openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_reproducer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,152 @@
 """
 Base class for extracting metadata dictionaries from files in topics
 and producing those dictionaries as JSON-formatted strings to another topic
 """
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 from ..data_file_io.actor.data_file_stream_reproducer import DataFileStreamReproducer
 from .metadata_json_message import MetadataJSONMessage
 
-class MetadataJSONReproducer(DataFileStreamReproducer,ABC) :
+
+class MetadataJSONReproducer(DataFileStreamReproducer, ABC):
     """
     A class to extend for processing a stream of DataFileChunks, extracting metadata from
     fully-reconstructed files, and producing those metadata fields as JSON to a different topic.
 
     This is a base class that cannot be instantiated on its own.
 
-    :param config_path: Path to the config file to use in defining the Broker connection, Consumers, and Producers
+    :param config_path: Path to the config file to use in defining the Broker connection,
+        Consumers, and Producers
     :type config_path: :class:`pathlib.Path`
     :param consumer_topic_name: Name of the topic to which the Consumer(s) should be subscribed
     :type consumer_topic_name: str
-    :param producer_topic_name: Name of the topic to which the Producer(s) should produce the processing results
+    :param producer_topic_name: Name of the topic to which the Producer(s) should produce
+        the processing results
     :type producer_topic_name: str
-    :param output_dir: Path to the directory where the log and csv registry files should be kept (if None a default
-        will be created in the current directory)
+    :param output_dir: Path to the directory where the log and csv registry files should be kept
+        (if None a default will be created in the current directory)
     :type output_dir: :class:`pathlib.Path`, optional
     :param datafile_type: the type of data file that recognized files should be reconstructed as
         (must be a subclass of :class:`~.data_file_io.DownloadDataFileToMemory`)
     :type datafile_type: :class:`~.data_file_io.DownloadDataFileToMemory`, optional
-    :param n_producer_threads: the number of producers to run. The total number of producer/consumer threads
-        started is `max(n_consumer_threads,n_producer_threads)`.
+    :param n_producer_threads: the number of producers to run. The total number of
+        producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_producer_threads: int, optional
-    :param n_consumer_threads: the number of consumers to run. The total number of producer/consumer threads
-        started is `max(n_consumer_threads,n_producer_threads)`.
+    :param n_consumer_threads: the number of consumers to run. The total number of
+        producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_consumer_threads: int, optional
     :param consumer_group_id: the group ID under which each consumer should be created
     :type consumer_group_id: str, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
         :class:`~.data_file_io.DownloadDataFileToMemory`
     """
 
-    def __init__(self,config_file,consumer_topic_name,producer_topic_name,**kwargs) :
+    def __init__(self, config_file, consumer_topic_name, producer_topic_name, **kwargs):
         """
         Constructor method signature duplicated above to display in Sphinx docs
         """
-        super().__init__(config_file,consumer_topic_name,producer_topic_name,**kwargs)
+        super().__init__(config_file, consumer_topic_name, producer_topic_name, **kwargs)
 
-    def _get_processing_result_message_for_file(self,datafile,lock) :
-        try :
+    def _get_processing_result_message_for_file(self, datafile, lock):
+        try:
             json_content = self._get_metadata_dict_for_file(datafile)
-        except Exception as exc :
-            errmsg = f'ERROR: failed to extract JSON metadata from {datafile.full_filepath}! '
-            errmsg+= 'Error will be logged below, but not reraised.'
-            self.logger.error(errmsg,exc_info=exc)
+        except Exception as exc:
+            errmsg = (
+                f"ERROR: failed to extract JSON metadata from {datafile.full_filepath}! "
+                "Error will be logged below, but not reraised."
+            )
+            self.logger.error(errmsg, exc_info=exc)
             return None
-        if not isinstance(json_content,dict) :
-            errmsg = f'ERROR: JSON content found for {datafile.full_filepath} is of type {type(json_content)}, '
-            errmsg+= 'not a dictionary! This file will be skipped.'
+        if not isinstance(json_content, dict):
+            errmsg = (
+                f"ERROR: JSON content found for {datafile.full_filepath} is of type "
+                f"{type(json_content)}, not a dictionary! This file will be skipped."
+            )
             self.logger.error(errmsg)
             return None
-        return MetadataJSONMessage(datafile,json_content=json_content)
+        return MetadataJSONMessage(datafile, json_content=json_content)
 
     @abstractmethod
-    def _get_metadata_dict_for_file(self,datafile) :
+    def _get_metadata_dict_for_file(self, datafile):
         """
-        Given a :class:`~.data_file_io.DownloadDataFileToMemory`, extract and return its metadata as a
-        dictionary. The returned dictionary will be serialized to JSON and produced to the destination topic.
+        Given a :class:`~.data_file_io.DownloadDataFileToMemory`, extract and return
+        its metadata as a dictionary. The returned dictionary will be serialized to
+        JSON and produced to the destination topic.
 
-        This function can raise errors to be logged if metadata extraction doesn't proceed as expected.
+        This function can raise errors to be logged if metadata extraction doesn't proceed
+        as expected.
 
         Not implemented in base class
 
-        :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object that has received
-            all of its messages from the topic
+        :param datafile: A :class:`~.data_file_io.DownloadDataFileToMemory` object
+            that has received all of its messages from the topic
         :type datafile: :class:`~.data_file_io.DownloadDataFileToMemory`
 
         :return: metadata keys/values
         :rtype: dict
         """
         raise NotImplementedError
 
-    def _on_shutdown(self) :
-        self.logger.info('Will quit after all currently enqueued messages are received.')
+    def _on_shutdown(self):
+        self.logger.info("Will quit after all currently enqueued messages are received.")
         self.logger.debug(self.progress_msg)
         super()._on_shutdown()
 
     @classmethod
-    def run_from_command_line(cls,args=None) :
+    def run_from_command_line(cls, args=None):
         """
         Run :func:`~produce_processing_results_for_files_as_read` to continually
         extract metadata from consumed files and produce them as json contents to another topic
         """
         # make the argument parser
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
-        metadata_reproducer = cls(args.config,args.consumer_topic_name,args.producer_topic_name,
-                                  consumer_group_id=args.consumer_group_id,
-                                  n_consumer_threads=args.n_consumer_threads,
-                                  n_producer_threads=args.n_producer_threads,
-                                  output_dir=args.output_dir,
-                                  update_secs=args.update_seconds,
-                                  streamlevel=args.logger_stream_level,filelevel=args.logger_file_level,
-                                  )
+        metadata_reproducer = cls(
+            args.config,
+            args.consumer_topic_name,
+            args.producer_topic_name,
+            consumer_group_id=args.consumer_group_id,
+            n_consumer_threads=args.n_consumer_threads,
+            n_producer_threads=args.n_producer_threads,
+            output_dir=args.output_dir,
+            update_secs=args.update_seconds,
+            streamlevel=args.logger_stream_level,
+            filelevel=args.logger_file_level,
+        )
         # cls.bucket_name = args.bucket_name
-        msg = f'Listening to the {args.consumer_topic_name} topic for XRD CSV files to send their metadata to the '
-        msg+= f'{args.producer_topic_name} topic....'
+        msg = (
+            f"Listening to the {args.consumer_topic_name} topic for XRD CSV files to "
+            f"send their metadata to the {args.producer_topic_name} topic...."
+        )
         metadata_reproducer.logger.info(msg)
-        n_r,n_p,f_r_fns,m_p_fns = metadata_reproducer.produce_processing_results_for_files_as_read()
+        (
+            n_m_r,
+            n_m_p,
+            n_f_r,
+            n_f_mp,
+            m_p_fns,
+        ) = metadata_reproducer.produce_processing_results_for_files_as_read()
         metadata_reproducer.close()
-        msg = ''
-        if n_r>0 :
-            msg+= f'{n_r} total message{"s were" if n_r!=1 else " was"} consumed, '
-        if n_p>0 :
-            msg+=f'{n_p} message{"s were" if n_p!=1 else " was"} successfully processed, '
-        if len(f_r_fns)>0 :
-            msg+=f'{len(f_r_fns)} file{"s were" if len(f_r_fns)!=1 else " was"} fully read, '
-        if len(m_p_fns)>0 :
-            msg+=f'{len(m_p_fns)} file{"s were" if len(m_p_fns)!=1 else " was"} files had json metadata produced'
-            msg+=f' to the "{args.producer_topic_name}" topic, '
+        msg = ""
+        if n_m_r > 0:
+            msg += f'{n_m_r} total message{"s were" if n_m_r!=1 else " was"} consumed, '
+        if n_m_p > 0:
+            msg += f'{n_m_p} message{"s were" if n_m_p!=1 else " was"} successfully processed, '
+        if n_f_r > 0:
+            msg += f'{n_f_r} file{"s were" if n_f_r!=1 else " was"} fully read, '
+        if n_f_mp > 0:
+            msg += (
+                f'{n_f_mp} file{"s" if n_f_mp!=1 else ""} had json metadata produced '
+                f'to the "{args.producer_topic_name}" topic, '
+            )
         metadata_reproducer.logger.info(msg[:-2])
-        if len(m_p_fns)>0 :
-            msg=f'the following {len(m_p_fns)} file'
-            msg+=' had' if len(m_p_fns)==1 else 's had'
-            msg+=f' json metadata produced to the {args.producer_topic_name} topic:'
-            for fn in m_p_fns :
-                msg+=f'\n\t{fn}'
+        if n_f_mp > 0:
+            msg = (
+                f'{n_f_mp} file{"" if n_f_mp==1 else "s"} had json metadata produced '
+                f"to the {args.producer_topic_name} topic. "
+                f"Up to {cls.N_RECENT_FILES} most recent:\n\t"
+            )
+            msg += "\n\t".join(m_p_fns)
             metadata_reproducer.logger.debug(msg)
```

### Comparing `openmsistream-1.3.4/openmsistream/s3_buckets/config_file_parser.py` & `openmsistream-1.4.0/openmsistream/s3_buckets/config_file_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Expands a ConfigFileParser for the S3 section of configs"""
 
-#imports
+# imports
 from ..utilities.config_file_parser import ConfigFileParser
 
-class S3ConfigFileParser(ConfigFileParser) :
+
+class S3ConfigFileParser(ConfigFileParser):
     """
     A class to parse S3 bucket configurations from files
     """
 
     @property
-    def s3_configs(self) :
+    def s3_configs(self):
         """
         The S3 section of the config file
         """
-        if self.__s3_configs is None :
-            self.__s3_configs = self._get_config_dict('s3')
+        if self.__s3_configs is None:
+            self.__s3_configs = self._get_config_dict("s3")
         return self.__s3_configs
 
-    def __init__(self,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.__s3_configs = None
```

### Comparing `openmsistream-1.3.4/openmsistream/s3_buckets/s3_service.py` & `openmsistream-1.4.0/openmsistream/s3_buckets/s3_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,109 @@
 """Utilities for working with S3 buckets"""
 
-# @author: Amir H. Sharifzadeh, https://pages.jh.edu/asharif9/
-# @project: OpenMSI
-# @date: 04/12/2022
-# @owner: The Institute of Data Intensive Engineering and Science, https://idies.jhu.edu/
-# Johns Hopkins University http://www.jhu.edu/
 import hashlib
 import boto3
 from ..utilities import LogOwner
 
-class S3Service(LogOwner) :
+
+class S3Service(LogOwner):
     """
     A class to work with an S3 connection session
     """
 
     def __init__(self, s3_config, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = boto3.session.Session()
 
-        self.bucket_name = s3_config['bucket_name']
-        endpoint_url = str(s3_config['endpoint_url'])
+        self.bucket_name = s3_config["bucket_name"]
+        endpoint_url = str(s3_config["endpoint_url"])
 
-        if not endpoint_url.startswith('https://'):
-            endpoint_url = 'https://' + endpoint_url
+        if not endpoint_url.startswith("https://"):
+            endpoint_url = "https://" + endpoint_url
         self.s3_client = self.session.client(
-            service_name='s3',
-            aws_access_key_id=s3_config['access_key_id'],
-            aws_secret_access_key=s3_config['secret_key_id'],
-            region_name=s3_config['region'],
-            endpoint_url= endpoint_url
+            service_name="s3",
+            aws_access_key_id=s3_config["access_key_id"],
+            aws_secret_access_key=s3_config["secret_key_id"],
+            region_name=s3_config["region"],
+            endpoint_url=endpoint_url,
         )
-        self.region = s3_config['region']
+        self.region = s3_config["region"]
         self.grant_read = 'uri="http://acs.amazonaws.com/groups/global/AllUsers"'
 
     def get_object_stream_by_object_key(self, bucket_name, object_key):
         """
         Return the stream of an object in a bucket given its key
         """
         s3_response_object = self.s3_client.get_object(Bucket=bucket_name, Key=object_key)
-        return s3_response_object['Body'].read()
+        return s3_response_object["Body"].read()
 
     def delete_object_from_bucket(self, bucket_name, object_key):
         """
         Delete an object with a given key from a bucket
         """
         try:
             # make sure object exits before deleting the object from the bucket
-            s3_response_object = self.s3_client.get_object(Bucket=bucket_name, Key=object_key)
+            s3_response_object = self.s3_client.get_object(
+                Bucket=bucket_name, Key=object_key
+            )
             if s3_response_object is None:
-                msg = 'The object ' + object_key + ' does not exist in this bucket: ' + bucket_name
+                msg = (
+                    "The object "
+                    + object_key
+                    + " does not exist in this bucket: "
+                    + bucket_name
+                )
                 self.logger.error(msg)
                 return
         except Exception:
-            msg  = 'A problem occurred while reading ' + object_key + ' from bucket: ' + bucket_name
+            msg = (
+                "A problem occurred while reading "
+                + object_key
+                + " from bucket: "
+                + bucket_name
+            )
             self.logger.error(msg)
             return
         # delete the object from the bucket safely
         try:
             self.s3_client.delete_object(Bucket=bucket_name, Key=object_key)
-            msg = object_key + ' was deleted successfully from bucket: ' + bucket_name
+            msg = object_key + " was deleted successfully from bucket: " + bucket_name
             self.logger.debug(msg)
         except Exception:
-            msg = 'Could not delete ' + object_key + ' from bucket: ' + bucket_name
+            msg = "Could not delete " + object_key + " from bucket: " + bucket_name
             self.logger.error(msg)
             return
 
-    def compare_producer_datafile_with_s3_object_stream(self, bucket_name, object_key, hashed_datafile_stream):
+    def compare_producer_datafile_with_s3_object_stream(
+        self, bucket_name, object_key, hashed_datafile_stream
+    ):
         """
         Compare a given DataFile hash with the hash of an object in a bucket
         """
         if hashed_datafile_stream is None:
             return False
         s3_response_object = self.s3_client.get_object(Bucket=bucket_name, Key=object_key)
-        object_content = s3_response_object['Body'].read()
+        object_content = s3_response_object["Body"].read()
         md5 = hashlib.md5()
         md5.update(object_content)
         if object_content is None:
             return False
         hhh = format(md5.hexdigest())
         return str(hhh) == hashed_datafile_stream
 
-    def compare_consumer_datafile_with_s3_object_stream(self, bucket_name, object_key, datafile):
+    def compare_consumer_datafile_with_s3_object_stream(
+        self, bucket_name, object_key, datafile
+    ):
         """
         Compare a given DataFile with an object in a bucket using their hashes
         """
         if datafile is None:
             return False
         s3_response_object = self.s3_client.get_object(Bucket=bucket_name, Key=object_key)
-        object_content = s3_response_object['Body'].read()
+        object_content = s3_response_object["Body"].read()
         if object_content is None:
             return False
         datafile_md5 = hashlib.md5()
         datafile_md5.update(datafile.bytestring)
         object_content_md5 = hashlib.md5()
         object_content_md5.update(object_content)
         return format(datafile_md5.hexdigest()) == format(object_content_md5.hexdigest())
```

### Comparing `openmsistream-1.3.4/openmsistream/s3_buckets/s3_transfer_stream_processor.py` & `openmsistream-1.4.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,168 @@
-"""Transfer contents of DataFiles read from chunks in a topic to an S3 bucket when complete files become available"""
+"""
+Transfer contents of DataFiles read from chunks in a topic to an S3 bucket
+when complete files become available
+"""
 
-#imports
+# imports
 from ..data_file_io.actor.data_file_stream_processor import DataFileStreamProcessor
 from .config_file_parser import S3ConfigFileParser
 from .s3_data_transfer import S3DataTransfer
 
-class S3TransferStreamProcessor(DataFileStreamProcessor) :
+
+class S3TransferStreamProcessor(DataFileStreamProcessor):
     """
     A class to reconstruct data files read as messages from a topic, hold them in memory,
     and transfer them to an S3 bucket when all of their messages have been received
 
     :param bucket_name: Name of the S3 bucket into which reconstructed files should be transferred
     :type bucket_name: str
-    :param config_path: Path to the config file to use in defining the Broker connection and Consumers
+    :param config_path: Path to the config file to use in defining the Broker connection
+        and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
     """
 
-    def __init__(self, bucket_name, config_path, topic_name, **kwargs) :
+    def __init__(self, bucket_name, config_path, topic_name, **kwargs):
         super().__init__(config_path, topic_name, **kwargs)
-        parser = S3ConfigFileParser(config_path,logger=self.logger)
+        parser = S3ConfigFileParser(config_path, logger=self.logger)
         self.__s3_config = parser.s3_configs
-        self.__s3_config['bucket_name'] = bucket_name
+        self.__s3_config["bucket_name"] = bucket_name
         self.bucket_name = bucket_name
-        self.s3d = S3DataTransfer(self.__s3_config,logger=self.logger)
+        self.s3d = S3DataTransfer(self.__s3_config, logger=self.logger)
 
     def make_stream(self):
         """
         Runs :func:`~DataFileStreamProcessor.process_files_as_read` to reconstruct files in memory
-        and transfer completed files to the S3 bucket. Runs until the user inputs a command to shut it down.
+        and transfer completed files to the S3 bucket.
+        Runs until the user inputs a command to shut it down.
 
         :return: the total number of messages consumed
         :rtype: int
         :return: the total number of messages processed (registered in memory)
         :rtype: int
         :return: the paths of files successfully transferred to the S3 bucket during the run
         :rtype: list
         """
         return self.process_files_as_read()
 
     def _process_downloaded_data_file(self, datafile, lock):
         """
-        Transfer a fully-reconstructed file to the S3 bucket and verify that its contents in the bucket
-        match its original hash from disk. Logs a warning if the file hashes don't match.
+        Transfer a fully-reconstructed file to the S3 bucket and verify that its contents
+        in the bucket match its original hash from disk.
+        Logs a warning if the file hashes don't match.
 
         :param datafile: A :class:`~DownloadDataFileToMemory` object that has received
             all of its messages from the topic
         :type datafile: :class:`~DownloadDataFileToMemory`
-        :param lock: Acquiring this :class:`threading.Lock` object would ensure that only one instance
+        :param lock: Acquiring this :class:`threading.Lock` object ensures that only one instance
             of :func:`~_process_downloaded_data_file` is running at once
         :type lock: :class:`threading.Lock`
 
         :return: None if processing was successful, a caught Exception otherwise
         """
         object_key = self.__get_datafile_object_key(datafile)
-        try :
+        try:
             self.s3d.transfer_object_stream(object_key, datafile)
-        except Exception as exc :
-            self.logger.error(f'ERROR: failed to transfer {datafile.filename} to the object store')
+        except Exception as exc:
+            self.logger.error(
+                f"ERROR: failed to transfer {datafile.filename} to the object store"
+            )
             return exc
-        if self.s3d.compare_consumer_datafile_with_s3_object_stream(self.bucket_name, object_key, datafile):
-            self.logger.debug(object_key + ' matched with consumer datafile')
+        if self.s3d.compare_consumer_datafile_with_s3_object_stream(
+            self.bucket_name, object_key, datafile
+        ):
+            self.logger.debug(object_key + " matched with consumer datafile")
             # self.s3d.delete_object_from_bucket(self.bucket_name, object_key)
-        else :
-            warnmsg = f'WARNING: {object_key} transferred to bucket but the file on the bucket does not match '
-            warnmsg+= 'the file originally read from disk!'
+        else:
+            warnmsg = (
+                f"WARNING: {object_key} transferred to bucket but the file in the bucket "
+                "does not match the file originally read from disk!"
+            )
             self.logger.warning(warnmsg)
         return None
 
-    def __get_datafile_object_key(self,datafile) :
-        file_name = str(datafile.filename)
+    def __get_datafile_object_key(self, datafile):
         sub_dir = datafile.subdir_str
-        object_key = self.topic_name
-        if sub_dir!='' :
-            object_key+= '/' + sub_dir
-        object_key+= '/' + file_name
-        return object_key
+        return (
+            f'{self.topic_name}{"/" if sub_dir!="" else ""}{sub_dir}/{datafile.filename}'
+        )
 
     @classmethod
     def get_command_line_arguments(cls):
         superargs, superkwargs = super().get_command_line_arguments()
-        args = [*superargs, 'bucket_name']
-        kwargs = {**superkwargs,'config':'test_s3_transfer'}
+        args = [*superargs, "bucket_name"]
+        kwargs = {**superkwargs, "config": "test_s3_transfer"}
         return args, kwargs
 
     @classmethod
     def run_from_command_line(cls, args=None):
         """
         Run a :class:`~S3TransferStreamProcessor` directly from the command line
 
         Calls :func:`~make_stream` on a :class:`~S3TransferStreamProcessor` defined by
         command line (or given) arguments
 
-        :param args: the list of arguments to send to the parser instead of getting them from sys.argv
+        :param args: the list of arguments to send to the parser instead of getting them
+            from sys.argv
         :type args: list, optional
         """
         # make the argument parser
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
-        s3_stream_proc = cls(args.bucket_name,
-                             args.config, args.topic_name,
-                             output_dir=args.output_dir,
-                             n_threads=args.n_threads,
-                             update_secs=args.update_seconds,
-                             consumer_group_id=args.consumer_group_id,
-                             streamlevel=args.logger_stream_level,filelevel=args.logger_file_level)
+        s3_stream_proc = cls(
+            args.bucket_name,
+            args.config,
+            args.topic_name,
+            output_dir=args.output_dir,
+            n_threads=args.n_threads,
+            update_secs=args.update_seconds,
+            consumer_group_id=args.consumer_group_id,
+            streamlevel=args.logger_stream_level,
+            filelevel=args.logger_file_level,
+        )
         # cls.bucket_name = args.bucket_name
-        msg = f'Listening to the {args.topic_name} topic for files to add to the {args.bucket_name} bucket....'
+        msg = (
+            f"Listening to the {args.topic_name} topic for files to add to the "
+            f"{args.bucket_name} bucket...."
+        )
         s3_stream_proc.logger.info(msg)
-        n_read,n_processed,complete_filenames = s3_stream_proc.make_stream()
+        n_read, n_processed, n_complete, complete_filenames = s3_stream_proc.make_stream()
         s3_stream_proc.close()
-        msg = f'{n_read} total messages were consumed, {n_processed} messages were successfully processed,'
-        msg+= f'and {len(complete_filenames)} files were transferred to the {args.bucket_name} bucket'
+        msg = (
+            f"{n_read} total messages were consumed, {n_processed} messages were "
+            f"successfully processed, and {len(complete_filenames)} files were transferred "
+            f"to the {args.bucket_name} bucket"
+        )
         s3_stream_proc.logger.info(msg)
-        if len(complete_filenames)>0 :
-            msg =f'The following {len(complete_filenames)} file'
-            msg+=' was' if len(complete_filenames)==1 else 's were'
-            msg+=f' successfully transferred to the {args.bucket_name} bucket'
-            for fn in complete_filenames :
-                msg+=f'\n\t{fn}'
+        if len(complete_filenames) > 0:
+            msg = (
+                f'{n_complete} file{" was" if n_complete==1 else "s were"} successfully '
+                f"transferred to the {args.bucket_name} bucket.\nTransferred filepaths "
+                f"(up to {cls.N_RECENT_FILES} most recent):\n\t"
+            )
+            msg += "\n\t".join(complete_filenames)
             s3_stream_proc.logger.debug(msg)
 
-    def _on_check(self) :
-        msg = f'{self.n_msgs_read} messages read, {self.n_msgs_processed} messages processed, '
-        msg+= f'{len(self.completely_processed_filepaths)} files transferred so far'
+    def _on_check(self):
+        msg = (
+            f"{self.n_msgs_read} messages read, {self.n_msgs_processed} messages processed, "
+            f"{self.n_processed_files} files transferred so far"
+        )
         self.logger.info(msg)
-        if len(self.files_in_progress_by_path)>0 or len(self.completely_processed_filepaths)>0 :
+        if (
+            len(self.files_in_progress_by_path) > 0
+            or len(self.recent_processed_filepaths) > 0
+        ):
             self.logger.debug(self.progress_msg)
 
+
 def main(args=None):
     """
     Main method to run from command line
     """
     S3TransferStreamProcessor.run_from_command_line(args)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/services/config.py` & `openmsistream-1.4.0/openmsistream/services/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,72 @@
 """Utility class holding constants and small calculations for working with Services/daemons"""
 
-#imports
+# imports
 import os, pathlib, importlib
 from inspect import isclass
 import pkg_resources
 from ..utilities import Logger
 
-class ServicesConstants :
+
+class ServicesConstants:
     """
     Constants for working with services
     """
 
-    WORKING_DIR = ( os.environ['OPENMSISTREAM_SERVICES_WORKING_DIR']
-                    if 'OPENMSISTREAM_SERVICES_WORKING_DIR' in os.environ else
-                    (pathlib.Path(__file__).parent/'working_dir').resolve() )
-    NSSM_PATH = WORKING_DIR / 'nssm.exe'
-    NSSM_DOWNLOAD_URL = 'https://nssm.cc/release/nssm-2.24.zip' # The URL to use for downloading NSSM when needed
-    ERROR_LOG_STEM = '_ERROR_LOG.txt'
-    SERVICE_EXECUTABLE_NAME_STEM = '_service_executable.py'
-    DAEMON_SERVICE_DIR = pathlib.Path('/etc/systemd/system/')
+    WORKING_DIR = (
+        os.environ["OPENMSISTREAM_SERVICES_WORKING_DIR"]
+        if "OPENMSISTREAM_SERVICES_WORKING_DIR" in os.environ
+        else (pathlib.Path(__file__).parent / "working_dir").resolve()
+    )
+    NSSM_PATH = WORKING_DIR / "nssm.exe"
+    # The URL to use for downloading NSSM when needed
+    NSSM_DOWNLOAD_URL = "https://nssm.cc/release/nssm-2.24.zip"
+    ERROR_LOG_STEM = "_ERROR_LOG.txt"
+    SERVICE_EXECUTABLE_NAME_STEM = "_service_executable.py"
+    DAEMON_SERVICE_DIR = pathlib.Path("/etc/systemd/system/")
 
     @property
-    def available_services(self) :
+    def available_services(self):
         """
         A dictionary with details of the services that are available
         """
         return self.service_dicts
 
-    def __init__(self) :
-        #make the Service dictionaries to use
+    def __init__(self):
+        # make the Service dictionaries to use
         self.service_dicts = []
-        for script in pkg_resources.iter_entry_points('console_scripts') :
-            if script.dist.key == 'openmsistream' :
-                if script.name in ('InstallService','ManageService','ProvisionNode') :
+        for script in pkg_resources.iter_entry_points("console_scripts"):
+            if script.dist.key == "openmsistream":
+                if script.name in ("InstallService", "ManageService", "ProvisionNode"):
                     continue
                 scriptstr = str(script)
                 cmd = (scriptstr.split())[0]
-                path = ((scriptstr.split())[2].split(':'))[0]
-                funcname = (((scriptstr.split())[2]).split(':'))[1]
+                path = ((scriptstr.split())[2].split(":"))[0]
+                funcname = (((scriptstr.split())[2]).split(":"))[1]
                 module = importlib.import_module(path)
-                run_classes = [getattr(module,x) for x in dir(module)
-                               if isclass(getattr(module,x)) and getattr(module,x).__name__==script.name]
-                if len(run_classes)!=1 :
-                    errmsg = f'ERROR: could not determine class for script {cmd} in file {path}! '
-                    errmsg+= f'Possibilities found: {run_classes}'
+                run_classes = [
+                    getattr(module, x)
+                    for x in dir(module)
+                    if isclass(getattr(module, x))
+                    and getattr(module, x).__name__ == script.name
+                ]
+                if len(run_classes) != 1:
+                    errmsg = (
+                        f"ERROR: could not determine class for script {cmd} in file {path}! "
+                        f"Possibilities found: {run_classes}"
+                    )
                     raise RuntimeError(errmsg)
-                self.service_dicts.append({'class_name':cmd,
-                                           'class':run_classes[0],
-                                           'filepath':path,
-                                           'func_name':funcname})
-        #make the logger to use
-        self.logger = Logger('Services',logger_filepath=self.WORKING_DIR/'Services.log')
+                self.service_dicts.append(
+                    {
+                        "class_name": cmd,
+                        "class": run_classes[0],
+                        "filepath": path,
+                        "func_name": funcname,
+                    }
+                )
+        # make the logger to use
+        self.logger = Logger(
+            "Services", logger_filepath=self.WORKING_DIR / "Services.log"
+        )
+
 
 SERVICE_CONST = ServicesConstants()
```

### Comparing `openmsistream-1.3.4/openmsistream/services/examples/runnable_example.py` & `openmsistream-1.4.0/openmsistream/services/examples/runnable_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Example of a general Runnable class that can be installed as a Service/daemon"""
 
-#imports
+# imports
 import datetime, time
 from openmsistream.utilities import Runnable
 
-class RunnableExample(Runnable) :
+
+class RunnableExample(Runnable):
     """
     A class that extends Runnable as an example of installing a Runnable's
     "run_from_command_line" method as a Service/daemon
     """
 
     @classmethod
-    def get_command_line_arguments(cls) :
-        return ['output_dir'], {}
+    def get_command_line_arguments(cls):
+        return ["output_dir"], {}
 
     @classmethod
-    def run_from_command_line(cls,args=None) :
+    def run_from_command_line(cls, args=None):
         parser = cls.get_argument_parser()
         args = parser.parse_args(args)
-        test_file_name = 'runnable_example_service_test.txt'
-        if not (args.output_dir/test_file_name).is_file() :
-            with open(args.output_dir/test_file_name,'w') as fp :
-                msg = "This file was created to test running a generic Runnable's 'run_from_command_line' "
-                msg+= "method as a Service/daemon"
+        test_file_name = "runnable_example_service_test.txt"
+        if not (args.output_dir / test_file_name).is_file():
+            with open(args.output_dir / test_file_name, "w") as fp:
+                msg = (
+                    "This file was created to test running a generic Runnable's "
+                    "'run_from_command_line' method as a Service/daemon"
+                )
                 fp.write(msg)
-        with open(args.output_dir/test_file_name,'a') as fp :
-            fp.write(f'\nService rerun {(datetime.datetime.now()).strftime("on %Y-%m-%d at %H:%M:%S")}')
+        with open(args.output_dir / test_file_name, "a") as fp:
+            fp.write(
+                f'\nService rerun {(datetime.datetime.now()).strftime("on %Y-%m-%d at %H:%M:%S")}'
+            )
         time.sleep(30)
```

### Comparing `openmsistream-1.3.4/openmsistream/services/examples/script_example.py` & `openmsistream-1.4.0/openmsistream/services/examples/script_example.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 """Example of a general script that can be installed as a Service/daemon"""
 
-#imports
+# imports
 import pathlib, datetime, time
 from argparse import ArgumentParser
 
-def main(args=None) :
+
+def main(args=None):
     """
     The main function that will be run as a Service/daemon
     """
     parser = ArgumentParser()
-    parser.add_argument('output_dir',type=pathlib.Path,
-                        help='Path to the directory where the test file should be created')
+    parser.add_argument(
+        "output_dir",
+        type=pathlib.Path,
+        help="Path to the directory where the test file should be created",
+    )
     args = parser.parse_args(args)
-    if not args.output_dir.is_dir() :
-        if args.output_dir.exists() :
-            raise ValueError(f'ERROR: given output directory {args.output_dir} exists but is not a directory!')
+    if not args.output_dir.is_dir():
+        if args.output_dir.exists():
+            raise ValueError(
+                f"ERROR: given output directory {args.output_dir} exists but is not a directory!"
+            )
         args.output_dir.mkdir(parents=True)
-    test_file_name = 'script_example_service_test.txt'
-    if not (args.output_dir/test_file_name).is_file() :
-        with open(args.output_dir/test_file_name,'w') as fp :
-            fp.write('This file was created to test running a generic Python script as a Service/daemon')
-    with open(args.output_dir/test_file_name,'a') as fp :
-        fp.write(f'\nService rerun {(datetime.datetime.now()).strftime("on %Y-%m-%d at %H:%M:%S")}')
+    test_file_name = "script_example_service_test.txt"
+    if not (args.output_dir / test_file_name).is_file():
+        with open(args.output_dir / test_file_name, "w") as fp:
+            fp.write(
+                "This file was created to test running a generic Python script as a Service/daemon"
+            )
+    with open(args.output_dir / test_file_name, "a") as fp:
+        fp.write(
+            f'\nService rerun {(datetime.datetime.now()).strftime("on %Y-%m-%d at %H:%M:%S")}'
+        )
     time.sleep(30)
 
-if __name__=='__main__' :
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/services/install_service.py` & `openmsistream-1.4.0/openmsistream/services/install_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,64 @@
-"""Script to use the OS-appropriate ServceManager to install code as a Windows Service or Linux daemon"""
+"""
+Script to use the OS-appropriate ServceManager to install code
+as a Windows Service or Linux daemon
+"""
 
-#imports
+# imports
 import sys
 from .config import SERVICE_CONST
 from .utilities import test_python_code, get_os_name
 from .service_manager_base import ServiceManagerBase
 from .windows_service_manager import WindowsServiceManager
 from .linux_service_manager import LinuxServiceManager
 
-def main(given_args=None) :
+
+def main(given_args=None):
     """
     Install a Windows Service/Linux daemon (depending on the OS that's running)
     """
-    #get the arguments
-    if given_args is None :
-        parser = ServiceManagerBase.get_argument_parser('install',sys.argv[1] if len(sys.argv)>1 else None)
+    # get the arguments
+    if given_args is None:
+        parser = ServiceManagerBase.get_argument_parser(
+            "install", sys.argv[1] if len(sys.argv) > 1 else None
+        )
         args, _ = parser.parse_known_args()
-    else :
-        parser = ServiceManagerBase.get_argument_parser('install',given_args[0] if len(given_args)>0 else None)
+    else:
+        parser = ServiceManagerBase.get_argument_parser(
+            "install", given_args[0] if len(given_args) > 0 else None
+        )
         args, _ = parser.parse_known_args(given_args)
-    #run the tests if requested
-    if args.service_spec_string=='test' :
+    # run the tests if requested
+    if args.service_spec_string == "test":
         test_python_code()
-    else :
-        if args.service_name is None :
-            #default name of the Service is just the class name
+    else:
+        if args.service_name is None:
+            # default name of the Service is just the class name
             service_name = args.service_spec_string
-        else :
+        else:
             service_name = args.service_name
-        #make the list of arguments that should be sent to the run function in the executable (removing "service_name")
+        # make the list of arguments that should be sent to the run function in the executable
         argslist = sys.argv[2:] if given_args is None else given_args[1:]
-        if '--service_name' in argslist :
-            index = argslist.index('--service_name')
+        if "--service_name" in argslist:
+            index = argslist.index("--service_name")
             argslist.pop(index)
             argslist.pop(index)
-        #define arguments to and create the ServiceManager
+        # define arguments to and create the ServiceManager
         manager_args = [service_name]
-        manager_kwargs = {'service_spec_string':args.service_spec_string,
-                          'argslist':argslist,
-                          'interactive':given_args is None,
-                          'logger':SERVICE_CONST.logger}
-        managers_by_os_name = {'Windows':WindowsServiceManager,
-                               'Linux':LinuxServiceManager,}
+        manager_kwargs = {
+            "service_spec_string": args.service_spec_string,
+            "argslist": argslist,
+            "interactive": given_args is None,
+            "logger": SERVICE_CONST.logger,
+        }
+        managers_by_os_name = {
+            "Windows": WindowsServiceManager,
+            "Linux": LinuxServiceManager,
+        }
         manager_class = managers_by_os_name[get_os_name()]
-        manager = manager_class(*manager_args,**manager_kwargs)
-        #install the service
+        manager = manager_class(*manager_args, **manager_kwargs)
+        # install the service
         manager.install_service()
 
-if __name__=='__main__' :
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/services/linux_service_manager.py` & `openmsistream-1.4.0/openmsistream/services/linux_service_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,227 @@
 """Manage Linux daemons"""
 
-#imports
+# imports
 import sys, os, pathlib, textwrap
 from .config import SERVICE_CONST
 from .utilities import run_cmd_in_subprocess
 from .service_manager_base import ServiceManagerBase
 
-class LinuxServiceManager(ServiceManagerBase) :
+
+class LinuxServiceManager(ServiceManagerBase):
     """
     Base class for working with Linux daemons
 
     :param service_name: The name of the daemon as installed
     :type service_name: str
     :param service_spec_string: A string specifying which code should be run as a daemon.
         Could be the name of an OpenMSIStream Runnable class, or the path to a custom Python code.
         Custom Services can also specify a :class:`~.utilities.Runnable` class name,
-        and/or a function in the file using special formatting like [class_name]=[path.to.file]:[function_name].
-        Only needed to initially install the daemon.
+        and/or a function in the file using special formatting like
+        [class_name]=[path.to.file]:[function_name]. Only needed to initially install the daemon.
     :type service_spec_string: str, optional
     :param argslist: The list of arguments (as from the command line) to pass to the
         :class:`~.utilities.Runnable` class.
         Only needed to initially install the daemon.
     :type argslist: list, optional
     :param interactive: if True, a few more messages/prompts will come up telling a user what to do
     :type interactive: bool, optional
     """
 
     @property
     def env_var_names(self):
         env_var_names = super().env_var_names
-        #get the names of environment variables from the env_var file
-        if self.env_var_filepath.is_file() :
-            with open(self.env_var_filepath,'r') as fp :
+        # get the names of environment variables from the env_var file
+        if self.env_var_filepath.is_file():
+            with open(self.env_var_filepath, "r") as fp:
                 lines = fp.readlines()
-            for line in lines :
-                linesplit = (line.strip()).split('=')
-                if len(linesplit)==2 :
+            for line in lines:
+                linesplit = (line.strip()).split("=")
+                if len(linesplit) == 2:
                     env_var_names.add(linesplit[0])
-        for evn in env_var_names :
+        for evn in env_var_names:
             yield evn
 
-    def __init__(self,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
-        self.daemon_working_dir_filepath = SERVICE_CONST.WORKING_DIR/f'{self.service_name}.service'
-        self.daemon_filepath = SERVICE_CONST.DAEMON_SERVICE_DIR/self.daemon_working_dir_filepath.name
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.daemon_working_dir_filepath = (
+            SERVICE_CONST.WORKING_DIR / f"{self.service_name}.service"
+        )
+        self.daemon_filepath = (
+            SERVICE_CONST.DAEMON_SERVICE_DIR / self.daemon_working_dir_filepath.name
+        )
 
-    def install_service(self) :
+    def install_service(self):
         """
         Install the daemon
         """
         super().install_service()
-        #make sure systemd is running
+        # make sure systemd is running
         self.__check_systemd_installed()
-        #write the daemon file pointing to the executable
+        # write the daemon file pointing to the executable
         self.__write_daemon_file()
-        #enable the service
-        run_cmd_in_subprocess(['sudo','systemctl','daemon-reload'],logger=self.logger)
-        run_cmd_in_subprocess(['sudo','systemctl','enable',f'{self.service_name}.service'],logger=self.logger)
-        self.logger.info(f'Done installing {self.service_name}')
+        # enable the service
+        run_cmd_in_subprocess(["sudo", "systemctl", "daemon-reload"], logger=self.logger)
+        run_cmd_in_subprocess(
+            ["sudo", "systemctl", "enable", f"{self.service_name}.service"],
+            logger=self.logger,
+        )
+        self.logger.info(f"Done installing {self.service_name}")
 
-    def start_service(self) :
+    def start_service(self):
         """
         Start the daemon
         """
-        self.logger.info(f'Starting {self.service_name}...')
+        self.logger.info(f"Starting {self.service_name}...")
         self.__check_systemd_installed()
-        run_cmd_in_subprocess(['sudo','systemctl','daemon-reload'],logger=self.logger)
-        run_cmd_in_subprocess(['sudo','systemctl','start',f'{self.service_name}.service'],logger=self.logger)
-        self.logger.info(f'Done starting {self.service_name}')
+        run_cmd_in_subprocess(["sudo", "systemctl", "daemon-reload"], logger=self.logger)
+        run_cmd_in_subprocess(
+            ["sudo", "systemctl", "start", f"{self.service_name}.service"],
+            logger=self.logger,
+        )
+        self.logger.info(f"Done starting {self.service_name}")
 
-    def service_status(self) :
+    def service_status(self):
         """
         Print the status of the daemon
         """
         self.__check_systemd_installed()
-        result = run_cmd_in_subprocess(['sudo','systemctl','status',f'{self.service_name}.service'],logger=self.logger)
-        self.logger.info(f'{self.service_name} status: {result.decode()}')
+        result = run_cmd_in_subprocess(
+            ["sudo", "systemctl", "status", f"{self.service_name}.service"],
+            logger=self.logger,
+        )
+        self.logger.info(f"{self.service_name} status: {result.decode()}")
 
-    def stop_service(self) :
+    def stop_service(self):
         """
         Stop the daemon
         """
-        self.logger.info(f'Stopping {self.service_name}...')
+        self.logger.info(f"Stopping {self.service_name}...")
         self.__check_systemd_installed()
-        run_cmd_in_subprocess(['sudo','systemctl','stop',f'{self.service_name}.service'],logger=self.logger)
-        self.logger.info(f'Done stopping {self.service_name}')
-
-    def remove_service(self,remove_env_vars=False,remove_install_args=False,remove_nssm=False) :
+        run_cmd_in_subprocess(
+            ["sudo", "systemctl", "stop", f"{self.service_name}.service"],
+            logger=self.logger,
+        )
+        self.logger.info(f"Done stopping {self.service_name}")
+
+    def remove_service(
+        self, remove_env_vars=False, remove_install_args=False, remove_nssm=False
+    ):
         """
         Remove the daemon.
 
-        :param remove_env_vars: if True, any environment variables needed by the daemon will be removed.
+        :param remove_env_vars: if True, any environment variables needed by the daemon
+            will be removed.
         :type remove_env_vars: bool, optional.
-        :param remove_install_args: if True, the file listing the arguments used to install the daemon
-            (to make it easier to re-install) will be removed.
+        :param remove_install_args: if True, the file listing the arguments used to
+            install the daemon (to make it easier to re-install) will be removed.
         :type remove_install_args: bool, optional
         :param remove_nssm: Not used for Linux daemons.
         :type remove_nssm: bool, optional
         """
-        self.logger.info(f'Removing {self.service_name}...')
+        self.logger.info(f"Removing {self.service_name}...")
         self.__check_systemd_installed()
-        try :
-            run_cmd_in_subprocess(['sudo','systemctl','disable',f'{self.service_name}.service'],logger=self.logger)
-        except Exception :
+        try:
+            run_cmd_in_subprocess(
+                ["sudo", "systemctl", "disable", f"{self.service_name}.service"],
+                logger=self.logger,
+            )
+        except Exception:
             pass
-        if self.daemon_filepath.exists() :
-            run_cmd_in_subprocess(['sudo','rm','-f',str(self.daemon_filepath)],logger=self.logger)
-        run_cmd_in_subprocess(['sudo','systemctl','daemon-reload'],logger=self.logger)
-        run_cmd_in_subprocess(['sudo','systemctl','reset-failed'],logger=self.logger)
-        self.logger.info('Service removed')
-        if remove_nssm :
-            warnmsg = "WARNING: requested to remove NSSM along with the Service, "
-            warnmsg+= "but Linux Services don't install NSSM so nothing was done."
+        if self.daemon_filepath.exists():
+            run_cmd_in_subprocess(
+                ["sudo", "rm", "-f", str(self.daemon_filepath)], logger=self.logger
+            )
+        run_cmd_in_subprocess(["sudo", "systemctl", "daemon-reload"], logger=self.logger)
+        run_cmd_in_subprocess(["sudo", "systemctl", "reset-failed"], logger=self.logger)
+        self.logger.info("Service removed")
+        if remove_nssm:
+            warnmsg = (
+                "WARNING: requested to remove NSSM along with the Service, but "
+                "Linux Services don't install NSSM so nothing was done."
+            )
             self.logger.warning(warnmsg)
-        super().remove_service(remove_env_vars=remove_env_vars,remove_install_args=remove_install_args)
-
-    def _write_env_var_file(self) :
-        code = ''
-        for evn in self.env_var_names :
-            val = os.path.expandvars(f'${evn}')
-            if val==f'${evn}' :
-                raise RuntimeError(f'ERROR: value not found for expected environment variable {evn}!')
-            code += f'{evn}={val}\n'
-        if code=='' :
+        super().remove_service(
+            remove_env_vars=remove_env_vars, remove_install_args=remove_install_args
+        )
+
+    def _write_env_var_file(self):
+        code = ""
+        for evn in self.env_var_names:
+            val = os.path.expandvars(f"${evn}")
+            if val == f"${evn}":
+                raise RuntimeError(
+                    f"ERROR: value not found for expected environment variable {evn}!"
+                )
+            code += f"{evn}={val}\n"
+        if code == "":
             return False
-        with open(self.env_var_filepath,'w') as fp :
+        with open(self.env_var_filepath, "w") as fp:
             fp.write(code)
-        run_cmd_in_subprocess(['chmod','go-rwx',self.env_var_filepath])
+        run_cmd_in_subprocess(["chmod", "go-rwx", self.env_var_filepath])
         return True
 
-    def __check_systemd_installed(self) :
+    def __check_systemd_installed(self):
         """
         Raises an error if systemd is not installed (systemd is needed to control Linux daemons)
         """
-        check = run_cmd_in_subprocess(['ps','--no-headers','-o','comm','1'],logger=self.logger)
-        if check.decode().rstrip()!='systemd' :
-            errmsg = 'ERROR: Installing programs as Services ("daemons") on Linux requires systemd!'
-            errmsg = 'You can install systemd with "sudo apt install systemd" (or similar) and try again.'
-            self.logger.error(errmsg,exc_type=RuntimeError)
+        check = run_cmd_in_subprocess(
+            ["ps", "--no-headers", "-o", "comm", "1"], logger=self.logger
+        )
+        if check.decode().rstrip() != "systemd":
+            errmsg = (
+                'ERROR: Installing programs as Services ("daemons") on Linux requires systemd!'
+                'You can install systemd with "sudo apt install systemd" (or similar) '
+                "and try again."
+            )
+            self.logger.error(errmsg, exc_type=RuntimeError)
 
-    def __write_daemon_file(self) :
+    def __write_daemon_file(self):
         """
         Write the Unit/.service file to the daemon directory that calls the Python executable
         """
-        #make sure the directory to hold the file exists
-        if not SERVICE_CONST.DAEMON_SERVICE_DIR.is_dir() :
-            SERVICE_CONST.logger.info(f'Creating a new daemon service directory at {SERVICE_CONST.DAEMON_SERVICE_DIR}')
+        # make sure the directory to hold the file exists
+        if not SERVICE_CONST.DAEMON_SERVICE_DIR.is_dir():
+            SERVICE_CONST.logger.info(
+                f"Creating a new daemon service directory at {SERVICE_CONST.DAEMON_SERVICE_DIR}"
+            )
             SERVICE_CONST.DAEMON_SERVICE_DIR.mkdir(parents=True)
-        #write out the file pointing to the python executable
-        description = 'Python script'
-        if self.service_dict['class'] is not None :
-            classdoc = self.service_dict['class'].__doc__
-            if classdoc is not None :
-                description = classdoc.strip().replace('\n',' ')
-            else :
-                description+=f" for a {self.service_dict['class']} object"
-        code = f'''\
+        # write out the file pointing to the python executable
+        description = "Python script"
+        if self.service_dict["class"] is not None:
+            classdoc = self.service_dict["class"].__doc__
+            if classdoc is not None:
+                description = classdoc.strip().replace("\n", " ")
+            else:
+                description += f" for a {self.service_dict['class']} object"
+        code = f"""\
             [Unit]
             Description = {description}
             Requires = network-online.target local-fs.target remote-fs.target
             After = network-online.target local-fs.target remote-fs.target
 
             [Service]
             Type = simple
             KillMode = none
             User = root
-            ExecStart = {sys.executable} {self.exec_fp}'''
-        if self.env_vars_needed :
-            code+=f'''\n\
-            EnvironmentFile = {self.env_var_filepath}'''
-        code+=f'''\n\
+            ExecStart = {sys.executable} {self.exec_fp}"""
+        if self.env_vars_needed:
+            code += f"""\n\
+            EnvironmentFile = {self.env_var_filepath}"""
+        code += f"""\n\
             WorkingDirectory = {pathlib.Path().resolve()}
             Restart = always
             RestartSec = 120
 
             [Install]
-            WantedBy = multi-user.target'''
-        with open(self.daemon_working_dir_filepath,'w') as fp :
+            WantedBy = multi-user.target"""
+        with open(self.daemon_working_dir_filepath, "w") as fp:
             fp.write(textwrap.dedent(code))
-        run_cmd_in_subprocess(['sudo','mv',str(self.daemon_working_dir_filepath),str(self.daemon_filepath.parent)],
-                              logger=self.logger)
+        run_cmd_in_subprocess(
+            [
+                "sudo",
+                "mv",
+                str(self.daemon_working_dir_filepath),
+                str(self.daemon_filepath.parent),
+            ],
+            logger=self.logger,
+        )
```

### Comparing `openmsistream-1.3.4/openmsistream/services/manage_service.py` & `openmsistream-1.4.0/openmsistream/services/manage_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 """Script to invoke the OS-appropriate ServiceManager class to do anything other than installing"""
 
-#imports
+# imports
 from .config import SERVICE_CONST
 from .utilities import get_os_name
 from .service_manager_base import ServiceManagerBase
 from .windows_service_manager import WindowsServiceManager
 from .linux_service_manager import LinuxServiceManager
 
-def main(given_args=None) :
+
+def main(given_args=None):
     """
-    Use the OS-appropriate ServiceManager class to manage a Service/daemon (i.e., anything except installing it)
+    Use the OS-appropriate ServiceManager class to manage a Service/daemon
+    (i.e., anything except installing it)
     """
-    #get the arguments
-    parser = ServiceManagerBase.get_argument_parser('manage')
+    # get the arguments
+    parser = ServiceManagerBase.get_argument_parser("manage")
     args = parser.parse_args() if given_args is None else parser.parse_args(given_args)
-    #get the name of the OS and start the object
+    # get the name of the OS and start the object
     operating_system = get_os_name()
     manager_args = [args.service_name]
-    manager_kwargs = {'interactive':given_args is None,
-                      'logger':SERVICE_CONST.logger}
-    managers_by_os_name = {'Windows':WindowsServiceManager,
-                           'Linux':LinuxServiceManager,}
+    manager_kwargs = {"interactive": given_args is None, "logger": SERVICE_CONST.logger}
+    managers_by_os_name = {
+        "Windows": WindowsServiceManager,
+        "Linux": LinuxServiceManager,
+    }
     manager_class = managers_by_os_name[operating_system]
-    manager = manager_class(*manager_args,**manager_kwargs)
-    #run some function based on the run mode
-    manager.run_manage_command(args.run_mode,
-                               remove_env_vars=args.remove_env_vars,
-                               remove_install_args=args.remove_install_args,
-                               remove_nssm=args.remove_nssm)
+    manager = manager_class(*manager_args, **manager_kwargs)
+    # run some function based on the run mode
+    manager.run_manage_command(
+        args.run_mode,
+        remove_env_vars=args.remove_env_vars,
+        remove_install_args=args.remove_install_args,
+        remove_nssm=args.remove_nssm,
+    )
+
 
-if __name__=='__main__' :
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/services/service_manager_base.py` & `openmsistream-1.4.0/openmsistream/services/service_manager_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,412 +1,531 @@
 """Functionality common to both Windows Services and Linux daemons"""
 
-#imports
+# imports
 import sys, pathlib, textwrap, importlib
 from abc import abstractmethod
 from subprocess import CalledProcessError
 from ..utilities import LogOwner, HasArgumentParser, Runnable, OpenMSIStreamArgumentParser
 from ..utilities.config_file_parser import ConfigFileParser
 from .config import SERVICE_CONST
 from .utilities import set_env_vars, remove_env_var
 
-class ServiceManagerBase(LogOwner,HasArgumentParser) :
+
+class ServiceManagerBase(LogOwner, HasArgumentParser):
     """
     Base class for working with Services in general
 
     :param service_name: The name of the Service/daemon as installed
     :type service_name: str
     :param service_spec_string: A string specifying which code should be run as a Service.
         Could be the name of an OpenMSIStream Runnable class, or the path to a custom Python code.
-        Custom Services can also specify a :class:`~Runnable` class name, and/or a function in the file
-        using special formatting like [class_name]=[path.to.file]:[function_name].
+        Custom Services can also specify a :class:`~Runnable` class name, and/or a function
+        in the file using special formatting like [class_name]=[path.to.file]:[function_name].
         Only needed to initially install the Service/daemon.
     :type service_spec_string: str, optional
-    :param argslist: The list of arguments (as from the command line) to pass to the :class:`~Runnable` class.
-        Only needed to initially install the Service/daemon.
+    :param argslist: The list of arguments (as from the command line) to pass to the
+        :class:`~Runnable` class. Only needed to initially install the Service/daemon.
     :type argslist: list, optional
     :param interactive: if True, a few more messages/prompts will come up telling a user what to do
     :type interactive: bool, optional
     """
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,service_name,*,service_spec_string=None,argslist=None,interactive=None,**kwargs) :
+    def __init__(
+        self,
+        service_name,
+        *,
+        service_spec_string=None,
+        argslist=None,
+        interactive=None,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         self.service_name = service_name
         self.service_spec_string = service_spec_string
         self.__set_service_dict()
         self.argslist = argslist
         self.interactive = interactive
-        self.env_var_filepath = SERVICE_CONST.WORKING_DIR/f'{self.service_name}_env_vars.txt'
-        self.install_args_filepath = SERVICE_CONST.WORKING_DIR/f'{self.service_name}_install_args.txt'
-        self.exec_fp = SERVICE_CONST.WORKING_DIR/f'{self.service_name}{SERVICE_CONST.SERVICE_EXECUTABLE_NAME_STEM}'
+        self.env_var_filepath = (
+            SERVICE_CONST.WORKING_DIR / f"{self.service_name}_env_vars.txt"
+        )
+        self.install_args_filepath = (
+            SERVICE_CONST.WORKING_DIR / f"{self.service_name}_install_args.txt"
+        )
+        self.exec_fp = (
+            SERVICE_CONST.WORKING_DIR
+            / f"{self.service_name}{SERVICE_CONST.SERVICE_EXECUTABLE_NAME_STEM}"
+        )
         self.env_vars_needed = None
 
-    def install_service(self) :
+    def install_service(self):
         """
         Install the Service
         child classes should call this method to get the setup done before they do anything specific
         """
-        #make sure the necessary information was supplied
-        if self.service_dict is None or self.argslist is None :
-            errmsg = 'ERROR: newly installing a Service requires specifying what to install '
-            errmsg+= 'and giving an argslist!'
-            self.logger.error(errmsg,exc_type=RuntimeError)
-        #set the environment variables
-        must_rerun = set_env_vars(self.env_var_names,interactive=self.interactive)
-        if must_rerun :
-            msg = 'New values for environment variables have been set. '
-            msg+= 'Please close this window and rerun InstallService so that their values get picked up.'
+        # make sure the necessary information was supplied
+        if self.service_dict is None or self.argslist is None:
+            errmsg = (
+                "ERROR: newly installing a Service requires specifying what to install "
+                "and giving an argslist!"
+            )
+            self.logger.error(errmsg, exc_type=RuntimeError)
+        # set the environment variables
+        must_rerun = set_env_vars(self.env_var_names, interactive=self.interactive)
+        if must_rerun:
+            msg = (
+                "New values for environment variables have been set. Please close this window "
+                "and rerun InstallService so that their values get picked up."
+            )
             self.logger.info(msg)
             sys.exit(0)
-        #write out the environment variable file
+        # write out the environment variable file
         self.env_vars_needed = self._write_env_var_file()
-        #write out the install arguments file
+        # write out the install arguments file
         self._write_install_args_file()
-        #write out the executable file
+        # write out the executable file
         self._write_executable_file()
-        #install the service
-        msg = 'Installing '
-        if self.service_dict['class_name'] is not None :
-            msg+='a'
-            if self.service_dict['class_name'].lower() in ('a','e','i','o','u','y') :
-                msg+='n'
-            msg+=f" {self.service_dict['class_name']} program "
-        else :
-            msg+=f"{self.service_dict['filepath']}"
-            if self.service_dict['func_name'] is not None :
-                msg+=f":{self.service_dict['func_name']}"
-        msg+=f' as "{self.service_name}" from executable at {self.exec_fp}'
+        # install the service
+        msg = "Installing "
+        if self.service_dict["class_name"] is not None:
+            msg += "a"
+            if self.service_dict["class_name"].lower() in ("a", "e", "i", "o", "u", "y"):
+                msg += "n"
+            msg += f" {self.service_dict['class_name']} program "
+        else:
+            msg += f"{self.service_dict['filepath']}"
+            if self.service_dict["func_name"] is not None:
+                msg += f":{self.service_dict['func_name']}"
+        msg += f' as "{self.service_name}" from executable at {self.exec_fp}'
         self.logger.info(msg)
 
-    def run_manage_command(self,run_mode,remove_env_vars=False,remove_install_args=False,remove_nssm=False) :
+    def run_manage_command(
+        self,
+        run_mode,
+        remove_env_vars=False,
+        remove_install_args=False,
+        remove_nssm=False,
+    ):
         """
         Run one of the other functions according to the action given
 
         :param run_mode: The string identifying the action(s) that should be taken
         :type run_mode: str
-        :param remove_env_vars: if True, any environment variables needed by the Service/daemon will be removed.
-            Only used when removing the Service/daemon.
+        :param remove_env_vars: if True, any environment variables needed by the Service/daemon
+            will be removed. Only used when removing the Service/daemon.
         :type remove_env_vars: bool, optional.
-        :param remove_install_args: if True, the file listing the arguments used to install the Service/daemon
-            (to make it easier to re-install) will be removed. Only used when removing the Service/daemon.
+        :param remove_install_args: if True, the file listing the arguments used to install
+            the Service/daemon (to make it easier to re-install) will be removed.
+            Only used when removing the Service/daemon.
         :type remove_install_args: bool, optional
-        :param remove_nssm: if True, the NSSM executable will be removed. Only used when removing the Service/daemon.
+        :param remove_nssm: if True, the NSSM executable will be removed.
+            Only used when removing the Service/daemon.
         :type remove_nssm: bool, optional
         """
-        if run_mode in ['start'] :
+        if run_mode in ["start"]:
             self.start_service()
-        if run_mode in ['status'] :
+        if run_mode in ["status"]:
             self.service_status()
-        if run_mode in ['stop','stop_and_remove','stop_and_reinstall','stop_and_restart'] :
+        if run_mode in [
+            "stop",
+            "stop_and_remove",
+            "stop_and_reinstall",
+            "stop_and_restart",
+        ]:
             self.stop_service()
-        if run_mode in ['remove','stop_and_remove','stop_and_reinstall','stop_and_restart'] :
-            self.remove_service(remove_env_vars=remove_env_vars,
-                                remove_install_args=remove_install_args,
-                                remove_nssm=remove_nssm)
-        if run_mode in ['reinstall','stop_and_reinstall','stop_and_restart'] :
+        if run_mode in [
+            "remove",
+            "stop_and_remove",
+            "stop_and_reinstall",
+            "stop_and_restart",
+        ]:
+            self.remove_service(
+                remove_env_vars=remove_env_vars,
+                remove_install_args=remove_install_args,
+                remove_nssm=remove_nssm,
+            )
+        if run_mode in ["reinstall", "stop_and_reinstall", "stop_and_restart"]:
             self.reinstall_service()
-        if run_mode in ['stop_and_restart'] :
+        if run_mode in ["stop_and_restart"]:
             self.start_service()
 
     @abstractmethod
-    def start_service(self) :
+    def start_service(self):
         """
         start the Service
         not implemented in the base class
         """
         raise NotImplementedError
 
     @abstractmethod
-    def service_status(self) :
+    def service_status(self):
         """
         get the status of the service
         not implemented in the base class
         """
         raise NotImplementedError
 
     @abstractmethod
-    def stop_service(self) :
+    def stop_service(self):
         """
         stop the Service
         not implemented in the base class
         """
         raise NotImplementedError
 
-    def remove_service(self,remove_env_vars=False,remove_install_args=False,remove_nssm=False) :
+    def remove_service(
+        self, remove_env_vars=False, remove_install_args=False, remove_nssm=False
+    ):
         """
         Remove the Service. Child classes should call this after doing whatever they need to do to
         optionally remove environment variables.
 
-        :param remove_env_vars: if True, any environment variables needed by the Service/daemon will be removed.
+        :param remove_env_vars: if True, any environment variables needed by the Service/daemon
+            will be removed.
         :type remove_env_vars: bool, optional.
-        :param remove_install_args: if True, the file listing the arguments used to install the Service/daemon
-            (to make it easier to re-install) will be removed.
+        :param remove_install_args: if True, the file listing the arguments used to install
+            the Service/daemon (to make it easier to re-install) will be removed.
         :type remove_install_args: bool, optional
         :param remove_nssm: if True, the NSSM executable will be removed. Only used on Windows.
         :type remove_nssm: bool, optional
         """
-        #remove the executable file
-        if self.exec_fp.is_file() :
+        # remove the executable file
+        if self.exec_fp.is_file():
             self.exec_fp.unlink()
-        #remove the environment variables that were set when the service was installed
-        if remove_env_vars :
-            try :
-                for env_var_name in self.env_var_names :
+        # remove the environment variables that were set when the service was installed
+        if remove_env_vars:
+            try:
+                for env_var_name in self.env_var_names:
                     remove_env_var(env_var_name)
-                    self.logger.info(f'{env_var_name} environment variable successfully removed')
-            except CalledProcessError :
-                warnmsg = 'WARNING: failed to remove environment variables. You should remove any username/password '
-                warnmsg+= 'environment variables manually even though the service is uninstalled!'
+                    self.logger.info(
+                        f"{env_var_name} environment variable successfully removed"
+                    )
+            except CalledProcessError:
+                warnmsg = (
+                    "WARNING: failed to remove environment variables. You should remove any "
+                    "username/password environment variables manually "
+                    "even though the service is uninstalled!"
+                )
                 self.logger.info(warnmsg)
-        else :
-            self.logger.info('Environment variables will be retained')
-        #remove the actual environment variable file
-        if self.env_var_filepath.is_file() :
+        else:
+            self.logger.info("Environment variables will be retained")
+        # remove the actual environment variable file
+        if self.env_var_filepath.is_file():
             self.env_var_filepath.unlink()
-        #remove the installation arguments file
-        if remove_install_args :
-            if self.install_args_filepath.is_file() :
+        # remove the installation arguments file
+        if remove_install_args:
+            if self.install_args_filepath.is_file():
                 self.install_args_filepath.unlink()
-                self.logger.info(f'Installation arguments file {self.install_args_filepath} deleted.')
-        else :
-            if self.install_args_filepath.is_file() :
-                self.logger.info(f'Installation arguments file {self.install_args_filepath} will be retained')
-        self.logger.info(f'Done removing {self.service_name}')
-        _ = remove_nssm # appease pyflakes / pylint
+                self.logger.info(
+                    f"Installation arguments file {self.install_args_filepath} deleted."
+                )
+        else:
+            if self.install_args_filepath.is_file():
+                self.logger.info(
+                    f"Installation arguments file {self.install_args_filepath} will be retained"
+                )
+        self.logger.info(f"Done removing {self.service_name}")
+        _ = remove_nssm  # appease pyflakes / pylint
 
-    def reinstall_service(self) :
+    def reinstall_service(self):
         """
         Install the service using the arguments defined in the service arguments file
         """
-        if not self.install_args_filepath.is_file() :
-            errmsg =  'ERROR: cannot reinstall service without an installation arguments file '
-            errmsg+= f'at {self.install_args_filepath}!'
-            self.logger.error(errmsg,exc_type=FileNotFoundError)
-        with open(self.install_args_filepath,'r') as fp :
+        if not self.install_args_filepath.is_file():
+            errmsg = (
+                f"ERROR: cannot reinstall service without an installation arguments file "
+                f"at {self.install_args_filepath}!"
+            )
+            self.logger.error(errmsg, exc_type=FileNotFoundError)
+        with open(self.install_args_filepath, "r") as fp:
             lines = fp.readlines()
-        if not len(lines)>0 :
-            errmsg = f'ERROR: installation arguments file {self.install_args_filepath} does not contain enough entries!'
-            self.logger.error(errmsg,exc_type=RuntimeError)
+        if not len(lines) > 0:
+            errmsg = (
+                f"ERROR: installation arguments file {self.install_args_filepath} "
+                "does not contain enough entries!"
+            )
+            self.logger.error(errmsg, exc_type=RuntimeError)
         self.service_spec_string = lines[0].strip()
         self.__set_service_dict()
-        self.argslist = [line.strip() for line in lines[1:]] if len(lines)>1 else []
-        if self.interactive :
-            msg = 'Running this reinstall would be like running the following from the command line:\n'
-            msg+= f'InstallService {self.service_spec_string} '
-            for arg in self.argslist :
-                msg+=f'{arg} '
-            msg+=f'--service_name {self.service_name}\n'
-            msg+='Does everything above look right? [(y)/n]: '
+        self.argslist = [line.strip() for line in lines[1:]] if len(lines) > 1 else []
+        if self.interactive:
+            msg = (
+                f"Running this reinstall would be like running the following from the "
+                f"command line:\nInstallService {self.service_spec_string} "
+            )
+            msg += " ".join(self.argslist)
+            msg += (
+                f" --service_name {self.service_name}\n"
+                "Does everything above look right? [(y)/n]: "
+            )
             check = input(msg)
-            if check.lower().startswith('n') :
-                msg = f'{self.service_name} will NOT be reinstalled. You can install it again by rerunning '
-                msg+= 'InstallService on its own.'
+            if check.lower().startswith("n"):
+                msg = (
+                    f"{self.service_name} will NOT be reinstalled. You can install it "
+                    "again by rerunning InstallService on its own."
+                )
                 self.logger.info(msg)
                 sys.exit(0)
-            else :
+            else:
                 self.install_service()
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
     @abstractmethod
-    def _write_env_var_file(self) :
+    def _write_env_var_file(self):
         """
-        Write and set permissions for the file holding the values of the environment variables needed by the Service
-        returns True if there are environment variables referenced, False if not
+        Write and set permissions for the file holding the values of the environment
+        variables needed by the Service
+
+        Returns True if there are environment variables referenced, False if not
 
         Not implemented in base class
         """
         raise NotImplementedError
 
-    def _write_install_args_file(self) :
+    def _write_install_args_file(self):
         """
         Write out a file storing the arguments used to install the Service so it can be
         reinstalled using the same configurations/setting if desired
         """
-        if self.service_spec_string is None or self.argslist is None :
-            errmsg = "ERROR: can't write the installation arguments file without a service_spec_string and argslist!"
-            self.logger.error(errmsg,exc_type=RuntimeError)
-        with open(self.install_args_filepath,'w') as fp :
-            for arg in [self.service_spec_string,*self.argslist] :
-                fp.write(f'{arg}\n')
+        if self.service_spec_string is None or self.argslist is None:
+            errmsg = (
+                "ERROR: can't write the installation arguments file without a "
+                "service_spec_string and argslist!"
+            )
+            self.logger.error(errmsg, exc_type=RuntimeError)
+        with open(self.install_args_filepath, "w") as fp:
+            for arg in [self.service_spec_string, *self.argslist]:
+                fp.write(f"{arg}\n")
 
-    def _write_executable_file(self,filepath=None) :
+    def _write_executable_file(self, filepath=None):
         """
         write out the executable python file that the service will actually be running
         """
-        error_log_path = pathlib.Path().resolve()/f'{self.service_name}{SERVICE_CONST.ERROR_LOG_STEM}'
-        code = '''\
+        error_log_path = (
+            pathlib.Path().resolve()
+            / f"{self.service_name}{SERVICE_CONST.ERROR_LOG_STEM}"
+        )
+        code = """\
             if __name__=='__main__' :
-                try :'''
-        if self.service_dict['func_name'] is not None :
-            code+=f'''
+                try :"""
+        if self.service_dict["func_name"] is not None:
+            code += f"""
                     from {self.service_dict['filepath']} import {self.service_dict['func_name']}
-                    {self.service_dict['func_name']}({self.argslist})'''
-        else :
-            code+=f'''
+                    {self.service_dict['func_name']}({self.argslist})"""
+        else:
+            code += f"""
                     from {self.service_dict['filepath']} import {self.service_dict['class_name']}
-                    {self.service_dict['class_name']}.run_from_command_line({self.argslist})'''
-        code+=f'''
+                    {self.service_dict['class_name']}.run_from_command_line({self.argslist})"""
+        code += f"""
                 except Exception :
                     import pathlib, traceback, datetime
                     output_filepath = pathlib.Path(r"{error_log_path}")
-                    with open(output_filepath,'a') as fp :'''
-        code+=r'''
-                        fp.write(f'{(datetime.datetime.now()).strftime("Error on %Y-%m-%d at %H:%M:%S")}. Exception:\n{traceback.format_exc()}')
+                    with open(output_filepath,'a') as fp :"""
+        code += r"""
+                        timestamp = (datetime.datetime.now()).strftime("%Y-%m-%d at %H:%M:%S")
+                        fp.write(f'Error on {timestamp}. Exception:\n{traceback.format_exc()}')
                     import sys
                     sys.exit(1)
-        '''
-        if filepath is not None :
-            warnmsg = f'WARNING: Services executable will be written to {filepath} instead of {self.exec_fp}'
+        """
+        if filepath is not None:
+            warnmsg = (
+                f"WARNING: Services executable will be written to {filepath} "
+                f"instead of {self.exec_fp}"
+            )
             self.logger.warning(warnmsg)
             exec_fp = filepath
-        else :
+        else:
             exec_fp = self.exec_fp
-        with open(exec_fp,'w') as fp :
+        with open(exec_fp, "w") as fp:
             fp.write(textwrap.dedent(code))
 
-    def __set_service_dict(self) :
+    def __set_service_dict(self):
         """
-        Set the service dict with information about the code that should be run based on the service_spec_string
+        Set the service dict with information about the code that should be run
+        based on the service_spec_string
         """
-        if self.service_spec_string is not None :
-            service_dict = [sd for sd in SERVICE_CONST.available_services
-                            if sd['class_name']==self.service_spec_string]
-            if len(service_dict)==1 :
+        if self.service_spec_string is not None:
+            service_dict = [
+                sd
+                for sd in SERVICE_CONST.available_services
+                if sd["class_name"] == self.service_spec_string
+            ]
+            if len(service_dict) == 1:
                 self.service_dict = service_dict[0]
-            elif len(service_dict)==0 :
-                f_p, c_n, r_c, f_n = self.__parse_custom_service_string(self.service_spec_string,self.logger)
-                self.service_dict = {'filepath':f_p,
-                                     'class_name':c_n,
-                                     'class':r_c,
-                                     'func_name':f_n}
-            else :
-                errmsg = f'ERROR: could not find the Service dictionary for {self.service_name} '
-                errmsg+= f'(a {self.service_spec_string} program)! service_dict = {service_dict}'
-                self.logger.error(errmsg,exc_type=RuntimeError)
-        else :
+            elif len(service_dict) == 0:
+                f_p, c_n, r_c, f_n = self.__parse_custom_service_string(
+                    self.service_spec_string, self.logger
+                )
+                self.service_dict = {
+                    "filepath": f_p,
+                    "class_name": c_n,
+                    "class": r_c,
+                    "func_name": f_n,
+                }
+            else:
+                errmsg = (
+                    f"ERROR: could not find the Service dictionary for {self.service_name} "
+                    f"(a {self.service_spec_string} program)! service_dict = {service_dict}"
+                )
+                self.logger.error(errmsg, exc_type=RuntimeError)
+        else:
             self.service_dict = None
 
     @staticmethod
-    def __parse_custom_service_string(service_spec_string,logger=SERVICE_CONST.logger) :
+    def __parse_custom_service_string(service_spec_string, logger=SERVICE_CONST.logger):
         """
         Get the filepath and optional class/function names from the custom Service string
         """
         filepath = None
         class_name = None
         run_class = None
         func_name = None
-        try :
-            #at minimum need a path to a file containing a class or function to run
-            if '=' in service_spec_string :
-                equals_split = service_spec_string.split('=')
-                assert len(equals_split)==2
+        try:
+            # at minimum need a path to a file containing a class or function to run
+            if "=" in service_spec_string:
+                equals_split = service_spec_string.split("=")
+                assert len(equals_split) == 2
                 class_name = equals_split[0]
                 for_path_and_func_name = equals_split[1]
-            else :
+            else:
                 class_name = None
                 for_path_and_func_name = service_spec_string
-            if ':' in service_spec_string :
-                colon_split = for_path_and_func_name.split(':')
-                assert len(colon_split)==2
+            if ":" in service_spec_string:
+                colon_split = for_path_and_func_name.split(":")
+                assert len(colon_split) == 2
                 filepath = colon_split[0]
                 func_name = colon_split[1]
-            else :
+            else:
                 filepath = for_path_and_func_name
             assert filepath is not None
-            #make sure the path is valid
+            # make sure the path is valid
             module = importlib.import_module(filepath)
             assert module is not None
-            #if the function name was specified, make sure that can be imported from the file, too
-            if func_name is not None :
-                function = getattr(module,func_name)
+            # if the function name was specified, make sure that can be imported from the file, too
+            if func_name is not None:
+                function = getattr(module, func_name)
                 assert function is not None
-            #If the class name was given without a function name, make sure the class can be imported from the file
-            elif class_name is not None and func_name is None :
-                run_class = getattr(module,class_name)
-                #and make sure the class extends Runnable, since we'll be calling its run_from_command_line function
-                assert issubclass(run_class,Runnable)
-            #make sure at least one of the function/class names was given
-            assert ((func_name is not None) or ((class_name is not None) and (run_class is not None)))
-        except Exception as exc :
-            errmsg = f'ERROR: service specification string {service_spec_string} is not valid! '
-            errmsg+= 'Will re-raise specific Exception.'
-            logger.error(errmsg,exc_info=exc,reraise=True)
+            # If the class name was given without a function name,
+            # make sure the class can be imported from the file
+            elif class_name is not None and func_name is None:
+                run_class = getattr(module, class_name)
+                # and make sure the class extends Runnable,
+                # since we'll be calling its run_from_command_line function
+                assert issubclass(run_class, Runnable)
+            # make sure at least one of the function/class names was given
+            assert (func_name is not None) or (
+                (class_name is not None) and (run_class is not None)
+            )
+        except Exception as exc:
+            errmsg = (
+                f"ERROR: service specification string {service_spec_string} is not valid! "
+                "Will re-raise specific Exception."
+            )
+            logger.error(errmsg, exc_info=exc, reraise=True)
         return filepath, class_name, run_class, func_name
 
     #################### CLASS METHODS ####################
 
     @classmethod
-    def get_argument_parser(cls,install_or_manage=None,class_name_or_spec_string=None) :
+    def get_argument_parser(cls, install_or_manage=None, class_name_or_spec_string=None):
         """
         Return the command line argument parser that should be used
 
         :param install_or_manage: Whether the parser used should accept commands for "install"-ing
             or "manage"-ing the Service/daemon
         :type install_or_manage: str
-        :param class_name_or_spec_string: the first argument to the install script, if that's being run.
-            Used to add subparsers for known Runnable classes or for custom Runnables defined at the time
-            the Service/daemon is being installed.
+        :param class_name_or_spec_string: the first argument to the install script,
+            if that's being run. Used to add subparsers for known Runnable classes or for
+            custom Runnables defined at the time the Service/daemon is being installed.
         :type class_name_or_spec_string: str, optional
 
         :return: the :class:`~.utilities.OpenMSIStreamArgumentParser` object that should be used
         :rtype: :class:`~.utilities.OpenMSIStreamArgumentParser`
 
         :raises ValueError: if `install_or_manage` is neither "install" nor "manage"
         """
         parser = OpenMSIStreamArgumentParser()
-        if install_or_manage=='install' :
-            #subparsers from the classes that could be run
-            subp_desc = 'The name of a "Runnable" class (or the specification for a custom Service code) to install '
-            subp_desc = 'as a service must be given as the first argument. Adding the name (or spec string) of a class '
-            subp_desc = 'that extends "Runnable" to the command line along with "-h" will show additional help.'
-            if class_name_or_spec_string in ('--help','-h') :
+        if install_or_manage == "install":
+            # subparsers from the classes that could be run
+            subp_desc = (
+                'The name of a "Runnable" class (or the specification for a custom Service code) '
+                "to install as a service must be given as the first argument. Adding the name "
+                '(or spec string) of a class that extends "Runnable" to the command line '
+                'along with "-h" will show additional help.'
+            )
+            if class_name_or_spec_string in ("--help", "-h"):
                 return parser
-            parser.add_subparsers(description=subp_desc,required=True,dest='service_spec_string')
-            if class_name_or_spec_string is None :
-                for service_dict in SERVICE_CONST.available_services :
-                    parser.add_subparser_arguments_from_class(service_dict['class'],addl_args=['optional_service_name'])
-            elif class_name_or_spec_string in [d['class_name'] for d in SERVICE_CONST.available_services] :
-                sds = [sd for sd in SERVICE_CONST.available_services if sd['class_name']==class_name_or_spec_string]
+            parser.add_subparsers(
+                description=subp_desc, required=True, dest="service_spec_string"
+            )
+            if class_name_or_spec_string is None:
+                for service_dict in SERVICE_CONST.available_services:
+                    parser.add_subparser_arguments_from_class(
+                        service_dict["class"], addl_args=["optional_service_name"]
+                    )
+            elif class_name_or_spec_string in [
+                d["class_name"] for d in SERVICE_CONST.available_services
+            ]:
+                sds = [
+                    sd
+                    for sd in SERVICE_CONST.available_services
+                    if sd["class_name"] == class_name_or_spec_string
+                ]
                 s_d = sds[0]
-                parser.add_subparser_arguments_from_class(s_d['class'],addl_args=['optional_service_name'])
-            else :
-                _, _, run_class, _ = cls.__parse_custom_service_string(class_name_or_spec_string)
-                if run_class is not None :
-                    parser.add_subparser_arguments_from_class(run_class,
-                                                              subp_name=class_name_or_spec_string,
-                                                              addl_args=['optional_service_name'])
-                else :
-                    parser.add_subparser_arguments(class_name_or_spec_string,['optional_service_name'])
-        elif install_or_manage=='manage' :
-            parser.add_arguments('service_name','run_mode','remove_env_vars','remove_install_args','remove_nssm')
-        else :
-            errmsg =  'ERROR: must call get_argument_parser with either "install" or "manage", '
-            errmsg+= f'not "{install_or_manage}"!'
+                parser.add_subparser_arguments_from_class(
+                    s_d["class"], addl_args=["optional_service_name"]
+                )
+            else:
+                _, _, run_class, _ = cls.__parse_custom_service_string(
+                    class_name_or_spec_string
+                )
+                if run_class is not None:
+                    parser.add_subparser_arguments_from_class(
+                        run_class,
+                        subp_name=class_name_or_spec_string,
+                        addl_args=["optional_service_name"],
+                    )
+                else:
+                    parser.add_subparser_arguments(
+                        class_name_or_spec_string, ["optional_service_name"]
+                    )
+        elif install_or_manage == "manage":
+            parser.add_arguments(
+                "service_name",
+                "run_mode",
+                "remove_env_vars",
+                "remove_install_args",
+                "remove_nssm",
+            )
+        else:
+            errmsg = (
+                f'ERROR: must call get_argument_parser with either "install" or "manage", '
+                f'not "{install_or_manage}"!'
+            )
             raise ValueError(errmsg)
         return parser
 
     #################### PROPERTIES ####################
 
     @property
-    def env_var_names(self) :
+    def env_var_names(self):
         """
         Names of the environment variables used by the service
         (any environment variables in the command line arguments or config file)
         """
-        #get the names of environment variables from the command line and config file
+        # get the names of environment variables from the command line and config file
         env_var_names = set()
-        if self.argslist is not None and self.service_dict is not None :
-            for arg in self.argslist :
-                if arg.startswith('$') :
+        if self.argslist is not None and self.service_dict is not None:
+            for arg in self.argslist:
+                if arg.startswith("$"):
                     env_var_names.add(arg)
-            if self.service_dict['class'] is not None :
-                parser = self.service_dict['class'].get_argument_parser()
+            if self.service_dict["class"] is not None:
+                parser = self.service_dict["class"].get_argument_parser()
                 argsdests = [action.dest for action in parser.actions]
-                if 'config' in argsdests :
+                if "config" in argsdests:
                     pargs = parser.parse_args(args=self.argslist)
-                    cfp = ConfigFileParser(pargs.config,logger=SERVICE_CONST.logger)
-                    for evn in cfp.env_var_names :
+                    cfp = ConfigFileParser(pargs.config, logger=SERVICE_CONST.logger)
+                    for evn in cfp.env_var_names:
                         env_var_names.add(evn)
         return env_var_names
```

### Comparing `openmsistream-1.3.4/openmsistream/services/windows_service_manager.py` & `openmsistream-1.4.0/openmsistream/services/windows_service_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,220 +1,293 @@
 """Manage Windows Services"""
 
-#imports
+# imports
 import sys, os, pathlib, shutil, ctypes.util
 from subprocess import CalledProcessError
 from ..utilities.misc import change_dir
 from .config import SERVICE_CONST
 from .utilities import run_cmd_in_subprocess
 from .service_manager_base import ServiceManagerBase
 
-class WindowsServiceManager(ServiceManagerBase) :
+
+class WindowsServiceManager(ServiceManagerBase):
     """
     Base class for working with Windows Services
 
     :param service_name: The name of the Service as installed
     :type service_name: str
     :param service_spec_string: A string specifying which code should be run as a Service.
         Could be the name of an OpenMSIStream Runnable class, or the path to a custom Python code.
         Custom Services can also specify a :class:`~.utilities.Runnable` class name,
-        and/or a function in the file using special formatting like [class_name]=[path.to.file]:[function_name].
-        Only needed to initially install the Service.
+        and/or a function in the file using special formatting like
+        [class_name]=[path.to.file]:[function_name]. Only needed to initially install the Service.
     :type service_spec_string: str, optional
     :param argslist: The list of arguments (as from the command line) to pass to the
         :class:`~.utilities.Runnable` class.
         Only needed to initially install the Service.
     :type argslist: list, optional
     :param interactive: if True, a few more messages/prompts will come up telling a user what to do
     :type interactive: bool, optional
     """
 
     @property
     def env_var_names(self):
         env_var_names = super().env_var_names
-        #get the names of environment variables from the env_var file
-        if self.env_var_filepath.is_file() :
-            with open(self.env_var_filepath,'r') as fp :
+        # get the names of environment variables from the env_var file
+        if self.env_var_filepath.is_file():
+            with open(self.env_var_filepath, "r") as fp:
                 lines = fp.readlines()
-            for line in lines :
+            for line in lines:
                 linestrip = line.strip()
-                if linestrip!='' :
+                if linestrip != "":
                     env_var_names.add(linestrip)
-        for evn in env_var_names :
+        for evn in env_var_names:
             yield evn
 
-    def install_service(self) :
+    def install_service(self):
         """
         Install the Service
         """
         super().install_service()
-        #if it doesn't exist there yet, copy the libsodium.dll file to C:\Windows\system32
+        # if it doesn't exist there yet, copy the libsodium.dll file to C:\Windows\system32
         self.__copy_lib_dlls_to_system32()
-        #find or install NSSM to run the executable
+        # find or install NSSM to run the executable
         self.__find_install_nssm()
-        #run NSSM to install the service
-        with change_dir(SERVICE_CONST.NSSM_PATH.parent) :
-            cmd = f'./{SERVICE_CONST.NSSM_PATH.name} install {self.service_name} "{sys.executable}" '
-            if ' ' in str(self.exec_fp) :
-                cmd+= f'"\""""{self.exec_fp}\"""'
-            else :
-                cmd+= f'\"{self.exec_fp}\"'
-            run_cmd_in_subprocess(['powershell.exe',cmd],logger=self.logger)
-            cmd = f'./{SERVICE_CONST.NSSM_PATH.name} set {self.service_name} DisplayName {self.service_name}'
-            run_cmd_in_subprocess(['powershell.exe',cmd],logger=self.logger)
-            cmd = f'./{SERVICE_CONST.NSSM_PATH.name} set {self.service_name} DependOnService "Network Connections"'
-            run_cmd_in_subprocess(['powershell.exe',cmd],logger=self.logger)
-        self.logger.info(f'Done installing {self.service_name}')
+        # run NSSM to install the service
+        with change_dir(SERVICE_CONST.NSSM_PATH.parent):
+            cmd = (
+                f"./{SERVICE_CONST.NSSM_PATH.name} install "
+                f'{self.service_name} "{sys.executable}" '
+            )
+            if " " in str(self.exec_fp):
+                cmd += f'"""""{self.exec_fp}"""'
+            else:
+                cmd += f'"{self.exec_fp}"'
+            run_cmd_in_subprocess(["powershell.exe", cmd], logger=self.logger)
+            cmd = (
+                f"./{SERVICE_CONST.NSSM_PATH.name} set {self.service_name} "
+                f"DisplayName {self.service_name}"
+            )
+            run_cmd_in_subprocess(["powershell.exe", cmd], logger=self.logger)
+            cmd = (
+                f"./{SERVICE_CONST.NSSM_PATH.name} set {self.service_name} "
+                'DependOnService "Network Connections"'
+            )
+            run_cmd_in_subprocess(["powershell.exe", cmd], logger=self.logger)
+        self.logger.info(f"Done installing {self.service_name}")
 
-    def start_service(self) :
+    def start_service(self):
         """
         Start the Service
         """
-        self.logger.info(f'Starting {self.service_name}...')
-        #start the service using net
-        cmds = ['powershell.exe',f'net start {self.service_name}']
-        run_cmd_in_subprocess(cmds,logger=self.logger)
-        self.logger.info(f'Done starting {self.service_name}')
+        self.logger.info(f"Starting {self.service_name}...")
+        # start the service using net
+        cmds = ["powershell.exe", f"net start {self.service_name}"]
+        run_cmd_in_subprocess(cmds, logger=self.logger)
+        self.logger.info(f"Done starting {self.service_name}")
 
-    def service_status(self) :
+    def service_status(self):
         """
         Print the status of the Service
         """
-        #find or install NSSM in the current directory
+        # find or install NSSM in the current directory
         self.__find_install_nssm()
-        #get the service status
-        with change_dir(SERVICE_CONST.NSSM_PATH.parent) :
-            cmds = ['powershell.exe',f'./{SERVICE_CONST.NSSM_PATH.name} status {self.service_name}']
-            result = run_cmd_in_subprocess(cmds,logger=self.logger)
-        self.logger.info(f'{self.service_name} status: {result.decode()}')
+        # get the service status
+        with change_dir(SERVICE_CONST.NSSM_PATH.parent):
+            cmds = [
+                "powershell.exe",
+                f"./{SERVICE_CONST.NSSM_PATH.name} status {self.service_name}",
+            ]
+            result = run_cmd_in_subprocess(cmds, logger=self.logger)
+        self.logger.info(f"{self.service_name} status: {result.decode()}")
 
-    def stop_service(self) :
+    def stop_service(self):
         """
         Stop the Service
         """
-        self.logger.info(f'Stopping {self.service_name}...')
-        #stop the service using net
-        cmds = ['powershell.exe',f'net stop {self.service_name}']
-        run_cmd_in_subprocess(cmds,logger=self.logger)
-        self.logger.info(f'Done stopping {self.service_name}')
-
-    def remove_service(self,remove_env_vars=False,remove_install_args=False,remove_nssm=False) :
+        self.logger.info(f"Stopping {self.service_name}...")
+        # stop the service using net
+        cmds = ["powershell.exe", f"net stop {self.service_name}"]
+        run_cmd_in_subprocess(cmds, logger=self.logger)
+        self.logger.info(f"Done stopping {self.service_name}")
+
+    def remove_service(
+        self, remove_env_vars=False, remove_install_args=False, remove_nssm=False
+    ):
         """
         Remove the Service
 
-        :param remove_env_vars: if True, any environment variables needed by the Service will be removed.
+        :param remove_env_vars: if True, any environment variables needed by the Service
+            will be removed.
         :type remove_env_vars: bool, optional.
-        :param remove_install_args: if True, the file listing the arguments used to install the Service
-            (to make it easier to re-install) will be removed.
+        :param remove_install_args: if True, the file listing the arguments used to
+            install the Service (to make it easier to re-install) will be removed.
         :type remove_install_args: bool, optional
         :param remove_nssm: if True, the NSSM executable will be removed.
         :type remove_nssm: bool, optional
         """
-        self.logger.info(f'Removing {self.service_name}...')
-        #find or install NSSM in the current directory
+        self.logger.info(f"Removing {self.service_name}...")
+        # find or install NSSM in the current directory
         self.__find_install_nssm()
-        #using NSSM
-        with change_dir(SERVICE_CONST.NSSM_PATH.parent) :
-            cmds = ['powershell.exe',f'./{SERVICE_CONST.NSSM_PATH.name} remove {self.service_name} confirm']
-            run_cmd_in_subprocess(cmds,logger=self.logger)
-        self.logger.info('Service removed')
-        #remove NSSM if requested
-        if remove_nssm :
-            if SERVICE_CONST.NSSM_PATH.is_file() :
-                try :
-                    run_cmd_in_subprocess(['powershell.exe',f'del "{SERVICE_CONST.NSSM_PATH}"'],logger=self.logger)
-                except CalledProcessError :
-                    msg = f'WARNING: failed to delete {SERVICE_CONST.NSSM_PATH}. '
-                    msg+= 'You are free to delete it manually if you would like.'
-                    self.logger.info(msg)
-            else :
-                msg = f'NSSM does not exist at {SERVICE_CONST.NSSM_PATH} so it will not be removed'
+        # using NSSM
+        with change_dir(SERVICE_CONST.NSSM_PATH.parent):
+            cmds = [
+                "powershell.exe",
+                f"./{SERVICE_CONST.NSSM_PATH.name} remove {self.service_name} confirm",
+            ]
+            run_cmd_in_subprocess(cmds, logger=self.logger)
+        self.logger.info("Service removed")
+        # remove NSSM if requested
+        if remove_nssm:
+            if SERVICE_CONST.NSSM_PATH.is_file():
+                try:
+                    run_cmd_in_subprocess(
+                        ["powershell.exe", f'del "{SERVICE_CONST.NSSM_PATH}"'],
+                        logger=self.logger,
+                    )
+                except CalledProcessError:
+                    msg = (
+                        f"WARNING: failed to delete {SERVICE_CONST.NSSM_PATH}. "
+                        "You are free to delete it manually if you would like."
+                    )
+                    self.logger.warning(msg)
+            else:
+                msg = f"NSSM does not exist at {SERVICE_CONST.NSSM_PATH} so it will not be removed"
                 self.logger.info(msg)
-        else :
-            if SERVICE_CONST.NSSM_PATH.is_file() :
-                msg = f'NSSM executable at {SERVICE_CONST.NSSM_PATH} will be retained'
+        else:
+            if SERVICE_CONST.NSSM_PATH.is_file():
+                msg = f"NSSM executable at {SERVICE_CONST.NSSM_PATH} will be retained"
                 self.logger.info(msg)
-        super().remove_service(remove_env_vars=remove_env_vars,remove_install_args=remove_install_args)
-
-    def _write_env_var_file(self) :
-        code = ''
-        for evn in self.env_var_names :
-            val = os.path.expandvars(f'${evn}')
-            if val==f'${evn}' :
-                raise RuntimeError(f'ERROR: value not found for expected environment variable {evn}!')
-            code += f'{evn}\n'
-        if code=='' :
+        super().remove_service(
+            remove_env_vars=remove_env_vars, remove_install_args=remove_install_args
+        )
+
+    def _write_env_var_file(self):
+        code = ""
+        for evn in self.env_var_names:
+            val = os.path.expandvars(f"${evn}")
+            if val == f"${evn}":
+                raise RuntimeError(
+                    f"ERROR: value not found for expected environment variable {evn}!"
+                )
+            code += f"{evn}\n"
+        if code == "":
             return False
-        with open(self.env_var_filepath,'w') as fp :
+        with open(self.env_var_filepath, "w") as fp:
             fp.write(code)
         return True
 
-    def __copy_lib_dlls_to_system32(self) :
+    def __copy_lib_dlls_to_system32(self):
         """
         Ensure that several .dll files exist in C:\\Windows\\system32
         (Needed to properly load it when running as a service)
         """
-        system32_path = pathlib.Path(r'C:\Windows\system32')
-        package_names = ['librdkafka-a2007a74','librdkafka-09f4f3ec',
-                         'libcrypto-1_1-x64-6d3f430c','libcurl-40bef7bc','libssl-1_1-x64-a125c0ba',
-                         'zlib1-50deb1cb','zstd-acd7910e',
-                         'libcrypto-1_1-x64','libssl-1_1-x64',
-                         'libsodium']
-        for pname in package_names :
+        system32_path = pathlib.Path(r"C:\Windows\system32")
+        package_names = [
+            "librdkafka-a2007a74",
+            "librdkafka-09f4f3ec",
+            "libcrypto-1_1-x64-6d3f430c",
+            "libcurl-40bef7bc",
+            "libssl-1_1-x64-a125c0ba",
+            "zlib1-50deb1cb",
+            "zstd-acd7910e",
+            "libcrypto-1_1-x64",
+            "libssl-1_1-x64",
+            "libsodium",
+        ]
+        for pname in package_names:
             current_env_dll = ctypes.util.find_library(pname)
-            if current_env_dll is not None :
+            if current_env_dll is not None:
                 current_env_dll_path = pathlib.Path(current_env_dll)
-                if (system32_path/current_env_dll_path.name).is_file() :
+                if (system32_path / current_env_dll_path.name).is_file():
                     continue
-                try :
-                    shutil.copy(current_env_dll_path,system32_path/current_env_dll_path.name)
-                except Exception as exc :
-                    warnmsg = f'WARNING: failed to copy {pname} DLL file from {current_env_dll_path} to '
-                    warnmsg+= f'{system32_path}. This will likely cause the Python code running as a Service '
-                    warnmsg+=  'to crash. Exception will be logged below, but not reraised.'
-                    self.logger.warning(warnmsg,exc_info=exc)
+                try:
+                    shutil.copy(
+                        current_env_dll_path, system32_path / current_env_dll_path.name
+                    )
+                except Exception as exc:
+                    warnmsg = (
+                        f"WARNING: failed to copy {pname} DLL file from {current_env_dll_path} "
+                        f"to {system32_path}. This will likely cause the Python code "
+                        "running as a Service to crash. "
+                        "Exception will be logged below, but not reraised."
+                    )
+                    self.logger.warning(warnmsg, exc_info=exc)
 
-    def __find_install_nssm(self,move_local=True) :
+    def __find_install_nssm(self, move_local=True):
         """
         Ensure the NSSM executable exists in the expected location.
         If it exists in the current directory, move it to the expected location.
-        If it doesn't exist anywhere, try to download it from the web, but that's finicky in powershell.
+        If it doesn't exist anywhere, try to download it from the web,
+        but that's finicky in powershell.
         """
-        if SERVICE_CONST.NSSM_PATH.is_file() :
+        if SERVICE_CONST.NSSM_PATH.is_file():
             return
-        if (pathlib.Path()/SERVICE_CONST.NSSM_PATH.name).is_file() and move_local :
-            (pathlib.Path()/SERVICE_CONST.NSSM_PATH.name).replace(SERVICE_CONST.NSSM_PATH)
+        if (pathlib.Path() / SERVICE_CONST.NSSM_PATH.name).is_file() and move_local:
+            (pathlib.Path() / SERVICE_CONST.NSSM_PATH.name).replace(
+                SERVICE_CONST.NSSM_PATH
+            )
             self.__find_install_nssm(move_local=False)
-        SERVICE_CONST.logger.info(f'Installing NSSM from {SERVICE_CONST.NSSM_DOWNLOAD_URL}...')
-        nssm_zip_file_name = SERVICE_CONST.NSSM_DOWNLOAD_URL.rsplit('/', maxsplit=1)[-1]
-        run_cmd_in_subprocess(['powershell.exe',
-                                '[Net.ServicePointManager]::SecurityProtocol=[Net.SecurityProtocolType]::Tls12'],
-                                logger=self.logger)
+        SERVICE_CONST.logger.info(
+            f"Installing NSSM from {SERVICE_CONST.NSSM_DOWNLOAD_URL}..."
+        )
+        nssm_zip_file_name = SERVICE_CONST.NSSM_DOWNLOAD_URL.rsplit("/", maxsplit=1)[-1]
+        run_cmd_in_subprocess(
+            [
+                "powershell.exe",
+                "[Net.ServicePointManager]::SecurityProtocol=[Net.SecurityProtocolType]::Tls12",
+            ],
+            logger=self.logger,
+        )
+        nssm_path = (
+            pathlib.Path() / nssm_zip_file_name.rstrip(".zip") / "win64" / "nssm.exe"
+        )
         cmd_tuples = [
-            (('curl',f'{SERVICE_CONST.NSSM_DOWNLOAD_URL}','-O'),
-             f'Invoke-WebRequest -Uri {SERVICE_CONST.NSSM_DOWNLOAD_URL} -OutFile {nssm_zip_file_name}'),
-            (('tar','-xf',f'"{pathlib.Path() / nssm_zip_file_name}"'),
-             f'Expand-Archive {nssm_zip_file_name} -DestinationPath "{pathlib.Path().resolve()}"'),
-            (('del',f'{nssm_zip_file_name}'),
-             f'Remove-Item -Path {nssm_zip_file_name}'),
-            (('move',f'"{pathlib.Path()/nssm_zip_file_name.rstrip(".zip")/"win64"/"nssm.exe"}"',
-              f'"{pathlib.Path()}"'),
-             f'''Move-Item -Path "{pathlib.Path()/nssm_zip_file_name.rstrip(".zip")/"win64"/"nssm.exe"}"
-                 -Destination "{SERVICE_CONST.NSSM_PATH}"'''),
-            (('rmdir','/S','/Q',f'{nssm_zip_file_name.rstrip(".zip")}'),
-             f'Remove-Item -Recurse -Force {nssm_zip_file_name.rstrip(".zip")}'),
+            (
+                ("curl", f"{SERVICE_CONST.NSSM_DOWNLOAD_URL}", "-O"),
+                (
+                    f"Invoke-WebRequest -Uri {SERVICE_CONST.NSSM_DOWNLOAD_URL} "
+                    f"-OutFile {nssm_zip_file_name}"
+                ),
+            ),
+            (
+                ("tar", "-xf", f'"{pathlib.Path() / nssm_zip_file_name}"'),
+                (
+                    f"Expand-Archive {nssm_zip_file_name} "
+                    f'-DestinationPath "{pathlib.Path().resolve()}"'
+                ),
+            ),
+            (("del", f"{nssm_zip_file_name}"), f"Remove-Item -Path {nssm_zip_file_name}"),
+            (
+                (
+                    "move",
+                    f'"{nssm_path}"',
+                    f'"{pathlib.Path()}"',
+                ),
+                (
+                    f'Move-Item -Path "{nssm_path}"'
+                    f'-Destination "{SERVICE_CONST.NSSM_PATH}"',
+                ),
+            ),
+            (
+                ("rmdir", "/S", "/Q", f'{nssm_zip_file_name.rstrip(".zip")}'),
+                f'Remove-Item -Recurse -Force {nssm_zip_file_name.rstrip(".zip")}',
+            ),
         ]
-        try :
-            for cmd in cmd_tuples :
-                try :
-                    run_cmd_in_subprocess(['powershell.exe',cmd[1]],logger=self.logger)
-                except CalledProcessError :
-                    run_cmd_in_subprocess(list(cmd[0]),shell=True,logger=self.logger)
-        except CalledProcessError :
+        try:
+            for cmd in cmd_tuples:
+                try:
+                    run_cmd_in_subprocess(["powershell.exe", cmd[1]], logger=self.logger)
+                except CalledProcessError:
+                    run_cmd_in_subprocess(list(cmd[0]), shell=True, logger=self.logger)
+        except CalledProcessError:
             pass
-        if SERVICE_CONST.NSSM_PATH.is_file() :
-            SERVICE_CONST.logger.debug('Done installing NSSM')
-        else :
-            errmsg =  'ERROR: failed to install NSSM automatically. Please download NSSM from '
-            errmsg+= f'{SERVICE_CONST.NSSM_DOWNLOAD_URL}, put the executable in the current directory '
-            errmsg+= f'or in {SERVICE_CONST.NSSM_PATH.parent}, and try again.'
+        if SERVICE_CONST.NSSM_PATH.is_file():
+            SERVICE_CONST.logger.debug("Done installing NSSM")
+        else:
+            errmsg = (
+                f"ERROR: failed to install NSSM automatically. "
+                f"Please download NSSM from {SERVICE_CONST.NSSM_DOWNLOAD_URL}, "
+                f"put the executable in the current directory or in "
+                f"{SERVICE_CONST.NSSM_PATH.parent}, and try again."
+            )
             SERVICE_CONST.logger.error(errmsg)
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/config.py` & `openmsistream-1.4.0/openmsistream/utilities/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """Constants used in running different controlled processes in general"""
 
-#imports
+# imports
 import os, pathlib
 
-class RunConstants :
+
+class RunConstants:
     """
     Constants used for running controlled processes, reading config files, etc.
     """
 
-    CONFIG_FILE_EXT = '.config'
-    CONFIG_FILE_DIR = ( os.environ['OPENMSISTREAM_CONFIG_FILE_DIR']
-                        if 'OPENMSISTREAM_CONFIG_FILE_DIR' in os.environ else
-                        (pathlib.Path(__file__).parent.parent / 'kafka_wrapper' / 'config_files').resolve() )
+    CONFIG_FILE_EXT = ".config"
+    CONFIG_FILE_DIR = (
+        os.environ["OPENMSISTREAM_CONFIG_FILE_DIR"]
+        if "OPENMSISTREAM_CONFIG_FILE_DIR" in os.environ
+        else (
+            pathlib.Path(__file__).parent.parent / "kafka_wrapper" / "config_files"
+        ).resolve()
+    )
     DEFAULT_N_THREADS = 2
     DEFAULT_UPDATE_SECONDS = 300
 
+
 RUN_CONST = RunConstants()
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/config_file_parser.py` & `openmsistream-1.4.0/openmsistream/utilities/config_file_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,94 @@
 """Wrapper around a Python ConfigParser to simplify some commonly-used operations"""
 
-#imports
+# imports
 import os, configparser
 from .logging import LogOwner
 
-class ConfigFileParser(LogOwner) :
+
+class ConfigFileParser(LogOwner):
     """
     A class to parse configurations from files
     """
 
     #################### PROPERTIES ####################
 
     @property
-    def has_default(self) :
+    def has_default(self):
         """
         True if a config file has a DEFAULT section
         """
-        return 'DEFAULT' in self._config
+        return "DEFAULT" in self._config
+
     @property
-    def available_group_names(self) :
+    def available_group_names(self):
         """
         The list of section names in the config file
         """
         return self._config.sections()
+
     @property
-    def env_var_names(self) :
+    def env_var_names(self):
         """
         A generator of the environment variable names used in the config file
         """
-        for csd in self._config.values() :
-            for v in csd.values() :
-                if v.startswith('$') :
+        for csd in self._config.values():
+            for v in csd.values():
+                if v.startswith("$"):
                     yield v[1:]
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,config_path,*args,**kwargs) :
+    def __init__(self, config_path, *args, **kwargs):
         """
         config_path = path to the config file to parse
         """
-        super().__init__(*args,**kwargs)
+        super().__init__(*args, **kwargs)
         self.filepath = config_path
-        if not config_path.is_file() :
-            self.logger.error(f'ERROR: configuration file {config_path} does not exist!',exc_type=FileNotFoundError)
+        if not config_path.is_file():
+            self.logger.error(
+                f"ERROR: configuration file {config_path} does not exist!",
+                exc_type=FileNotFoundError,
+            )
         self._config = configparser.ConfigParser()
         self._config.read(config_path)
 
-    def get_config_dict_for_groups(self,group_names) :
+    def get_config_dict_for_groups(self, group_names):
         """
         Return a config dictionary populated with configurations from groups with the given names
 
         group_names = the list of group names to add to the dictionary (or a single string)
         """
-        if isinstance(group_names,str) :
+        if isinstance(group_names, str):
             group_names = [group_names]
         config_dict = {}
-        for group_name in group_names :
-            if group_name not in self._config :
-                errmsg = f'ERROR: {group_name} is not a recognized section in {self.filepath}!'
-                self.logger.error(errmsg,exc_type=ValueError)
-            for key, value in self._config[group_name].items() :
-                #don't add the 'node_id' to groups for brokers, producers, or consumers
-                if key=='node_id' and group_name in ['broker','producer','consumer'] :
+        for group_name in group_names:
+            if group_name not in self._config:
+                errmsg = (
+                    f"ERROR: {group_name} is not a recognized section in {self.filepath}!"
+                )
+                self.logger.error(errmsg, exc_type=ValueError)
+            for key, value in self._config[group_name].items():
+                # don't add the 'node_id' to groups for brokers, producers, or consumers
+                if key == "node_id" and group_name in ["broker", "producer", "consumer"]:
                     continue
-                #if the value is an environment variable, expand it on the current system
-                if value.startswith('$') :
+                # if the value is an environment variable, expand it on the current system
+                if value.startswith("$"):
                     exp_value = os.path.expandvars(value)
-                    if exp_value == value :
-                        errmsg = f'ERROR: Expanding {value} in {self.filepath} as an environment variable failed '
-                        errmsg+= '(must be set on system)'
-                        self.logger.error(errmsg,exc_type=ValueError)
-                    else :
+                    if exp_value == value:
+                        errmsg = (
+                            f"ERROR: Expanding {value} in {self.filepath} as an environment "
+                            "variable failed (must be set on system)"
+                        )
+                        self.logger.error(errmsg, exc_type=ValueError)
+                    else:
                         value = exp_value
                 config_dict[key] = value
         return config_dict
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def _get_config_dict(self,group_name) :
+    def _get_config_dict(self, group_name):
         to_return = {}
-        if group_name in self.available_group_names :
+        if group_name in self.available_group_names:
             to_return = self.get_config_dict_for_groups(group_name)
         return to_return
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/controlled_process.py` & `openmsistream-1.4.0/openmsistream/utilities/controlled_process.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,107 +1,117 @@
 """
 A process that will run while waiting for user input to check progress/status or shut it down
 """
 
-#imports
+# imports
 import datetime
 from queue import Queue, Empty
 from threading import Thread
 from abc import ABC, abstractmethod
 from ..utilities.misc import add_user_input
 from ..utilities.logging import LogOwner
 from .config import RUN_CONST
 
-class ControlledProcess(LogOwner,ABC) :
+
+class ControlledProcess(LogOwner, ABC):
     """
-    A class to use when running processes that should remain active until they are explicitly shut down
+    A class to use when running processes that should remain active until they are
+    explicitly shut down
 
-    :param update_secs: number of seconds to wait between printing a progress character to the console
-        to indicate the program is alive
+    :param update_secs: number of seconds to wait between printing a progress character
+        to the console to indicate the program is alive
     :type update_secs: int, optional
     """
 
     #################### PROPERTIES ####################
 
     @property
-    def alive(self) :
+    def alive(self):
         """
         Read-only boolean indicating if the process is running
         """
         return self.__alive
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,*args,update_secs=RUN_CONST.DEFAULT_UPDATE_SECONDS,**other_kwargs) :
+    def __init__(
+        self, *args, update_secs=RUN_CONST.DEFAULT_UPDATE_SECONDS, **other_kwargs
+    ):
         self.__update_secs = update_secs
-        #start up a Queue that will hold the control commands
+        # start up a Queue that will hold the control commands
         self.control_command_queue = Queue()
-        #use a daemon thread to allow a user to input control commands from the command line
-        #while the process is running
-        user_input_thread = Thread(target=add_user_input,args=(self.control_command_queue,))
-        user_input_thread.daemon=True
+        # use a daemon thread to allow a user to input control commands from the command line
+        # while the process is running
+        user_input_thread = Thread(
+            target=add_user_input, args=(self.control_command_queue,)
+        )
+        user_input_thread.daemon = True
         user_input_thread.start()
-        #a variable to indicate if the process has been shut down yet
+        # a variable to indicate if the process has been shut down yet
         self.__alive = False
-        #the last time the "still alive" character was printed
+        # the last time the "still alive" character was printed
         self.__last_update = datetime.datetime.now()
-        super().__init__(*args,**other_kwargs)
+        super().__init__(*args, **other_kwargs)
 
-    def shutdown(self) :
+    def shutdown(self):
         """
         Stop the process running.
         """
         self.control_command_queue.task_done()
         self.__alive = False
         self._on_shutdown()
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def _print_still_alive(self) :
-        #print the "still alive" character
-        if self.__update_secs!=-1 and (datetime.datetime.now()-self.__last_update).total_seconds()>self.__update_secs:
-            self.logger.debug('.')
+    def _print_still_alive(self):
+        # print the "still alive" character
+        if (
+            self.__update_secs != -1
+            and (datetime.datetime.now() - self.__last_update).total_seconds()
+            > self.__update_secs
+        ):
+            self.logger.debug(".")
             self.__last_update = datetime.datetime.now()
 
-    def _check_control_command_queue(self) :
-        #if anything exists in the control command queue
-        try :
-            cmd = self.control_command_queue.get(block=True,timeout=0.5)
-        except Empty :
+    def _check_control_command_queue(self):
+        # if anything exists in the control command queue
+        try:
+            cmd = self.control_command_queue.get(block=True, timeout=0.05)
+        except Empty:
             cmd = None
-        if cmd is not None :
-            if cmd.lower() in ('q','quit') : # shut down the process
+        if cmd is not None:
+            if cmd.lower() in ("q", "quit"):  # shut down the process
                 self.shutdown()
-            elif cmd.lower() in ('c','check') : # run the on_check function
+            elif cmd.lower() in ("c", "check"):  # run the on_check function
                 self._on_check()
-            else : # otherwise just skip this unrecognized command
+            else:  # otherwise just skip this unrecognized command
                 self._check_control_command_queue()
 
     #################### ABSTRACT METHODS ####################
 
     @abstractmethod
-    def run(self) :
+    def run(self):
         """
         Classes extending this base class should include the logic of actually
         running the controlled process in this function, and should call super().run()
         before anything else to set some internal variables
         """
         self.__alive = True
         self.__last_update = datetime.datetime.now()
 
     @abstractmethod
-    def _on_check(self) :
+    def _on_check(self):
         """
         This function is run when the "check" command is found in the control queue.
 
         Not implemented in the base class
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _on_shutdown(self) :
+    def _on_shutdown(self):
         """
         This function is run when the process is stopped; it's called from :func:`~shutdown`.
 
         Not implemented in the base class
         """
         raise NotImplementedError
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/controlled_process_multi_threaded.py` & `openmsistream-1.4.0/openmsistream/utilities/controlled_process_multi_threaded.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,120 +1,136 @@
 """
 A ControlledProcess running with more than one thread
 """
 
-#imports
+# imports
 from threading import Lock
 from abc import ABC, abstractmethod
 from ..utilities.exception_tracking_thread import ExceptionTrackingThread
 from .config import RUN_CONST
 from .controlled_process import ControlledProcess
 
-class ControlledProcessMultiThreaded(ControlledProcess,ABC) :
+
+class ControlledProcessMultiThreaded(ControlledProcess, ABC):
     """
     A class for running a group of processes in multiple threads until they're explicitly shut down.
 
     :param n_threads: the number of threads to use in the group of processes
     :type n_threads: int, optional
     """
 
-    def __init__(self,*args,n_threads=RUN_CONST.DEFAULT_N_THREADS,**kwargs) :
+    def __init__(self, *args, n_threads=RUN_CONST.DEFAULT_N_THREADS, **kwargs):
         self.n_threads = n_threads
-        super().__init__(*args,**kwargs)
+        super().__init__(*args, **kwargs)
         self.lock = Lock()
         self.__args_per_thread = []
         self.__kwargs_per_thread = {}
         self.__threads = []
 
-    def run(self,args_per_thread=None,kwargs_per_thread=None) :
+    def run(self, args_per_thread=None, kwargs_per_thread=None):
         """
-        Create and start the set of independent threads running :func:`~_run_worker`, which can accept optional
-        arguments/keyword arguments from the call to this function. Once the threads are started they will be
-        automatically restarted if they crash.
+        Create and start the set of independent threads running :func:`~_run_worker`,
+        which can accept optional arguments/keyword arguments from the call to this function.
+        Once the threads are started they will be automatically restarted if they crash.
 
-        :param args_per_thread: a list of lists of arguments that should be given to the independent threads
-            (one list of arguments per thread)
+        :param args_per_thread: a list of lists of arguments that should be given to the
+            independent threads (one list of arguments per thread)
         :type args_per_thread: list, optional
-        :param kwargs_per_thread: a list of dicts of keyword arguments that should be given to the independent threads
-            (one dict of keyword arguments per thread)
+        :param kwargs_per_thread: a list of dicts of keyword arguments that should be given
+            to the independent threads (one dict of keyword arguments per thread)
         :type kwargs_per_thread: dict, optional
         """
         super().run()
-        #correct the arguments for each thread
-        if args_per_thread is not None :
+        # correct the arguments for each thread
+        if args_per_thread is not None:
             self.__args_per_thread = args_per_thread
-        if self.__args_per_thread==[] or (not isinstance(self.__args_per_thread,list)) :
+        if self.__args_per_thread == [] or (not isinstance(self.__args_per_thread, list)):
             self.__args_per_thread = [self.__args_per_thread]
-        if not len(self.__args_per_thread)==self.n_threads :
-            if not len(self.__args_per_thread)==1 :
-                errmsg = 'ERROR: ControlledProcessMultiThreaded.run was given a list of arguments with '
-                errmsg+= f'{len(self.__args_per_thread)} entries, but was set up to use {self.n_threads} threads!'
-                self.logger.error(errmsg,exc_type=ValueError)
-            else :
-                self.__args_per_thread = self.n_threads*self.__args_per_thread
-        #correct the keyword arguments for each thread
-        if kwargs_per_thread is not None :
+        if not len(self.__args_per_thread) == self.n_threads:
+            if not len(self.__args_per_thread) == 1:
+                errmsg = (
+                    f"ERROR: ControlledProcessMultiThreaded.run was given a list of arguments "
+                    f"with {len(self.__args_per_thread)} entries, but was set up to use "
+                    f"{self.n_threads} threads!"
+                )
+                self.logger.error(errmsg, exc_type=ValueError)
+            else:
+                self.__args_per_thread = self.n_threads * self.__args_per_thread
+        # correct the keyword arguments for each thread
+        if kwargs_per_thread is not None:
             self.__kwargs_per_thread = kwargs_per_thread
-        if not isinstance(self.__kwargs_per_thread,list) :
+        if not isinstance(self.__kwargs_per_thread, list):
             self.__kwargs_per_thread = [self.__kwargs_per_thread]
-        if not len(self.__kwargs_per_thread)==self.n_threads :
-            if not len(self.__kwargs_per_thread)==1 :
-                errmsg = 'ERROR: ControlledProcessMultiThreaded.run was given a list of arguments with '
-                errmsg+= f'{len(self.__kwargs_per_thread)} entries, but was set up to use {self.n_threads} threads!'
-                self.logger.error(errmsg,exc_type=ValueError)
-            else :
-                self.__kwargs_per_thread = self.n_threads*self.__kwargs_per_thread
-        #create and start the independent threads
-        for i in range(self.n_threads) :
-            self.__threads.append(ExceptionTrackingThread(target=self._run_worker,
-                                           args=self.__args_per_thread[i],
-                                           kwargs=self.__kwargs_per_thread[i]))
+        if not len(self.__kwargs_per_thread) == self.n_threads:
+            if not len(self.__kwargs_per_thread) == 1:
+                errmsg = (
+                    f"ERROR: ControlledProcessMultiThreaded.run was given a list of arguments "
+                    f"with {len(self.__kwargs_per_thread)} entries, but was set up to use "
+                    f"{self.n_threads} threads!"
+                )
+                self.logger.error(errmsg, exc_type=ValueError)
+            else:
+                self.__kwargs_per_thread = self.n_threads * self.__kwargs_per_thread
+        # create and start the independent threads
+        for i in range(self.n_threads):
+            self.__threads.append(
+                ExceptionTrackingThread(
+                    target=self._run_worker,
+                    args=self.__args_per_thread[i],
+                    kwargs=self.__kwargs_per_thread[i],
+                )
+            )
             self.__threads[-1].start()
-        #loop while the process is alive, checking the control command queue and printing the "still alive" character
-        while self.alive :
+        # loop while the process is alive
+        while self.alive:
             self._print_still_alive()
             self._check_control_command_queue()
             self.__restart_crashed_threads()
 
-    def _on_shutdown(self) :
+    def _on_shutdown(self):
         """
-        Join all of the running threads. Can override this method further in subclasses, just be sure to also call
-        :func:`super()._on_shutdown()`.
+        Join all of the running threads. Can override this method further in subclasses,
+        just be sure to also call :func:`super()._on_shutdown()`.
         """
-        for thread in self.__threads :
+        for thread in self.__threads:
             thread.join()
 
     @abstractmethod
-    def _run_worker(self) :
+    def _run_worker(self):
         """
-        The function that will actually be run in multiple threads while the process is alive. Should include a
-        "while self.alive" loop to keep it running.
+        The function that will actually be run in multiple threads while the process is alive.
+        Should include a "while self.alive" loop to keep it running.
 
         `self.lock` can be used to guarantee exactly one copy of this function is running at a time.
 
         Not implemented in the base class.
         """
         raise NotImplementedError
 
-    def __restart_crashed_threads(self) :
+    def __restart_crashed_threads(self):
         """
-        Log (but don't re-raise) Exceptions thrown by any of the threads and restart them based on the args/kwargs
-        initially passed to :func:`~run`.
+        Log (but don't re-raise) Exceptions thrown by any of the threads and restart them
+        based on the args/kwargs initially passed to :func:`~run`.
         """
-        for ti,thread in enumerate(self.__threads) :
-            if thread.caught_exception is not None :
-                #log the error
-                warnmsg = 'WARNING: a thread raised an Exception, which will be logged as an error below but not '
-                warnmsg+= 're-raised. The thread that raised the error will be restarted.'
-                self.logger.warning(warnmsg,exc_info=thread.caught_exception)
-                #try to join the thread
-                try :
+        for ti, thread in enumerate(self.__threads):
+            if thread.caught_exception is not None:
+                # log the error
+                warnmsg = (
+                    "WARNING: a thread raised an Exception, which will be logged as an "
+                    "error below but not re-raised. The thread that raised the error "
+                    "will be restarted."
+                )
+                self.logger.warning(warnmsg, exc_info=thread.caught_exception)
+                # try to join the thread
+                try:
                     thread.join()
-                except Exception :
+                except Exception:
                     pass
-                finally :
+                finally:
                     self.__threads[ti] = None
-                #restart the thread
-                self.__threads[ti] = ExceptionTrackingThread(target=self._run_worker,
-                                              args=self.__args_per_thread[ti],
-                                              kwargs=self.__kwargs_per_thread[ti])
+                # restart the thread
+                self.__threads[ti] = ExceptionTrackingThread(
+                    target=self._run_worker,
+                    args=self.__args_per_thread[ti],
+                    kwargs=self.__kwargs_per_thread[ti],
+                )
                 self.__threads[ti].start()
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/controlled_process_single_thread.py` & `openmsistream-1.4.0/openmsistream/utilities/controlled_process_single_thread.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 A controlled process that is only running in a single thread
 """
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 from .controlled_process import ControlledProcess
 
-class ControlledProcessSingleThread(ControlledProcess,ABC) :
+
+class ControlledProcessSingleThread(ControlledProcess, ABC):
     """
     A class for running a process in a single thread in a loop until it's explicitly shut down.
     Every iteration a single function is called, and then the control command queue is checked.
     """
 
-    def run(self) :
+    def run(self):
         """
         Start the process and call :func:`~_run_iteration` until the process is shut down
         """
         super().run()
-        while self.alive :
+        while self.alive:
             self._run_iteration()
             self._print_still_alive()
             self._check_control_command_queue()
 
     @abstractmethod
-    def _run_iteration(self) :
+    def _run_iteration(self):
         """
         The function that is called repeatedly in an infinite loop as long as the process is alive.
 
         Not implemented in the base class.
         """
         raise NotImplementedError
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/dataclass_table.py` & `openmsistream-1.4.0/openmsistream/utilities/dataclass_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,488 +1,572 @@
 """
-A couple utility classes (and a helper function) to represent a set of (relatively arbitrary) dataclass objects
-serialized to/deseralized from a corresponding CSV file in an atomic and (relatively) thread-safe way
+A couple utility classes (and a helper function) to represent a set of (relatively arbitrary)
+dataclass objects serialized to/deseralized from a corresponding CSV file in an atomic and
+(relatively) thread-safe way
 """
 
-#imports
+# imports
 import pathlib, functools, datetime, typing, copy, os, time
 from abc import ABC
 from threading import Lock
 from dataclasses import fields, is_dataclass
 import methodtools
 from atomicwrites import atomic_write
 from .logging import LogOwner
 
-def get_nested_types() :
+
+def get_nested_types():
     """
-    Helper function to generate the class constant that holds the supported nested types for dataclass tables
+    Helper function to generate the class constant that holds the supported nested types
+    for dataclass tables
     """
-    simple_types = [str,int,float,complex,bool]
-    container_types = [(typing.List,list,'[]'),(typing.Tuple,tuple,'()'),(typing.Set,set,'set()')]
+    simple_types = [str, int, float, complex, bool]
+    container_types = [
+        (typing.List, list, "[]"),
+        (typing.Tuple, tuple, "()"),
+        (typing.Set, set, "set()"),
+    ]
     nested_types_dict = {}
-    for c_t in container_types :
-        for s_t in simple_types :
-            nested_types_dict[c_t[0][s_t]] = (c_t[1],s_t,c_t[2])
+    for c_t in container_types:
+        for s_t in simple_types:
+            nested_types_dict[c_t[0][s_t]] = (c_t[1], s_t, c_t[2])
     return nested_types_dict
 
-class DataclassTableBase(LogOwner,ABC) :
+
+class DataclassTableBase(LogOwner, ABC):
     """
     A base class for DataclassTable objects
 
-    :param dataclass_type: The :class:`dataclasses.dataclass` defining the entries in the table/csv file
+    :param dataclass_type: The :class:`dataclasses.dataclass` defining the entries
+        in the table/csv file
     :type dataclass_type: :class:`dataclasses.dataclass`
     :param filepath: The path to the .csv file that should be created (or read from) on startup.
         The default is a file named after the dataclass type in the current directory.
     :type filepath: :class:`pathlib.Path` or None, optional
     :param create_if_missing: If True, the file at the given path will be created as an empty file
         if it doesn't already exist
     :type create_if_missing: bool
     """
 
     #################### CONSTANTS ####################
 
-    DELIMETER = ';' #can't use a comma or containers would display incorrectly
-    DATETIME_FORMAT = '%a %b %d, %Y at %H:%M:%S'
-    UPDATE_FILE_EVERY = 5 #only update the .csv file automatically every 5 seconds to make updates less expensive
+    DELIMETER = ";"  # can't use a comma or containers would display incorrectly
+    DATETIME_FORMAT = "%a %b %d, %Y at %H:%M:%S"
+    # only update the .csv file automatically every 5 seconds to make updates less expensive
+    UPDATE_FILE_EVERY = 5
     NESTED_TYPES = get_nested_types()
 
     #################### PUBLIC FUNCTIONS ####################
 
-    def __init__(self,dataclass_type,*,filepath=None,create_if_missing=True,**kwargs) :
+    def __init__(
+        self, dataclass_type, *, filepath=None, create_if_missing=True, **kwargs
+    ):
         """
         Constructor method
         """
-        #init the LogOwner
+        # init the LogOwner
         super().__init__(**kwargs)
-        #create the thread lock for the table
+        # create the thread lock for the table
         self.lock = Lock()
-        #figure out what type of objects the table/file will be describing
+        # figure out what type of objects the table/file will be describing
         self.__dataclass_type = dataclass_type
-        if not is_dataclass(self.__dataclass_type) :
-            self.logger.error(f'ERROR: "{self.__dataclass_type}" is not a dataclass!',exc_type=TypeError)
-        if len(fields(self.__dataclass_type)) <= 0 :
-            errmsg = f'ERROR: dataclass type {self.__dataclass_type} does not have any fields '
-            errmsg+= f'and so cannot be used in a {self.__class__.__name__}!'
-            self.logger.error(errmsg,exc_type=ValueError)
+        if not is_dataclass(self.__dataclass_type):
+            self.logger.error(
+                f'ERROR: "{self.__dataclass_type}" is not a dataclass!',
+                exc_type=TypeError,
+            )
+        if len(fields(self.__dataclass_type)) <= 0:
+            errmsg = (
+                f"ERROR: dataclass type {self.__dataclass_type} does not have any fields "
+                f"and so cannot be used in a {self.__class__.__name__}!"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
         self.__field_names = [field.name for field in fields(self.__dataclass_type)]
         self.__field_types = [field.type for field in fields(self.__dataclass_type)]
-        #figure out where the csv file should go
-        self.__filepath = filepath if filepath is not None else pathlib.Path() / f'{self.__dataclass_type.__name__}.csv'
-        #set some other variables
+        # figure out where the csv file should go
+        self.__filepath = (
+            filepath
+            if filepath is not None
+            else pathlib.Path() / f"{self.__dataclass_type.__name__}.csv"
+        )
+        # set some other variables
         self._entry_objs = {}
         self._entry_lines = {}
-        #read or create the file to finish setting up the table
+        # read or create the file to finish setting up the table
         self._file_last_updated = datetime.datetime.now()
-        if self.__filepath.is_file() :
+        if self.__filepath.is_file():
             self.__read_csv_file()
-        elif create_if_missing :
-            msg = f'Creating new {self.__class__.__name__} csv file at {self.__filepath} '
-            msg+= f'to hold {self.__dataclass_type.__name__} entries'
+        elif create_if_missing:
+            msg = (
+                f"Creating new {self.__class__.__name__} csv file at {self.__filepath} "
+                f"to hold {self.__dataclass_type.__name__} entries"
+            )
             self.logger.debug(msg)
             self.dump_to_file()
 
-    def get_entry_attrs(self,entry_obj_address,*args) :
+    def get_entry_attrs(self, entry_obj_address, *args):
         """
         Return copies of all or some of the current attributes of an entry in the table.
         Returning copies ensures the original objects cannot be modified by accident.
 
         Use `args` to get a dictionary of desired attribute values returned.
         If only one arg is given the return value is just that single attribute.
         The default (no additional arguments) returns a dictionary of all attributes for the entry
 
-        :param entry_obj_address: the address in memory of the object to return copies of attributes for
+        :param entry_obj_address: the address in memory of the object to return copies
+            of attributes for
         :type entry_obj_address: hex(id(object))
-        :param args: Add other arguments that are names of attributes to get only those specific attributes of the entry
+        :param args: Add other arguments that are names of attributes to get only those
+            specific attributes of the entry
         :type args: str, optional
 
         :return: copies of some or all attributes for an entry in the table
         :rtype: depends on arguments, or dict
 
-        :raises ValueError: if `entry_obj_address` doesn't correspond to an object listed in the table
+        :raises ValueError: if `entry_obj_address` doesn't correspond to an object
+            listed in the table
         """
-        if entry_obj_address not in self._entry_objs :
-            errmsg = f'ERROR: address {entry_obj_address} sent to get_entry_attrs is not registered!'
-            self.logger.error(errmsg,exc_type=ValueError)
+        if entry_obj_address not in self._entry_objs:
+            self.logger.error(
+                f"ERROR: address {entry_obj_address} is not registered!",
+                exc_type=ValueError,
+            )
         obj = self._entry_objs[entry_obj_address]
-        if len(args)==1 :
-            return copy.deepcopy(getattr(obj,args[0]))
+        if len(args) == 1:
+            return copy.deepcopy(getattr(obj, args[0]))
         to_return = {}
-        for fname in self.__field_names :
-            if (not args) or (fname in args) :
-                to_return[fname] = copy.deepcopy(getattr(obj,fname))
-        if args :
-            for arg in args :
-                if arg not in to_return :
-                    errmsg = f'WARNING: attribute name {arg} is not a name of a {self.__dataclass_type} '
-                    errmsg+= 'Field and will not be returned from get_entry_attrs!'
-                    self.logger.warning(errmsg)
+        for fname in self.__field_names:
+            if (not args) or (fname in args):
+                to_return[fname] = copy.deepcopy(getattr(obj, fname))
+        if args:
+            for arg in args:
+                if arg not in to_return:
+                    warnmsg = (
+                        f"WARNING: attribute name {arg} is not a name of a {self.__dataclass_type} "
+                        "Field and will not be returned from get_entry_attrs!"
+                    )
+                    self.logger.warning(warnmsg)
         return to_return
 
     @functools.lru_cache(maxsize=8)
-    def obj_addresses_by_key_attr(self,key_attr_name) :
+    def obj_addresses_by_key_attr(self, key_attr_name):
         """
         Return a dictionary whose keys are the values of some given attribute for each object
         and whose values are lists of the addresses in memory of the objects in the table
         that have each value of the requested attribute.
 
         Useful to find objects in the table by attribute values so they can be efficiently updated
         without compromising the integrity of the objects in the table and their attributes.
 
         Up to five calls are cached so if nothing changes this happens a little faster.
 
-        :param key_attr_name: the name of the attribute whose values should be used as keys in the returned dictionary
+        :param key_attr_name: the name of the attribute whose values should be used as keys
+            in the returned dictionary
         :type key_attr_name: str
 
-        :return: A dictionary listing all objects in the table, keyed by their values of `key_attr_name`
+        :return: A dictionary listing all objects in the table, keyed by their values
+            of `key_attr_name`
         :rtype: dict
 
-        :raises ValueError: if `key_attr_name` is not recognized as the name of an attribute for entries in the table
+        :raises ValueError: if `key_attr_name` is not recognized as the name of an attribute
+            for entries in the table
         """
-        if key_attr_name not in self.__field_names :
-            errmsg = f'ERROR: {key_attr_name} is not a name of a Field for {self.__dataclass_type} objects!'
-            self.logger.error(errmsg,exc_type=ValueError)
+        if key_attr_name not in self.__field_names:
+            errmsg = (
+                f"ERROR: {key_attr_name} is not a name of a Field "
+                f"for {self.__dataclass_type} objects!"
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
         to_return = {}
         locked_internally = False
-        if not self.lock.locked() :
+        if not self.lock.locked():
             locked_internally = True
             self.lock.acquire()
-        for addr,obj in self._entry_objs.items() :
-            rkey = getattr(obj,key_attr_name)
-            if rkey not in to_return :
+        for addr, obj in self._entry_objs.items():
+            rkey = getattr(obj, key_attr_name)
+            if rkey not in to_return:
                 to_return[rkey] = []
             to_return[rkey].append(addr)
-        if locked_internally :
+        if locked_internally:
             self.lock.release()
         return to_return
 
-    def dump_to_file(self,reraise_exc=True,retries=2) :
+    def dump_to_file(self, reraise_exc=True, retries=2):
         """
         Dump the contents of the table to a csv file.
         Call this to force the file to update and reflect the current state of objects.
         Automatically called in several contexts.
 
-        :param reraise_exc: if True, Exceptions raised when writing out to the file will be re-raised
+        :param reraise_exc: if True, Exceptions raised when writing out to the file
+            will be re-raised
         :type reraise_exc: bool, optional
         :param retries: how many times to retry writing out the file
         :type retries: int, optional
         """
         lines_to_write = [self.csv_header_line]
-        if len(self._entry_lines)>0 :
-            lines_to_write+=list(self._entry_lines.values())
+        if len(self._entry_lines) > 0:
+            lines_to_write += list(self._entry_lines.values())
         locked_internally = False
-        if not self.lock.locked() :
+        if not self.lock.locked():
             locked_internally = True
             self.lock.acquire()
-        self.__write_lines(lines_to_write,reraise_exc=reraise_exc,retries=retries)
-        if locked_internally :
+        self.__write_lines(lines_to_write, reraise_exc=reraise_exc, retries=retries)
+        if locked_internally:
             self.lock.release()
 
     #################### PROPERTIES ####################
 
     @methodtools.lru_cache()
     @property
-    def csv_header_line(self) :
+    def csv_header_line(self):
         """
         The first line in the CSV file (OS-dependent)
         """
-        header_line = ''
-        #add an extra line when running on Windows to seamlessly open the file in Excel
-        if os.name=='nt' :
-            header_line+=f'sep={self.DELIMETER}\n'
-        for fieldname in self.__field_names :
-            header_line+=f'{fieldname}{self.DELIMETER}'
+        header_line = ""
+        # add an extra line when running on Windows to seamlessly open the file in Excel
+        if os.name == "nt":
+            header_line += f"sep={self.DELIMETER}\n"
+        for fieldname in self.__field_names:
+            header_line += f"{fieldname}{self.DELIMETER}"
         return header_line[:-1]
 
     @property
-    def obj_addresses(self) :
+    def obj_addresses(self):
         """
         All recognized object hex addresses
         """
         return list(self._entry_objs.keys())
 
     @property
-    def filepath(self) :
+    def filepath(self):
         """
         Path to the CSV file
         """
         return self.__filepath
 
     @property
-    def n_entries(self) :
+    def n_entries(self):
         """
         The number of entries in the file
         """
         return len(self._entry_objs)
 
     @property
-    def dataclass_type(self) :
+    def dataclass_type(self):
         """
         The type of the Dataclass objects contained in the table
         """
         return self.__dataclass_type
 
     #################### PRIVATE HELPER FUNCTIONS ####################
 
-    def __read_csv_file(self) :
+    def __read_csv_file(self):
         """
         Read in a csv file with lines of the expected dataclass type
         """
-        #read the file
-        with open(self.__filepath,'r') as fp :
+        # read the file
+        with open(self.__filepath, "r") as fp:
             lines_as_read = fp.readlines()
-        #first make sure the header line matches what we'd expect for the dataclass
-        n_header_lines = len(self.csv_header_line.split('\n'))
-        for ihl in range(n_header_lines) :
-            if lines_as_read[ihl].strip()!=(self.csv_header_line.split('\n'))[ihl] :
-                errmsg = f'ERROR: header line in {self.__filepath} ({lines_as_read[0]}) does not match expectation for '
-                errmsg+= f'{self.__dataclass_type} ({self.csv_header_line})!'
-                self.logger.error(errmsg,exc_type=RuntimeError)
-        #add entry lines and objects
-        for line in lines_as_read[n_header_lines:] :
+        # first make sure the header line matches what we'd expect for the dataclass
+        n_header_lines = len(self.csv_header_line.split("\n"))
+        for ihl in range(n_header_lines):
+            if lines_as_read[ihl].strip() != (self.csv_header_line.split("\n"))[ihl]:
+                errmsg = (
+                    f"ERROR: header line in {self.__filepath} ({lines_as_read[0]}) "
+                    f"does not match expectation for {self.__dataclass_type} "
+                    f"({self.csv_header_line})!"
+                )
+                self.logger.error(errmsg, exc_type=RuntimeError)
+        # add entry lines and objects
+        for line in lines_as_read[n_header_lines:]:
             obj = self.__obj_from_line(line)
-            #key both dictionaries by the address of the object in memory
+            # key both dictionaries by the address of the object in memory
             dkey = hex(id(obj))
             self._entry_objs[dkey] = obj
             self._entry_lines[dkey] = line
-        msg = f'Found {len(self._entry_objs)} {self.__dataclass_type.__name__} entries in {self.__filepath}'
+        msg = (
+            f"Found {len(self._entry_objs)} {self.__dataclass_type.__name__} "
+            f"entries in {self.__filepath}"
+        )
         self.logger.debug(msg)
 
-    def __write_lines(self,lines,overwrite=True,reraise_exc=True,retries=2) :
+    def __write_lines(self, lines, overwrite=True, reraise_exc=True, retries=2):
         """
         Write a line or container of lines to the csv file, in a thread-safe and atomic way
         """
-        if isinstance(lines,str) :
+        if isinstance(lines, str):
             lines = [lines]
-        lines_string = ''
-        for line in lines :
-            lines_string+=f'{line.strip()}\n'
+        lines_string = "\n".join([line.strip() for line in lines])
         n_retries_left = retries
         caught_exc = None
-        while n_retries_left>0 :
-            try :
-                with atomic_write(self.__filepath,overwrite=overwrite) as fp :
+        while n_retries_left > 0:
+            try:
+                with atomic_write(
+                    self.__filepath, overwrite=overwrite, encoding="utf8"
+                ) as fp:
                     fp.write(lines_string)
                 self._file_last_updated = datetime.datetime.now()
                 return
-            except Exception as exc :
+            except Exception as exc:
                 caught_exc = exc
-                n_retries_left-=1
+                n_retries_left -= 1
                 time.sleep(0.1)
                 continue
-        if caught_exc is not None :
-            if not isinstance(caught_exc,FileNotFoundError) : #This is common to see and okay when running multithreaded
-                if reraise_exc :
-                    errmsg = f'ERROR: failed to write to {self.__class__.__name__} csv file at {self.__filepath} '
-                    errmsg+= f'after {retries-n_retries_left+1} attempts! Will reraise exception.'
-                    self.logger.error(errmsg,exc_info=caught_exc,reraise=True)
-                else :
-                    msg = f'WARNING: failed in {retries-n_retries_left+1} attempts to write to '
-                    msg+= f'{self.__class__.__name__} csv file at {self.__filepath}! '
-                    msg+= f'Exception ({type(caught_exc)}): {caught_exc}'
-                    self.logger.warning(msg)
+        if caught_exc is not None:
+            if not isinstance(
+                caught_exc, FileNotFoundError
+            ):  # This is common to see and okay when running multithreaded
+                if reraise_exc:
+                    errmsg = (
+                        f"ERROR: failed to write to {self.__class__.__name__} csv file at "
+                        f"{self.__filepath} after {retries-n_retries_left+1} attempts! "
+                        "Will reraise exception."
+                    )
+                    self.logger.error(errmsg, exc_info=caught_exc, reraise=True)
+                else:
+                    msg = (
+                        f"WARNING: failed in {retries-n_retries_left+1} attempts to write "
+                        f"to {self.__class__.__name__} csv file at {self.__filepath}! "
+                        "Exception info below"
+                    )
+                    self.logger.warning(msg, exc_info=caught_exc)
 
-    def _line_from_obj(self,obj) :
+    def _line_from_obj(self, obj):
         """
         Return the csv file line for a given object
         """
-        if obj.__class__ != self.__dataclass_type :
-            self.logger.error(f'ERROR: "{obj}" is mismatched to type {self.__dataclass_type}!',exc_type=TypeError)
-        obj_line = ''
-        for fname,ftype in zip(self.__field_names,self.__field_types) :
-            obj_line+=f'{self.__get_str_from_attribute(getattr(obj,fname),ftype)}{self.DELIMETER}'
-        return obj_line[:-1]
+        if obj.__class__ != self.__dataclass_type:
+            self.logger.error(
+                f'ERROR: "{obj}" is mismatched to type {self.__dataclass_type}!',
+                exc_type=TypeError,
+            )
+        return self.DELIMETER.join(
+            [
+                self.__get_str_from_attribute(getattr(obj, fname), ftype)
+                for fname, ftype in zip(self.__field_names, self.__field_types)
+            ]
+        )
 
-    def __obj_from_line(self,line) :
+    def __obj_from_line(self, line):
         """
         Return the dataclass instance for a given csv file line string
         """
         args = []
-        for attrtype,attrstr in zip(self.__field_types,(line.strip().split(self.DELIMETER))) :
-            args.append(self.__get_attribute_from_str(attrstr,attrtype))
+        for attrtype, attrstr in zip(
+            self.__field_types, (line.strip().split(self.DELIMETER))
+        ):
+            args.append(self.__get_attribute_from_str(attrstr, attrtype))
         return self.__dataclass_type(*args)
 
-    def __get_str_from_attribute(self,attrobj,attrtype) :
+    def __get_str_from_attribute(self, attrobj, attrtype):
         """
         Given an object and the type it is in the dataclass,
         return the string representation of it that should go in the file
         """
-        if attrtype==datetime.datetime :
+        if attrtype == datetime.datetime:
             return repr(attrobj.strftime(self.DATETIME_FORMAT))
-        if attrtype==pathlib.Path :
+        if attrtype == pathlib.Path:
             return repr(str(attrobj))
         return repr(attrobj)
 
-    def __get_attribute_from_str(self,attrstr,attrtype) :
+    def __get_attribute_from_str(self, attrstr, attrtype):
         """
-        Given the string of the repr() output of some object and the datatype it represents, return the actual object
+        Given the string of the repr() output of some object and the datatype it represents,
+        return the actual object
         """
-        #datetime objects are handled in a custom way
-        if attrtype==datetime.datetime :
-            return datetime.datetime.strptime(attrstr[1:-1],self.DATETIME_FORMAT)
-        #so are path objects
-        if attrtype==pathlib.Path :
+        # datetime objects are handled in a custom way
+        if attrtype == datetime.datetime:
+            return datetime.datetime.strptime(attrstr[1:-1], self.DATETIME_FORMAT)
+        # so are path objects
+        if attrtype == pathlib.Path:
             return pathlib.Path(attrstr[1:-1])
-        #strings have extra quotes on either end
-        if attrtype==str :
+        # strings have extra quotes on either end
+        if attrtype == str:
             return attrtype(attrstr[1:-1])
-        #int, float, complex, and bool can all be directly re-casted
-        if attrtype in (int,float,complex,bool) :
+        # int, float, complex, and bool can all be directly re-casted
+        if attrtype in (int, float, complex, bool):
             return attrtype(attrstr)
-        #some simply-nested container types can be casted in two steps
-        if attrtype in self.NESTED_TYPES :
-            #empty collections
-            if attrstr==self.NESTED_TYPES[attrtype][2] :
+        # some simply-nested container types can be casted in two steps
+        if attrtype in self.NESTED_TYPES:
+            # empty collections
+            if attrstr == self.NESTED_TYPES[attrtype][2]:
                 return self.NESTED_TYPES[attrtype][0]()
             to_cast = []
-            for vstr in attrstr[1:-1].split(',') :
+            for vstr in attrstr[1:-1].split(","):
                 to_cast.append(self.NESTED_TYPES[attrtype][1](vstr))
             return self.NESTED_TYPES[attrtype][0](to_cast)
-        errmsg = f'ERROR: attribute type "{attrtype}" is not recognized for a {self.__class__.__name__}!'
-        self.logger.error(errmsg,exc_type=ValueError)
+        errmsg = (
+            f'ERROR: attribute type "{attrtype}" is not recognized '
+            f"for a {self.__class__.__name__}!"
+        )
+        self.logger.error(errmsg, exc_type=ValueError)
         return None
 
-class DataclassTableReadOnly(DataclassTableBase) :
+
+class DataclassTableReadOnly(DataclassTableBase):
     """
     A class to read dataclass objects stored in a csv file
     """
 
-    def __init__(self,dataclass_type,*,filepath=None,**kwargs) :
+    def __init__(self, dataclass_type, *, filepath=None, **kwargs):
         """
         Signature duplicated here for documentation
         """
-        super().__init__(dataclass_type,filepath=filepath,create_if_missing=False,**kwargs)
+        super().__init__(
+            dataclass_type, filepath=filepath, create_if_missing=False, **kwargs
+        )
 
     @property
-    def objects(self) :
+    def objects(self):
         """
         A list of all the dataclass objects in the file
         """
         return self._entry_objs.values()
 
     @property
-    def lines(self) :
+    def lines(self):
         """
         A list of all the text lines in the file
         """
         return self._entry_lines.values()
 
-class DataclassTableAppendOnly(DataclassTableBase) :
+
+class DataclassTableAppendOnly(DataclassTableBase):
     """
-    A class to work with an atomic csv file that's holding dataclass entries. Only includes methods to add lines
-    to the file like a log and not to edit the objects themselves, which can be much more efficient.
+    A class to work with an atomic csv file that's holding dataclass entries. Only includes
+    methods to add lines to the file like a log and not to edit the objects themselves,
+    which can be much more efficient.
     """
 
-    def __init__(self,dataclass_type,*,filepath=None,**kwargs) :
+    def __init__(self, dataclass_type, *, filepath=None, **kwargs):
         """
         Signature duplicated here for documentation
         """
-        super().__init__(dataclass_type,filepath=filepath,**kwargs)
+        super().__init__(dataclass_type, filepath=filepath, **kwargs)
 
-    def add_entries(self,new_entries) :
+    def add_entries(self, new_entries):
         """
         Add a new set of entries to the table.
 
         :param new_entries: the new entry or entries to add to the table
         :type new_entries: :class:`dataclasses.dataclass` or list(:class:`dataclasses.dataclass`)
 
         :raises ValueError: if any of the objects in `new_entries` already exists in the table
         """
-        if is_dataclass(new_entries) :
+        if is_dataclass(new_entries):
             new_entries = [new_entries]
-        for entry in new_entries :
+        for entry in new_entries:
             entry_addr = hex(id(entry))
-            if entry_addr in self._entry_objs or entry_addr in self._entry_lines :
-                errmsg = 'ERROR: address of object sent to add_entries is already registered!'
-                self.logger.error(errmsg,exc_type=ValueError)
+            if entry_addr in self._entry_objs or entry_addr in self._entry_lines:
+                errmsg = (
+                    "ERROR: address of object sent to add_entries is already registered!"
+                )
+                self.logger.error(errmsg, exc_type=ValueError)
             locked_internally = False
-            if not self.lock.locked() :
+            if not self.lock.locked():
                 locked_internally = True
                 self.lock.acquire()
             self._entry_objs[entry_addr] = entry
             self._entry_lines[entry_addr] = self._line_from_obj(entry)
             self.obj_addresses_by_key_attr.cache_clear()
-            if locked_internally :
+            if locked_internally:
                 self.lock.release()
-        if (datetime.datetime.now()-self._file_last_updated).total_seconds()>self.UPDATE_FILE_EVERY :
+        if (
+            datetime.datetime.now() - self._file_last_updated
+        ).total_seconds() > self.UPDATE_FILE_EVERY:
             self.dump_to_file()
 
-    def as_read_only(self) :
+    def as_read_only(self):
         """
         Returns a "read only" version of the table
         """
-        return DataclassTableReadOnly(self.dataclass_type,filepath=self.filepath,logger=self.logger)
+        return DataclassTableReadOnly(
+            self.dataclass_type, filepath=self.filepath, logger=self.logger
+        )
+
 
-class DataclassTable(DataclassTableAppendOnly) :
+class DataclassTable(DataclassTableAppendOnly):
     """
     A class to work with an atomic csv file that's holding dataclass entries in a thread-safe way
 
-    :param dataclass_type: The :class:`dataclasses.dataclass` defining the entries in the table/csv file
+    :param dataclass_type: The :class:`dataclasses.dataclass` defining the entries
+        in the table/csv file
     :type dataclass_type: :class:`dataclasses.dataclass`
     :param filepath: The path to the .csv file that should be created (or read from) on startup.
         The default is a file named after the dataclass type in the current directory.
     :type filepath: :class:`pathlib.Path` or None, optional
     """
 
-    def __init__(self,dataclass_type,*,filepath=None,**kwargs) :
+    def __init__(self, dataclass_type, *, filepath=None, **kwargs):
         """
         Signature duplicated here for documentation
         """
-        super().__init__(dataclass_type,filepath=filepath,**kwargs)
+        super().__init__(dataclass_type, filepath=filepath, **kwargs)
 
-    def __del__(self) :
+    def __del__(self):
         self.dump_to_file(reraise_exc=False)
 
-    def remove_entries(self,entry_obj_addresses) :
+    def remove_entries(self, entry_obj_addresses):
         """
         Remove an entry or entries from the table
 
-        :param entry_obj_addresses: a single value or container of entry addresses (object IDs in hex form) to remove
-            from the table
+        :param entry_obj_addresses: a single value or container of entry addresses
+            (object IDs in hex form) to remove from the table
         :type entry_obj_addresses: hex(id(object)) or list(hex(id(object)))
 
-        :raises ValueError: if any of the hex addresses in `entry_obj_addresses` is not present in the table
+        :raises ValueError: if any of the hex addresses in `entry_obj_addresses` is
+            not present in the table
         """
-        if isinstance(entry_obj_addresses,str) :
+        if isinstance(entry_obj_addresses, str):
             entry_obj_addresses = [entry_obj_addresses]
-        for entry_addr in entry_obj_addresses :
-            if (entry_addr not in self._entry_objs) or (entry_addr not in self._entry_lines) :
-                errmsg = f'ERROR: address {entry_addr} sent to remove_entries is not registered!'
-                self.logger.error(errmsg,exc_type=ValueError)
+        for entry_addr in entry_obj_addresses:
+            if (entry_addr not in self._entry_objs) or (
+                entry_addr not in self._entry_lines
+            ):
+                errmsg = f"ERROR: address {entry_addr} sent to remove_entries is not registered!"
+                self.logger.error(errmsg, exc_type=ValueError)
             locked_internally = False
-            if not self.lock.locked() :
+            if not self.lock.locked():
                 locked_internally = True
                 self.lock.acquire()
             self._entry_objs.pop(entry_addr)
             self._entry_lines.pop(entry_addr)
             self.obj_addresses_by_key_attr.cache_clear()
-            if locked_internally :
+            if locked_internally:
                 self.lock.release()
-        if (datetime.datetime.now()-self._file_last_updated).total_seconds()>self.UPDATE_FILE_EVERY :
+        if (
+            datetime.datetime.now() - self._file_last_updated
+        ).total_seconds() > self.UPDATE_FILE_EVERY:
             self.dump_to_file()
 
-    def set_entry_attrs(self,entry_obj_address,**kwargs) :
+    def set_entry_attrs(self, entry_obj_address, **kwargs):
         """
         Modify attributes of an entry that already exists in the table
 
         :param entry_obj_address: The address in memory of the entry object to modify
         :type entry_obj_address: hex(id(object))
         :param kwargs: Attributes to set (keys are names, values are values for those named attrs)
         :type kwargs: dict
 
-        :raises ValueError: if `entry_obj_address` doesn't correspond to an object listed in the table
+        :raises ValueError: if `entry_obj_address` doesn't correspond to an object
+            listed in the table
         """
-        if entry_obj_address not in self._entry_objs :
-            errmsg = f'ERROR: address {entry_obj_address} sent to set_entry_attrs is not registered!'
-            self.logger.error(errmsg,exc_type=ValueError)
+        if entry_obj_address not in self._entry_objs:
+            self.logger.error(
+                f"ERROR: address {entry_obj_address} is not registered!",
+                exc_type=ValueError,
+            )
         locked_internally = False
-        if not self.lock.locked() :
+        if not self.lock.locked():
             locked_internally = True
             self.lock.acquire()
         obj = self._entry_objs[entry_obj_address]
-        for fname,fval in kwargs.items() :
-            setattr(obj,fname,fval)
+        for fname, fval in kwargs.items():
+            setattr(obj, fname, fval)
         self._entry_lines[entry_obj_address] = self._line_from_obj(obj)
         self.obj_addresses_by_key_attr.cache_clear()
-        if locked_internally :
+        if locked_internally:
             self.lock.release()
-        if (datetime.datetime.now()-self._file_last_updated).total_seconds()>self.UPDATE_FILE_EVERY :
+        if (
+            datetime.datetime.now() - self._file_last_updated
+        ).total_seconds() > self.UPDATE_FILE_EVERY:
             self.dump_to_file()
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/exception_tracking_thread.py` & `openmsistream-1.4.0/openmsistream/utilities/exception_tracking_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """A Thread that re-raises any Exceptions it encounters during running when it is join()ed"""
 
-#imports
+# imports
 from threading import Thread
 
-class ExceptionTrackingThread(Thread) :
+
+class ExceptionTrackingThread(Thread):
     """
     A small utility class to keep track of any exceptions thrown in a child thread
     and raise them at some point
     """
 
     @property
-    def caught_exception(self) :
+    def caught_exception(self):
         """
         Variable to hold any Exception encountered while the thread is running
         """
         return self.__exc
 
-    def __init__(self,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.__exc = None
 
-    def run(self,*args,**kwargs) :
+    def run(self, *args, **kwargs):
         """
         Wrapper around Thread.run that holds onto any Exception raised during running
         """
-        try :
-            super().run(*args,**kwargs)
-        except Exception as exc :
+        try:
+            super().run(*args, **kwargs)
+        except Exception as exc:
             self.__exc = exc
 
-    def join(self,*args,**kwargs) :
+    def join(self, *args, **kwargs):
         """
         Wrapper around Thread.run that re-raises any Exceptions that were encountered
         """
-        super().join(*args,**kwargs)
-        if self.__exc is not None :
+        super().join(*args, **kwargs)
+        if self.__exc is not None:
             raise self.__exc
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/has_arguments.py` & `openmsistream-1.4.0/openmsistream/utilities/has_arguments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 A class for anything that should have associated command line arguments
 if anything extending it also extends Runnable
 """
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 
-class HasArguments(ABC) :
+
+class HasArguments(ABC):
     """
     A small utility class for anything that should have associated command line arguments
     """
 
     @classmethod
     @abstractmethod
-    def get_command_line_arguments(cls) :
+    def get_command_line_arguments(cls):
         """
-        Get the list of argument names and the dictionary of argument names/default values to add to the argument parser
+        Get the list of argument names and the dictionary of argument names/default values
+        to add to the argument parser
 
         :return: args, a list of argument names recognized by the argument parser
         :rtype: list(str)
         :return: kwargs, a dictionary of default argument values keyed by argument names
             recognized by the argument parser
         :rtype: dict
         """
-        return [],{}
+        return [], {}
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/logging.py` & `openmsistream-1.4.0/openmsistream/utilities/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,220 +1,261 @@
 """Classes for OpenMSIStream logging infrastructure"""
 
-#imports
+# imports
 import pathlib, logging
 from .has_arguments import HasArguments
 
-class OpenMSIStreamFormatter(logging.Formatter) :
+
+class OpenMSIStreamFormatter(logging.Formatter):
     """
-    Very small extension of the usual logging.Formatter to allow modification of format based on message content
+    Very small extension of the usual logging.Formatter to allow modification of format
+    based on message content
     """
 
-    def __init__(self,*args,**kwargs) :
-        super().__init__(*args,**kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
     def format(self, record):
         """
-        If a message starts with a newline, start the actual logging line with the newline before any of the rest
+        If a message starts with a newline, start the actual logging line with the newline
+        before any of the rest
         """
-        formatted = ''
-        if record.msg.startswith('\n') :
-            record.msg = record.msg.lstrip('\n')
-            formatted+='\n'
-        formatted+=super().format(record)
+        formatted = ""
+        if record.msg.startswith("\n"):
+            record.msg = record.msg.lstrip("\n")
+            formatted += "\n"
+        formatted += super().format(record)
         return formatted
 
-class Logger :
+
+class Logger:
     """
     Class for a general logger in OpenMSIStream format.
 
-    :param logger_name: The name for the logger to use (automatically inferred from the running module if not given)
+    :param logger_name: The name for the logger to use
+        (automatically inferred from the running module if not given)
     :type logger_name: str, optional
     :param streamlevel: The level at/above which messages should be logged to the stream/console
     :type streamlevel: logging level int, optional
-    :param logger_filepath: The path to a logger file to use or directory in which an automatically-named
-        logger file should be created
+    :param logger_filepath: The path to a logger file to use or directory in which
+        an automatically-named logger file should be created
     :type logger_filepath: :class:`pathlib.Path`, optional
     :param filelevel: The level at/above which messages should be written to the logfile
     :type filelevel: logging level int, optional
     """
 
-    FORMATTER = OpenMSIStreamFormatter('[%(name)s at %(asctime)s] %(message)s','%Y-%m-%d %H:%M:%S')
-
-    def __init__(self,logger_name=None,streamlevel=logging.INFO,logger_filepath=None,filelevel=logging.WARNING) :
+    FORMATTER = OpenMSIStreamFormatter(
+        "[%(name)s %(asctime)s] %(message)s", "%Y-%m-%d %H:%M:%S"
+    )
+
+    def __init__(
+        self,
+        logger_name=None,
+        streamlevel=logging.INFO,
+        logger_filepath=None,
+        filelevel=logging.WARNING,
+    ):
         """
         name = the name for this logger to use (probably something like the top module that owns it)
         """
         self._name = logger_name
-        if self._name is None :
+        if self._name is None:
             self._name = self.__class__.__name__
         self._logger_obj = logging.getLogger(self._name)
         self._logger_obj.setLevel(logging.DEBUG)
         self._streamhandler = logging.StreamHandler()
         self._streamhandler.setLevel(streamlevel)
         self._streamhandler.setFormatter(self.FORMATTER)
         self._logger_obj.addHandler(self._streamhandler)
         self._filehandler = None
-        if logger_filepath is not None :
-            self.add_file_handler(logger_filepath,level=filelevel)
+        if logger_filepath is not None:
+            self.add_file_handler(logger_filepath, level=filelevel)
 
-    def set_level(self,level) :
+    def set_level(self, level):
         """
         Set the level of the entire underlying logger
 
         :param level: The level to set
         :type level: logging level int
         """
         self._logger_obj.setLevel(level)
 
-    def set_stream_level(self,level) :
+    def set_stream_level(self, level):
         """
         Set the level of the underlying logger's streamhandler
 
         :param level: The level to set
         :type level: logging level int
         """
         self._streamhandler.setLevel(level)
 
-    def set_file_level(self,level) :
+    def set_file_level(self, level):
         """
         Set the level of the underlying logger's filehandler
 
         :param level: The level to set
         :type level: logging level int
         """
-        if self._filehandler is None :
-            errmsg = f'ERROR: Logger {self._name} does not have a filehandler set but set_file_level was called!'
+        if self._filehandler is None:
+            errmsg = (
+                f"ERROR: Logger {self._name} does not have a filehandler set "
+                "but set_file_level was called!"
+            )
             raise RuntimeError(errmsg)
         self._filehandler.setLevel(level)
 
-    def add_file_handler(self,filepath,level=logging.INFO) :
+    def add_file_handler(self, filepath, level=logging.INFO):
         """
         Add an additional :class:`logging.FileHandler` to the logger
 
         :param filepath: The path to the new logger file
         :type filepath: :class:`pathlib.Path`
         :param level: The level to set
         :type level: logging level int
         """
-        if not isinstance(filepath,pathlib.PurePath) :
-            self.error(f'ERROR: {filepath} is a {type(filepath)} object, not a Path object!',exc_type=TypeError)
-        if not filepath.is_file() :
-            if not filepath.parent.is_dir() :
+        if not isinstance(filepath, pathlib.PurePath):
+            self.error(
+                f"ERROR: {filepath} is a {type(filepath)} object, not a Path object!",
+                exc_type=TypeError,
+            )
+        if not filepath.is_file():
+            if not filepath.parent.is_dir():
                 filepath.parent.mkdir(parents=True)
             filepath.touch()
         self._filehandler = logging.FileHandler(filepath)
         self._filehandler.setLevel(level)
         self._filehandler.setFormatter(self.FORMATTER)
         self._logger_obj.addHandler(self._filehandler)
 
-    #methods for logging different levels of messages
+    # methods for logging different levels of messages
 
-    def debug(self,msg,*args,**kwargs) :
+    def debug(self, msg, *args, **kwargs):
         """
-        Log a message at DEBUG level. Additional args/kwargs are sent to the underlying logger object's debug call.
+        Log a message at DEBUG level. Additional args/kwargs are sent to
+        the underlying logger object's debug call.
 
         :param msg: the message to log
         :type msg: str
         """
-        self._logger_obj.debug(msg,*args,**kwargs)
+        self._logger_obj.debug(msg, *args, **kwargs)
 
-    def info(self,msg,*args,**kwargs) :
+    def info(self, msg, *args, **kwargs):
         """
-        Log a message at INFO level. Additional args/kwargs are sent to the underlying logger object's info call.
+        Log a message at INFO level. Additional args/kwargs are sent to
+        the underlying logger object's info call.
 
         :param msg: the message to log
         :type msg: str
         """
-        self._logger_obj.info(msg,*args,**kwargs)
+        self._logger_obj.info(msg, *args, **kwargs)
 
-    def warning(self,msg,*args,**kwargs) :
+    def warning(self, msg, *args, **kwargs):
         """
-        Log a message at WARNING level. Additional args/kwargs are sent to the underlying logger object's warning call.
+        Log a message at WARNING level. Additional args/kwargs are sent to
+        the underlying logger object's warning call.
 
         :param msg: the message to log (will have "WARNING: " prepended if it doesn't start with it)
         :type msg: str
         """
-        if not msg.startswith('WARNING:') :
-            msg = f'WARNING: {msg}'
-        self._logger_obj.warning(msg,*args,**kwargs)
-
-    #log an error message and optionally raise an exception with the same message, or raise a different exception
-    def error(self,msg,*,exc_type=None,reraise=False,**kwargs) :
-        """
-        Log a message at ERROR level. Optionally raise an exception of a given type with the same message, or
-        re-raise an Exception object passed through the `exc_info` kwarg (after logging its traceback).
+        if not msg.startswith("WARNING:"):
+            msg = f"WARNING: {msg}"
+        self._logger_obj.warning(msg, *args, **kwargs)
+
+    def error(self, msg, *, exc_type=None, reraise=False, **kwargs):
+        """
+        Log a message at ERROR level. Optionally raise an exception of a given type
+        with the same message, or re-raise an Exception object passed through the
+        `exc_info` kwarg (after logging its traceback).
 
         Additional kwargs are sent to the underlying logger object's error call.
 
         :param msg: the message to log
         :type msg: str
         :param exc_type: The type of Exception to raise with the same message as `msg`
         :type exc_type: :class:`Exception`, optional
-        :param reraise: if True, any :class:`Exception` object passed through the `exc_info` will be re-raised
-            after its traceback is logged.
+        :param reraise: if True, any :class:`Exception` object passed through the `exc_info`
+            will be re-raised after its traceback is logged.
         :type reraise: bool, optional
         """
-        if not msg.startswith('ERROR:') :
-            msg = f'ERROR: {msg}'
-        self._logger_obj.error(msg,**kwargs)
-        if reraise and ('exc_info' in kwargs) and isinstance(kwargs['exc_info'],Exception) :
-            raise kwargs['exc_info']
-        if exc_type is not None :
+        if not msg.startswith("ERROR:"):
+            msg = f"ERROR: {msg}"
+        self._logger_obj.error(msg, **kwargs)
+        if (
+            reraise
+            and ("exc_info" in kwargs)
+            and isinstance(kwargs["exc_info"], Exception)
+        ):
+            raise kwargs["exc_info"]
+        if exc_type is not None:
             raise exc_type(msg)
 
-class LogOwner(HasArguments) :
+
+class LogOwner(HasArguments):
     """
-    Any subclasses extending this one will have access to a Logger defined by the first class in the MRO to extend it
+    Any subclasses extending this one will have access to a Logger defined by
+    the first class in the MRO to extend it
 
-    :param logger: a :class:`~.utilities.Logger` object that this class should have access to. If this
-        parameter is given it will override any of the others provided.
+    :param logger: a :class:`~.utilities.Logger` object that this class should have access to.
+        If this parameter is given it will override any of the others provided.
     :type logger: :class:`~.utilities.Logger`, optional
-    :param logger_name: The name for the logger to use (automatically inferred from the running module if not given)
+    :param logger_name: The name for the logger to use
+        (automatically inferred from the running module if not given)
     :type logger_name: str, optional
     :param streamlevel: The level at/above which messages should be logged to the stream/console
     :type streamlevel: logging level int, optional
-    :param logger_filepath: The path to a logger file to use or directory in which an automatically-named
-        logger file should be created
+    :param logger_filepath: The path to a logger file to use or directory in which
+        an automatically-named logger file should be created
     :type logger_filepath: :class:`pathlib.Path`, optional
     :param filelevel: The level at/above which messages should be written to the logfile
     :type filelevel: logging level int, optional
     """
 
     @property
-    def logger(self) :
+    def logger(self):
         """
         The logger object that the class can use
         """
         return self.__logger
 
     @logger.setter
-    def logger(self,logger) :
-        if ( hasattr(self,'_LogOwner__logger') and
-             self.__logger is not None and
-             (not isinstance(self.__logger,type(logger))) ) :
-            errmsg = f'ERROR: tried to reset a logger of type {type(self.__logger)} to a new logger of type {logger}!'
-            self.__logger.error(errmsg,exc_type=ValueError)
-        else :
+    def logger(self, logger):
+        if (
+            hasattr(self, "_LogOwner__logger")
+            and self.__logger is not None
+            and (not isinstance(self.__logger, type(logger)))
+        ):
+            errmsg = (
+                f"ERROR: tried to reset a logger of type {type(self.__logger)} "
+                f"to a new logger of type {logger}!"
+            )
+            self.__logger.error(errmsg, exc_type=ValueError)
+        else:
             self.__logger = logger
 
-    def __init__(self,*args,
-                 logger=None,logger_name=None,streamlevel=logging.INFO,logger_file=None,filelevel=logging.WARNING,
-                 **other_kwargs) :
-        if logger is not None :
+    def __init__(
+        self,
+        *args,
+        logger=None,
+        logger_name=None,
+        streamlevel=logging.INFO,
+        logger_file=None,
+        filelevel=logging.WARNING,
+        **other_kwargs,
+    ):
+        if logger is not None:
             self.__logger = logger
-        else :
-            if logger_name is None :
+        else:
+            if logger_name is None:
                 logger_name = self.__class__.__name__
             logger_filepath = logger_file
-            if logger_file is not None and logger_file.is_dir() :
-                logger_filepath = logger_file / f'{self.__class__.__name__}.log'
-            self.__logger = Logger(logger_name,streamlevel,logger_filepath,filelevel)
-        super().__init__(*args,**other_kwargs)
+            if logger_file is not None and logger_file.is_dir():
+                logger_filepath = logger_file / f"{self.__class__.__name__}.log"
+            self.__logger = Logger(logger_name, streamlevel, logger_filepath, filelevel)
+        super().__init__(*args, **other_kwargs)
 
     @classmethod
-    def get_command_line_arguments(cls) :
+    def get_command_line_arguments(cls):
         """
         Return the names of arguments for the logger stream and file levels.
         """
         superargs, superkwargs = super().get_command_line_arguments()
-        return [*superargs,'logger_stream_level','logger_file_level'], superkwargs
+        return [*superargs, "logger_stream_level", "logger_file_level"], superkwargs
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/misc.py` & `openmsistream-1.4.0/openmsistream/utilities/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,91 +1,103 @@
 """Some miscellaneous functions that are universally internally available"""
 
-#imports
+# imports
 import os, sys, inspect, time, contextlib
 
-def add_user_input(input_queue) :
+
+def add_user_input(input_queue):
     """
     Listen for and add user input to a queue at one second intervals
     """
-    while True :
+    while True:
         time.sleep(1)
         input_queue.put((sys.stdin.read(1)).strip())
 
-def raise_err_with_optional_logger(logger,errmsg,exc_type) :
+
+def raise_err_with_optional_logger(logger, errmsg, exc_type):
     """
-    If logger is not None, log the error message with the given exception type, otherwise raise the error
+    If logger is not None, log the error message with the given exception type,
+    otherwise raise the error
     """
-    if logger is not None :
-        logger.error(errmsg,exc_type=exc_type)
-    else :
+    if logger is not None:
+        logger.error(errmsg, exc_type=exc_type)
+    else:
         raise exc_type(errmsg)
 
-def debug_msg_with_optional_logger(logger,msg) :
+
+def debug_msg_with_optional_logger(logger, msg):
     """
     Log a given message at debug level if logger is not None, otherwise print it
     """
-    if logger is not None :
+    if logger is not None:
         logger.debug(msg)
-    else :
+    else:
         print(msg)
 
-def _ensure_classes_or_types_match_for_key(key,test,options,logger=None) :
-    """
-    Raise errors if "test" is not a subclass of the possibilities in "options" if "options" holds classes,
-    or if the type of "test" is not in "options" if "options" holds objects
+
+def _ensure_classes_or_types_match_for_key(key, test, options, logger=None):
     """
-    #if the options are classes
-    if inspect.isclass(options[0] if isinstance(options,tuple) else options) :
-        #make sure the test argument is also a class
-        if not inspect.isclass(test) :
+    Raise errors if "test" is not a subclass of the possibilities in "options"
+    if "options" holds classes, or if the type of "test" is not in "options"
+    if "options" holds objects
+    """
+    # if the options are classes
+    if inspect.isclass(options[0] if isinstance(options, tuple) else options):
+        # make sure the test argument is also a class
+        if not inspect.isclass(test):
             errmsg = f'ERROR: Argument "{key}" expected to be a class, not an object!'
-            raise_err_with_optional_logger(logger,errmsg,RuntimeError)
-        #make sure the test argument is a subtype of any of the classes specified in the defaults
-        if not issubclass(test,options[1:] if isinstance(options,tuple) else options) :
-            errmsg = f'ERROR: Class type mismatch for argument "{key}", got {test} '
-            errmsg+= f'but expected {options[1:] if isinstance(options,tuple) else options}'
-            raise_err_with_optional_logger(logger,errmsg,RuntimeError)
-    #if the options are objects instead, make sure the type of the test argument matches
-    #one of the possible types in the defaults
-    elif ( (isinstance(options,tuple) and type(test) not in options[1:]) or
-           (not isinstance(options,tuple) and not isinstance(test,type(options))) ) :
-        errmsg = f'ERROR: Type mismatch replacing argument "{key}" with {test} '
-        errmsg+= '(expected '
-        if isinstance(options,tuple) :
-            for typestring in options[1:] :
-                errmsg+=f'{typestring}, '
-        else :
-            errmsg+=f'{type(options)}'
-        errmsg+=f'but got {type(test)})'
-        raise_err_with_optional_logger(logger,errmsg,TypeError)
+            raise_err_with_optional_logger(logger, errmsg, RuntimeError)
+        # make sure the test argument is a subtype of any of the classes in the defaults
+        if not issubclass(test, options[1:] if isinstance(options, tuple) else options):
+            errmsg = (
+                f'ERROR: Class type mismatch for argument "{key}", got {test} '
+                f"but expected {options[1:] if isinstance(options,tuple) else options}"
+            )
+            raise_err_with_optional_logger(logger, errmsg, RuntimeError)
+    # if the options are objects instead, make sure the type of the test argument matches
+    # one of the possible types in the defaults
+    elif (isinstance(options, tuple) and type(test) not in options[1:]) or (
+        not isinstance(options, tuple) and not isinstance(test, type(options))
+    ):
+        errmsg = f'ERROR: Type mismatch replacing argument "{key}" with {test} (expected '
+        if isinstance(options, tuple):
+            for typestring in options[1:]:
+                errmsg += f"{typestring}, "
+        else:
+            errmsg += f"{type(options)}"
+        errmsg += f"but got {type(test)})"
+        raise_err_with_optional_logger(logger, errmsg, TypeError)
+
 
-def populated_kwargs(given_kwargs,defaults,logger=None) :
+def populated_kwargs(given_kwargs, defaults, logger=None):
     """
     Return a kwargs dictionary where every possible entry from the defaults has a valid value
     Can use this to make sure certain entries are present in kwargs
     """
-    #for all the needed keys
-    for key in defaults.keys() :
-        #if it was given and is not None
-        if key in given_kwargs.keys() and given_kwargs[key] is not None :
+    # for all the needed keys
+    for key in defaults.keys():
+        # if it was given and is not None
+        if key in given_kwargs.keys() and given_kwargs[key] is not None:
             # if there's just the default option it doesn't need to be a tuple
-            if isinstance(defaults[key],tuple) :
-                if len(defaults[key])==1 :
+            if isinstance(defaults[key], tuple):
+                if len(defaults[key]) == 1:
                     defaults[key] = (defaults[key])[0]
-            #check the options for what the argument is allowed to be
-            _ensure_classes_or_types_match_for_key(key,given_kwargs[key],defaults[key],logger)
-        #if it wasn't given, then just add it to the dictionary as the default
-        else :
-            if isinstance(defaults[key],tuple) :
+            # check the options for what the argument is allowed to be
+            _ensure_classes_or_types_match_for_key(
+                key, given_kwargs[key], defaults[key], logger
+            )
+        # if it wasn't given, then just add it to the dictionary as the default
+        else:
+            if isinstance(defaults[key], tuple):
                 given_kwargs[key] = (defaults[key])[0]
-            else :
+            else:
                 given_kwargs[key] = defaults[key]
     return given_kwargs
 
+
 @contextlib.contextmanager
 def change_dir(dirpath):
     """
     Change the current working directory to a different directory,
     and go back when leaving the context manager.
     """
     cdminus = os.getcwd()
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/provision_wrapper.py` & `openmsistream-1.4.0/openmsistream/utilities/provision_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,187 @@
 """
 A wrapper around KafkaCrypto provision scripts to automatically
 move the output in the location expected by OpenMSIStream
 """
 
-#imports
+# imports
 import pathlib, shutil, logging, warnings
 from argparse import ArgumentParser
 import urllib.request
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import kafkacrypto
 from ..utilities.config import RUN_CONST
 from .logging import Logger
 from .config_file_parser import ConfigFileParser
 from .misc import change_dir
 
-#constants
-LOGGER = Logger('ProvisionNode',logging.INFO)
+# constants
+LOGGER = Logger("ProvisionNode", logging.INFO)
 KC_PATH = kafkacrypto.__path__
-SP_NAME = 'simple-provision.py'
-OP_NAME = 'online-provision.py'
-GITHUB_URL = f'https://raw.githubusercontent.com/tmcqueen-materials/kafkacrypto/master/tools/{SP_NAME}'
-TEMP_DIR_PATH = RUN_CONST.CONFIG_FILE_DIR/'temp_kafkacrypto_dir'
+SP_NAME = "simple-provision.py"
+OP_NAME = "online-provision.py"
+GITHUB_PREPEND = "https://raw.githubusercontent.com/"
+GITHUB_URL = f"{GITHUB_PREPEND}tmcqueen-materials/kafkacrypto/master/tools/{SP_NAME}"
+TEMP_DIR_PATH = RUN_CONST.CONFIG_FILE_DIR / "temp_kafkacrypto_dir"
+
 
-def get_script_location_and_code_from_input(args) :
+def get_script_location_and_code_from_input(args):
     """
     Use a given path to get the script code
     """
     p_code = None
     p_loc = None
-    if args.script_path.is_file() :
+    if args.script_path.is_file():
         p_loc = args.script_path
-        with open(args.script_path,'rb') as fp :
+        with open(args.script_path, "rb") as fp:
             p_code = fp.read()
-    #directory containing the script was given
-    elif args.script_path.is_dir() :
-        if (args.script_path/SP_NAME).is_file() :
-            p_loc = args.script_path/SP_NAME
-            with open(args.script_path/SP_NAME,'rb') as fp :
+    # directory containing the script was given
+    elif args.script_path.is_dir():
+        if (args.script_path / SP_NAME).is_file():
+            p_loc = args.script_path / SP_NAME
+            with open(args.script_path / SP_NAME, "rb") as fp:
                 p_code = fp.read()
-        elif (args.script_path/OP_NAME).is_file() :
-            p_loc = args.script_path/OP_NAME
-            with open(args.script_path/OP_NAME,'rb') as fp :
+        elif (args.script_path / OP_NAME).is_file():
+            p_loc = args.script_path / OP_NAME
+            with open(args.script_path / OP_NAME, "rb") as fp:
                 p_code = fp.read()
     return p_loc, p_code
 
-def get_script_location_and_code(args) :
+
+def get_script_location_and_code(args):
     """
     Return the location of the provision script and its text contents, given the arguments
     """
     p_code = None
     p_loc = None
     if args.script_path is not None:
-        #path to the script itself was given
+        # path to the script itself was given
         p_loc, p_code = get_script_location_and_code_from_input(args)
-    #if not set yet, try getting from the kafkacrypto install location (works if installed with --editable)
-    if len(KC_PATH)==1 :
-        if args.mode=='simple' :
-            to_try = pathlib.Path(KC_PATH[0]).parent/'tools'/SP_NAME
-        elif args.mode=='online' :
-            to_try = pathlib.Path(KC_PATH[0]).parent/'tools'/OP_NAME
-        if to_try.is_file() :
+    # if not set yet, try getting from the kafkacrypto install location
+    if len(KC_PATH) == 1:
+        if args.mode == "simple":
+            to_try = pathlib.Path(KC_PATH[0]).parent / "tools" / SP_NAME
+        elif args.mode == "online":
+            to_try = pathlib.Path(KC_PATH[0]).parent / "tools" / OP_NAME
+        if to_try.is_file():
             p_loc = to_try
-            with open(to_try,'rb') as fp :
+            with open(to_try, "rb") as fp:
                 p_code = fp.read()
-    if p_code is None :
-        #if all else fails, try getting from the Github webpage (only simple-provision can be fetched this way)
-        if args.mode=='simple' :
-            try :
-                with urllib.request.urlopen(GITHUB_URL) as urlp :
+    if p_code is None:
+        # if all else fails, try getting from the Github webpage
+        if args.mode == "simple":
+            try:
+                with urllib.request.urlopen(GITHUB_URL) as urlp:
                     p_code = urlp.read()
                 p_loc = GITHUB_URL
-            except Exception :
+            except Exception:
                 pass
-    if p_loc is None or p_code is None :
-        LOGGER.error('ERROR: failed to find the provisioning script to use!',exc_type=RuntimeError)
+    if p_loc is None or p_code is None:
+        LOGGER.error(
+            "ERROR: failed to find the provisioning script to use!", exc_type=RuntimeError
+        )
     return p_loc, p_code
 
-def move_files(p_loc) :
+
+def move_files(p_loc):
     """
     Move the created files into the expected locations
     """
-    try :
+    try:
         new_files = {}
-        exts = ['.config','.seed','.crypto']
-        for ext in exts :
+        exts = [".config", ".seed", ".crypto"]
+        for ext in exts:
             n_files = 0
-            for fp in TEMP_DIR_PATH.glob(f'*{ext}') :
-                n_files+=1
+            for fp in TEMP_DIR_PATH.glob(f"*{ext}"):
+                n_files += 1
                 new_files[ext] = fp.resolve()
-            if n_files!=1 :
-                LOGGER.error(f'ERROR: found {n_files} new {ext} files in {TEMP_DIR_PATH}',exc_type=RuntimeError)
+            if n_files != 1:
+                LOGGER.error(
+                    f"ERROR: found {n_files} new {ext} files in {TEMP_DIR_PATH}",
+                    exc_type=RuntimeError,
+                )
         node_id = None
-        for ext in exts :
+        for ext in exts:
             filename = new_files[ext].name
             this_node_id = ((filename).split(ext))[0]
-            if node_id is None :
+            if node_id is None:
                 node_id = this_node_id
-            elif node_id!=this_node_id :
-                errmsg = f'ERROR: found a file called {filename} that conflicts with node_id {node_id}!'
-                LOGGER.error(errmsg,exc_type=RuntimeError)
-        cfp = ConfigFileParser(new_files['.config'],logger=LOGGER)
-        default_dict = cfp.get_config_dict_for_groups('DEFAULT')
-        if 'node_id' not in default_dict :
-            LOGGER.error(f"ERROR: node_id not listed in {new_files['.config']}!",exc_type=ValueError)
-        elif default_dict['node_id']!=node_id :
-            errmsg = f"ERROR: node_id listed in {new_files['.config']} mismatched to filenames ({node_id})!"
-            LOGGER.error(errmsg,exc_type=ValueError)
-        new_dirpath = TEMP_DIR_PATH.parent/node_id
+            elif node_id != this_node_id:
+                errmsg = (
+                    f"ERROR: found a file called {filename} "
+                    f"that conflicts with node_id {node_id}!"
+                )
+                LOGGER.error(errmsg, exc_type=RuntimeError)
+        cfp = ConfigFileParser(new_files[".config"], logger=LOGGER)
+        default_dict = cfp.get_config_dict_for_groups("DEFAULT")
+        if "node_id" not in default_dict:
+            LOGGER.error(
+                f"ERROR: node_id not listed in {new_files['.config']}!",
+                exc_type=ValueError,
+            )
+        elif default_dict["node_id"] != node_id:
+            errmsg = (
+                f"ERROR: node_id listed in {new_files['.config']} mismatched "
+                f"to filenames ({node_id})!"
+            )
+            LOGGER.error(errmsg, exc_type=ValueError)
+        new_dirpath = TEMP_DIR_PATH.parent / node_id
         TEMP_DIR_PATH.rename(new_dirpath)
         LOGGER.info(f'Successfuly set up new KafkaCrypto node called "{node_id}"')
-    except Exception as exc :
-        errmsg = f'ERROR: Running {p_loc} did not produce the expected output! Temporary directories '
-        errmsg+= 'will be removed and you will need to try again. Exception will be logged and re-raised.'
-        LOGGER.error(errmsg,exc_info=exc,reraise=True)
-    finally :
-        if TEMP_DIR_PATH.is_dir() :
+    except Exception as exc:
+        errmsg = (
+            f"ERROR: Running {p_loc} did not produce the expected output! "
+            "Temporary directories will be removed and you will need to try again. "
+            "Exception will be logged and re-raised."
+        )
+        LOGGER.error(errmsg, exc_info=exc, reraise=True)
+    finally:
+        if TEMP_DIR_PATH.is_dir():
             shutil.rmtree(TEMP_DIR_PATH)
 
-def main() :
+
+def main():
     """
     Script to run either simple or online provision for KafkaCrypto and
     move the output to the location expected by OpenMSIStream
     """
-    #command line arguments
+    # command line arguments
     parser = ArgumentParser()
     group = parser.add_mutually_exclusive_group()
-    group.add_argument('--mode', choices=['simple','online'], default='simple',
-                       help='''Choice of which known type of provisioning to use.
-                               Can also provide a path to the script to run instead.''')
-    group.add_argument('--script-path', type=pathlib.Path, default='.',
-                        help='Path to the provision script to run')
+    group.add_argument(
+        "--mode",
+        choices=["simple", "online"],
+        default="simple",
+        help="""Choice of which known type of provisioning to use.
+                               Can also provide a path to the script to run instead.""",
+    )
+    group.add_argument(
+        "--script-path",
+        type=pathlib.Path,
+        default=".",
+        help="Path to the provision script to run",
+    )
     args = parser.parse_args()
-    if TEMP_DIR_PATH.is_dir() :
+    if TEMP_DIR_PATH.is_dir():
         shutil.rmtree(TEMP_DIR_PATH)
-    #get the location/content of the simple-provision script
+    # get the location/content of the simple-provision script
     p_loc, p_code = get_script_location_and_code(args)
-    #run the script
-    try :
-        if not TEMP_DIR_PATH.is_dir() :
+    # run the script
+    try:
+        if not TEMP_DIR_PATH.is_dir():
             TEMP_DIR_PATH.mkdir(parents=True)
-        with change_dir(TEMP_DIR_PATH) :
+        with change_dir(TEMP_DIR_PATH):
             exec(p_code)
-    except Exception as exc :
-        errmsg = f'ERROR: failed to run provisioning using {p_loc}! Exception will be logged and re-raised.'
-        LOGGER.error(errmsg,exc_info=exc,reraise=True)
-    #make sure required files exist and move them into a new directory named for the node_ID
+    except Exception as exc:
+        errmsg = (
+            f"ERROR: failed to run provisioning using {p_loc}! "
+            "Exception will be logged and re-raised."
+        )
+        LOGGER.error(errmsg, exc_info=exc, reraise=True)
+    # make sure required files exist and move them into a new directory named for the node_ID
     move_files(p_loc)
 
-if __name__=='__main__' :
+
+if __name__ == "__main__":
     main()
```

### Comparing `openmsistream-1.3.4/openmsistream/utilities/runnable.py` & `openmsistream-1.4.0/openmsistream/utilities/runnable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 """
-Class defining the general OpenMSIStream workflow for running from the command line (or as a Service/daemon)
+Class defining the general OpenMSIStream workflow for running from the command line
+(or as a Service/daemon)
 """
 
-#imports
+# imports
 from abc import ABC, abstractmethod
 from .has_arguments import HasArguments
 from .has_argument_parser import HasArgumentParser
 from .argument_parsing import OpenMSIStreamArgumentParser
 
-class Runnable(HasArguments,HasArgumentParser,ABC) :
+
+class Runnable(HasArguments, HasArgumentParser, ABC):
     """
     Abstract base class for any child classes that want to define some behavior
     for running from the command line (i.e. as a module)
     """
 
     ARGUMENT_PARSER_TYPE = OpenMSIStreamArgumentParser
 
     @classmethod
-    def get_argument_parser(cls,*args,**kwargs) :
+    def get_argument_parser(cls, *args, **kwargs):
         """
         Get the argument parser used to run the code
 
         :param args: Any arguments to this method are names of arguments recognized
             by Argument parsers of the :attr:`~Runnable.ARGUMENT_PARSER_TYPE` type
         :type args: list
-        :param kwargs: Any keyword arguments to this method define custom default values for their given arguments,
-            whose names must be recognized by Argument parsers of the :attr:`~Runnable.ARGUMENT_PARSER_TYPE` type
+        :param kwargs: Any keyword arguments to this method define custom default values
+            for their given arguments, whose names must be recognized by Argument parsers
+            of the :attr:`~Runnable.ARGUMENT_PARSER_TYPE` type
         :type kwargs: dict
 
-        :return: An argument parser of the :attr:`~Runnable.ARGUMENT_PARSER_TYPE` type to use for the object
+        :return: An argument parser of the :attr:`~Runnable.ARGUMENT_PARSER_TYPE` type to use
+            for the object
         """
-        parser = cls.ARGUMENT_PARSER_TYPE(*args,**kwargs)
+        parser = cls.ARGUMENT_PARSER_TYPE(*args, **kwargs)
         cl_args, cl_kwargs = cls.get_command_line_arguments()
-        parser.add_arguments(*cl_args,**cl_kwargs)
+        parser.add_arguments(*cl_args, **cl_kwargs)
         return parser
 
     @classmethod
     @abstractmethod
-    def run_from_command_line(cls,args=None) :
+    def run_from_command_line(cls, args=None):
         """
-        Child classes should implement this function to do whatever it is they do when they run from the command line
+        Child classes should implement this function to do whatever it is they do
+        when they run from the command line
 
-        :param args: the list of arguments to send to the parser instead of getting them from sys.argv
+        :param args: the list of arguments to send to the parser instead of
+            getting them from sys.argv
         :type args: list
         """
         raise NotImplementedError
```

### Comparing `openmsistream-1.3.4/openmsistream.egg-info/PKG-INFO` & `openmsistream-1.4.0/openmsistream.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.3.4.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.4.0.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
@@ -18,15 +18,15 @@
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 
-[![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![GitHub Release Date](https://img.shields.io/github/release-date/openmsi/openmsistream) ![GitHub last commit](https://img.shields.io/github/last-commit/openmsi/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
+[![JOSS DOI](https://joss.theoj.org/papers/10.21105/joss.04896/status.svg)](https://doi.org/10.21105/joss.04896) ![PyPI](https://img.shields.io/pypi/v/openmsistream) ![License](https://img.shields.io/github/license/openmsi/openmsistream) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openmsistream) ![CircleCI](https://img.shields.io/circleci/build/github/openmsi/openmsistream/main) [![Documentation Status](https://readthedocs.org/projects/openmsistream/badge/?version=latest)](https://openmsistream.readthedocs.io/en/latest/?badge=latest) [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/PyCQA/pylint)
 
 Applications for laboratory, analysis, and computational materials data streaming using [Apache Kafka](https://kafka.apache.org/)
 
 Available on PyPI at https://pypi.org/project/openmsistream and GitHub at https://github.com/openmsi/openmsistream 
 
 Official documentation at https://openmsistream.readthedocs.io/en/latest/
```

### Comparing `openmsistream-1.3.4/openmsistream.egg-info/SOURCES.txt` & `openmsistream-1.4.0/openmsistream.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 openmsistream/__init__.py
 openmsistream.egg-info/PKG-INFO
 openmsistream.egg-info/SOURCES.txt
 openmsistream.egg-info/dependency_links.txt
 openmsistream.egg-info/entry_points.txt
@@ -26,14 +27,15 @@
 openmsistream/data_file_io/entity/__init__.py
 openmsistream/data_file_io/entity/data_file.py
 openmsistream/data_file_io/entity/data_file_chunk.py
 openmsistream/data_file_io/entity/data_file_directory.py
 openmsistream/data_file_io/entity/download_data_file.py
 openmsistream/data_file_io/entity/reproducer_message.py
 openmsistream/data_file_io/entity/upload_data_file.py
+openmsistream/data_file_io/entity/upload_directory_event_handler.py
 openmsistream/kafka_wrapper/__init__.py
 openmsistream/kafka_wrapper/config_file_parser.py
 openmsistream/kafka_wrapper/consumer_and_producer_group.py
 openmsistream/kafka_wrapper/consumer_group.py
 openmsistream/kafka_wrapper/controlled_message_processor.py
 openmsistream/kafka_wrapper/controlled_message_reproducer.py
 openmsistream/kafka_wrapper/openmsistream_consumer.py
```

### Comparing `openmsistream-1.3.4/openmsistream.egg-info/entry_points.txt` & `openmsistream-1.4.0/openmsistream.egg-info/entry_points.txt`

 * *Files identical despite different names*

