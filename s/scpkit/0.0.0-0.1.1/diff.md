# Comparing `tmp/scpkit-0.0.0.tar.gz` & `tmp/scpkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.0.0.tar", last modified: Mon Dec 12 14:24:16 2022, max compression
+gzip compressed data, was "scpkit-0.1.1.tar", last modified: Tue Apr 25 00:52:00 2023, max compression
```

## Comparing `scpkit-0.0.0.tar` & `scpkit-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,26 @@
-drwxr-xr-x   0 dgwhited   (501) staff       (20)        0 2022-12-12 14:24:16.828650 scpkit-0.0.0/
--rw-r--r--   0 dgwhited   (501) staff       (20)      259 2022-12-12 14:24:16.828538 scpkit-0.0.0/PKG-INFO
--rw-r--r--   0 dgwhited   (501) staff       (20)       58 2022-12-12 14:24:16.000000 scpkit-0.0.0/README.md
-drwxr-xr-x   0 dgwhited   (501) staff       (20)        0 2022-12-12 14:24:16.828387 scpkit-0.0.0/scpkit.egg-info/
--rw-r--r--   0 dgwhited   (501) staff       (20)      259 2022-12-12 14:24:16.000000 scpkit-0.0.0/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 dgwhited   (501) staff       (20)      154 2022-12-12 14:24:16.000000 scpkit-0.0.0/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 dgwhited   (501) staff       (20)        1 2022-12-12 14:24:16.000000 scpkit-0.0.0/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 dgwhited   (501) staff       (20)        1 2022-12-12 14:24:16.000000 scpkit-0.0.0/scpkit.egg-info/top_level.txt
--rw-r--r--   0 dgwhited   (501) staff       (20)        1 2022-12-12 14:24:16.000000 scpkit-0.0.0/scpkit.egg-info/zip-safe
--rw-r--r--   0 dgwhited   (501) staff       (20)       38 2022-12-12 14:24:16.828690 scpkit-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 00:51:51.000000 scpkit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-25 00:52:00.847450 scpkit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-25 00:51:51.000000 scpkit-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 00:51:51.000000 scpkit-0.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.843450 scpkit-0.1.1/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-25 00:51:51.000000 scpkit-0.1.1/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 00:52:00.000000 scpkit-0.1.1/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 00:52:00.847450 scpkit-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:51:51.000000 scpkit-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:52:00.847450 scpkit-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-25 00:51:51.000000 scpkit-0.1.1/tests/test.py
```

