# Comparing `tmp/bkapi_plugins_py-0.1.tar.gz` & `tmp/bkapi_plugins_py-0.425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi_plugins_py-0.1.tar", last modified: Tue Apr 11 06:00:08 2023, max compression
+gzip compressed data, was "bkapi_plugins_py-0.425.tar", last modified: Tue Apr 25 03:08:16 2023, max compression
```

## Comparing `bkapi_plugins_py-0.1.tar` & `bkapi_plugins_py-0.425.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 06:00:08.120666 bkapi_plugins_py-0.1/
--rw-rw-rw-   0        0        0       43 2023-04-11 05:29:47.000000 bkapi_plugins_py-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      177 2023-04-11 06:00:08.121661 bkapi_plugins_py-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 06:00:08.098560 bkapi_plugins_py-0.1/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:00:08.107541 bkapi_plugins_py-0.1/bkapi_plugins/files/
--rw-rw-rw-   0        0        0   133894 2023-04-11 02:05:58.000000 bkapi_plugins_py-0.1/bkapi_plugins/files/data.zip
-drwxrwxrwx   0        0        0        0 2023-04-11 06:00:08.118673 bkapi_plugins_py-0.1/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      177 2023-04-11 06:00:08.000000 bkapi_plugins_py-0.1/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-04-11 06:00:08.000000 bkapi_plugins_py-0.1/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:00:08.000000 bkapi_plugins_py-0.1/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:00:08.000000 bkapi_plugins_py-0.1/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 06:00:08.124654 bkapi_plugins_py-0.1/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-04-11 06:00:06.000000 bkapi_plugins_py-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.171012 bkapi_plugins_py-0.425/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi_plugins_py-0.425/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-04-25 03:08:16.171012 bkapi_plugins_py-0.425/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.140111 bkapi_plugins_py-0.425/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.158052 bkapi_plugins_py-0.425/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0  3640951 2023-03-24 05:13:43.000000 bkapi_plugins_py-0.425/bkapi_plugins/files/generator1.0.tar.gz
+-rw-rw-rw-   0        0        0   579136 2023-04-25 03:01:45.000000 bkapi_plugins_py-0.425/bkapi_plugins/files/ph-live-nginx-master.zip
+drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.169014 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 03:08:16.175000 bkapi_plugins_py-0.425/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-04-25 03:08:13.000000 bkapi_plugins_py-0.425/setup.py
```

