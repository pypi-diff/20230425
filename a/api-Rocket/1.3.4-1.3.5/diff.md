# Comparing `tmp/api-Rocket-1.3.4.tar.gz` & `tmp/api-Rocket-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.3.4.tar", last modified: Tue Apr 25 06:30:18 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.3.5.tar", last modified: Tue Apr 25 06:38:25 2023, max compression
```

## Comparing `api-Rocket-1.3.4.tar` & `api-Rocket-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.766601 api-Rocket-1.3.4/
--rw-rw-rw-   0        0        0       20 2023-04-25 06:30:17.000000 api-Rocket-1.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-04-25 06:30:18.767578 api-Rocket-1.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.726562 api-Rocket-1.3.4/api_Rocket/
--rw-rw-rw-   0        0        0      671 2023-04-24 12:39:34.000000 api-Rocket-1.3.4/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.714843 api-Rocket-1.3.4/api_Rocket/lib/
-drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.740234 api-Rocket-1.3.4/api_Rocket/lib/clients/
--rw-rw-rw-   0        0        0     5648 2023-04-21 14:19:08.000000 api-Rocket-1.3.4/api_Rocket/lib/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 06:30:18.738281 api-Rocket-1.3.4/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      390 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 06:30:18.000000 api-Rocket-1.3.4/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 06:30:18.770507 api-Rocket-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-04-25 06:30:17.000000 api-Rocket-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:38:25.120117 api-Rocket-1.3.5/
+-rw-rw-rw-   0        0        0       20 2023-04-25 06:38:23.000000 api-Rocket-1.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      526 2023-04-25 06:38:25.121093 api-Rocket-1.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 06:38:25.096679 api-Rocket-1.3.5/api_Rocket/
+-rw-rw-rw-   0        0        0      671 2023-04-25 06:34:35.000000 api-Rocket-1.3.5/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:38:25.083984 api-Rocket-1.3.5/api_Rocket/lib/
+drwxrwxrwx   0        0        0        0 2023-04-25 06:38:25.115234 api-Rocket-1.3.5/api_Rocket/lib/clients/
+-rw-rw-rw-   0        0        0      418 2023-03-20 11:34:29.000000 api-Rocket-1.3.5/api_Rocket/lib/clients/async_client.py
+-rw-rw-rw-   0        0        0     5648 2023-04-21 14:19:08.000000 api-Rocket-1.3.5/api_Rocket/lib/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:38:25.118164 api-Rocket-1.3.5/api_Rocket/lib/clients/exception/
+-rw-rw-rw-   0        0        0     1718 2023-03-24 14:12:55.000000 api-Rocket-1.3.5/api_Rocket/lib/clients/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:38:25.108398 api-Rocket-1.3.5/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-25 06:38:24.000000 api-Rocket-1.3.5/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-25 06:38:24.000000 api-Rocket-1.3.5/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:38:24.000000 api-Rocket-1.3.5/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 06:38:24.000000 api-Rocket-1.3.5/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:38:25.124023 api-Rocket-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-04-25 06:38:23.000000 api-Rocket-1.3.5/setup.py
```

### Comparing `api-Rocket-1.3.4/api_Rocket/__init__.py` & `api-Rocket-1.3.5/api_Rocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 __author__ = "Redpiar"
 
 __license__ = "MIT"
 
 __copyright__ = "Copyright 2023 Redpiar"
 
-__version__ = '1.3.0'
+__version__ = '1.3.5'
 
 __status__ = "(Beta)"
 
 __newest__ = json.loads(requests.get("https://pypi.org/pypi/api-Rocket/json").text)["info"]["version"]
 
 if __version__ != __newest__:
 	print(f"""
```

### Comparing `api-Rocket-1.3.4/api_Rocket/lib/clients/client.py` & `api-Rocket-1.3.5/api_Rocket/lib/clients/client.py`

 * *Files identical despite different names*

