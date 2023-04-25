# Comparing `tmp/api-Rocket-1.3.3.tar.gz` & `tmp/api-Rocket-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.3.3.tar", last modified: Tue Apr 25 06:26:11 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.3.4.tar", last modified: Tue Apr 25 06:30:18 2023, max compression
```

## Comparing `api-Rocket-1.3.3.tar` & `api-Rocket-1.3.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:26:11.642578 api-Rocket-1.3.3/
--rw-rw-rw-   0        0        0       20 2023-04-25 06:26:10.000000 api-Rocket-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-04-25 06:26:11.643554 api-Rocket-1.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 06:26:11.626953 api-Rocket-1.3.3/api_Rocket/
--rw-rw-rw-   0        0        0      671 2023-04-24 12:39:34.000000 api-Rocket-1.3.3/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:26:11.640625 api-Rocket-1.3.3/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      390 2023-04-25 06:26:11.000000 api-Rocket-1.3.3/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-25 06:26:11.000000 api-Rocket-1.3.3/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:26:11.000000 api-Rocket-1.3.3/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 06:26:11.000000 api-Rocket-1.3.3/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:26:11.645507 api-Rocket-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-04-25 06:26:10.000000 api-Rocket-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.766601 api-Rocket-1.3.4/
+-rw-rw-rw-   0        0        0       20 2023-04-25 06:30:17.000000 api-Rocket-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-04-25 06:30:18.767578 api-Rocket-1.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.726562 api-Rocket-1.3.4/api_Rocket/
+-rw-rw-rw-   0        0        0      671 2023-04-24 12:39:34.000000 api-Rocket-1.3.4/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.714843 api-Rocket-1.3.4/api_Rocket/lib/
+drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.740234 api-Rocket-1.3.4/api_Rocket/lib/clients/
+-rw-rw-rw-   0        0        0     5648 2023-04-21 14:19:08.000000 api-Rocket-1.3.4/api_Rocket/lib/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.738281 api-Rocket-1.3.4/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:30:18.770507 api-Rocket-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-04-25 06:30:17.000000 api-Rocket-1.3.4/setup.py
```

### Comparing `api-Rocket-1.3.3/api_Rocket/__init__.py` & `api-Rocket-1.3.4/api_Rocket/__init__.py`

 * *Files identical despite different names*

