# Comparing `tmp/ho-protocols-0.0.2.dev3.tar.gz` & `tmp/ho-protocols-0.0.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vitaljok/Projects/ho-protocols/dist/tmpuvcqzgy9/ho-protocols-0.0.2.dev3.tar", last modified: Thu Feb  2 10:27:32 2023, max compression
+gzip compressed data, was "ho-protocols-0.0.2.dev4.tar", last modified: Tue Apr 25 05:47:49 2023, max compression
```

## Comparing `ho-protocols-0.0.2.dev3.tar` & `ho-protocols-0.0.2.dev4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      991 2022-01-04 14:45:51.000000 ho-protocols-0.0.2.dev3/setup.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1393 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.0.2.dev3/LICENCE
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/setup.cfg
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.0.2.dev3/README.md
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/map/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    22191 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/map/map_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/map/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     7956 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/map/map_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5247 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/common_pb2.py
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1696 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/common_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/query/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/query/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    12698 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/query/query_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    34222 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/query/query_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    36118 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/data_in_pb2.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/cmd/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5881 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/cmd/cmd_pb2.pyi
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/cmd/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    16637 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/cmd/cmd_pb2.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5119 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/sensors_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6003 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/actuators_pb2.pyi
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    17081 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/actuators_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3435 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    12035 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/models_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     8208 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/live_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    14268 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/sensors_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1154 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/system_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4638 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/models_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2780 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/live/live_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5312 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/example_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13934 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/data_in_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1820 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/example_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5787 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/bees_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1612 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/alert_pb2.pyi
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10655 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4545 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/alert_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3722 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/system_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2038 2023-02-02 10:27:24.000000 ho-protocols-0.0.2.dev3/src/ho_protocols/alert/bees_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1393 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/top_level.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/requires.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/SOURCES.txt
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 10:27:32.000000 ho-protocols-0.0.2.dev3/test/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.0.2.dev3/test/test.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.0.2.dev4/LICENCE
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1356 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.0.2.dev4/README.md
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/setup.cfg
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      991 2022-01-04 14:45:51.000000 ho-protocols-0.0.2.dev4/setup.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.444407 ho-protocols-0.0.2.dev4/src/
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.448407 ho-protocols-0.0.2.dev4/src/ho_protocols/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/__init__.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/common_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/common_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/live/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/actuators_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/actuators_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2575 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5829 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1275 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1273 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.452407 ho-protocols-0.0.2.dev4/src/ho_protocols/map/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/map/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3526 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     8143 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/src/ho_protocols/query/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/query/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-04-25 05:45:18.000000 ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.448407 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1356 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/requires.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-04-25 05:47:49.000000 ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/top_level.txt
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 05:47:49.456407 ho-protocols-0.0.2.dev4/test/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.0.2.dev4/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ho-protocols-0.0.2.dev3/setup.py` & `ho-protocols-0.0.2.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev3/PKG-INFO` & `ho-protocols-0.0.2.dev4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.0.2.dev3
+Version: 0.0.2.dev4
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -64,9 +62,7 @@
 ```
 
 Publish to PyPi
 ```bash
 twine upload dist/*
 ```
 
-
-
```

### Comparing `ho-protocols-0.0.2.dev3/LICENCE` & `ho-protocols-0.0.2.dev4/LICENCE`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev3/README.md` & `ho-protocols-0.0.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/map/map_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/map/map_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,179 +1,203 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import ho_protocols.common_pb2
-import typing
-import typing_extensions
+import sys
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class MapRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     HEADER_FIELD_NUMBER: builtins.int
     WEATHER_FORECAST_FIELD_NUMBER: builtins.int
     HARVESTING_RESOURCES_FIELD_NUMBER: builtins.int
-
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
-
     @property
     def weather_forecast(self) -> global___WeatherForecast: ...
-
     @property
     def harvesting_resources(self) -> global___HarvestingResources: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        header : typing.Optional[ho_protocols.common_pb2.Header] = ...,
-        weather_forecast : typing.Optional[global___WeatherForecast] = ...,
-        harvesting_resources : typing.Optional[global___HarvestingResources] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"harvesting_resources",b"harvesting_resources",u"header",b"header",u"query",b"query",u"weather_forecast",b"weather_forecast"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"harvesting_resources",b"harvesting_resources",u"header",b"header",u"query",b"query",u"weather_forecast",b"weather_forecast"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"query",b"query"]) -> typing_extensions.Literal["weather_forecast","harvesting_resources"]: ...
+        header: ho_protocols.common_pb2.Header | None = ...,
+        weather_forecast: global___WeatherForecast | None = ...,
+        harvesting_resources: global___HarvestingResources | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "header", b"header", "query", b"query", "weather_forecast", b"weather_forecast"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "header", b"header", "query", b"query", "weather_forecast", b"weather_forecast"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["query", b"query"]) -> typing_extensions.Literal["weather_forecast", "harvesting_resources"] | None: ...
+
 global___MapRequest = MapRequest
 
+@typing_extensions.final
 class MapResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     WEATHER_FORECAST_FIELD_NUMBER: builtins.int
     HARVESTING_RESOURCES_FIELD_NUMBER: builtins.int
-
     @property
     def weather_forecast(self) -> global___WeatherForecastResult: ...
-
     @property
     def harvesting_resources(self) -> global___HarvestingResourcesResult: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        weather_forecast : typing.Optional[global___WeatherForecastResult] = ...,
-        harvesting_resources : typing.Optional[global___HarvestingResourcesResult] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"harvesting_resources",b"harvesting_resources",u"result",b"result",u"weather_forecast",b"weather_forecast"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"harvesting_resources",b"harvesting_resources",u"result",b"result",u"weather_forecast",b"weather_forecast"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"result",b"result"]) -> typing_extensions.Literal["weather_forecast","harvesting_resources"]: ...
+        weather_forecast: global___WeatherForecastResult | None = ...,
+        harvesting_resources: global___HarvestingResourcesResult | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "result", b"result", "weather_forecast", b"weather_forecast"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "result", b"result", "weather_forecast", b"weather_forecast"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["weather_forecast", "harvesting_resources"] | None: ...
+
 global___MapResponse = MapResponse
 
+@typing_extensions.final
 class WeatherForecast(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    """#####"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     LAT_FIELD_NUMBER: builtins.int
     LNG_FIELD_NUMBER: builtins.int
     PERIODS_FIELD_NUMBER: builtins.int
-    lat: builtins.float = ...
-    lng: builtins.float = ...
-    periods: builtins.int = ...
-
-    def __init__(self,
-        *,
-        lat : builtins.float = ...,
-        lng : builtins.float = ...,
-        periods : builtins.int = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"lat",b"lat",u"lng",b"lng",u"periods",b"periods"]) -> None: ...
+    lat: builtins.float
+    lng: builtins.float
+    periods: builtins.int
+    def __init__(
+        self,
+        *,
+        lat: builtins.float = ...,
+        lng: builtins.float = ...,
+        periods: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["lat", b"lat", "lng", b"lng", "periods", b"periods"]) -> None: ...
+
 global___WeatherForecast = WeatherForecast
 
+@typing_extensions.final
 class WeatherForecastResult(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class Item(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         TS_FIELD_NUMBER: builtins.int
         TEMPERATURE_FIELD_NUMBER: builtins.int
         HUMIDITY_FIELD_NUMBER: builtins.int
         WIND_SPEED_FIELD_NUMBER: builtins.int
         WIND_DEG_FIELD_NUMBER: builtins.int
-        ts: builtins.int = ...
-        temperature: builtins.float = ...
-        humidity: builtins.float = ...
-        wind_speed: builtins.float = ...
-        wind_deg: builtins.float = ...
-
-        def __init__(self,
+        ts: builtins.int
+        temperature: builtins.float
+        humidity: builtins.float
+        wind_speed: builtins.float
+        wind_deg: builtins.float
+        def __init__(
+            self,
             *,
-            ts : builtins.int = ...,
-            temperature : builtins.float = ...,
-            humidity : builtins.float = ...,
-            wind_speed : builtins.float = ...,
-            wind_deg : builtins.float = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"humidity",b"humidity",u"temperature",b"temperature",u"ts",b"ts",u"wind_deg",b"wind_deg",u"wind_speed",b"wind_speed"]) -> None: ...
+            ts: builtins.int = ...,
+            temperature: builtins.float = ...,
+            humidity: builtins.float = ...,
+            wind_speed: builtins.float = ...,
+            wind_deg: builtins.float = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["humidity", b"humidity", "temperature", b"temperature", "ts", b"ts", "wind_deg", b"wind_deg", "wind_speed", b"wind_speed"]) -> None: ...
 
     ITEM_FIELD_NUMBER: builtins.int
-
     @property
     def item(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___WeatherForecastResult.Item]: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        item : typing.Optional[typing.Iterable[global___WeatherForecastResult.Item]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"item",b"item"]) -> None: ...
+        item: collections.abc.Iterable[global___WeatherForecastResult.Item] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["item", b"item"]) -> None: ...
+
 global___WeatherForecastResult = WeatherForecastResult
 
+@typing_extensions.final
 class HarvestingResources(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    """#####"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     LAT_FIELD_NUMBER: builtins.int
     LNG_FIELD_NUMBER: builtins.int
     TS_FIELD_NUMBER: builtins.int
-    lat: builtins.float = ...
-    lng: builtins.float = ...
-    ts: builtins.int = ...
-
-    def __init__(self,
-        *,
-        lat : builtins.float = ...,
-        lng : builtins.float = ...,
-        ts : builtins.int = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"lat",b"lat",u"lng",b"lng",u"ts",b"ts"]) -> None: ...
+    lat: builtins.float
+    lng: builtins.float
+    ts: builtins.int
+    def __init__(
+        self,
+        *,
+        lat: builtins.float = ...,
+        lng: builtins.float = ...,
+        ts: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["lat", b"lat", "lng", b"lng", "ts", b"ts"]) -> None: ...
+
 global___HarvestingResources = HarvestingResources
 
+@typing_extensions.final
 class HarvestingResourcesResult(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class Field(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         PLANT_NAME_FIELD_NUMBER: builtins.int
         AMOUNT_FIELD_NUMBER: builtins.int
         DIR_FIELD_NUMBER: builtins.int
-        plant_name: typing.Text = ...
-        amount: builtins.float = ...
-        dir: builtins.float = ...
-
-        def __init__(self,
+        plant_name: builtins.str
+        amount: builtins.float
+        dir: builtins.float
+        def __init__(
+            self,
             *,
-            plant_name : typing.Text = ...,
-            amount : builtins.float = ...,
-            dir : builtins.float = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"amount",b"amount",u"dir",b"dir",u"plant_name",b"plant_name"]) -> None: ...
+            plant_name: builtins.str = ...,
+            amount: builtins.float = ...,
+            dir: builtins.float = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "dir", b"dir", "plant_name", b"plant_name"]) -> None: ...
 
     OVERALL_INDEX_FIELD_NUMBER: builtins.int
     NECTAR_INDEX_FIELD_NUMBER: builtins.int
     POLLEN_INDEX_FIELD_NUMBER: builtins.int
     WATER_INDEX_FIELD_NUMBER: builtins.int
     ROAD_INDEX_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
-    overall_index: builtins.float = ...
-    nectar_index: builtins.float = ...
-    pollen_index: builtins.float = ...
-    water_index: builtins.float = ...
-    road_index: builtins.float = ...
-
+    overall_index: builtins.float
+    nectar_index: builtins.float
+    pollen_index: builtins.float
+    water_index: builtins.float
+    road_index: builtins.float
     @property
     def field(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HarvestingResourcesResult.Field]: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        overall_index : builtins.float = ...,
-        nectar_index : builtins.float = ...,
-        pollen_index : builtins.float = ...,
-        water_index : builtins.float = ...,
-        road_index : builtins.float = ...,
-        field : typing.Optional[typing.Iterable[global___HarvestingResourcesResult.Field]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"field",b"field",u"nectar_index",b"nectar_index",u"overall_index",b"overall_index",u"pollen_index",b"pollen_index",u"road_index",b"road_index",u"water_index",b"water_index"]) -> None: ...
+        overall_index: builtins.float = ...,
+        nectar_index: builtins.float = ...,
+        pollen_index: builtins.float = ...,
+        water_index: builtins.float = ...,
+        road_index: builtins.float = ...,
+        field: collections.abc.Iterable[global___HarvestingResourcesResult.Field] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["field", b"field", "nectar_index", b"nectar_index", "overall_index", b"overall_index", "pollen_index", b"pollen_index", "road_index", b"road_index", "water_index", b"water_index"]) -> None: ...
+
 global___HarvestingResourcesResult = HarvestingResourcesResult
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/common_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/alert_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
-import typing
-import typing_extensions
-
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
-
-class Header(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class TagEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text = ...
-        value: typing.Text = ...
-
-        def __init__(self,
-            *,
-            key : typing.Text = ...,
-            value : typing.Text = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
-
-    MODULE_FIELD_NUMBER: builtins.int
-    INSTANCE_FIELD_NUMBER: builtins.int
-    TS_FIELD_NUMBER: builtins.int
-    TAG_FIELD_NUMBER: builtins.int
-    module: typing.Text = ...
-    instance: typing.Text = ...
-    ts: builtins.int = ...
-
+import ho_protocols.alert.bees_pb2
+import ho_protocols.alert.system_pb2
+import ho_protocols.common_pb2
+import sys
+
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
+
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
+class AlertMessage(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    HEADER_FIELD_NUMBER: builtins.int
+    SYSTEM_FIELD_NUMBER: builtins.int
+    BEES_FIELD_NUMBER: builtins.int
     @property
-    def tag(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
-
-    def __init__(self,
+    def header(self) -> ho_protocols.common_pb2.Header: ...
+    @property
+    def system(self) -> ho_protocols.alert.system_pb2.SystemAlert: ...
+    @property
+    def bees(self) -> ho_protocols.alert.bees_pb2.BeesAlert: ...
+    def __init__(
+        self,
         *,
-        module : typing.Text = ...,
-        instance : typing.Text = ...,
-        ts : builtins.int = ...,
-        tag : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"instance",b"instance",u"module",b"module",u"tag",b"tag",u"ts",b"ts"]) -> None: ...
-global___Header = Header
+        header: ho_protocols.common_pb2.Header | None = ...,
+        system: ho_protocols.alert.system_pb2.SystemAlert | None = ...,
+        bees: ho_protocols.alert.bees_pb2.BeesAlert | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["bees", b"bees", "header", b"header", "payload", b"payload", "system", b"system"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bees", b"bees", "header", b"header", "payload", b"payload", "system", b"system"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["payload", b"payload"]) -> typing_extensions.Literal["system", "bees"] | None: ...
+
+global___AlertMessage = AlertMessage
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/query/query_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/query/query_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,294 +1,304 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import ho_protocols.common_pb2
+import sys
 import typing
-import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class QueryRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     HEADER_FIELD_NUMBER: builtins.int
     HISTORICAL_WEIGHT_FIELD_NUMBER: builtins.int
     RECENT_TEMPERATURE_FIELD_NUMBER: builtins.int
-
+    LATEST_HIVE_PARAMETERS_FIELD_NUMBER: builtins.int
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
-
     @property
     def historical_weight(self) -> global___HistoricalWeight: ...
-
     @property
     def recent_temperature(self) -> global___RecentTemperature: ...
-
-    def __init__(self,
+    @property
+    def latest_hive_parameters(self) -> global___LatestHiveParameters: ...
+    def __init__(
+        self,
         *,
-        header : typing.Optional[ho_protocols.common_pb2.Header] = ...,
-        historical_weight : typing.Optional[global___HistoricalWeight] = ...,
-        recent_temperature : typing.Optional[global___RecentTemperature] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"header",b"header",u"historical_weight",b"historical_weight",u"query",b"query",u"recent_temperature",b"recent_temperature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"header",b"header",u"historical_weight",b"historical_weight",u"query",b"query",u"recent_temperature",b"recent_temperature"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"query",b"query"]) -> typing_extensions.Literal["historical_weight","recent_temperature"]: ...
+        header: ho_protocols.common_pb2.Header | None = ...,
+        historical_weight: global___HistoricalWeight | None = ...,
+        recent_temperature: global___RecentTemperature | None = ...,
+        latest_hive_parameters: global___LatestHiveParameters | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "query", b"query", "recent_temperature", b"recent_temperature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "query", b"query", "recent_temperature", b"recent_temperature"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["query", b"query"]) -> typing_extensions.Literal["historical_weight", "recent_temperature", "latest_hive_parameters"] | None: ...
+
 global___QueryRequest = QueryRequest
 
+@typing_extensions.final
 class QueryResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    HEADER_FIELD_NUMBER: builtins.int
     HISTORICAL_WEIGHT_FIELD_NUMBER: builtins.int
     RECENT_TEMPERATURE_FIELD_NUMBER: builtins.int
-
+    LATEST_HIVE_PARAMETERS_FIELD_NUMBER: builtins.int
+    @property
+    def header(self) -> ho_protocols.common_pb2.Header: ...
     @property
     def historical_weight(self) -> global___HistoricalWeightResult: ...
-
     @property
     def recent_temperature(self) -> global___RecentTemperatureResult: ...
-
-    def __init__(self,
+    @property
+    def latest_hive_parameters(self) -> global___LatestHiveParametersResult: ...
+    def __init__(
+        self,
         *,
-        historical_weight : typing.Optional[global___HistoricalWeightResult] = ...,
-        recent_temperature : typing.Optional[global___RecentTemperatureResult] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"historical_weight",b"historical_weight",u"recent_temperature",b"recent_temperature",u"result",b"result"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"historical_weight",b"historical_weight",u"recent_temperature",b"recent_temperature",u"result",b"result"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"result",b"result"]) -> typing_extensions.Literal["historical_weight","recent_temperature"]: ...
+        header: ho_protocols.common_pb2.Header | None = ...,
+        historical_weight: global___HistoricalWeightResult | None = ...,
+        recent_temperature: global___RecentTemperatureResult | None = ...,
+        latest_hive_parameters: global___LatestHiveParametersResult | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "recent_temperature", b"recent_temperature", "result", b"result"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["header", b"header", "historical_weight", b"historical_weight", "latest_hive_parameters", b"latest_hive_parameters", "recent_temperature", b"recent_temperature", "result", b"result"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["historical_weight", "recent_temperature", "latest_hive_parameters"] | None: ...
+
 global___QueryResponse = QueryResponse
 
+@typing_extensions.final
 class HistoricalWeight(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    """### Historical weight query"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     START_TS_FIELD_NUMBER: builtins.int
     END_TS_FIELD_NUMBER: builtins.int
-    start_ts: builtins.int = ...
-    end_ts: builtins.int = ...
-
-    def __init__(self,
+    start_ts: builtins.int
+    end_ts: builtins.int
+    def __init__(
+        self,
         *,
-        start_ts : builtins.int = ...,
-        end_ts : builtins.int = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"end_ts",b"end_ts",u"start_ts",b"start_ts"]) -> None: ...
+        start_ts: builtins.int = ...,
+        end_ts: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["end_ts", b"end_ts", "start_ts", b"start_ts"]) -> None: ...
+
 global___HistoricalWeight = HistoricalWeight
 
+@typing_extensions.final
 class HistoricalWeightResult(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MIN_WEIGHT_FIELD_NUMBER: builtins.int
     MAX_WEIGHT_FIELD_NUMBER: builtins.int
     MEAN_WEIGHT_FIELD_NUMBER: builtins.int
-    min_weight: builtins.float = ...
-    max_weight: builtins.float = ...
-    mean_weight: builtins.float = ...
-
-    def __init__(self,
+    min_weight: builtins.float
+    max_weight: builtins.float
+    mean_weight: builtins.float
+    def __init__(
+        self,
         *,
-        min_weight : builtins.float = ...,
-        max_weight : builtins.float = ...,
-        mean_weight : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"max_weight",b"max_weight",u"mean_weight",b"mean_weight",u"min_weight",b"min_weight"]) -> None: ...
+        min_weight: builtins.float = ...,
+        max_weight: builtins.float = ...,
+        mean_weight: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["max_weight", b"max_weight", "mean_weight", b"mean_weight", "min_weight", b"min_weight"]) -> None: ...
+
 global___HistoricalWeightResult = HistoricalWeightResult
 
+@typing_extensions.final
 class RecentTemperature(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Resolution(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Resolution.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Minute = RecentTemperature.Resolution.V(0)
-        Hour = RecentTemperature.Resolution.V(1)
-        Day = RecentTemperature.Resolution.V(2)
-    class Resolution(metaclass=_Resolution):
-        V = typing.NewType('V', builtins.int)
-    Minute = RecentTemperature.Resolution.V(0)
-    Hour = RecentTemperature.Resolution.V(1)
-    Day = RecentTemperature.Resolution.V(2)
+    """### Recent temperatures"""
 
-    RESOLUTION_FIELD_NUMBER: builtins.int
-    resolution: global___RecentTemperature.Resolution.V = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Resolution:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _ResolutionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[RecentTemperature._Resolution.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        Minute: RecentTemperature._Resolution.ValueType  # 0
+        Hour: RecentTemperature._Resolution.ValueType  # 1
+        Day: RecentTemperature._Resolution.ValueType  # 2
+
+    class Resolution(_Resolution, metaclass=_ResolutionEnumTypeWrapper): ...
+    Minute: RecentTemperature.Resolution.ValueType  # 0
+    Hour: RecentTemperature.Resolution.ValueType  # 1
+    Day: RecentTemperature.Resolution.ValueType  # 2
 
-    def __init__(self,
+    RESOLUTION_FIELD_NUMBER: builtins.int
+    resolution: global___RecentTemperature.Resolution.ValueType
+    def __init__(
+        self,
         *,
-        resolution : global___RecentTemperature.Resolution.V = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"resolution",b"resolution"]) -> None: ...
+        resolution: global___RecentTemperature.Resolution.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resolution", b"resolution"]) -> None: ...
+
 global___RecentTemperature = RecentTemperature
 
+@typing_extensions.final
 class RecentTemperatureResult(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class Record(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         TS_FIELD_NUMBER: builtins.int
         MIN_FIELD_NUMBER: builtins.int
         MAX_FIELD_NUMBER: builtins.int
         MEAN_FIELD_NUMBER: builtins.int
-        ts: builtins.int = ...
-        min: builtins.float = ...
-        max: builtins.float = ...
-        mean: builtins.float = ...
-
-        def __init__(self,
+        ts: builtins.int
+        min: builtins.float
+        max: builtins.float
+        mean: builtins.float
+        def __init__(
+            self,
             *,
-            ts : builtins.int = ...,
-            min : builtins.float = ...,
-            max : builtins.float = ...,
-            mean : builtins.float = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"max",b"max",u"mean",b"mean",u"min",b"min",u"ts",b"ts"]) -> None: ...
+            ts: builtins.int = ...,
+            min: builtins.float = ...,
+            max: builtins.float = ...,
+            mean: builtins.float = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["max", b"max", "mean", b"mean", "min", b"min", "ts", b"ts"]) -> None: ...
 
     START_TS_FIELD_NUMBER: builtins.int
     END_TS_FIELD_NUMBER: builtins.int
     RECORDS_FIELD_NUMBER: builtins.int
-    start_ts: builtins.int = ...
-    end_ts: builtins.int = ...
-
+    start_ts: builtins.int
+    end_ts: builtins.int
     @property
     def records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RecentTemperatureResult.Record]: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        start_ts : builtins.int = ...,
-        end_ts : builtins.int = ...,
-        records : typing.Optional[typing.Iterable[global___RecentTemperatureResult.Record]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"end_ts",b"end_ts",u"records",b"records",u"start_ts",b"start_ts"]) -> None: ...
-global___RecentTemperatureResult = RecentTemperatureResult
+        start_ts: builtins.int = ...,
+        end_ts: builtins.int = ...,
+        records: collections.abc.Iterable[global___RecentTemperatureResult.Record] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["end_ts", b"end_ts", "records", b"records", "start_ts", b"start_ts"]) -> None: ...
 
-class AggHistory(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _AggFunc(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[AggFunc.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Last = AggHistory.AggFunc.V(0)
-        Mean = AggHistory.AggFunc.V(1)
-    class AggFunc(metaclass=_AggFunc):
-        V = typing.NewType('V', builtins.int)
-    Last = AggHistory.AggFunc.V(0)
-    Mean = AggHistory.AggFunc.V(1)
-
-    class _Window(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Window.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Minute = AggHistory.Window.V(0)
-        Hour = AggHistory.Window.V(1)
-        Day = AggHistory.Window.V(2)
-        Week = AggHistory.Window.V(3)
-        Month = AggHistory.Window.V(4)
-    class Window(metaclass=_Window):
-        V = typing.NewType('V', builtins.int)
-    Minute = AggHistory.Window.V(0)
-    Hour = AggHistory.Window.V(1)
-    Day = AggHistory.Window.V(2)
-    Week = AggHistory.Window.V(3)
-    Month = AggHistory.Window.V(4)
+global___RecentTemperatureResult = RecentTemperatureResult
 
-    HEADER_FIELD_NUMBER: builtins.int
-    START_TS_FIELD_NUMBER: builtins.int
-    END_TS_FIELD_NUMBER: builtins.int
-    AGG_FUNC_FIELD_NUMBER: builtins.int
-    WINDOW_FIELD_NUMBER: builtins.int
-    start_ts: builtins.int = ...
-    end_ts: builtins.int = ...
-    agg_func: global___AggHistory.AggFunc.V = ...
-    window: global___AggHistory.Window.V = ...
+@typing_extensions.final
+class LatestHiveParameters(google.protobuf.message.Message):
+    """### Latest hive parameters"""
 
-    @property
-    def header(self) -> ho_protocols.common_pb2.Header: ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    HIVE_ID_FIELD_NUMBER: builtins.int
+    START_TS_FIELD_NUMBER: builtins.int
+    hive_id: builtins.str
+    start_ts: builtins.int
+    def __init__(
+        self,
         *,
-        header : typing.Optional[ho_protocols.common_pb2.Header] = ...,
-        start_ts : builtins.int = ...,
-        end_ts : builtins.int = ...,
-        agg_func : global___AggHistory.AggFunc.V = ...,
-        window : global___AggHistory.Window.V = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"header",b"header"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"agg_func",b"agg_func",u"end_ts",b"end_ts",u"header",b"header",u"start_ts",b"start_ts",u"window",b"window"]) -> None: ...
-global___AggHistory = AggHistory
-
-class AggHistoryResult(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class Row(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        TS_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        ts: builtins.int = ...
-        value: builtins.float = ...
-
-        def __init__(self,
-            *,
-            ts : builtins.int = ...,
-            value : builtins.float = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"ts",b"ts",u"value",b"value"]) -> None: ...
-
-    class Table(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        ROW_FIELD_NUMBER: builtins.int
-
+        hive_id: builtins.str = ...,
+        start_ts: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["hive_id", b"hive_id", "start_ts", b"start_ts"]) -> None: ...
+
+global___LatestHiveParameters = LatestHiveParameters
+
+@typing_extensions.final
+class LatestHiveParametersResult(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
+    class Traffic(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        ID_FIELD_NUMBER: builtins.int
+        BEES_IN_FIELD_NUMBER: builtins.int
+        BEES_OUT_FIELD_NUMBER: builtins.int
+        id: builtins.str
         @property
-        def row(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AggHistoryResult.Row]: ...
-
-        def __init__(self,
+        def bees_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+        @property
+        def bees_out(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+        def __init__(
+            self,
             *,
-            row : typing.Optional[typing.Iterable[global___AggHistoryResult.Row]] = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"row",b"row"]) -> None: ...
-
-    class RecordsEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text = ...
+            id: builtins.str = ...,
+            bees_in: collections.abc.Iterable[builtins.float] | None = ...,
+            bees_out: collections.abc.Iterable[builtins.float] | None = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["bees_in", b"bees_in", "bees_out", b"bees_out", "id", b"id"]) -> None: ...
 
+    @typing_extensions.final
+    class Broodnest(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        ID_FIELD_NUMBER: builtins.int
+        WIDTH_FIELD_NUMBER: builtins.int
+        HEIGHT_FIELD_NUMBER: builtins.int
+        VALUES_FIELD_NUMBER: builtins.int
+        PNG_FIELD_NUMBER: builtins.int
+        id: builtins.str
+        width: builtins.int
+        height: builtins.int
         @property
-        def value(self) -> global___AggHistoryResult.Table: ...
-
-        def __init__(self,
+        def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+        png: builtins.bytes
+        def __init__(
+            self,
             *,
-            key : typing.Text = ...,
-            value : typing.Optional[global___AggHistoryResult.Table] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
-
-    RECORDS_FIELD_NUMBER: builtins.int
-
-    @property
-    def records(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, global___AggHistoryResult.Table]: ...
-
-    def __init__(self,
-        *,
-        records : typing.Optional[typing.Mapping[typing.Text, global___AggHistoryResult.Table]] = ...,
+            id: builtins.str = ...,
+            width: builtins.int = ...,
+            height: builtins.int = ...,
+            values: collections.abc.Iterable[builtins.float] | None = ...,
+            png: builtins.bytes = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"records",b"records"]) -> None: ...
-global___AggHistoryResult = AggHistoryResult
+        def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "id", b"id", "png", b"png", "values", b"values", "width", b"width"]) -> None: ...
 
-class ResultTable(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class Row(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        TS_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        ts: builtins.int = ...
-        value: builtins.float = ...
-
-        def __init__(self,
+    @typing_extensions.final
+    class Harvester(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        ID_FIELD_NUMBER: builtins.int
+        WEIGHT_FIELD_NUMBER: builtins.int
+        id: builtins.str
+        weight: builtins.float
+        def __init__(
+            self,
             *,
-            ts : builtins.int = ...,
-            value : builtins.float = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"ts",b"ts",u"value",b"value"]) -> None: ...
-
-    ROW_FIELD_NUMBER: builtins.int
+            id: builtins.str = ...,
+            weight: builtins.float = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "weight", b"weight"]) -> None: ...
 
+    TRAFFIC_FIELD_NUMBER: builtins.int
+    BROODNEST_FIELD_NUMBER: builtins.int
+    HARVESTER_FIELD_NUMBER: builtins.int
     @property
-    def row(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResultTable.Row]: ...
-
-    def __init__(self,
+    def traffic(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LatestHiveParametersResult.Traffic]: ...
+    @property
+    def broodnest(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LatestHiveParametersResult.Broodnest]: ...
+    @property
+    def harvester(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LatestHiveParametersResult.Harvester]: ...
+    def __init__(
+        self,
         *,
-        row : typing.Optional[typing.Iterable[global___ResultTable.Row]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"row",b"row"]) -> None: ...
-global___ResultTable = ResultTable
+        traffic: collections.abc.Iterable[global___LatestHiveParametersResult.Traffic] | None = ...,
+        broodnest: collections.abc.Iterable[global___LatestHiveParametersResult.Broodnest] | None = ...,
+        harvester: collections.abc.Iterable[global___LatestHiveParametersResult.Harvester] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["broodnest", b"broodnest", "harvester", b"harvester", "traffic", b"traffic"]) -> None: ...
+
+global___LatestHiveParametersResult = LatestHiveParametersResult
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/cmd/cmd_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/cmd/cmd_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,135 +4,157 @@
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.struct_pb2
 import ho_protocols.common_pb2
+import sys
 import typing
-import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class CommandRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     HEADER_FIELD_NUMBER: builtins.int
     EVAC_START_FIELD_NUMBER: builtins.int
     EVAC_STOP_FIELD_NUMBER: builtins.int
     HARVESTER_OPEN_FIELD_NUMBER: builtins.int
     HARVESTER_CLOSE_FIELD_NUMBER: builtins.int
-
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
-
     @property
     def evac_start(self) -> global___EvacuationStart: ...
-
     @property
     def evac_stop(self) -> global___EvacuationStop: ...
-
     @property
     def harvester_open(self) -> global___HarvesterOpen: ...
-
     @property
     def harvester_close(self) -> global___HarvesterClose: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        header : typing.Optional[ho_protocols.common_pb2.Header] = ...,
-        evac_start : typing.Optional[global___EvacuationStart] = ...,
-        evac_stop : typing.Optional[global___EvacuationStop] = ...,
-        harvester_open : typing.Optional[global___HarvesterOpen] = ...,
-        harvester_close : typing.Optional[global___HarvesterClose] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"command",b"command",u"evac_start",b"evac_start",u"evac_stop",b"evac_stop",u"harvester_close",b"harvester_close",u"harvester_open",b"harvester_open",u"header",b"header"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"command",b"command",u"evac_start",b"evac_start",u"evac_stop",b"evac_stop",u"harvester_close",b"harvester_close",u"harvester_open",b"harvester_open",u"header",b"header"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"command",b"command"]) -> typing_extensions.Literal["evac_start","evac_stop","harvester_open","harvester_close"]: ...
+        header: ho_protocols.common_pb2.Header | None = ...,
+        evac_start: global___EvacuationStart | None = ...,
+        evac_stop: global___EvacuationStop | None = ...,
+        harvester_open: global___HarvesterOpen | None = ...,
+        harvester_close: global___HarvesterClose | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["command", b"command", "evac_start", b"evac_start", "evac_stop", b"evac_stop", "harvester_close", b"harvester_close", "harvester_open", b"harvester_open", "header", b"header"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["command", b"command", "evac_start", b"evac_start", "evac_stop", b"evac_stop", "harvester_close", b"harvester_close", "harvester_open", b"harvester_open", "header", b"header"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["command", b"command"]) -> typing_extensions.Literal["evac_start", "evac_stop", "harvester_open", "harvester_close"] | None: ...
+
 global___CommandRequest = CommandRequest
 
+@typing_extensions.final
 class CommandResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class ACKResult(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        def __init__(self,
-            ) -> None: ...
+        def __init__(
+            self,
+        ) -> None: ...
 
+    @typing_extensions.final
     class NACKResult(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        class _Reason(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Reason.V], builtins.type):
-            DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-            Unknown = CommandResponse.NACKResult.Reason.V(0)
-            SenderError = CommandResponse.NACKResult.Reason.V(1)
-            ReceiverError = CommandResponse.NACKResult.Reason.V(2)
-        class Reason(metaclass=_Reason):
-            V = typing.NewType('V', builtins.int)
-        Unknown = CommandResponse.NACKResult.Reason.V(0)
-        SenderError = CommandResponse.NACKResult.Reason.V(1)
-        ReceiverError = CommandResponse.NACKResult.Reason.V(2)
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        class _Reason:
+            ValueType = typing.NewType("ValueType", builtins.int)
+            V: typing_extensions.TypeAlias = ValueType
+
+        class _ReasonEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[CommandResponse.NACKResult._Reason.ValueType], builtins.type):  # noqa: F821
+            DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+            Unknown: CommandResponse.NACKResult._Reason.ValueType  # 0
+            SenderError: CommandResponse.NACKResult._Reason.ValueType  # 1
+            ReceiverError: CommandResponse.NACKResult._Reason.ValueType  # 2
+
+        class Reason(_Reason, metaclass=_ReasonEnumTypeWrapper): ...
+        Unknown: CommandResponse.NACKResult.Reason.ValueType  # 0
+        SenderError: CommandResponse.NACKResult.Reason.ValueType  # 1
+        ReceiverError: CommandResponse.NACKResult.Reason.ValueType  # 2
 
         REASON_FIELD_NUMBER: builtins.int
         DETAILS_FIELD_NUMBER: builtins.int
-        reason: global___CommandResponse.NACKResult.Reason.V = ...
-
+        reason: global___CommandResponse.NACKResult.Reason.ValueType
         @property
         def details(self) -> google.protobuf.struct_pb2.Struct: ...
-
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            reason : global___CommandResponse.NACKResult.Reason.V = ...,
-            details : typing.Optional[google.protobuf.struct_pb2.Struct] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"details",b"details"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"details",b"details",u"reason",b"reason"]) -> None: ...
+            reason: global___CommandResponse.NACKResult.Reason.ValueType = ...,
+            details: google.protobuf.struct_pb2.Struct | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["details", b"details"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["details", b"details", "reason", b"reason"]) -> None: ...
 
     HEADER_FIELD_NUMBER: builtins.int
     ACK_FIELD_NUMBER: builtins.int
     NACK_FIELD_NUMBER: builtins.int
-
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
-
     @property
     def ack(self) -> global___CommandResponse.ACKResult: ...
-
     @property
     def nack(self) -> global___CommandResponse.NACKResult: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        header : typing.Optional[ho_protocols.common_pb2.Header] = ...,
-        ack : typing.Optional[global___CommandResponse.ACKResult] = ...,
-        nack : typing.Optional[global___CommandResponse.NACKResult] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"ack",b"ack",u"header",b"header",u"nack",b"nack",u"result",b"result"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"ack",b"ack",u"header",b"header",u"nack",b"nack",u"result",b"result"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"result",b"result"]) -> typing_extensions.Literal["ack","nack"]: ...
+        header: ho_protocols.common_pb2.Header | None = ...,
+        ack: global___CommandResponse.ACKResult | None = ...,
+        nack: global___CommandResponse.NACKResult | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["ack", b"ack", "header", b"header", "nack", b"nack", "result", b"result"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ack", b"ack", "header", b"header", "nack", b"nack", "result", b"result"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["ack", "nack"] | None: ...
+
 global___CommandResponse = CommandResponse
 
+@typing_extensions.final
 class EvacuationStart(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___EvacuationStart = EvacuationStart
 
+@typing_extensions.final
 class EvacuationStop(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___EvacuationStop = EvacuationStop
 
+@typing_extensions.final
 class HarvesterOpen(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___HarvesterOpen = HarvesterOpen
 
+@typing_extensions.final
 class HarvesterClose(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___HarvesterClose = HarvesterClose
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/live/sensors_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/live/sensors_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,148 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import sys
 import typing
-import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class SensorLiveItem(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     BROODNEST_FIELD_NUMBER: builtins.int
     TRAFFIC_FLOW_FIELD_NUMBER: builtins.int
-    HIVE_SCALES_FIELD_NUMBER: builtins.int
+    HARVESTER_FIELD_NUMBER: builtins.int
     POWER_SUPPLY_FIELD_NUMBER: builtins.int
-
     @property
     def broodnest(self) -> global___Broodnest: ...
-
     @property
     def traffic_flow(self) -> global___TrafficFlow: ...
-
     @property
-    def hive_scales(self) -> global___Scales: ...
-
+    def harvester(self) -> global___Harvester: ...
     @property
     def power_supply(self) -> global___PowerSupply: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        broodnest : typing.Optional[global___Broodnest] = ...,
-        traffic_flow : typing.Optional[global___TrafficFlow] = ...,
-        hive_scales : typing.Optional[global___Scales] = ...,
-        power_supply : typing.Optional[global___PowerSupply] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"broodnest",b"broodnest",u"hive_scales",b"hive_scales",u"power_supply",b"power_supply",u"sensors",b"sensors",u"traffic_flow",b"traffic_flow"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"broodnest",b"broodnest",u"hive_scales",b"hive_scales",u"power_supply",b"power_supply",u"sensors",b"sensors",u"traffic_flow",b"traffic_flow"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"sensors",b"sensors"]) -> typing_extensions.Literal["broodnest","traffic_flow","hive_scales","power_supply"]: ...
+        broodnest: global___Broodnest | None = ...,
+        traffic_flow: global___TrafficFlow | None = ...,
+        harvester: global___Harvester | None = ...,
+        power_supply: global___PowerSupply | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["broodnest", b"broodnest", "harvester", b"harvester", "power_supply", b"power_supply", "sensors", b"sensors", "traffic_flow", b"traffic_flow"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["broodnest", b"broodnest", "harvester", b"harvester", "power_supply", b"power_supply", "sensors", b"sensors", "traffic_flow", b"traffic_flow"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sensors", b"sensors"]) -> typing_extensions.Literal["broodnest", "traffic_flow", "harvester", "power_supply"] | None: ...
+
 global___SensorLiveItem = SensorLiveItem
 
+@typing_extensions.final
 class Broodnest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     TEMP_FIELD_NUMBER: builtins.int
     RH_FIELD_NUMBER: builtins.int
     CO2_FIELD_NUMBER: builtins.int
-    temp: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    rh: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    co2: builtins.float = ...
-
-    def __init__(self,
+    @property
+    def temp(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def rh(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    co2: builtins.float
+    def __init__(
+        self,
         *,
-        temp : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        rh : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        co2 : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"co2",b"co2",u"rh",b"rh",u"temp",b"temp"]) -> None: ...
+        temp: collections.abc.Iterable[builtins.float] | None = ...,
+        rh: collections.abc.Iterable[builtins.float] | None = ...,
+        co2: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["co2", b"co2", "rh", b"rh", "temp", b"temp"]) -> None: ...
+
 global___Broodnest = Broodnest
 
+@typing_extensions.final
 class TrafficFlow(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     BEES_IN_FIELD_NUMBER: builtins.int
     BEES_OUT_FIELD_NUMBER: builtins.int
-    bees_in: builtins.float = ...
-    bees_out: builtins.float = ...
-
-    def __init__(self,
+    @property
+    def bees_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def bees_out(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
         *,
-        bees_in : builtins.float = ...,
-        bees_out : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"bees_in",b"bees_in",u"bees_out",b"bees_out"]) -> None: ...
+        bees_in: collections.abc.Iterable[builtins.float] | None = ...,
+        bees_out: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bees_in", b"bees_in", "bees_out", b"bees_out"]) -> None: ...
+
 global___TrafficFlow = TrafficFlow
 
-class Scales(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    WEIGHT_FIELD_NUMBER: builtins.int
-    weight: builtins.float = ...
+@typing_extensions.final
+class Harvester(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    WEIGHT_FIELD_NUMBER: builtins.int
+    weight: builtins.float
+    def __init__(
+        self,
         *,
-        weight : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"weight",b"weight"]) -> None: ...
-global___Scales = Scales
+        weight: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["weight", b"weight"]) -> None: ...
+
+global___Harvester = Harvester
 
+@typing_extensions.final
 class PowerSupply(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Level(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Level.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Unknown = PowerSupply.Level.V(0)
-        Low = PowerSupply.Level.V(1)
-        Medium = PowerSupply.Level.V(2)
-        High = PowerSupply.Level.V(3)
-    class Level(metaclass=_Level):
-        V = typing.NewType('V', builtins.int)
-    Unknown = PowerSupply.Level.V(0)
-    Low = PowerSupply.Level.V(1)
-    Medium = PowerSupply.Level.V(2)
-    High = PowerSupply.Level.V(3)
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Level:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _LevelEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[PowerSupply._Level.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        Unknown: PowerSupply._Level.ValueType  # 0
+        Low: PowerSupply._Level.ValueType  # 1
+        Medium: PowerSupply._Level.ValueType  # 2
+        High: PowerSupply._Level.ValueType  # 3
+
+    class Level(_Level, metaclass=_LevelEnumTypeWrapper): ...
+    Unknown: PowerSupply.Level.ValueType  # 0
+    Low: PowerSupply.Level.ValueType  # 1
+    Medium: PowerSupply.Level.ValueType  # 2
+    High: PowerSupply.Level.ValueType  # 3
 
     VOLTAGE_FIELD_NUMBER: builtins.int
     CURRENT_DRAW_FIELD_NUMBER: builtins.int
     CURRENT_RATE_FIELD_NUMBER: builtins.int
     LEVEL_FIELD_NUMBER: builtins.int
-    voltage: builtins.float = ...
-    current_draw: builtins.float = ...
-    current_rate: builtins.float = ...
-    level: global___PowerSupply.Level.V = ...
-
-    def __init__(self,
+    voltage: builtins.float
+    current_draw: builtins.float
+    current_rate: builtins.float
+    level: global___PowerSupply.Level.ValueType
+    def __init__(
+        self,
         *,
-        voltage : builtins.float = ...,
-        current_draw : builtins.float = ...,
-        current_rate : builtins.float = ...,
-        level : global___PowerSupply.Level.V = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"current_draw",b"current_draw",u"current_rate",b"current_rate",u"level",b"level",u"voltage",b"voltage"]) -> None: ...
+        voltage: builtins.float = ...,
+        current_draw: builtins.float = ...,
+        current_rate: builtins.float = ...,
+        level: global___PowerSupply.Level.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["current_draw", b"current_draw", "current_rate", b"current_rate", "level", b"level", "voltage", b"voltage"]) -> None: ...
+
 global___PowerSupply = PowerSupply
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/live/system_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/live/system_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import typing
-import typing_extensions
+import sys
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class SystemLiveItem(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    DISK_FIELD_NUMBER: builtins.int
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    DISK_FIELD_NUMBER: builtins.int
     @property
     def disk(self) -> global___Disk: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        disk : typing.Optional[global___Disk] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"disk",b"disk",u"system",b"system"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"disk",b"disk",u"system",b"system"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"system",b"system"]) -> typing_extensions.Literal["disk"]: ...
+        disk: global___Disk | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["disk", b"disk", "system", b"system"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["disk", b"disk", "system", b"system"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["system", b"system"]) -> typing_extensions.Literal["disk"] | None: ...
+
 global___SystemLiveItem = SystemLiveItem
 
+@typing_extensions.final
 class Disk(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___Disk = Disk
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/live/models_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/live/models_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,103 +2,127 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import sys
 import typing
-import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class ModelLiveItem(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     HARVEST_TIME_FIELD_NUMBER: builtins.int
     COLONY_COLLAPSE_FIELD_NUMBER: builtins.int
     HARVESTING_PROCEDURE_FIELD_NUMBER: builtins.int
-
     @property
     def harvest_time(self) -> global___HarvestTime: ...
-
     @property
     def colony_collapse(self) -> global___ColonyCollapse: ...
-
     @property
     def harvesting_procedure(self) -> global___HarvestingProcedure: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        harvest_time : typing.Optional[global___HarvestTime] = ...,
-        colony_collapse : typing.Optional[global___ColonyCollapse] = ...,
-        harvesting_procedure : typing.Optional[global___HarvestingProcedure] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"colony_collapse",b"colony_collapse",u"harvest_time",b"harvest_time",u"harvesting_procedure",b"harvesting_procedure",u"models",b"models"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"colony_collapse",b"colony_collapse",u"harvest_time",b"harvest_time",u"harvesting_procedure",b"harvesting_procedure",u"models",b"models"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"models",b"models"]) -> typing_extensions.Literal["harvest_time","colony_collapse","harvesting_procedure"]: ...
+        harvest_time: global___HarvestTime | None = ...,
+        colony_collapse: global___ColonyCollapse | None = ...,
+        harvesting_procedure: global___HarvestingProcedure | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["colony_collapse", b"colony_collapse", "harvest_time", b"harvest_time", "harvesting_procedure", b"harvesting_procedure", "models", b"models"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["colony_collapse", b"colony_collapse", "harvest_time", b"harvest_time", "harvesting_procedure", b"harvesting_procedure", "models", b"models"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["models", b"models"]) -> typing_extensions.Literal["harvest_time", "colony_collapse", "harvesting_procedure"] | None: ...
+
 global___ModelLiveItem = ModelLiveItem
 
+@typing_extensions.final
 class HarvestTime(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Status(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Status.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Unknown = HarvestTime.Status.V(0)
-        NotReadyYet = HarvestTime.Status.V(1)
-        ReadyToHarvest = HarvestTime.Status.V(2)
-    class Status(metaclass=_Status):
-        V = typing.NewType('V', builtins.int)
-    Unknown = HarvestTime.Status.V(0)
-    NotReadyYet = HarvestTime.Status.V(1)
-    ReadyToHarvest = HarvestTime.Status.V(2)
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Status:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _StatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[HarvestTime._Status.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        Unknown: HarvestTime._Status.ValueType  # 0
+        NotReadyYet: HarvestTime._Status.ValueType  # 1
+        ReadyToHarvest: HarvestTime._Status.ValueType  # 2
+
+    class Status(_Status, metaclass=_StatusEnumTypeWrapper): ...
+    Unknown: HarvestTime.Status.ValueType  # 0
+    NotReadyYet: HarvestTime.Status.ValueType  # 1
+    ReadyToHarvest: HarvestTime.Status.ValueType  # 2
 
     STATUS_FIELD_NUMBER: builtins.int
     WEIGHT_FIELD_NUMBER: builtins.int
-    status: global___HarvestTime.Status.V = ...
-    weight: builtins.float = ...
-
-    def __init__(self,
+    status: global___HarvestTime.Status.ValueType
+    weight: builtins.float
+    """int64 time_estimation = 3;"""
+    def __init__(
+        self,
         *,
-        status : global___HarvestTime.Status.V = ...,
-        weight : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"status",b"status",u"weight",b"weight"]) -> None: ...
+        status: global___HarvestTime.Status.ValueType = ...,
+        weight: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["status", b"status", "weight", b"weight"]) -> None: ...
+
 global___HarvestTime = HarvestTime
 
+@typing_extensions.final
 class ColonyCollapse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    COLLAPSE_PROBABILITY_FIELD_NUMBER: builtins.int
-    collapse_probability: builtins.float = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    COLLAPSE_PROBABILITY_FIELD_NUMBER: builtins.int
+    collapse_probability: builtins.float
+    """int64 time_horizon = 2;"""
+    def __init__(
+        self,
         *,
-        collapse_probability : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"collapse_probability",b"collapse_probability"]) -> None: ...
+        collapse_probability: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["collapse_probability", b"collapse_probability"]) -> None: ...
+
 global___ColonyCollapse = ColonyCollapse
 
+@typing_extensions.final
 class HarvestingProcedure(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Status(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Status.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Unknown = HarvestingProcedure.Status.V(0)
-        Success = HarvestingProcedure.Status.V(1)
-        Interrupted = HarvestingProcedure.Status.V(2)
-        Failure = HarvestingProcedure.Status.V(3)
-    class Status(metaclass=_Status):
-        V = typing.NewType('V', builtins.int)
-    Unknown = HarvestingProcedure.Status.V(0)
-    Success = HarvestingProcedure.Status.V(1)
-    Interrupted = HarvestingProcedure.Status.V(2)
-    Failure = HarvestingProcedure.Status.V(3)
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Status:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _StatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[HarvestingProcedure._Status.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        Unknown: HarvestingProcedure._Status.ValueType  # 0
+        Success: HarvestingProcedure._Status.ValueType  # 1
+        Interrupted: HarvestingProcedure._Status.ValueType  # 2
+        Failure: HarvestingProcedure._Status.ValueType  # 3
+
+    class Status(_Status, metaclass=_StatusEnumTypeWrapper): ...
+    Unknown: HarvestingProcedure.Status.ValueType  # 0
+    Success: HarvestingProcedure.Status.ValueType  # 1
+    Interrupted: HarvestingProcedure.Status.ValueType  # 2
+    Failure: HarvestingProcedure.Status.ValueType  # 3
 
     STATUS_FIELD_NUMBER: builtins.int
     HARVESTED_AMOUNT_FIELD_NUMBER: builtins.int
-    status: global___HarvestingProcedure.Status.V = ...
-    harvested_amount: builtins.float = ...
-
-    def __init__(self,
+    status: global___HarvestingProcedure.Status.ValueType
+    harvested_amount: builtins.float
+    def __init__(
+        self,
         *,
-        status : global___HarvestingProcedure.Status.V = ...,
-        harvested_amount : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"harvested_amount",b"harvested_amount",u"status",b"status"]) -> None: ...
+        status: global___HarvestingProcedure.Status.ValueType = ...,
+        harvested_amount: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["harvested_amount", b"harvested_amount", "status", b"status"]) -> None: ...
+
 global___HarvestingProcedure = HarvestingProcedure
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/live/live_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/live/live_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -7,59 +7,64 @@
 import google.protobuf.message
 import google.protobuf.struct_pb2
 import ho_protocols.common_pb2
 import ho_protocols.live.actuators_pb2
 import ho_protocols.live.models_pb2
 import ho_protocols.live.sensors_pb2
 import ho_protocols.live.system_pb2
-import typing
-import typing_extensions
+import sys
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class LiveStreamItem(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     HEADER_FIELD_NUMBER: builtins.int
     SENSORS_FIELD_NUMBER: builtins.int
     ACTUATORS_FIELD_NUMBER: builtins.int
     SYSTEM_FIELD_NUMBER: builtins.int
     MODELS_FIELD_NUMBER: builtins.int
     UNMAPPED_FIELD_NUMBER: builtins.int
-
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
-
     @property
     def sensors(self) -> ho_protocols.live.sensors_pb2.SensorLiveItem: ...
-
     @property
     def actuators(self) -> ho_protocols.live.actuators_pb2.ActuatorLiveItem: ...
-
     @property
     def system(self) -> ho_protocols.live.system_pb2.SystemLiveItem: ...
-
     @property
     def models(self) -> ho_protocols.live.models_pb2.ModelLiveItem: ...
-
     @property
-    def unmapped(self) -> google.protobuf.struct_pb2.Struct: ...
-
-    def __init__(self,
+    def unmapped(self) -> google.protobuf.struct_pb2.Struct:
+        """structure for unmapped fields as a fallback"""
+    def __init__(
+        self,
         *,
-        header : typing.Optional[ho_protocols.common_pb2.Header] = ...,
-        sensors : typing.Optional[ho_protocols.live.sensors_pb2.SensorLiveItem] = ...,
-        actuators : typing.Optional[ho_protocols.live.actuators_pb2.ActuatorLiveItem] = ...,
-        system : typing.Optional[ho_protocols.live.system_pb2.SystemLiveItem] = ...,
-        models : typing.Optional[ho_protocols.live.models_pb2.ModelLiveItem] = ...,
-        unmapped : typing.Optional[google.protobuf.struct_pb2.Struct] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"actuators",b"actuators",u"header",b"header",u"models",b"models",u"payload",b"payload",u"sensors",b"sensors",u"system",b"system",u"unmapped",b"unmapped"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"actuators",b"actuators",u"header",b"header",u"models",b"models",u"payload",b"payload",u"sensors",b"sensors",u"system",b"system",u"unmapped",b"unmapped"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"payload",b"payload"]) -> typing_extensions.Literal["sensors","actuators","system","models"]: ...
+        header: ho_protocols.common_pb2.Header | None = ...,
+        sensors: ho_protocols.live.sensors_pb2.SensorLiveItem | None = ...,
+        actuators: ho_protocols.live.actuators_pb2.ActuatorLiveItem | None = ...,
+        system: ho_protocols.live.system_pb2.SystemLiveItem | None = ...,
+        models: ho_protocols.live.models_pb2.ModelLiveItem | None = ...,
+        unmapped: google.protobuf.struct_pb2.Struct | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["actuators", b"actuators", "header", b"header", "models", b"models", "payload", b"payload", "sensors", b"sensors", "system", b"system", "unmapped", b"unmapped"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["actuators", b"actuators", "header", b"header", "models", b"models", "payload", b"payload", "sensors", b"sensors", "system", b"system", "unmapped", b"unmapped"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["payload", b"payload"]) -> typing_extensions.Literal["sensors", "actuators", "system", "models"] | None: ...
+
 global___LiveStreamItem = LiveStreamItem
 
+@typing_extensions.final
 class ArchiveStreamItem(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___ArchiveStreamItem = ArchiveStreamItem
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/data_in_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/data_in_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,299 +1,361 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import sys
 import typing
-import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class DataInWrapper(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     TS_FIELD_NUMBER: builtins.int
     INSTANCE_FIELD_NUMBER: builtins.int
     TRAFFIC_FLOW_FIELD_NUMBER: builtins.int
     BROOD_NEST_FIELD_NUMBER: builtins.int
     ENV_MONITOR_FIELD_NUMBER: builtins.int
     HIVE_SCALE_FIELD_NUMBER: builtins.int
     WEATHER_STATION_FIELD_NUMBER: builtins.int
     WEATHER_FORECAST_FIELD_NUMBER: builtins.int
     DANCE_DETECTION_FIELD_NUMBER: builtins.int
     ACTUATOR_STATUS_FIELD_NUMBER: builtins.int
     GNSS_FIELD_NUMBER: builtins.int
     POWER_SUPPLY_FIELD_NUMBER: builtins.int
-    ts: builtins.int = ...
-    instance: builtins.int = ...
-
+    ts: builtins.int
+    instance: builtins.int
     @property
     def traffic_flow(self) -> global___TrafficFlow: ...
-
     @property
     def brood_nest(self) -> global___BroodNest: ...
-
     @property
     def env_monitor(self) -> global___EnvironmentMonitor: ...
-
     @property
     def hive_scale(self) -> global___HiveScale: ...
-
     @property
     def weather_station(self) -> global___WeatherStation: ...
-
     @property
     def weather_forecast(self) -> global___WeatherForecast: ...
-
     @property
     def dance_detection(self) -> global___DanceDetection: ...
-
     @property
     def actuator_status(self) -> global___ActuatorStatus: ...
-
     @property
     def gnss(self) -> global___GNSS: ...
-
     @property
     def power_supply(self) -> global___PowerSupply: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        ts : builtins.int = ...,
-        instance : builtins.int = ...,
-        traffic_flow : typing.Optional[global___TrafficFlow] = ...,
-        brood_nest : typing.Optional[global___BroodNest] = ...,
-        env_monitor : typing.Optional[global___EnvironmentMonitor] = ...,
-        hive_scale : typing.Optional[global___HiveScale] = ...,
-        weather_station : typing.Optional[global___WeatherStation] = ...,
-        weather_forecast : typing.Optional[global___WeatherForecast] = ...,
-        dance_detection : typing.Optional[global___DanceDetection] = ...,
-        actuator_status : typing.Optional[global___ActuatorStatus] = ...,
-        gnss : typing.Optional[global___GNSS] = ...,
-        power_supply : typing.Optional[global___PowerSupply] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"actuator_status",b"actuator_status",u"brood_nest",b"brood_nest",u"dance_detection",b"dance_detection",u"data",b"data",u"env_monitor",b"env_monitor",u"gnss",b"gnss",u"hive_scale",b"hive_scale",u"power_supply",b"power_supply",u"traffic_flow",b"traffic_flow",u"weather_forecast",b"weather_forecast",u"weather_station",b"weather_station"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"actuator_status",b"actuator_status",u"brood_nest",b"brood_nest",u"dance_detection",b"dance_detection",u"data",b"data",u"env_monitor",b"env_monitor",u"gnss",b"gnss",u"hive_scale",b"hive_scale",u"instance",b"instance",u"power_supply",b"power_supply",u"traffic_flow",b"traffic_flow",u"ts",b"ts",u"weather_forecast",b"weather_forecast",u"weather_station",b"weather_station"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"data",b"data"]) -> typing_extensions.Literal["traffic_flow","brood_nest","env_monitor","hive_scale","weather_station","weather_forecast","dance_detection","actuator_status","gnss","power_supply"]: ...
+        ts: builtins.int = ...,
+        instance: builtins.int = ...,
+        traffic_flow: global___TrafficFlow | None = ...,
+        brood_nest: global___BroodNest | None = ...,
+        env_monitor: global___EnvironmentMonitor | None = ...,
+        hive_scale: global___HiveScale | None = ...,
+        weather_station: global___WeatherStation | None = ...,
+        weather_forecast: global___WeatherForecast | None = ...,
+        dance_detection: global___DanceDetection | None = ...,
+        actuator_status: global___ActuatorStatus | None = ...,
+        gnss: global___GNSS | None = ...,
+        power_supply: global___PowerSupply | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["actuator_status", b"actuator_status", "brood_nest", b"brood_nest", "dance_detection", b"dance_detection", "data", b"data", "env_monitor", b"env_monitor", "gnss", b"gnss", "hive_scale", b"hive_scale", "power_supply", b"power_supply", "traffic_flow", b"traffic_flow", "weather_forecast", b"weather_forecast", "weather_station", b"weather_station"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["actuator_status", b"actuator_status", "brood_nest", b"brood_nest", "dance_detection", b"dance_detection", "data", b"data", "env_monitor", b"env_monitor", "gnss", b"gnss", "hive_scale", b"hive_scale", "instance", b"instance", "power_supply", b"power_supply", "traffic_flow", b"traffic_flow", "ts", b"ts", "weather_forecast", b"weather_forecast", "weather_station", b"weather_station"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["data", b"data"]) -> typing_extensions.Literal["traffic_flow", "brood_nest", "env_monitor", "hive_scale", "weather_station", "weather_forecast", "dance_detection", "actuator_status", "gnss", "power_supply"] | None: ...
+
 global___DataInWrapper = DataInWrapper
 
+@typing_extensions.final
 class TrafficFlow(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     BEESIN_FIELD_NUMBER: builtins.int
     BEESOUT_FIELD_NUMBER: builtins.int
-    beesIn: builtins.int = ...
-    beesOut: builtins.int = ...
+    beesIn: builtins.int
+    beesOut: builtins.int
+    def __init__(
+        self,
+        *,
+        beesIn: builtins.int = ...,
+        beesOut: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["beesIn", b"beesIn", "beesOut", b"beesOut"]) -> None: ...
 
-    def __init__(self,
-        *,
-        beesIn : builtins.int = ...,
-        beesOut : builtins.int = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"beesIn",b"beesIn",u"beesOut",b"beesOut"]) -> None: ...
 global___TrafficFlow = TrafficFlow
 
+@typing_extensions.final
 class BroodNest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     CO2_FIELD_NUMBER: builtins.int
     HUMIDITY_FIELD_NUMBER: builtins.int
     TEMPERATURE_FIELD_NUMBER: builtins.int
-    co2: builtins.float = ...
-    humidity: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    temperature: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-
-    def __init__(self,
-        *,
-        co2 : builtins.float = ...,
-        humidity : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        temperature : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"co2",b"co2",u"humidity",b"humidity",u"temperature",b"temperature"]) -> None: ...
+    co2: builtins.float
+    @property
+    def humidity(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def temperature(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        co2: builtins.float = ...,
+        humidity: collections.abc.Iterable[builtins.float] | None = ...,
+        temperature: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["co2", b"co2", "humidity", b"humidity", "temperature", b"temperature"]) -> None: ...
+
 global___BroodNest = BroodNest
 
+@typing_extensions.final
 class EnvironmentMonitor(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     CO2_FIELD_NUMBER: builtins.int
     HUMIDITY_FIELD_NUMBER: builtins.int
     TEMPERATURE_FIELD_NUMBER: builtins.int
     SYS_HEALTH_FIELD_NUMBER: builtins.int
-    co2: builtins.float = ...
-    humidity: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    temperature: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    sys_health: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-
-    def __init__(self,
-        *,
-        co2 : builtins.float = ...,
-        humidity : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        temperature : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        sys_health : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"co2",b"co2",u"humidity",b"humidity",u"sys_health",b"sys_health",u"temperature",b"temperature"]) -> None: ...
+    co2: builtins.float
+    @property
+    def humidity(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def temperature(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def sys_health(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        co2: builtins.float = ...,
+        humidity: collections.abc.Iterable[builtins.float] | None = ...,
+        temperature: collections.abc.Iterable[builtins.float] | None = ...,
+        sys_health: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["co2", b"co2", "humidity", b"humidity", "sys_health", b"sys_health", "temperature", b"temperature"]) -> None: ...
+
 global___EnvironmentMonitor = EnvironmentMonitor
 
+@typing_extensions.final
 class HiveScale(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     WEIGHT_FIELD_NUMBER: builtins.int
-    weight: builtins.float = ...
+    weight: builtins.float
+    def __init__(
+        self,
+        *,
+        weight: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["weight", b"weight"]) -> None: ...
 
-    def __init__(self,
-        *,
-        weight : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"weight",b"weight"]) -> None: ...
 global___HiveScale = HiveScale
 
+@typing_extensions.final
 class WeatherStation(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     INDOOR_FIELD_NUMBER: builtins.int
     OUTDOOR_FIELD_NUMBER: builtins.int
-    indoor: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    outdoor: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
+    @property
+    def indoor(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
+        """TODO: define parameter names"""
+    @property
+    def outdoor(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        indoor: collections.abc.Iterable[builtins.float] | None = ...,
+        outdoor: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["indoor", b"indoor", "outdoor", b"outdoor"]) -> None: ...
 
-    def __init__(self,
-        *,
-        indoor : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        outdoor : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"indoor",b"indoor",u"outdoor",b"outdoor"]) -> None: ...
 global___WeatherStation = WeatherStation
 
+@typing_extensions.final
 class WeatherForecast(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     CURRENT_FIELD_NUMBER: builtins.int
     NEXT_HOUR_FIELD_NUMBER: builtins.int
     NEXT_2DAYS_FIELD_NUMBER: builtins.int
     NEXT_7DAYS_FIELD_NUMBER: builtins.int
-    current: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    next_hour: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    next_2days: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    next_7days: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-
-    def __init__(self,
-        *,
-        current : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        next_hour : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        next_2days : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        next_7days : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"current",b"current",u"next_2days",b"next_2days",u"next_7days",b"next_7days",u"next_hour",b"next_hour"]) -> None: ...
+    @property
+    def current(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
+        """TODO: check value types, define better names, split into various arrays"""
+    @property
+    def next_hour(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def next_2days(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    @property
+    def next_7days(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        current: collections.abc.Iterable[builtins.float] | None = ...,
+        next_hour: collections.abc.Iterable[builtins.float] | None = ...,
+        next_2days: collections.abc.Iterable[builtins.float] | None = ...,
+        next_7days: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["current", b"current", "next_2days", b"next_2days", "next_7days", b"next_7days", "next_hour", b"next_hour"]) -> None: ...
+
 global___WeatherForecast = WeatherForecast
 
+@typing_extensions.final
 class DanceDetection(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     WAGGLE_RUN_INFO_FIELD_NUMBER: builtins.int
     DANCE_INFO_FIELD_NUMBER: builtins.int
-    waggle_run_info: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
-    dance_info: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
+    @property
+    def waggle_run_info(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
+        """TODO: split into defined parts?"""
+    @property
+    def dance_info(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        waggle_run_info: collections.abc.Iterable[builtins.float] | None = ...,
+        dance_info: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dance_info", b"dance_info", "waggle_run_info", b"waggle_run_info"]) -> None: ...
 
-    def __init__(self,
-        *,
-        waggle_run_info : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        dance_info : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"dance_info",b"dance_info",u"waggle_run_info",b"waggle_run_info"]) -> None: ...
 global___DanceDetection = DanceDetection
 
+@typing_extensions.final
 class ActuatorStatus(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Type(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Type.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        FrontGateClosure = ActuatorStatus.Type.V(0)
-        TrafficControlModulator = ActuatorStatus.Type.V(1)
-        HoneyHarvester = ActuatorStatus.Type.V(2)
-        DanceRobot = ActuatorStatus.Type.V(3)
-        DanceInhibitor = ActuatorStatus.Type.V(4)
-        BroodNestHeater = ActuatorStatus.Type.V(5)
-    class Type(metaclass=_Type):
-        V = typing.NewType('V', builtins.int)
-    FrontGateClosure = ActuatorStatus.Type.V(0)
-    TrafficControlModulator = ActuatorStatus.Type.V(1)
-    HoneyHarvester = ActuatorStatus.Type.V(2)
-    DanceRobot = ActuatorStatus.Type.V(3)
-    DanceInhibitor = ActuatorStatus.Type.V(4)
-    BroodNestHeater = ActuatorStatus.Type.V(5)
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class _Type:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ActuatorStatus._Type.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        FrontGateClosure: ActuatorStatus._Type.ValueType  # 0
+        TrafficControlModulator: ActuatorStatus._Type.ValueType  # 1
+        HoneyHarvester: ActuatorStatus._Type.ValueType  # 2
+        DanceRobot: ActuatorStatus._Type.ValueType  # 3
+        DanceInhibitor: ActuatorStatus._Type.ValueType  # 4
+        BroodNestHeater: ActuatorStatus._Type.ValueType  # 5
+        """TODO: is it heater?"""
+
+    class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
+    FrontGateClosure: ActuatorStatus.Type.ValueType  # 0
+    TrafficControlModulator: ActuatorStatus.Type.ValueType  # 1
+    HoneyHarvester: ActuatorStatus.Type.ValueType  # 2
+    DanceRobot: ActuatorStatus.Type.ValueType  # 3
+    DanceInhibitor: ActuatorStatus.Type.ValueType  # 4
+    BroodNestHeater: ActuatorStatus.Type.ValueType  # 5
+    """TODO: is it heater?"""
+
+    @typing_extensions.final
     class Status(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         CODE_FIELD_NUMBER: builtins.int
         DATA_FIELD_NUMBER: builtins.int
-        code: typing.Text = ...
-        data: builtins.bytes = ...
-
-        def __init__(self,
+        code: builtins.str
+        data: builtins.bytes
+        def __init__(
+            self,
             *,
-            code : typing.Text = ...,
-            data : builtins.bytes = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"code",b"code",u"data",b"data"]) -> None: ...
+            code: builtins.str = ...,
+            data: builtins.bytes = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "data", b"data"]) -> None: ...
 
     TYPE_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
-    type: global___ActuatorStatus.Type.V = ...
-
+    type: global___ActuatorStatus.Type.ValueType
     @property
     def status(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ActuatorStatus.Status]: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        type : global___ActuatorStatus.Type.V = ...,
-        status : typing.Optional[typing.Iterable[global___ActuatorStatus.Status]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"status",b"status",u"type",b"type"]) -> None: ...
+        type: global___ActuatorStatus.Type.ValueType = ...,
+        status: collections.abc.Iterable[global___ActuatorStatus.Status] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["status", b"status", "type", b"type"]) -> None: ...
+
 global___ActuatorStatus = ActuatorStatus
 
+@typing_extensions.final
 class GNSS(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     TIME_REF_FIELD_NUMBER: builtins.int
     POS_FIELD_NUMBER: builtins.int
-    time_ref: builtins.int = ...
-    pos: google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float] = ...
+    time_ref: builtins.int
+    @property
+    def pos(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    def __init__(
+        self,
+        *,
+        time_ref: builtins.int = ...,
+        pos: collections.abc.Iterable[builtins.float] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pos", b"pos", "time_ref", b"time_ref"]) -> None: ...
 
-    def __init__(self,
-        *,
-        time_ref : builtins.int = ...,
-        pos : typing.Optional[typing.Iterable[builtins.float]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"pos",b"pos",u"time_ref",b"time_ref"]) -> None: ...
 global___GNSS = GNSS
 
+@typing_extensions.final
 class PowerSupply(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     VOLTAGE_FIELD_NUMBER: builtins.int
     CURRENT_DRAW_FIELD_NUMBER: builtins.int
     CURRENT_RATE_FIELD_NUMBER: builtins.int
-    voltage: builtins.float = ...
-    current_draw: builtins.float = ...
-    current_rate: builtins.float = ...
-
-    def __init__(self,
-        *,
-        voltage : builtins.float = ...,
-        current_draw : builtins.float = ...,
-        current_rate : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"current_draw",b"current_draw",u"current_rate",b"current_rate",u"voltage",b"voltage"]) -> None: ...
+    voltage: builtins.float
+    current_draw: builtins.float
+    current_rate: builtins.float
+    def __init__(
+        self,
+        *,
+        voltage: builtins.float = ...,
+        current_draw: builtins.float = ...,
+        current_rate: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["current_draw", b"current_draw", "current_rate", b"current_rate", "voltage", b"voltage"]) -> None: ...
+
 global___PowerSupply = PowerSupply
 
+@typing_extensions.final
 class DataInResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Status(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Status.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        Ok = DataInResponse.Status.V(0)
-        Nok = DataInResponse.Status.V(1)
-    class Status(metaclass=_Status):
-        V = typing.NewType('V', builtins.int)
-    Ok = DataInResponse.Status.V(0)
-    Nok = DataInResponse.Status.V(1)
+    """not used currently"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Status:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _StatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[DataInResponse._Status.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        Ok: DataInResponse._Status.ValueType  # 0
+        Nok: DataInResponse._Status.ValueType  # 1
+
+    class Status(_Status, metaclass=_StatusEnumTypeWrapper): ...
+    Ok: DataInResponse.Status.ValueType  # 0
+    Nok: DataInResponse.Status.ValueType  # 1
 
     STATUS_FIELD_NUMBER: builtins.int
-    status: global___DataInResponse.Status.V = ...
+    status: global___DataInResponse.Status.ValueType
+    def __init__(
+        self,
+        *,
+        status: global___DataInResponse.Status.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["status", b"status"]) -> None: ...
 
-    def __init__(self,
-        *,
-        status : global___DataInResponse.Status.V = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"status",b"status"]) -> None: ...
 global___DataInResponse = DataInResponse
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/example_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/example_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -2,50 +2,65 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import sys
 import typing
-import typing_extensions
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class ExampleRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class _Type(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[Type.V], builtins.type):
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
-        One = ExampleRequest.Type.V(0)
-        Two = ExampleRequest.Type.V(1)
-    class Type(metaclass=_Type):
-        V = typing.NewType('V', builtins.int)
-    One = ExampleRequest.Type.V(0)
-    Two = ExampleRequest.Type.V(1)
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _Type:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ExampleRequest._Type.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        One: ExampleRequest._Type.ValueType  # 0
+        Two: ExampleRequest._Type.ValueType  # 1
+
+    class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
+    One: ExampleRequest.Type.ValueType  # 0
+    Two: ExampleRequest.Type.ValueType  # 1
 
     TYPE_FIELD_NUMBER: builtins.int
     PARAM_FIELD_NUMBER: builtins.int
-    type: global___ExampleRequest.Type.V = ...
-    param: builtins.int = ...
-
-    def __init__(self,
+    type: global___ExampleRequest.Type.ValueType
+    param: builtins.int
+    def __init__(
+        self,
         *,
-        type : global___ExampleRequest.Type.V = ...,
-        param : builtins.int = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"param",b"param",u"type",b"type"]) -> None: ...
+        type: global___ExampleRequest.Type.ValueType = ...,
+        param: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["param", b"param", "type", b"type"]) -> None: ...
+
 global___ExampleRequest = ExampleRequest
 
+@typing_extensions.final
 class ExampleResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     VALUEA_FIELD_NUMBER: builtins.int
     VALUEB_FIELD_NUMBER: builtins.int
-    valueA: typing.Text = ...
-    valueB: builtins.float = ...
-
-    def __init__(self,
+    valueA: builtins.str
+    valueB: builtins.float
+    def __init__(
+        self,
         *,
-        valueA : typing.Text = ...,
-        valueB : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"valueA",b"valueA",u"valueB",b"valueB"]) -> None: ...
+        valueA: builtins.str = ...,
+        valueB: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["valueA", b"valueA", "valueB", b"valueB"]) -> None: ...
+
 global___ExampleResponse = ExampleResponse
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/alert/system_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/system_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,103 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import typing
-import typing_extensions
+import sys
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class SystemAlert(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     BROODNEST_OVEREHEATING_FIELD_NUMBER: builtins.int
     POWER_FAILURE_FIELD_NUMBER: builtins.int
     HARVESTING_FAILURE_FIELD_NUMBER: builtins.int
     HARVESTING_INTERRUPT_FIELD_NUMBER: builtins.int
-
     @property
     def broodnest_overeheating(self) -> global___BroodnestOverheating: ...
-
     @property
     def power_failure(self) -> global___PowerFailure: ...
-
     @property
     def harvesting_failure(self) -> global___HarvestingFailure: ...
-
     @property
     def harvesting_interrupt(self) -> global___HarvestingInterrupt: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        broodnest_overeheating : typing.Optional[global___BroodnestOverheating] = ...,
-        power_failure : typing.Optional[global___PowerFailure] = ...,
-        harvesting_failure : typing.Optional[global___HarvestingFailure] = ...,
-        harvesting_interrupt : typing.Optional[global___HarvestingInterrupt] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"broodnest_overeheating",b"broodnest_overeheating",u"harvesting_failure",b"harvesting_failure",u"harvesting_interrupt",b"harvesting_interrupt",u"power_failure",b"power_failure",u"type",b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"broodnest_overeheating",b"broodnest_overeheating",u"harvesting_failure",b"harvesting_failure",u"harvesting_interrupt",b"harvesting_interrupt",u"power_failure",b"power_failure",u"type",b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"type",b"type"]) -> typing_extensions.Literal["broodnest_overeheating","power_failure","harvesting_failure","harvesting_interrupt"]: ...
+        broodnest_overeheating: global___BroodnestOverheating | None = ...,
+        power_failure: global___PowerFailure | None = ...,
+        harvesting_failure: global___HarvestingFailure | None = ...,
+        harvesting_interrupt: global___HarvestingInterrupt | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["broodnest_overeheating", b"broodnest_overeheating", "harvesting_failure", b"harvesting_failure", "harvesting_interrupt", b"harvesting_interrupt", "power_failure", b"power_failure", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["broodnest_overeheating", b"broodnest_overeheating", "harvesting_failure", b"harvesting_failure", "harvesting_interrupt", b"harvesting_interrupt", "power_failure", b"power_failure", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["broodnest_overeheating", "power_failure", "harvesting_failure", "harvesting_interrupt"] | None: ...
+
 global___SystemAlert = SystemAlert
 
+@typing_extensions.final
 class BroodnestOverheating(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MEAN_TEMP_FIELD_NUMBER: builtins.int
     SENSOR_ID_FIELD_NUMBER: builtins.int
-    mean_temp: builtins.float = ...
-    sensor_id: typing.Text = ...
-
-    def __init__(self,
+    mean_temp: builtins.float
+    sensor_id: builtins.str
+    def __init__(
+        self,
         *,
-        mean_temp : builtins.float = ...,
-        sensor_id : typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"mean_temp",b"mean_temp",u"sensor_id",b"sensor_id"]) -> None: ...
+        mean_temp: builtins.float = ...,
+        sensor_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["mean_temp", b"mean_temp", "sensor_id", b"sensor_id"]) -> None: ...
+
 global___BroodnestOverheating = BroodnestOverheating
 
+@typing_extensions.final
 class PowerFailure(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
 
-    def __init__(self,
-        ) -> None: ...
 global___PowerFailure = PowerFailure
 
+@typing_extensions.final
 class HarvestingFailure(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    REASON_FIELD_NUMBER: builtins.int
-    reason: typing.Text = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    REASON_FIELD_NUMBER: builtins.int
+    reason: builtins.str
+    def __init__(
+        self,
         *,
-        reason : typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"reason",b"reason"]) -> None: ...
+        reason: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["reason", b"reason"]) -> None: ...
+
 global___HarvestingFailure = HarvestingFailure
 
+@typing_extensions.final
 class HarvestingInterrupt(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    REASON_FIELD_NUMBER: builtins.int
-    reason: typing.Text = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    REASON_FIELD_NUMBER: builtins.int
+    reason: builtins.str
+    def __init__(
+        self,
         *,
-        reason : typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"reason",b"reason"]) -> None: ...
+        reason: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["reason", b"reason"]) -> None: ...
+
 global___HarvestingInterrupt = HarvestingInterrupt
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols/alert/bees_pb2.pyi` & `ho-protocols-0.0.2.dev4/src/ho_protocols/alert/bees_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import typing
-import typing_extensions
+import sys
 
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
+if sys.version_info >= (3, 8):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
+DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
+
+@typing_extensions.final
 class BeesAlert(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     SWARMING_FIELD_NUMBER: builtins.int
     DEATH_FIELD_NUMBER: builtins.int
-
     @property
     def swarming(self) -> global___Swarming: ...
-
     @property
     def death(self) -> global___Death: ...
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        swarming : typing.Optional[global___Swarming] = ...,
-        death : typing.Optional[global___Death] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"death",b"death",u"swarming",b"swarming",u"type",b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"death",b"death",u"swarming",b"swarming",u"type",b"type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal[u"type",b"type"]) -> typing_extensions.Literal["swarming","death"]: ...
+        swarming: global___Swarming | None = ...,
+        death: global___Death | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["death", b"death", "swarming", b"swarming", "type", b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["death", b"death", "swarming", b"swarming", "type", b"type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["type", b"type"]) -> typing_extensions.Literal["swarming", "death"] | None: ...
+
 global___BeesAlert = BeesAlert
 
+@typing_extensions.final
 class Swarming(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    PROBABILITY_FIELD_NUMBER: builtins.int
-    probability: builtins.float = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    PROBABILITY_FIELD_NUMBER: builtins.int
+    probability: builtins.float
+    def __init__(
+        self,
         *,
-        probability : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"probability",b"probability"]) -> None: ...
+        probability: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["probability", b"probability"]) -> None: ...
+
 global___Swarming = Swarming
 
+@typing_extensions.final
 class Death(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    PROBABILITY_FIELD_NUMBER: builtins.int
-    probability: builtins.float = ...
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    def __init__(self,
+    PROBABILITY_FIELD_NUMBER: builtins.int
+    probability: builtins.float
+    def __init__(
+        self,
         *,
-        probability : builtins.float = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"probability",b"probability"]) -> None: ...
+        probability: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["probability", b"probability"]) -> None: ...
+
 global___Death = Death
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/PKG-INFO` & `ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.0.2.dev3
+Version: 0.0.2.dev4
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -64,9 +62,7 @@
 ```
 
 Publish to PyPi
 ```bash
 twine upload dist/*
 ```
 
-
-
```

### Comparing `ho-protocols-0.0.2.dev3/src/ho_protocols.egg-info/SOURCES.txt` & `ho-protocols-0.0.2.dev4/src/ho_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.0.2.dev3/test/test.py` & `ho-protocols-0.0.2.dev4/test/test.py`

 * *Files identical despite different names*

