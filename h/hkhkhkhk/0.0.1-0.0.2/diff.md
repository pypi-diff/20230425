# Comparing `tmp/hkhkhkhk-0.0.1.tar.gz` & `tmp/hkhkhkhk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkhkhkhk-0.0.1.tar", last modified: Fri Mar 17 08:53:18 2023, max compression
+gzip compressed data, was "hkhkhkhk-0.0.2.tar", last modified: Tue Apr 25 07:27:32 2023, max compression
```

## Comparing `hkhkhkhk-0.0.1.tar` & `hkhkhkhk-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 08:53:18.761392 hkhkhkhk-0.0.1/
--rw-rw-rw-   0        0        0      246 2023-03-17 08:53:18.759394 hkhkhkhk-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-17 08:53:18.718392 hkhkhkhk-0.0.1/hkhkhkhk/
--rw-rw-rw-   0        0        0        0 2023-03-17 08:41:58.000000 hkhkhkhk-0.0.1/hkhkhkhk/__init__.py
--rw-rw-rw-   0        0        0      552 2023-03-17 08:41:08.000000 hkhkhkhk-0.0.1/hkhkhkhk/cFunction.py
-drwxrwxrwx   0        0        0        0 2023-03-17 08:53:18.755394 hkhkhkhk-0.0.1/hkhkhkhk.egg-info/
--rw-rw-rw-   0        0        0      246 2023-03-17 08:53:17.000000 hkhkhkhk-0.0.1/hkhkhkhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-03-17 08:53:18.000000 hkhkhkhk-0.0.1/hkhkhkhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 08:53:17.000000 hkhkhkhk-0.0.1/hkhkhkhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-17 08:53:17.000000 hkhkhkhk-0.0.1/hkhkhkhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-17 08:53:17.000000 hkhkhkhk-0.0.1/hkhkhkhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 08:53:18.761392 hkhkhkhk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      977 2023-03-17 08:52:55.000000 hkhkhkhk-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:27:32.927553 hkhkhkhk-0.0.2/
+-rw-rw-rw-   0        0        0      246 2023-04-25 07:27:32.926553 hkhkhkhk-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 07:27:32.879599 hkhkhkhk-0.0.2/hkhkhkhk/
+-rw-rw-rw-   0        0        0        0 2023-03-17 08:41:58.000000 hkhkhkhk-0.0.2/hkhkhkhk/__init__.py
+-rw-rw-rw-   0        0        0      564 2023-04-25 07:26:29.000000 hkhkhkhk-0.0.2/hkhkhkhk/cFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:27:32.923555 hkhkhkhk-0.0.2/hkhkhkhk.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-04-25 07:27:32.000000 hkhkhkhk-0.0.2/hkhkhkhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-25 07:27:32.000000 hkhkhkhk-0.0.2/hkhkhkhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:27:32.000000 hkhkhkhk-0.0.2/hkhkhkhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 07:27:32.000000 hkhkhkhk-0.0.2/hkhkhkhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 07:27:32.000000 hkhkhkhk-0.0.2/hkhkhkhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:27:32.928552 hkhkhkhk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-04-25 07:27:22.000000 hkhkhkhk-0.0.2/setup.py
```

