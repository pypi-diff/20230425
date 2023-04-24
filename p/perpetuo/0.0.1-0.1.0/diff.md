# Comparing `tmp/perpetuo-0.0.1.tar.gz` & `tmp/perpetuo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "perpetuo-0.1.0.tar", last modified: Mon Apr 24 21:49:25 2023, max compression
```

## Comparing `perpetuo-0.0.1.tar` & `perpetuo-0.1.0.tar`

### file list

```diff
@@ -1,3 +1,30 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 perpetuo-0.0.1/perpetuo.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 perpetuo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 perpetuo-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    49965 2023-04-24 21:49:14.000000 perpetuo-0.1.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 21:49:14.000000 perpetuo-0.1.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:49:14.000000 perpetuo-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 21:49:14.000000 perpetuo-0.1.0/LICENSE.APACHE2
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-24 21:49:14.000000 perpetuo-0.1.0/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 21:49:14.000000 perpetuo-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-24 21:49:25.053749 perpetuo-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-24 21:49:14.000000 perpetuo-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 21:49:14.000000 perpetuo-0.1.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 21:49:14.000000 perpetuo-0.1.0/prep-manylinux-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-24 21:49:14.000000 perpetuo-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.049749 perpetuo-0.1.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/python/perpetuo/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/_perpetuo.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:14.000000 perpetuo-0.1.0/python/perpetuo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/python/perpetuo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:49:24.000000 perpetuo-0.1.0/python/perpetuo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 21:49:25.000000 perpetuo-0.1.0/python/perpetuo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:49:25.053749 perpetuo-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 21:49:14.000000 perpetuo-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:49:25.053749 perpetuo-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 21:49:14.000000 perpetuo-0.1.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-24 21:49:14.000000 perpetuo-0.1.0/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-24 21:49:14.000000 perpetuo-0.1.0/src/shmem.rs
```

