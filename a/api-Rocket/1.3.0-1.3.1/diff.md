# Comparing `tmp/api-Rocket-1.3.0.tar.gz` & `tmp/api-Rocket-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.3.0.tar", last modified: Mon Apr 24 09:35:22 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.3.1.tar", last modified: Mon Apr 24 12:47:15 2023, max compression
```

## Comparing `api-Rocket-1.3.0.tar` & `api-Rocket-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:35:22.757101 api-Rocket-1.3.0/
--rw-rw-rw-   0        0        0       20 2023-04-24 09:35:21.000000 api-Rocket-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      526 2023-04-24 09:35:22.759054 api-Rocket-1.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 09:35:22.741476 api-Rocket-1.3.0/api_Rocket/
--rw-rw-rw-   0        0        0      671 2023-03-24 14:25:46.000000 api-Rocket-1.3.0/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:35:22.755148 api-Rocket-1.3.0/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 09:35:22.000000 api-Rocket-1.3.0/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 09:35:22.763937 api-Rocket-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-04-24 09:35:21.000000 api-Rocket-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:47:15.372336 api-Rocket-1.3.1/
+-rw-rw-rw-   0        0        0       20 2023-04-24 12:47:14.000000 api-Rocket-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-04-24 12:47:15.373312 api-Rocket-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 12:47:15.359640 api-Rocket-1.3.1/api_Rocket/
+-rw-rw-rw-   0        0        0      671 2023-04-24 12:39:34.000000 api-Rocket-1.3.1/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:47:15.370382 api-Rocket-1.3.1/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 12:47:15.000000 api-Rocket-1.3.1/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:47:15.375265 api-Rocket-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-04-24 12:47:14.000000 api-Rocket-1.3.1/setup.py
```

### Comparing `api-Rocket-1.3.0/api_Rocket/__init__.py` & `api-Rocket-1.3.1/api_Rocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 __author__ = "Redpiar"
 
 __license__ = "MIT"
 
 __copyright__ = "Copyright 2023 Redpiar"
 
-__version__ = '1.1.0'
+__version__ = '1.3.0'
 
 __status__ = "(Beta)"
 
 __newest__ = json.loads(requests.get("https://pypi.org/pypi/api-Rocket/json").text)["info"]["version"]
 
 if __version__ != __newest__:
 	print(f"""
```

