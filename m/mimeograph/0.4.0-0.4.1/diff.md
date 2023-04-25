# Comparing `tmp/mimeograph-0.4.0.tar.gz` & `tmp/mimeograph-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.4.0.tar", last modified: Mon Apr 24 16:21:39 2023, max compression
+gzip compressed data, was "mimeograph-0.4.1.tar", last modified: Tue Apr 25 07:14:50 2023, max compression
```

## Comparing `mimeograph-0.4.0.tar` & `mimeograph-0.4.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.763099 mimeograph-0.4.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-24 16:21:39.763099 mimeograph-0.4.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    20615 2023-04-24 13:03:27.000000 mimeograph-0.4.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2023-04-24 16:21:01.000000 mimeograph-0.4.0/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 16:21:39.763099 mimeograph-0.4.0/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.751099 mimeograph-0.4.0/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-24 16:21:01.000000 mimeograph-0.4.0/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9574 2023-04-24 16:21:01.000000 mimeograph-0.4.0/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      553 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12842 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-20 08:22:52.000000 mimeograph-0.4.0/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/annotations.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6402 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)      194 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      165 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2101 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      860 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2128 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      101 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/exc.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-20 08:22:48.000000 mimeograph-0.4.0/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      680 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5677 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-20 08:22:47.000000 mimeograph-0.4.0/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-20 08:22:45.000000 mimeograph-0.4.0/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      458 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)      330 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8714 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7286 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/utils/renderer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.763099 mimeograph-0.4.0/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1774 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       98 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.763099 mimeograph-0.4.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    31417 2023-04-24 13:03:27.000000 mimeograph-0.4.0/tests/test_mimeo_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 09:39:06.000000 mimeograph-0.4.0/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      465 2023-04-24 13:03:27.000000 mimeograph-0.4.0/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.511719 mimeograph-0.4.1/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.1/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.1/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-25 07:14:50.511719 mimeograph-0.4.1/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20615 2023-04-24 13:03:27.000000 mimeograph-0.4.1/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2023-04-25 07:14:26.000000 mimeograph-0.4.1/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-25 07:14:50.511719 mimeograph-0.4.1/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-25 07:13:50.000000 mimeograph-0.4.1/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9574 2023-04-25 07:13:50.000000 mimeograph-0.4.1/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      553 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12842 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.503719 mimeograph-0.4.1/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-20 08:22:52.000000 mimeograph-0.4.1/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/annotations.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6402 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      194 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      165 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2101 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      860 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2128 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      101 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/exc.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-20 08:22:48.000000 mimeograph-0.4.1/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      680 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5677 2023-04-24 16:19:51.000000 mimeograph-0.4.1/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-20 08:22:47.000000 mimeograph-0.4.1/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-20 08:22:45.000000 mimeograph-0.4.1/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.1/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      458 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.507719 mimeograph-0.4.1/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      330 2023-04-24 13:03:27.000000 mimeograph-0.4.1/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 09:39:06.000000 mimeograph-0.4.1/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8714 2023-04-25 07:12:18.000000 mimeograph-0.4.1/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7433 2023-04-25 07:12:18.000000 mimeograph-0.4.1/src/mimeo/utils/renderer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.511719 mimeograph-0.4.1/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1774 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       98 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-25 07:14:50.000000 mimeograph-0.4.1/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-25 07:14:50.511719 mimeograph-0.4.1/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    31417 2023-04-24 13:03:27.000000 mimeograph-0.4.1/tests/test_mimeo_cli.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 09:39:06.000000 mimeograph-0.4.1/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      465 2023-04-24 13:03:27.000000 mimeograph-0.4.1/tests/test_tools.py
```

### Comparing `mimeograph-0.4.0/LICENSE` & `mimeograph-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/PKG-INFO` & `mimeograph-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mimeograph-0.4.0/README.md` & `mimeograph-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/pyproject.toml` & `mimeograph-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.4.0"
+version = "0.4.1"
 description = "Generate data based on a simple template"
 readme = "README.md"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
@@ -32,15 +32,15 @@
 [project.optional-dependencies]
 dev = ["bumpver", "build", "twine", "pylama", "isort", "pytest", "pytest-cov", "responses"]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.4.0"
+current_version = "0.4.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mimeograph-0.4.0/src/mimeo/__main__.py` & `mimeograph-0.4.1/src/mimeo/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         super().__init__(
             prog="mimeo",
             description="Generate data based on a template")
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.4.0")
+            version="%(prog)s v0.4.1")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configurations")
 
         mimeo_config_args = self.add_argument_group("Mimeo Configuration arguments")
```

### Comparing `mimeograph-0.4.0/src/mimeo/config/exc.py` & `mimeograph-0.4.1/src/mimeo/config/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/config/mimeo_config.py` & `mimeograph-0.4.1/src/mimeo/config/mimeo_config.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.4.1/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.4.1/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.4.1/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/context/annotations.py` & `mimeograph-0.4.1/src/mimeo/context/annotations.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/context/mimeo_context.py` & `mimeograph-0.4.1/src/mimeo/context/mimeo_context.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.4.1/src/mimeo/context/mimeo_context_manager.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.4.1/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/database/cities.py` & `mimeograph-0.4.1/src/mimeo/database/cities.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/database/countries.py` & `mimeograph-0.4.1/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/database/first_names.py` & `mimeograph-0.4.1/src/mimeo/database/first_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/database/last_names.py` & `mimeograph-0.4.1/src/mimeo/database/last_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/database/mimeo_db.py` & `mimeograph-0.4.1/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/generators/generator.py` & `mimeograph-0.4.1/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/generators/generator_factory.py` & `mimeograph-0.4.1/src/mimeo/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/generators/xml_generator.py` & `mimeograph-0.4.1/src/mimeo/generators/xml_generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/meta/alive.py` & `mimeograph-0.4.1/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/mimeo.py` & `mimeograph-0.4.1/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/resources/cities.csv` & `mimeograph-0.4.1/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/resources/countries.csv` & `mimeograph-0.4.1/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/resources/forenames.csv` & `mimeograph-0.4.1/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/resources/logging.yaml` & `mimeograph-0.4.1/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/resources/surnames.txt` & `mimeograph-0.4.1/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.4.1/src/mimeo/utils/mimeo_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class RandomIntegerUtil(MimeoUtil):
 
     KEY = "random_int"
 
     def __init__(self, **kwargs):
-        self.__start = kwargs.get("limit", 1)
+        self.__start = kwargs.get("start", 1)
         self.__limit = kwargs.get("limit", 100)
 
     def render(self):
         return random.randrange(self.__start, self.__limit + 1)
 
 
 class RandomItemUtil(MimeoUtil):
```

### Comparing `mimeograph-0.4.0/src/mimeo/utils/renderer.py` & `mimeograph-0.4.1/src/mimeo/utils/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,13 +169,15 @@
         rendered_value = UtilsRenderer.render_raw(value[1:][:-1])
         return cls.render(rendered_value)
 
     @classmethod
     def _render_parametrized_mimeo_util(cls, value: dict):
         mimeo_util = value[MimeoConfig.MODEL_MIMEO_UTIL_KEY]
         mimeo_util = cls._render_mimeo_util_parameters(mimeo_util)
+        logger.fine(f"Pre-rendered mimeo util [{mimeo_util}]")
         rendered_value = UtilsRenderer.render_parametrized(mimeo_util)
         return cls.render(rendered_value)
 
     @classmethod
     def _render_mimeo_util_parameters(cls, mimeo_util_config: dict) -> dict:
-        return {key: cls.render(value) for key, value in mimeo_util_config.items()}
+        logger.fine("Rendering mimeo util parameters")
+        return {key: cls.render(value) if key != "_name" else value for key, value in mimeo_util_config.items()}
```

### Comparing `mimeograph-0.4.0/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.4.1/src/mimeograph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mimeograph-0.4.0/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.4.1/src/mimeograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/tests/test_mimeo_cli.py` & `mimeograph-0.4.1/tests/test_mimeo_cli.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.0/tests/test_mimeograph.py` & `mimeograph-0.4.1/tests/test_mimeograph.py`

 * *Files identical despite different names*

