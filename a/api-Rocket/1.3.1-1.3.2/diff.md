# Comparing `tmp/api-Rocket-1.3.1.tar.gz` & `tmp/api-Rocket-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.3.1.tar", last modified: Mon Apr 24 12:47:15 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.3.2.tar", last modified: Tue Apr 25 06:21:23 2023, max compression
```

## Comparing `api-Rocket-1.3.1.tar` & `api-Rocket-1.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:47:15.372336 api-Rocket-1.3.1/
--rw-rw-rw-   0        0        0       20 2023-04-24 12:47:14.000000 api-Rocket-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-04-24 12:47:15.373312 api-Rocket-1.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 12:47:15.359640 api-Rocket-1.3.1/api_Rocket/
--rw-rw-rw-   0        0        0      671 2023-04-24 12:39:34.000000 api-Rocket-1.3.1/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:47:15.370382 api-Rocket-1.3.1/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      390 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 12:47:15.375265 api-Rocket-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-04-24 12:47:14.000000 api-Rocket-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:21:23.145507 api-Rocket-1.3.2/
+-rw-rw-rw-   0        0        0       20 2023-04-25 06:21:18.000000 api-Rocket-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-04-25 06:21:23.146484 api-Rocket-1.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 06:21:23.127929 api-Rocket-1.3.2/api_Rocket/
+-rw-rw-rw-   0        0        0      671 2023-04-24 12:39:34.000000 api-Rocket-1.3.2/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:21:23.141601 api-Rocket-1.3.2/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-04-25 06:21:21.000000 api-Rocket-1.3.2/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-25 06:21:21.000000 api-Rocket-1.3.2/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:21:21.000000 api-Rocket-1.3.2/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 06:21:21.000000 api-Rocket-1.3.2/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:21:23.148437 api-Rocket-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-04-25 06:21:18.000000 api-Rocket-1.3.2/setup.py
```

### Comparing `api-Rocket-1.3.1/api_Rocket/__init__.py` & `api-Rocket-1.3.2/api_Rocket/__init__.py`

 * *Files identical despite different names*

