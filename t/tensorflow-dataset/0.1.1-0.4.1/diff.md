# Comparing `tmp/tensorflow_dataset-0.1.1.tar.gz` & `tmp/tensorflow_dataset-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow_dataset-0.1.1.tar", last modified: Mon Mar 27 07:25:08 2023, max compression
+gzip compressed data, was "tensorflow_dataset-0.4.1.tar", last modified: Tue Apr 25 05:32:11 2023, max compression
```

## Comparing `tensorflow_dataset-0.1.1.tar` & `tensorflow_dataset-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 07:25:08.694619 tensorflow_dataset-0.1.1/
--rw-rw-rw-   0        0        0      201 2023-03-27 07:25:08.694619 tensorflow_dataset-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-03-27 07:25:08.694619 tensorflow_dataset-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      313 2023-03-27 07:24:58.000000 tensorflow_dataset-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:25:08.694619 tensorflow_dataset-0.1.1/tensorflow_dataset/
--rw-rw-rw-   0        0        0      274 2023-03-27 07:10:22.000000 tensorflow_dataset-0.1.1/tensorflow_dataset/tensorflow_dataset.py
-drwxrwxrwx   0        0        0        0 2023-03-27 07:25:08.694619 tensorflow_dataset-0.1.1/tensorflow_dataset.egg-info/
--rw-rw-rw-   0        0        0      201 2023-03-27 07:25:08.000000 tensorflow_dataset-0.1.1/tensorflow_dataset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-03-27 07:25:08.000000 tensorflow_dataset-0.1.1/tensorflow_dataset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 07:25:08.000000 tensorflow_dataset-0.1.1/tensorflow_dataset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-27 07:25:08.000000 tensorflow_dataset-0.1.1/tensorflow_dataset.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-27 07:25:08.000000 tensorflow_dataset-0.1.1/tensorflow_dataset.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 05:32:11.592982 tensorflow_dataset-0.4.1/
+-rw-rw-rw-   0        0        0      121 2023-04-25 05:32:11.584993 tensorflow_dataset-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-25 05:32:11.592982 tensorflow_dataset-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      287 2023-04-25 05:31:55.000000 tensorflow_dataset-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:32:11.577000 tensorflow_dataset-0.4.1/tensorflow_dataset/
+-rw-rw-rw-   0        0        0     3392 2023-04-25 05:31:41.000000 tensorflow_dataset-0.4.1/tensorflow_dataset/tensorflow_dataset.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:32:11.584993 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/
+-rw-rw-rw-   0        0        0      121 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-25 05:32:11.000000 tensorflow_dataset-0.4.1/tensorflow_dataset.egg-info/top_level.txt
```

