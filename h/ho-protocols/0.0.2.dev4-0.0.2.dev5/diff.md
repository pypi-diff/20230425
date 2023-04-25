# Comparing `tmp/ho-protocols-0.0.2.dev4.tar.gz` & `tmp/ho-protocols-0.0.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ho-protocols-0.0.2.dev4.tar", last modified: Tue Apr 25 05:47:49 2023, max compression
+gzip compressed data, was "ho-protocols-0.0.2.dev5.tar", last modified: Tue Apr 25 07:41:17 2023, max compression
```

## Comparing `ho-protocols-0.0.2.dev4.tar` & `ho-protocols-0.0.2.dev5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.0.2.dev4/LICENCE
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1356 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.0.2.dev4/README.md
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/setup.cfg
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      991 2022-01-04 14:45:51.000000 ho-protocols-0.0.2.dev4/setup.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.444407 ho-protocols-0.0.2.dev4/src/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.448407 ho-protocols-0.0.2.dev4/src/ho_protocols/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/__init__.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/common_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/common_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/live/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/actuators_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/actuators_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2575 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5829 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1275 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1273 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/map/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/map/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3526 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     8143 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/src/ho_protocols/query/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/query/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.448407 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1356 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/requires.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/top_level.txt
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/test/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.0.2.dev4/test/test.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.0.2.dev5/LICENCE
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1356 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.0.2.dev5/README.md
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/setup.cfg
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1002 2023-04-25 07:40:03.000000 ho-protocols-0.0.2.dev5/setup.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.539598 ho-protocols-0.0.2.dev5/src/
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.543598 ho-protocols-0.0.2.dev5/src/ho_protocols/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/__init__.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.543598 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/alert_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/alert_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/bees_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/bees_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/alert/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.543598 ho-protocols-0.0.2.dev5/src/ho_protocols/cmd/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/cmd/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/cmd/cmd_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/cmd/cmd_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/common_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/common_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/data_in_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/data_in_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/example_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/example_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/src/ho_protocols/live/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/actuators_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/actuators_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/live_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/live_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/models_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/models_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2575 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/sensors_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5829 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/sensors_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1275 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1273 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/live/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/src/ho_protocols/map/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/map/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3526 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/map/map_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     8143 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/map/map_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/src/ho_protocols/query/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/query/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/query/query_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev5/src/ho_protocols/query/query_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.543598 ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1356 2023-04-25 07:41:17.000000 ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-04-25 07:41:17.000000 ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-04-25 07:41:17.000000 ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-04-25 07:41:17.000000 ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/requires.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-04-25 07:41:17.000000 ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/top_level.txt
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 07:41:17.547598 ho-protocols-0.0.2.dev5/test/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.0.2.dev5/test/test.py
```

### Comparing `ho-protocols-0.0.2.dev4/LICENCE` & `ho-protocols-0.0.2.dev5/LICENCE`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/PKG-INFO` & `ho-protocols-0.0.2.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.0.2.dev4
+Version: 0.0.2.dev5
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.0.2.dev4/README.md` & `ho-protocols-0.0.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/setup.py` & `ho-protocols-0.0.2.dev5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 packages = setuptools.find_packages(where="src")
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
-    version_config={
+    setuptools_git_versioning={
         "template": "{tag}",
         "dev_template": "{tag}.dev{ccount}",
         "dirty_template": "{tag}.dev{ccount}"
     },
     setup_requires=["setuptools-git-versioning"],
     name='ho-protocols',
     description='ProtoBuf definitions for HO components',
@@ -24,12 +24,12 @@
     ],
     package_dir={'': 'src'},
     packages=packages,
     package_data={
         "ho_protocols": ["py.typed", "*.pyi", "**/*.pyi"]
     },
     install_requires=[
-        'protobuf==3.15.5',
+        'protobuf~=4.22.0',
     ],
     python_requires='>=3.6'
 
 )
```

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/alert/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/alert/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/alert/bees_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/alert/bees_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/alert/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/alert/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/cmd/cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/cmd/cmd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/common_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/common_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/data_in_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/data_in_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/example_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/actuators_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/actuators_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/actuators_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/actuators_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/live_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/live_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/models_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/sensors_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/sensors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/live/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/map/map_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/map/map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.py` & `ho-protocols-0.0.2.dev5/src/ho_protocols/query/query_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.pyi` & `ho-protocols-0.0.2.dev5/src/ho_protocols/query/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/PKG-INFO` & `ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.0.2.dev4
+Version: 0.0.2.dev5
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/SOURCES.txt` & `ho-protocols-0.0.2.dev5/src/ho_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev4/test/test.py` & `ho-protocols-0.0.2.dev5/test/test.py`

 * *Files identical despite different names*

