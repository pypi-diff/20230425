# Comparing `tmp/airthings-exporter-0.0.2.tar.gz` & `tmp/airthings-exporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airthings-exporter-0.0.2.tar", last modified: Sun Apr 16 21:56:18 2023, max compression
+gzip compressed data, was "airthings-exporter-0.0.3.tar", last modified: Tue Apr 25 04:51:33 2023, max compression
```

## Comparing `airthings-exporter-0.0.2.tar` & `airthings-exporter-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.698779 airthings-exporter-0.0.2/
--rw-r--r--   0 max        (501) staff       (20)      113 2023-04-16 21:56:18.698656 airthings-exporter-0.0.2/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      812 2022-11-27 23:09:31.000000 airthings-exporter-0.0.2/README.md
--rw-r--r--   0 max        (501) staff       (20)      387 2023-04-16 21:56:08.000000 airthings-exporter-0.0.2/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       38 2023-04-16 21:56:18.698813 airthings-exporter-0.0.2/setup.cfg
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.696733 airthings-exporter-0.0.2/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.697723 airthings-exporter-0.0.2/src/airthings/
--rw-r--r--   0 max        (501) staff       (20)     3326 2023-04-16 21:32:40.000000 airthings-exporter-0.0.2/src/airthings/CloudCollector.py
--rw-r--r--   0 max        (501) staff       (20)        0 2022-11-27 23:11:13.000000 airthings-exporter-0.0.2/src/airthings/__init__.py
--rw-r--r--   0 max        (501) staff       (20)      666 2023-04-16 21:24:49.000000 airthings-exporter-0.0.2/src/airthings/main.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-16 21:56:18.698513 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/
--rw-r--r--   0 max        (501) staff       (20)      113 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      382 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       59 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)       43 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       10 2023-04-16 21:56:18.000000 airthings-exporter-0.0.2/src/airthings_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 04:51:33.376509 airthings-exporter-0.0.3/
+-rw-r--r--   0 max        (501) staff       (20)     1774 2023-04-25 04:51:33.376391 airthings-exporter-0.0.3/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     1464 2023-04-16 22:54:35.000000 airthings-exporter-0.0.3/README.md
+-rw-r--r--   0 max        (501) staff       (20)      564 2023-04-25 04:50:59.000000 airthings-exporter-0.0.3/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-04-25 04:51:33.376547 airthings-exporter-0.0.3/setup.cfg
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 04:51:33.374718 airthings-exporter-0.0.3/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 04:51:33.375447 airthings-exporter-0.0.3/src/airthings/
+-rw-r--r--   0 max        (501) staff       (20)     4027 2023-04-25 04:40:27.000000 airthings-exporter-0.0.3/src/airthings/CloudCollector.py
+-rw-r--r--   0 max        (501) staff       (20)        0 2022-11-27 23:11:13.000000 airthings-exporter-0.0.3/src/airthings/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)      666 2023-04-16 21:24:49.000000 airthings-exporter-0.0.3/src/airthings/main.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-25 04:51:33.376255 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     1774 2023-04-25 04:51:33.000000 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      382 2023-04-25 04:51:33.000000 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-04-25 04:51:33.000000 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       59 2023-04-25 04:51:33.000000 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)       43 2023-04-25 04:51:33.000000 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)       10 2023-04-25 04:51:33.000000 airthings-exporter-0.0.3/src/airthings_exporter.egg-info/top_level.txt
```

### Comparing `airthings-exporter-0.0.2/src/airthings/main.py` & `airthings-exporter-0.0.3/src/airthings/main.py`

 * *Files identical despite different names*

