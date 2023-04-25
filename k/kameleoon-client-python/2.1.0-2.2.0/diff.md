# Comparing `tmp/kameleoon-client-python-2.1.0.tar.gz` & `tmp/kameleoon-client-python-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kameleoon-client-python-2.1.0.tar", last modified: Thu Feb  2 12:35:07 2023, max compression
+gzip compressed data, was "kameleoon-client-python-2.2.0.tar", last modified: Tue Apr 25 07:14:20 2023, max compression
```

## Comparing `kameleoon-client-python-2.1.0.tar` & `kameleoon-client-python-2.2.0.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.154809 kameleoon-client-python-2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       52 2021-11-12 07:27:06.000000 kameleoon-client-python-2.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10298 2023-02-02 12:35:07.154809 kameleoon-client-python-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9427 2023-01-30 08:55:57.000000 kameleoon-client-python-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.114808 kameleoon-client-python-2.1.0/kameleoon/
--rw-rw-rw-   0 root         (0) root         (0)      187 2021-10-18 08:53:33.000000 kameleoon-client-python-2.1.0/kameleoon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    66204 2023-02-02 04:03:27.000000 kameleoon-client-python-2.1.0/kameleoon/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-01-24 06:17:12.000000 kameleoon-client-python-2.1.0/kameleoon/client_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.114808 kameleoon-client-python-2.1.0/kameleoon/configuration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-01-27 11:32:52.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/feature_flag_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     1960 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/rule.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/variable.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-01-27 11:32:52.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/variation.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/configuration/variation_by_exposition.py
--rw-rw-rw-   0 root         (0) root         (0)     6673 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/data.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-02-02 04:03:27.000000 kameleoon-client-python-2.1.0/kameleoon/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     3890 2023-01-27 12:05:12.000000 kameleoon-client-python-2.1.0/kameleoon/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.115808 kameleoon-client-python-2.1.0/kameleoon/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-10-18 08:53:33.000000 kameleoon-client-python-2.1.0/kameleoon/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/helpers/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3160 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/helpers/functions.py
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/helpers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/helpers/multi_threading.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/helpers/repeat_timer.py
--rw-rw-rw-   0 root         (0) root         (0)     1961 2021-10-18 08:53:33.000000 kameleoon-client-python-2.1.0/kameleoon/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.115808 kameleoon-client-python-2.1.0/kameleoon/real_time/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-08 12:03:33.000000 kameleoon-client-python-2.1.0/kameleoon/real_time/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2928 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/real_time/real_time_configuration_service.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/real_time/real_time_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.115808 kameleoon-client-python-2.1.0/kameleoon/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-05 11:57:47.000000 kameleoon-client-python-2.1.0/kameleoon/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2474 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/storage/varation_storage.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/storage/visitor_variation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.116809 kameleoon-client-python-2.1.0/kameleoon/targeting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-10-18 08:53:33.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.116809 kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-10-18 08:53:33.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3482 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/custom_datum.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/exclusive_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/target_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5763 2023-01-26 15:15:24.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/tree_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-01-26 14:38:45.000000 kameleoon-client-python-2.1.0/kameleoon/targeting/tree_condition_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-01-24 04:14:05.000000 kameleoon-client-python-2.1.0/kameleoon/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.117808 kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10298 2023-02-02 12:35:07.000000 kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2023-02-02 12:35:07.000000 kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-02 12:35:07.000000 kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      397 2023-02-02 12:35:07.000000 kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-02 12:35:07.000000 kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-02-02 12:35:07.154809 kameleoon-client-python-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3377 2021-11-12 07:27:06.000000 kameleoon-client-python-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.113808 kameleoon-client-python-2.1.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.110808 kameleoon-client-python-2.1.0/tests/integration/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.117808 kameleoon-client-python-2.1.0/tests/integration/proj/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.135809 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      605 2022-10-21 06:30:26.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.142809 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/models.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2023-01-30 08:55:57.000000 kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/views.py
--rwxrwxrwx   0 root         (0) root         (0)      772 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.142809 kameleoon-client-python-2.1.0/tests/integration/proj/proj/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/proj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/proj/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3308 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/proj/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/proj/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2021-11-11 09:38:25.000000 kameleoon-client-python-2.1.0/tests/integration/proj/proj/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 12:35:07.143808 kameleoon-client-python-2.1.0/tests/resources/
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-11-14 10:25:45.000000 kameleoon-client-python-2.1.0/tests/resources/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.211462 kameleoon-client-python-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10298 2023-04-25 07:14:20.211462 kameleoon-client-python-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9427 2023-01-30 09:46:34.000000 kameleoon-client-python-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.185462 kameleoon-client-python-2.2.0/kameleoon/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2021-08-02 18:42:51.000000 kameleoon-client-python-2.2.0/kameleoon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    65734 2023-04-25 04:12:12.000000 kameleoon-client-python-2.2.0/kameleoon/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-01-24 06:17:59.000000 kameleoon-client-python-2.2.0/kameleoon/client_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.186462 kameleoon-client-python-2.2.0/kameleoon/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-04-25 04:12:12.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/feature_flag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-04-25 04:12:12.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1304 2023-04-25 04:12:12.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/variable.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-01-27 11:33:40.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/variation.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/configuration/variation_by_exposition.py
+-rw-rw-rw-   0 root         (0) root         (0)     7369 2023-03-16 12:35:52.000000 kameleoon-client-python-2.2.0/kameleoon/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-02-02 04:05:00.000000 kameleoon-client-python-2.2.0/kameleoon/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     3890 2023-01-27 12:11:57.000000 kameleoon-client-python-2.2.0/kameleoon/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.186462 kameleoon-client-python-2.2.0/kameleoon/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-02 18:42:51.000000 kameleoon-client-python-2.2.0/kameleoon/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/helpers/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2023-04-25 04:12:12.000000 kameleoon-client-python-2.2.0/kameleoon/helpers/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/helpers/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/helpers/multi_threading.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/helpers/repeat_timer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2021-08-02 18:42:51.000000 kameleoon-client-python-2.2.0/kameleoon/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.187462 kameleoon-client-python-2.2.0/kameleoon/real_time/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-08 12:16:41.000000 kameleoon-client-python-2.2.0/kameleoon/real_time/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2928 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/real_time/real_time_configuration_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/real_time/real_time_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.187462 kameleoon-client-python-2.2.0/kameleoon/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-05 11:57:47.000000 kameleoon-client-python-2.2.0/kameleoon/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2023-04-25 03:46:51.000000 kameleoon-client-python-2.2.0/kameleoon/storage/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-04-25 03:46:51.000000 kameleoon-client-python-2.2.0/kameleoon/storage/cache_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-04-25 03:46:51.000000 kameleoon-client-python-2.2.0/kameleoon/storage/cache_factory_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-25 03:46:51.000000 kameleoon-client-python-2.2.0/kameleoon/storage/cache_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/storage/varation_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/storage/visitor_variation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.188462 kameleoon-client-python-2.2.0/kameleoon/targeting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-02 18:42:51.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.188462 kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-02 18:42:51.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-25 03:46:51.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/custom_datum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/exclusive_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/target_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5763 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/tree_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-01-26 15:13:56.000000 kameleoon-client-python-2.2.0/kameleoon/targeting/tree_condition_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-24 07:06:37.000000 kameleoon-client-python-2.2.0/kameleoon/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.188462 kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10298 2023-04-25 07:14:20.000000 kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-04-25 07:14:20.000000 kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:14:20.000000 kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-25 07:14:20.000000 kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-25 07:14:20.000000 kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-04-25 07:14:20.212462 kameleoon-client-python-2.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3377 2021-11-11 12:25:32.000000 kameleoon-client-python-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.184462 kameleoon-client-python-2.2.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.184462 kameleoon-client-python-2.2.0/tests/integration/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.189462 kameleoon-client-python-2.2.0/tests/integration/proj/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.207462 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      605 2022-10-21 06:16:11.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.207462 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-25 04:12:12.000000 kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/views.py
+-rwxrwxrwx   0 root         (0) root         (0)      772 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.208462 kameleoon-client-python-2.2.0/tests/integration/proj/proj/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/proj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/proj/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3308 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/proj/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/proj/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2021-11-11 09:41:31.000000 kameleoon-client-python-2.2.0/tests/integration/proj/proj/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:14:20.208462 kameleoon-client-python-2.2.0/tests/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2022-08-08 12:00:56.000000 kameleoon-client-python-2.2.0/tests/resources/config.yml
```

### Comparing `kameleoon-client-python-2.1.0/PKG-INFO` & `kameleoon-client-python-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kameleoon-client-python
-Version: 2.1.0
+Version: 2.2.0
 Summary: Kameleoon Client Python Software Development Kit.
 Home-page: https://developers.kameleoon.com/python-sdk.html
 Author: Kameleoon
 Author-email: sdk@kameleoon.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kameleoon-client-python-2.1.0/README.md` & `kameleoon-client-python-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/client.py` & `kameleoon-client-python-2.2.0/kameleoon/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 from urllib.parse import urlencode
 import warnings
 from dateutil import parser
 
 import requests
 from requests import Response
 from kameleoon.client_configuration import KameleoonClientConfiguration
-from kameleoon.configuration.feature_flag_v2 import FeatureFlagV2
+from kameleoon.configuration.feature_flag import FeatureFlag
 from kameleoon.configuration.rule import Rule
 from kameleoon.configuration.settings import Settings
 from kameleoon.configuration.variation import Variation
+from kameleoon.configuration.variation_by_exposition import VariationByExposition
+from kameleoon.hybrid.hybrid_manager_impl import HybridManagerImpl
+from kameleoon.storage.cache_factory_impl import CacheFactoryImpl
 
 from kameleoon.data import Conversion, get_nonce, Data, UserAgent
 from kameleoon.defaults import (
     DEFAULT_CONFIGURATION_PATH,
     DEFAULT_TIMEOUT_MILLISECONDS,
     DEFAULT_VISITOR_DATA_MAXIMUM_SIZE,
     DEFAULT_CONFIGURATION_UPDATE_INTERVAL,
@@ -41,15 +44,15 @@
     VariationConfigurationNotFound,
     FeatureConfigurationNotFound,
     FeatureVariableNotFound,
 )
 from kameleoon.helpers.functions import (
     check_visitor_code,
     obtain_hash_double,
-    obtain_hash_double_v2,
+    obtain_hash_double_rule,
     get_size,
     read_kameleoon_cookie_value,
 )
 from kameleoon.helpers.logger import get_logger
 from kameleoon.helpers.config import config
 from kameleoon.targeting.models import Segment
 
@@ -60,14 +63,15 @@
 REFERENCE = 0
 X_PAGINATION_PAGE_COUNT = "X-Pagination-Page-Count"
 SEGMENT = "targetingSegment"
 KAMELEOON_TRACK_EXPERIMENT_THREAD = "KameleoonTrackExperimentThread"
 KAMELEOON_TRACK_DATA_THREAD = "KameleoonTrackDataThread"
 STATUS_ACTIVE = "ACTIVE"
 FEATURE_STATUS_DEACTIVATED = "DEACTIVATED"
+HYBRID_MANAGER_CACHE_TIMEOUT_SECONDS = 5.0
 
 
 # pylint: disable=R0904
 class KameleoonClient:
     """
     KameleoonClient
 
@@ -111,29 +115,33 @@
                                 This field is optional set to None by default.
         :type configuration: KameleoonClientConfiguration
         :param logger: Optional component which provides a log method to log messages. By default see method get_logger.
         """
         # pylint: disable=too-many-instance-attributes
         # Eight is reasonable in this case.
         self.site_code = site_code
-        self.experiments: List[Dict[str, Any]] = []
-        self.feature_flags: List[Dict[str, str]] = []
-        self.feature_flags_v2: List[FeatureFlagV2] = []
+        self._experiments: List[Dict[str, Any]] = []
+        self._feature_flags: List[FeatureFlag] = []
         self.settings = Settings()
         self.logger = logger or get_logger()
         self.automation_base_url = "https://api.kameleoon.com/"
         self.client_config_url = "https://client-config.kameleoon.com/"
         self.api_data_url = "https://api-data.kameleoon.com/"
         self.events_url = "https://events.kameleoon.com:8110/"
         self.variation_storage = VariationStorage()
         self.real_time_configuration_service: Optional[
             RealTimeConfigurationService
         ] = None
         self.update_configuration_handler: Optional[Callable[[], None]] = None
         self._setup_client_configuration(configuration_path, configuration_object)
+        self.hybrid_manager = HybridManagerImpl(
+            HYBRID_MANAGER_CACHE_TIMEOUT_SECONDS,
+            CacheFactoryImpl(),
+            self.multi_threading,
+        )
 
         self.data: Dict[str, List[Data]] = {}
         self.user_agent_data: Dict[str, UserAgent] = {}
 
         self._init_fetch_configuration()
 
     def __del__(self):
@@ -242,50 +250,43 @@
                 response = JsonResponse({...})
                 # set a cookie
                 response.set_cookie(**kameleoon_cookie)
         """
         # pylint: disable=too-many-locals,no-else-return,no-else-raise
         # pylint: disable=too-many-branches,too-many-statements,too-many-nested-blocks
         check_visitor_code(visitor_code)
-        try:
-            experiment = [
+        experiment = next(
+            (
                 experiment
-                for experiment in self.experiments
-                if int(experiment["id"]) == int(experiment_id)
-            ][0]
-        except IndexError as ex:
-            raise ExperimentConfigurationNotFound from ex
-        self._check_site_code_enable(experiment)
-        if self._check_targeting(visitor_code, experiment):
-            saved_variation_id = self._is_valid_saved_variation(
-                visitor_code, experiment_id, experiment["respoolTime"]
-            )
-            variation_id = (
-                saved_variation_id
-                or self._calculate_variation_for_experiment(visitor_code, experiment)
-            )
-            if variation_id is not None:
-                self._track_experiment_multithread(
-                    visitor_code, experiment_id, variation_id
-                )
-                if saved_variation_id is None:
-                    self.variation_storage.update_variation(
-                        visitor_code=visitor_code,
-                        experiment_id=experiment_id,
-                        variation_id=variation_id,
-                    )
+                for experiment in self._experiments
+                if experiment["id"] == experiment_id
+            ),
+            None,
+        )
+        if not experiment:
+            raise ExperimentConfigurationNotFound(experiment_id)
+        self.__check_site_code_enable(experiment)
+        if self.__check_targeting(visitor_code, experiment):
+            # Disable storage (sticky allocation)
+            # saved_variation_id = self.__is_valid_saved_variation(
+            #     visitor_code, experiment_id, experiment["respoolTime"]
+            # )
+            variation_id = self.__calculate_variation_for_experiment(
+                visitor_code, experiment
+            )
+            none_variation = variation_id is None
+            self.__send_tracking_request(
+                visitor_code, experiment_id, variation_id, none_variation
+            )
+            if not none_variation:
+                self.__save_variation(visitor_code, experiment_id, variation_id)
                 return variation_id
             else:
-                self._track_experiment_multithread(
-                    visitor_code, experiment_id, REFERENCE, True
-                )
-                raise NotAllocated(
-                    visitor_code=visitor_code, campaign_key_id=experiment_id
-                )
-        raise NotTargeted(visitor_code=visitor_code, campaign_key_id=experiment_id)
+                raise NotAllocated(visitor_code, experiment_id)
+        raise NotTargeted(visitor_code, experiment_id)
 
     def add_data(self, visitor_code: str, *args) -> None:
         """
         To associate various data with the current user, we can use the add_data() method.
         This method requires the visitor_code as a first parameter, and then accepts several additional parameters.
         These additional parameters represent the various Data Types allowed in Kameleoon.
 
@@ -428,15 +429,15 @@
         """
         variations = list(
             filter(
                 lambda variation: variation["id"] == variation_id,
                 [
                     variation
                     for variations in [
-                        experiment["variations"] for experiment in self.experiments
+                        experiment["variations"] for experiment in self._experiments
                     ]
                     for variation in variations
                 ],
             )
         )
         if not variations:
             raise VariationConfigurationNotFound(variation_id)
@@ -497,20 +498,20 @@
                 except FeatureConfigurationNotFound:
                     # The user will not be counted into the experiment, but should see the reference variation
                     logger.debug(...)
 
                 if has_new_checkout:
                     # Implement new checkout code here
         """
-        (_, variation_key) = self._get_feature_variation_key(visitor_code, feature_key)
+        (_, variation_key) = self.__get_feature_variation_key(visitor_code, feature_key)
         return variation_key != Variation.Type.OFF.value
 
     def obtain_feature_variable(
-        self, feature_key: Union[str, int], variable_key: str
-    ) -> Union[bool, str, float, Dict[str, Any]]:
+        self, feature_key: str, variable_key: str
+    ) -> Union[bool, str, float, Dict[str, Any], None]:
         """
         Retrieve a feature variable.
         A feature variable can be changed easily via our web application.
 
         :param feature_key: Union[str, int] ID or Key of the feature you want to obtain to a user.
                             This field is mandatory.
         :param variable_key: str  Key of the variable. This field is mandatory.
@@ -540,28 +541,20 @@
         """
         warnings.warn(
             "Call to deprecated function `obtain_feature_variable`. "
             "Please use `get_feature_variable` instead.",
             category=DeprecationWarning,
             stacklevel=2,
         )
-        # pylint: disable=no-else-raise
-        self._check_feature_key(feature_key)
-        feature_flag = self.get_feature_flag(feature_key)
-        custom_json = None
-        try:
-            custom_json = json.loads(feature_flag["variations"][0]["customJson"])[
-                variable_key
-            ]
-        except (IndexError, KeyError) as ex:
-            self.logger.error(ex)
-            raise FeatureVariableNotFound(variable_key) from ex
-        if not custom_json:
-            raise FeatureVariableNotFound(variable_key)
-        return self._parse_json(custom_json)
+        variables = self.get_feature_all_variables(
+            feature_key, Variation.Type.OFF.value
+        )
+        if variable_key in variables:
+            return variables[variable_key]
+        raise FeatureVariableNotFound(variable_key)
 
     def get_feature_all_variables(
         self, feature_key: str, variation_key: str
     ) -> Dict[str, Any]:
         """
         Retrieve all feature variables.
         A feature variables can be changed easily via our web application.
@@ -586,15 +579,15 @@
                     # The feature is not yet activated on Kameleoon's side
                 except VariationConfigurationNotFound:
                     # The variation key is not found for current feature flag
                     pass
         """
 
         # pylint: disable=no-else-raise
-        feature_flag = self._find_feature_flag_v2(feature_key)
+        feature_flag = self.__find_feature_flag(feature_key)
         variation = feature_flag.get_variation(variation_key)
         if not variation:
             raise VariationConfigurationNotFound(variation_key)
         variables: Dict[str, Any] = {}
         for var in variation.variables:
             variables[var.key] = var.get_value()
         return variables
@@ -607,19 +600,19 @@
             "Call to deprecated function `obtain_feature_all_variables`. "
             "Please use `get_feature_all_variables` instead.",
             category=DeprecationWarning,
             stacklevel=2,
         )
         return self.get_feature_all_variables(feature_key, variation_key)
 
-    def retrieve_data_from_remote_source(
+    def get_remote_data(
         self, key: str, timeout: Optional[float] = None
     ) -> Optional[Any]:
         """
-        The retrieved_data_from_remote_source method allows you to retrieve data (according to a key passed as
+        The get_remote_data method allows you to retrieve data (according to a key passed as
         argument)stored on a remote Kameleoon server. Usually data will be stored on our remote servers
         via the use of our Data API. This method, along with the availability of our highly scalable servers
         for this purpose, provides a convenient way to quickly store massive amounts of data that
         can be later retrieved for each of your visitors / users.
 
         :param key: key you want to retrieve data. This field is mandatory.
         :type key: str
@@ -637,23 +630,43 @@
         return self._make_sync_request(
             url=self._get_api_data_request_url(key),
             method="get",
             headers=self._get_header_client(),
             timeout=timeout,
         )
 
+    def retrieve_data_from_remote_source(
+        self, key: str, timeout: Optional[float] = None
+    ) -> Optional[Any]:
+        """
+        Deprecated, please use `get_remote_data`
+
+        The retrieve_data_from_remote_source method uses for obtaining a list of experiment IDs:
+        - currently available for the SDK
+
+        :return: List of all experiments IDs
+        :rtype: List[int]
+        """
+        warnings.warn(
+            "Call to deprecated function `retrieve_data_from_remote_source`. "
+            "Please use `get_remote_data` instead.",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.get_remote_data(key, timeout)
+
     def get_experiment_list(self) -> List[int]:
         """
         The get_experiment_list method uses for obtaining a list of experiment IDs:
         - currently available for the SDK
 
         :return: List of all experiments IDs
         :rtype: List[int]
         """
-        return list(map(lambda experiment: experiment["id"], self.experiments))
+        return list(map(lambda experiment: experiment["id"], self._experiments))
 
     def get_experiment_list_for_visitor(
         self, visitor_code: str, only_allocated: bool = True
     ) -> List[int]:
         """
         The get_experiment_list method uses for obtaining a list of experiment IDs:
         - currently targeted for a visitor
@@ -666,32 +679,30 @@
         :type only_allocated: bool
 
         :return: List of all experiments IDs (targeted or targeted and allocated simultaneously)
                  for current visitorCode
         :rtype: List[int]
         """
 
-        def check_conditions(experiment: Dict[str, Any]) -> bool:
-            if self._check_targeting(visitor_code, experiment):
-                if (
-                    not only_allocated
-                    or self._calculate_variation_for_experiment(
-                        visitor_code, experiment
-                    )
-                    is not None
-                ):
-                    return True
-            return False
+        def filter_conditions(experiment: Dict[str, Any]) -> bool:
+            if not self.__check_targeting(visitor_code, experiment):
+                return False
+
+            return (
+                not only_allocated
+                or self.__calculate_variation_for_experiment(visitor_code, experiment)
+                is not None
+            )
 
         return list(
             map(
                 lambda experiment: experiment["id"],
                 filter(
-                    check_conditions,
-                    self.experiments,
+                    filter_conditions,
+                    self._experiments,
                 ),
             )
         )
 
     def obtain_experiment_list(
         self, visitor_code: Optional[str] = None, only_allocated: bool = True
     ) -> List[int]:
@@ -711,15 +722,15 @@
         The get_feature_list method uses for obtaining a list of feature flag IDs:
         - currently available for the SDK
 
         :return: List of all feature flag IDs
         :rtype: List[int]
         """
         return list(
-            map(lambda feature_flag: feature_flag.feature_key, self.feature_flags_v2)
+            map(lambda feature_flag: feature_flag.feature_key, self._feature_flags)
         )
 
     def get_active_feature_list_for_visitor(self, visitor_code: str) -> List[str]:
         """
         The get_active_feature_list_for_visitor method uses for obtaining a list of feature flag IDs:
         - currently targeted and active simultaneously for a visitor
 
@@ -727,26 +738,29 @@
         :type visitor_code: Optional[str]
 
         :return: List of all feature flag IDs or targeted and active simultaneously
                  for current visitorCode
         :rtype: List[int]
         """
 
-        def check_conditions(feature_flag: FeatureFlagV2) -> bool:
-            (variation_key, _) = self._calculate_variation_key_for_feature(
+        def filter_conditions(feature_flag: FeatureFlag) -> bool:
+            (variation, rule) = self.__calculate_variation_rule_for_feature(
                 visitor_code, feature_flag
             )
+            variation_key = self.__calculate_variation_key(
+                variation, rule, feature_flag
+            )
             return variation_key != Variation.Type.OFF.value
 
         return list(
             map(
                 lambda feature_flag: feature_flag.feature_key,
                 filter(
-                    check_conditions,
-                    self.feature_flags_v2,
+                    filter_conditions,
+                    self._feature_flags,
                 ),
             )
         )
 
     # pylint: disable=W0613
     def obtain_feature_list(
         self,
@@ -758,15 +772,15 @@
             "Call to deprecated function `obtain_experiment_list`. "
             "Please use `get_feature_list` or `get_active_feature_list_for_visitor` instead.",
             category=DeprecationWarning,
             stacklevel=2,
         )
         if visitor_code is None:
             return self.get_feature_list()
-        return self.get_active_feature_list_for_visitor(visitor_code=visitor_code)
+        return self.get_active_feature_list_for_visitor(visitor_code)
 
     def get_feature_variation_key(self, visitor_code: str, feature_key: str) -> str:
         """
         Returns a variation key for visitor code
 
         This method takes a visitor_code and feature_key as mandatory arguments and
         returns a variation assigned for a given visitor
@@ -787,15 +801,15 @@
                                           the internal configuration of the SDK. This is usually normal and means that
                                           the feature flag has not yet been activated on Kameleoon's side
                                           (but code implementing the feature is already deployed on the
                                           web-application's side).
             VisitorCodeNotValid: Raise when the provided visitor code is not valid
                                  (empty, or longer than 255 characters)
         """
-        (_, variation_key) = self._get_feature_variation_key(visitor_code, feature_key)
+        (_, variation_key) = self.__get_feature_variation_key(visitor_code, feature_key)
         return variation_key
 
     def get_feature_variable(
         self, visitor_code: str, feature_key: str, variable_key: str
     ) -> Union[bool, str, float, Dict[str, Any], List[Any], None]:
         """
         Retrieves a feature variable value from assigned for visitor variation
@@ -818,15 +832,15 @@
                                           (but code implementing the feature is already deployed on the
                                           web-application's side).
             FeatureVariableNotFound: Variable provided name doesn't exist in this feature
             VisitorCodeNotValid: Raise when the provided visitor code is not valid
                                  (empty, or longer than 255 characters)
         """
 
-        (feature_flag, variation_key) = self._get_feature_variation_key(
+        (feature_flag, variation_key) = self.__get_feature_variation_key(
             visitor_code, feature_key
         )
         variation = feature_flag.get_variation(variation_key)
         variable = variation.get_variable_by_key(variable_key) if variation else None
         if variable is None:
             raise FeatureVariableNotFound(variable_key)
         return variable.get_value()
@@ -863,15 +877,14 @@
         # pylint: disable=too-many-arguments
         if payload is None:
             payload = {}
         if filters:
             payload["filter"] = json.dumps(filters)
         resp_dict: Any = {}
         user_timeout = (timeout or self.default_timeout) / MILLISECONDS_IN_SECOND
-        print(f"user_timeout: {user_timeout}")
         if method == "post":
             try:
                 resp_dict = requests.post(
                     url, data=payload, headers=headers, timeout=user_timeout
                 )
             except requests.exceptions.RequestException as ex:
                 self.logger.error(ex)
@@ -889,42 +902,43 @@
             resp = resp_dict.json()
         except JSONDecodeError:
             resp = None
             if isinstance(resp_dict, (Dict, str, Response)):
                 resp = resp_dict
         return resp
 
-    def _is_valid_saved_variation(
-        self, visitor_code: str, experiment_id: int, respool_times: Dict[str, int]
-    ) -> Optional[int]:
-        # get saved variation
-        saved_variation_id = self.variation_storage.get_variation_id(
-            visitor_code, experiment_id
-        )
-        if saved_variation_id is not None:
-            # get respool time for saved variation id
-            respool_time = respool_times.get(str(saved_variation_id))
-            # checking variation for validity along with respoolTime
-            return self.variation_storage.is_variation_id_valid(
-                visitor_code, experiment_id, respool_time
-            )
-        return None
+    # Useless without storage
+    # def __is_valid_saved_variation(
+    #     self, visitor_code: str, experiment_id: int, respool_times: Dict[str, int]
+    # ) -> Optional[int]:
+    #     # get saved variation
+    #     saved_variation_id = self.variation_storage.get_variation_id(
+    #         visitor_code, experiment_id
+    #     )
+    #     if saved_variation_id is not None:
+    #         # get respool time for saved variation id
+    #         respool_time = respool_times.get(str(saved_variation_id))
+    #         # checking variation for validity along with respoolTime
+    #         return self.variation_storage.is_variation_id_valid(
+    #             visitor_code, experiment_id, respool_time
+    #         )
+    #     return None
 
-    def _check_targeting(self, visitor_code: str, campaign: Dict[str, Any]):
+    def __check_targeting(self, visitor_code: str, campaign: Dict[str, Any]):
         return (
             SEGMENT not in campaign
             or campaign[SEGMENT] is None
             or campaign[SEGMENT].check_tree(
                 lambda type: self._get_condition_data(
                     type, visitor_code, campaign["id"]
                 )
             )
         )
 
-    def _check_targeting_id_object(
+    def __check_targeting_id_object(
         self, visitor_code: str, campaign_id: int, targeting_object: Rule
     ) -> bool:
         return (
             targeting_object.targeting_segment is None
             or targeting_object.targeting_segment.check_tree(
                 lambda type: self._get_condition_data(type, visitor_code, campaign_id)
             )
@@ -999,15 +1013,15 @@
             return str(custom_json["value"])
         if custom_json["type"] == "Number":
             return float(custom_json["value"])
         if custom_json["type"] == "JSON":
             return json.loads(custom_json["value"])
         raise TypeError("Unknown type for feature variable")
 
-    def _calculate_variation_for_experiment(
+    def __calculate_variation_for_experiment(
         self, visitor_code: str, experiment: Dict[str, Any]
     ) -> Optional[int]:
         """Calculates the variation for a given visitor_code and experiment"""
         threshold = obtain_hash_double(
             visitor_code, experiment["respoolTime"], experiment["id"]
         )
         for variation_id, value in experiment["deviations"].items():
@@ -1031,17 +1045,16 @@
         fetch configuration from CDN service
         :return:  None
         """
         # pylint: disable=W0703
         try:
             configuration_json = self._obtain_configuration(self.site_code, time_stamp)
             if configuration_json:
-                self.experiments = self._fetch_experiments(configuration_json)
-                self.feature_flags = self._fetch_feature_flags(configuration_json)
-                self.feature_flags_v2 = FeatureFlagV2.from_array(
+                self._experiments = self._fetch_experiments(configuration_json)
+                self._feature_flags = FeatureFlag.from_array(
                     configuration_json["featureFlagConfigurations"]
                 )
                 self.settings = self._fetch_settings(configuration_json)
                 self._call_update_handler_if_needed(time_stamp is not None)
         except Exception as ex:
             self.logger.error(ex)
         self._manage_configuration_update(self.settings.real_time_update)
@@ -1070,14 +1083,25 @@
                 )
         else:
             if self.real_time_configuration_service is not None:
                 self.real_time_configuration_service.close()
                 self.real_time_configuration_service = None
             self._add_fetch_configuration_timer()
 
+    def get_engine_tracking_code(self, visitor_code: str) -> str:
+        """
+        The `get_engine_tracking_code` returns the JavaScript code to be inserted in your page
+        to send automatically the exposure events to the analytics solution you are using.
+        :param visitor_code: Unique identifier of the user. This field is mandatory.
+        :type visitor_code: str
+        :return: Tracking code
+        :rtype: str
+        """
+        return self.hybrid_manager.get_engine_tracking_code(visitor_code)
+
     def on_update_configuration(self, handler: Callable[[], None]):
         """
         The `on_update_configuration()` method allows you to handle the event when configuration
         has updated data. It takes one input parameter: callable **handler**. The handler
         that will be called when the configuration is updated using a real-time configuration event.
         :param handler: The handler that will be called when the configuration
         is updated using a real-time configuration event.
@@ -1153,15 +1177,14 @@
         """
         :param campaign (experiment or feature_flag):
         :type: dict
         :return: campaign (experiment or feature_flag)
         :rtype: dict
         """
         campaign["id"] = int(campaign["id"])
-        campaign["status"] = campaign["status"]
         if "respoolTime" in campaign and campaign["respoolTime"] is not None:
             campaign["respoolTime"] = {
                 (
                     "origin"
                     if respoolTime["variationId"] == "0"
                     else respoolTime["variationId"]
                 ): respoolTime["value"]
@@ -1208,34 +1231,14 @@
         if experiments:
             experiments = [
                 self._complete_experiment(experiment) for experiment in experiments
             ]
             self.logger.debug("Experiment are fetched: %s", experiments)
         return experiments
 
-    def _fetch_feature_flags(
-        self, configuration: Optional[Dict[str, Any]]
-    ) -> List[Dict[str, Any]]:
-        """
-        Fethcing feature flags from CDN response
-        :param configuration: Full configuration of experiments and feature flags
-        :type: Optional[Dict[str, Any]]
-        :return: List of feature flags
-        :rtype: List[Dict[str, Any]]
-        """
-        feature_flags = (
-            configuration["featureFlags"] if configuration is not None else []
-        )
-        if feature_flags:
-            feature_flags = [
-                self._complete_campaign(feature_flag) for feature_flag in feature_flags
-            ]
-            self.logger.debug("Feature Flags are fetched: %s", feature_flags)
-        return feature_flags
-
     def _fetch_settings(self, configuration: Optional[Dict[str, Any]]) -> Settings:
         """
         Fethcing configuration settings from CDN response
         :param configuration: Full configuration of experiments and feature flags
         :type: Optional[Dict[str, Any]]
         :return: Settings of configuration
         :rtype: Dict[str, Any]
@@ -1302,38 +1305,14 @@
         Return configured url for Real Time configuration service (SSE client)
         :param site_code: site code you're subscribing for real time updates
         :type: str
         :return:
         """
         return self.events_url + "sse?siteCode=" + site_code
 
-    def get_feature_flag(self, feature_key: Union[int, str]) -> Dict[str, Any]:
-        """
-
-        :param feature_key:
-        :return:
-        """
-        if isinstance(feature_key, str):
-            _id = "identificationKey"
-        elif isinstance(feature_key, int):
-            _id = "id"
-        else:
-            raise TypeError("Feature key should be a String or an Integer.")
-        feature_flags = [
-            feature_flag
-            for feature_flag in self.feature_flags
-            if feature_flag[_id] == feature_key
-        ]
-        feature_flag = None
-        if feature_flags:
-            feature_flag = feature_flags[0]
-        if feature_flag is None:
-            raise FeatureConfigurationNotFound(message=str(feature_key))
-        return feature_flag
-
     def _track_experiment(
         self, visitor_code: str, experiment_id, variation_id=None, none_variation=False
     ) -> None:
         """
         Track experiment
         :param visitor_code:
         :param experiment_id:
@@ -1346,18 +1325,21 @@
 
         options = {
             "path": self._get_experiment_register_url(
                 visitor_code, experiment_id, variation_id, none_variation
             ),
             "body": (
                 "\n".join(
-                    [
-                        data_instance.obtain_full_post_text_line()
-                        for data_instance in data
-                    ]
+                    filter(
+                        lambda body_text: len(body_text) > 0,
+                        (
+                            data_instance.obtain_full_post_text_line()
+                            for data_instance in data
+                        ),
+                    )
                 )
                 or ""
             ).encode("UTF-8"),
         }
         trial = 0
         self.logger.debug("Start post tracking experiment: %s", data_not_sent)
         success = False
@@ -1380,45 +1362,58 @@
                 "Post to experiment tracking is done after %s trials", trial
             )
         else:
             self.logger.error(
                 "Post to experiment tracking is not done after %s trials", trial
             )
 
-    def _track_experiment_multithread(
+    def __send_tracking_request(
         self,
         visitor_code: str,
-        experiment_id: int,
+        experiment_id: Optional[int],
         variation_id: Optional[int] = None,
         none_variation=False,
     ) -> None:
-        run_in_threads_if_required(
-            background_thread=self.multi_threading,
-            func=self._track_experiment,
-            args=[visitor_code, experiment_id, variation_id, none_variation],
-            thread_name=KAMELEOON_TRACK_EXPERIMENT_THREAD,
-        )
+        if experiment_id is not None:
+            run_in_threads_if_required(
+                background_thread=self.multi_threading,
+                func=self._track_experiment,
+                args=[
+                    visitor_code,
+                    experiment_id,
+                    variation_id or REFERENCE,
+                    none_variation,
+                ],
+                thread_name=KAMELEOON_TRACK_EXPERIMENT_THREAD,
+            )
+        else:
+            self.logger.debug(
+                "An attempt to send a request with null experimentId was blocked"
+            )
 
     def _track_data(self, visitor_code: Optional[str] = None):
         """
         Tracking data
         :param visitor_code: Optional[str]
         :return:
         """
         trials = 10
         data_not_sent = self._data_not_sent(visitor_code)
 
         self.logger.debug("Start post tracking data: %s", data_not_sent)
 
         while trials > 0 and data_not_sent:
             for v_code, data_list_instances in data_not_sent.items():
-                body = [
-                    data_instance.obtain_full_post_text_line()
-                    for data_instance in data_list_instances
-                ]
+                body = filter(
+                    lambda body_text: len(body_text) > 0,
+                    (
+                        data_instance.obtain_full_post_text_line()
+                        for data_instance in data_list_instances
+                    ),
+                )
                 options = {
                     "path": self._get_data_register_url(v_code),
                     "body": ("\n".join(body)).encode("UTF-8"),
                 }
                 self.logger.debug(
                     "Post tracking data for visitor_code: %s with options: %s",
                     data_list_instances,
@@ -1463,36 +1458,23 @@
                     data[vis_code] = [
                         data_instance
                         for data_instance in data_list
                         if not data_instance.sent
                     ]
         return data
 
-    def _check_site_code_enable(self, exp_or_ff: Dict[str, Any]):
+    def __check_site_code_enable(self, exp_or_ff: Dict[str, Any]):
         """
         raise SiteCodeDisabled if site of Experiment or Feature Flag is disabled
         :param exp_or_ff:
         :type exp_or_ff: Dict[str, Any]
         """
         if exp_or_ff.get("siteEnabled") is not True:
             raise SiteCodeDisabled(self.site_code)
 
-    def _check_feature_key(self, feature_key: Union[str, int]):
-        """
-        warning user that feature_id is deprecated and need to pass feature_key with `str` type
-        :param feature_key:
-        :type feature_key: Union[str, int]
-        """
-        if isinstance(feature_key, int):
-            warnings.warn(
-                "Passing `feature_key` with type of `int` to `activate_feature` or `obtain_feature_variable` "
-                "is deprecated, it will be removed in next releases. This is necessary to support multi-environment "
-                "feature"
-            )
-
     def _setup_client_configuration(  # noqa: C901
         self,
         configuration_path: str,
         configuration_object: Optional[KameleoonClientConfiguration],
     ):
         """
         helper method to parse client configuration and setup client
@@ -1541,84 +1523,103 @@
         if len(self.user_agent_data) > USER_AGENT_MAX_COUNT:
             self.user_agent_data = {}
         self.user_agent_data[visitor_code] = user_agent
 
     def _get_user_agent(self, visitor_code: str) -> Optional[UserAgent]:
         return self.user_agent_data.get(visitor_code)
 
-    def _get_feature_variation_key(
+    def __get_feature_variation_key(
         self, visitor_code: str, feature_key: str
-    ) -> Tuple[FeatureFlagV2, str]:
+    ) -> Tuple[FeatureFlag, str]:
         """
         helper method for getting variation key for feature flag
         """
-
         check_visitor_code(visitor_code)
-        feature_flag = self._find_feature_flag_v2(feature_key)
-        (variation_key, rule) = self._calculate_variation_key_for_feature(
+        feature_flag = self.__find_feature_flag(feature_key)
+        (variation, rule) = self.__calculate_variation_rule_for_feature(
             visitor_code, feature_flag
         )
-        if rule and rule.type == Rule.Type.EXPERIMENTATION.value:
-            self._send_tracking_request(visitor_code, variation_key, rule)
+        variation_key = self.__calculate_variation_key(variation, rule, feature_flag)
+        if rule:
+            variation_id = variation.variation_id if variation else None
+            self.__send_tracking_request(
+                visitor_code,
+                rule.experiment_id,
+                variation_id,
+                variation is None,
+            )
+            self.__save_variation(visitor_code, rule.experiment_id, variation_id)
         return (feature_flag, variation_key)
 
-    def _calculate_variation_key_for_feature(
-        self, visitor_code: str, feature_flag: FeatureFlagV2
-    ) -> Tuple[str, Optional[Rule]]:
+    def __calculate_variation_rule_for_feature(
+        self, visitor_code: str, feature_flag: FeatureFlag
+    ) -> Tuple[Optional[VariationByExposition], Optional[Rule]]:
         """helper method for calculate variation key for feature flag"""
-        # no rules -> return default_variation_key
-        if len(feature_flag.rules) > 0:
+        for rule in feature_flag.rules:
+            # check if visitor is targeted for rule, else next rule
+            if not self.__check_targeting_id_object(
+                visitor_code, feature_flag.id_, rule
+            ):
+                continue
             # uses for rule exposition
-            hash_rule = obtain_hash_double_v2(visitor_code, feature_flag.id_)
-            # uses for variation's expositions
-            hash_variation = obtain_hash_double_v2(
-                visitor_code, feature_flag.id_, "variation"
-            )
-            for rule in feature_flag.rules:
-                # check if visitor is targeted for rule, else next rule
-                if (
-                    self._check_targeting_id_object(
-                        visitor_code, feature_flag.id_, rule
-                    )
-                    is False
-                ):
-                    continue
-                # check main expostion for rule with hashRule
-                if hash_rule < rule.exposition:
-                    # get variation key with new hash_variation
-                    variation_key = rule.get_variation_key(hash_variation)
-                    # variation_key can be nil for experiment rules only, for targeted rule will be always exist
-                    if variation_key is not None:
-                        return (variation_key, rule)
-                # if visitor is targeted but not bucketed for targeted rule then break cycle -> return default
-                elif rule.type == Rule.Type.TARGETED_DELIVERY.value:
-                    break
-        return (feature_flag.default_variation_key, None)
-
-    def _send_tracking_request(self, visitor_code: str, variation_key: str, rule: Rule):
-        if rule.experiment_id:
-            run_in_threads_if_required(
-                background_thread=self.multi_threading,
-                func=self._track_experiment,
-                args=[
-                    visitor_code,
-                    rule.experiment_id,
-                    rule.get_variation_id_by_key(variation_key),
-                ],
-                thread_name=KAMELEOON_TRACK_EXPERIMENT_THREAD,
-            )
-        else:
-            self.logger.debug(
-                "An attempt to send a request with null experimentId was blocked"
+            hash_rule = obtain_hash_double_rule(
+                visitor_code, rule.id_, rule.respool_time
             )
+            # check main expostion for rule with hashRule
+            if hash_rule <= rule.exposition:
+                if rule.is_targeted_delivery and len(rule.variation_by_exposition) > 0:
+                    return (rule.variation_by_exposition[0], rule)
+
+                # uses for variation's expositions
+                hash_variation = obtain_hash_double_rule(
+                    visitor_code, rule.experiment_id, rule.respool_time
+                )
+                # get variation with hash_variation
+                variation = rule.get_variation(hash_variation)
+                if variation:
+                    return (variation, rule)
+            elif rule.is_targeted_delivery:
+                break
+        return (None, None)
+
+    def __calculate_variation_key(
+        self,
+        var_by_exp: Optional[VariationByExposition],
+        rule: Optional[Rule],
+        feature_flag: FeatureFlag,
+    ) -> str:
+        if var_by_exp:
+            return var_by_exp.variation_key
+        if rule and rule.is_experimentation:
+            return Variation.Type.OFF.value
+        return feature_flag.default_variation_key
 
-    def _find_feature_flag_v2(self, feature_key: str) -> FeatureFlagV2:
+    def __find_feature_flag(self, feature_key: str) -> FeatureFlag:
         """
         helper method for getting the feature flag v2 from the list
         """
         feature_flag = next(
-            (ff for ff in self.feature_flags_v2 if ff.feature_key == feature_key),
+            (ff for ff in self._feature_flags if ff.feature_key == feature_key),
             None,
         )
         if feature_flag is None:
-            raise FeatureConfigurationNotFound(message=str(feature_key))
+            raise FeatureConfigurationNotFound(feature_key)
         return feature_flag
+
+    def __save_variation(
+        self,
+        visitor_code: str,
+        experiment_id: Optional[int],
+        variation_id: Optional[int],
+    ):
+        """
+        helper method for saving variations (to variation_storage and hybrid_manager)
+        """
+        if experiment_id is not None and variation_id is not None:
+            self.variation_storage.update_variation(
+                visitor_code,
+                experiment_id,
+                variation_id,
+            )
+            self.hybrid_manager.add_tracking_variation(
+                visitor_code, experiment_id, variation_id
+            )
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon/client_configuration.py` & `kameleoon-client-python-2.2.0/kameleoon/client_configuration.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/configuration/feature_flag_v2.py` & `kameleoon-client-python-2.2.0/kameleoon/configuration/feature_flag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from typing import Any, List, Dict, Optional
 
 from kameleoon.configuration.rule import Rule
 from kameleoon.configuration.variation import Variation
 
 
-class FeatureFlagV2:
+class FeatureFlag:
     """
-    FeatureFlagV2 is used for operating feature flags (v2) with rules
+    FeatureFlag is used for operating feature flags with rules
     """
 
     @staticmethod
-    def from_array(array: List[Dict[str, Any]]) -> List["FeatureFlagV2"]:
+    def from_array(array: List[Dict[str, Any]]) -> List["FeatureFlag"]:
         """Create a list of FeatureFlags from the json array"""
-        return [FeatureFlagV2(item) for item in array]
+        return [FeatureFlag(item) for item in array]
 
     def __init__(self, dict_json: Dict[str, Any]):
         self.id_: int = dict_json.get("id", 0)
         self.feature_key: str = dict_json.get("featureKey", "")
         self.default_variation_key: str = dict_json.get("defaultVariationKey", "")
         self.variations: List[Variation] = Variation.from_array(
             dict_json.get("variations", [])
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon/configuration/rule.py` & `kameleoon-client-python-2.2.0/kameleoon/configuration/rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,34 +19,39 @@
 
     @staticmethod
     def from_array(array: List[Dict[str, Any]]) -> List["Rule"]:
         """Create a list of Rules from the json array"""
         return [Rule(item) for item in array]
 
     def __init__(self, dict_json: Dict[str, Any]):
+        self.id_: int = dict_json["id"]
         self.order: int = dict_json.get("order", 0)
         self.type: str = dict_json.get("type", "")
         self.exposition: float = dict_json.get("exposition", 0.0)
-        self.experiment_id = dict_json.get("experiment_id", None)
+        self.experiment_id: int = dict_json.get("experimentId", 0)
+        self.respool_time: Optional[int] = dict_json.get("respoolTime", None)
         self.variation_by_exposition: List[
             VariationByExposition
         ] = VariationByExposition.from_array(dict_json.get("variationByExposition", []))
         segment = dict_json.get("segment")
         self.targeting_segment: Optional[Segment] = (
             Segment(segment) if segment else None
         )
 
-    def get_variation_key(self, hash_double: float) -> Optional[str]:
+    def get_variation(self, hash_double: float) -> Optional[VariationByExposition]:
         """Calculates the variation key for the given hash of visitor"""
         total = 0.0
         for var_by_exp in self.variation_by_exposition:
             total += var_by_exp.exposition
             if total >= hash_double:
-                return var_by_exp.variation_key
+                return var_by_exp
         return None
 
-    def get_variation_id_by_key(self, key: str) -> Optional[int]:
-        """Find the variation id for the given variation key"""
-        var_by_exp = next(
-            (v for v in self.variation_by_exposition if v.variation_key == key), None
-        )
-        return var_by_exp.variation_id if var_by_exp else None
+    @property
+    def is_experimentation(self) -> bool:
+        """Return `true` if rule is `experimentation` type"""
+        return self.type == Rule.Type.EXPERIMENTATION.value
+
+    @property
+    def is_targeted_delivery(self) -> bool:
+        """Return `true` if rule is `targeted delivery` type"""
+        return self.type == Rule.Type.TARGETED_DELIVERY.value
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon/configuration/variable.py` & `kameleoon-client-python-2.2.0/kameleoon/configuration/variable.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     @staticmethod
     def from_array(array: List[Dict[str, Any]]) -> List["Variable"]:
         """Create a list of variables from the json array"""
         return [Variable(item) for item in array]
 
     def __init__(self, dict_json: Dict[str, Any]):
         self.key: str = dict_json.get("key", "")
-        self.type: str = dict_json.get("type", "")
-        self.value: Union[bool, float, str] = dict_json.get("value", False)
+        self.__type: str = dict_json.get("type", "")
+        self.__value: Union[bool, float, str] = dict_json.get("value", False)
 
     def get_value(self) -> Union[bool, float, str, List[Any], Dict[str, Any], None]:
         """Returns a bare value of variable"""
-        if self.type in (
+        if self.__type in (
             Variable.Type.BOOLEAN.value,
             Variable.Type.NUMBER.value,
             Variable.Type.STRING.value,
         ):
-            return self.value
-        if self.type == Variable.Type.JSON.value and isinstance(self.value, str):
-            return json.loads(self.value)
+            return self.__value
+        if self.__type == Variable.Type.JSON.value and isinstance(self.__value, str):
+            return json.loads(self.__value)
         return None
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon/configuration/variation.py` & `kameleoon-client-python-2.2.0/kameleoon/configuration/variation.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/configuration/variation_by_exposition.py` & `kameleoon-client-python-2.2.0/kameleoon/configuration/variation_by_exposition.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/data.py` & `kameleoon-client-python-2.2.0/kameleoon/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Kameleoon data module"""
 import random
+import warnings
 from enum import Enum, IntEnum
-from typing import Optional, Literal, List
+from typing import Optional, Literal, List, Tuple
 from urllib.parse import quote
 
 from kameleoon.exceptions import KameleoonException
 
 ALPHA_NUMERIC_CHARS = "abcdef0123456789"
 NONCE_LENGTH = 16
 
@@ -37,15 +38,15 @@
     PHONE: str = "PHONE"
     TABLET: str = "TABLET"
     DESKTOP: str = "DESKTOP"
 
 
 def get_nonce() -> str:
     """Generates alphanumeric characters"""
-    return "".join(random.choice(ALPHA_NUMERIC_CHARS) for i in range(NONCE_LENGTH))
+    return "".join(random.choice(ALPHA_NUMERIC_CHARS) for _ in range(NONCE_LENGTH))
 
 
 class Data:
     """Base data class"""
 
     def __init__(self) -> None:
         self.nonce: str = get_nonce()
@@ -72,35 +73,52 @@
         """
         return quote(to_encode, safe="~()*!.'")
 
 
 class CustomData(Data):
     """Custom data."""
 
-    def __init__(self, id: int, value: str):
+    @property
+    def values(self) -> Tuple[str, ...]:
+        """Stored values."""
+        return self.__values
+
+    def __init__(self, id: int, *args: str, value: Optional[str] = None):
         """
         :param id: Index / ID of the custom data to be stored. This field is mandatory.
         :type id: int
-        :param value: Value of the custom data to be stored. This field is mandatory.
-        :type value: str
+        :param `*args`: Values of the custom data to be stored. This field is optional.
+        :type `*args`: Tuple[str, ...]
+        :param value: Single value of the custom data to be stored. This field is optional.
+        :type value: Optional[str]
 
         Example:
 
         .. code-block:: python3
 
-                kameleoon_client.add_data(visitor_code, CustomData("test-id", "test-value"))
+                kameleoon_client.add_data(visitor_code, CustomData(123, "some-value"))
         """
         # pylint: disable=invalid-name,redefined-builtin
         self.id = str(id)
-        self.value: str = value
+        if value is None:
+            self.__values = args
+        else:
+            self.__values = (*args, value)
+            warnings.warn(
+                "Passing deprecated parameter `value`. Please pass variadic parameter list instead.",
+                category=DeprecationWarning,
+            )
         self.instance = DataType.CUSTOM.value
         super().__init__()
 
     def obtain_full_post_text_line(self) -> str:
-        encoded_value = self.encode(f'[["{self.value}",1]]')
+        if len(self.__values) == 0:
+            return ""
+        str_values = ",".join((f'["{v}",1]' for v in self.__values))
+        encoded_value = self.encode(f"[{str_values}]")
         return f"eventType=customData&index={self.id}&valueToCount={encoded_value}&overwrite=true&nonce={self.nonce}"
 
 
 class Browser(Data):
     """Browser data."""
 
     def __init__(
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon/defaults.py` & `kameleoon-client-python-2.2.0/kameleoon/defaults.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/exceptions.py` & `kameleoon-client-python-2.2.0/kameleoon/exceptions.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/helpers/config.py` & `kameleoon-client-python-2.2.0/kameleoon/helpers/config.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/helpers/functions.py` & `kameleoon-client-python-2.2.0/kameleoon/helpers/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Helper functions"""
 import hashlib
 import json
 import math
 import sys
 from http.cookies import SimpleCookie
 from secrets import token_urlsafe
-from typing import Dict, Any, Union
+from typing import Dict, Any, Optional, Union
 
 from kameleoon.defaults import (
     KAMELEOON_COOKIE_VALUE_LENGTH,
     KAMELEOON_VISITOR_CODE_LENGTH,
     KAMELEOON_COOKIE_NAME,
     KAMELEOON_KEY_JS_COOKIE,
 )
@@ -19,20 +19,22 @@
 def obtain_hash_double(
     visitor_code: str, respool_times=None, container_id: str = ""
 ) -> float:
     """Calculate the hash value for a given visitor_code"""
     return _obtain_hash_double(visitor_code, respool_times, container_id)
 
 
-def obtain_hash_double_v2(
-    visitor_code: str, container_id: Union[str, int] = "", suffix: str = ""
+def obtain_hash_double_rule(
+    visitor_code: str, container_id: int, respool_time: Optional[int] = None
 ) -> float:
     """Calculate the hash value for feature flag v2 for a given visitor_code"""
     return _obtain_hash_double(
-        visitor_code=visitor_code, container_id=container_id, suffix=suffix
+        visitor_code=visitor_code,
+        container_id=container_id,
+        suffix=str(respool_time) if respool_time else "",
     )
 
 
 def _obtain_hash_double(
     visitor_code: str,
     respool_times=None,
     container_id: Union[str, int] = "",
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon/helpers/multi_threading.py` & `kameleoon-client-python-2.2.0/kameleoon/helpers/multi_threading.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/middleware.py` & `kameleoon-client-python-2.2.0/kameleoon/middleware.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/real_time/real_time_configuration_service.py` & `kameleoon-client-python-2.2.0/kameleoon/real_time/real_time_configuration_service.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/real_time/real_time_event.py` & `kameleoon-client-python-2.2.0/kameleoon/real_time/real_time_event.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/storage/varation_storage.py` & `kameleoon-client-python-2.2.0/kameleoon/storage/varation_storage.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/storage/visitor_variation.py` & `kameleoon-client-python-2.2.0/kameleoon/storage/visitor_variation.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/exclusive_experiment.py` & `kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/exclusive_experiment.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/targeting/conditions/target_experiment.py` & `kameleoon-client-python-2.2.0/kameleoon/targeting/conditions/target_experiment.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/targeting/models.py` & `kameleoon-client-python-2.2.0/kameleoon/targeting/models.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/targeting/tree_builder.py` & `kameleoon-client-python-2.2.0/kameleoon/targeting/tree_builder.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon/targeting/tree_condition_factory.py` & `kameleoon-client-python-2.2.0/kameleoon/targeting/tree_condition_factory.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/PKG-INFO` & `kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kameleoon-client-python
-Version: 2.1.0
+Version: 2.2.0
 Summary: Kameleoon Client Python Software Development Kit.
 Home-page: https://developers.kameleoon.com/python-sdk.html
 Author: Kameleoon
 Author-email: sdk@kameleoon.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kameleoon-client-python-2.1.0/kameleoon_client_python.egg-info/SOURCES.txt` & `kameleoon-client-python-2.2.0/kameleoon_client_python.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 kameleoon/client_configuration.py
 kameleoon/data.py
 kameleoon/defaults.py
 kameleoon/exceptions.py
 kameleoon/middleware.py
 kameleoon/version.py
 kameleoon/configuration/__init__.py
-kameleoon/configuration/feature_flag_v2.py
+kameleoon/configuration/feature_flag.py
 kameleoon/configuration/rule.py
 kameleoon/configuration/settings.py
 kameleoon/configuration/variable.py
 kameleoon/configuration/variation.py
 kameleoon/configuration/variation_by_exposition.py
 kameleoon/helpers/__init__.py
 kameleoon/helpers/config.py
@@ -23,14 +23,18 @@
 kameleoon/helpers/logger.py
 kameleoon/helpers/multi_threading.py
 kameleoon/helpers/repeat_timer.py
 kameleoon/real_time/__init__.py
 kameleoon/real_time/real_time_configuration_service.py
 kameleoon/real_time/real_time_event.py
 kameleoon/storage/__init__.py
+kameleoon/storage/cache.py
+kameleoon/storage/cache_factory.py
+kameleoon/storage/cache_factory_impl.py
+kameleoon/storage/cache_impl.py
 kameleoon/storage/varation_storage.py
 kameleoon/storage/visitor_variation.py
 kameleoon/targeting/__init__.py
 kameleoon/targeting/condition.py
 kameleoon/targeting/models.py
 kameleoon/targeting/tree_builder.py
 kameleoon/targeting/tree_condition_factory.py
```

### Comparing `kameleoon-client-python-2.1.0/setup.cfg` & `kameleoon-client-python-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/setup.py` & `kameleoon-client-python-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/apps.py` & `kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/apps.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/tests/integration/proj/kameleoon_app/views.py` & `kameleoon-client-python-2.2.0/tests/integration/proj/kameleoon_app/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     deviations = {"1": 0.5, "2": 0.25, "3": 0.25}
     experiment = {
         "id": experiment_id,
         "deviations": deviations,
         "respoolTime": {},
         "siteEnabled": True,
     }
-    client.experiments.append(experiment)
+    client._experiments.append(experiment)
     visitor_code = client.get_visitor_code(request.COOKIES, local_ip)
 
     variation_id = None
     try:
         variation_id = client.trigger_experiment(visitor_code, experiment_id)
     except NotAllocated:
         variation_id = 0
```

### Comparing `kameleoon-client-python-2.1.0/tests/integration/proj/manage.py` & `kameleoon-client-python-2.2.0/tests/integration/proj/manage.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/tests/integration/proj/proj/settings.py` & `kameleoon-client-python-2.2.0/tests/integration/proj/proj/settings.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/tests/integration/proj/proj/urls.py` & `kameleoon-client-python-2.2.0/tests/integration/proj/proj/urls.py`

 * *Files identical despite different names*

### Comparing `kameleoon-client-python-2.1.0/tests/integration/proj/proj/wsgi.py` & `kameleoon-client-python-2.2.0/tests/integration/proj/proj/wsgi.py`

 * *Files identical despite different names*

