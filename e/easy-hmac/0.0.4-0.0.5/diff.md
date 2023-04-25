# Comparing `tmp/easy-hmac-0.0.4.tar.gz` & `tmp/easy-hmac-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-hmac-0.0.4.tar", last modified: Tue Apr 25 01:13:38 2023, max compression
+gzip compressed data, was "easy-hmac-0.0.5.tar", last modified: Tue Apr 25 01:24:05 2023, max compression
```

## Comparing `easy-hmac-0.0.4.tar` & `easy-hmac-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:13:38.982029 easy-hmac-0.0.4/
--rw-r--r--   0 garrethcain   (501) staff       (20)     1264 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/LICENSE
--rw-r--r--   0 garrethcain   (501) staff       (20)       25 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/MANIFEST.in
--rw-r--r--   0 garrethcain   (501) staff       (20)      725 2023-04-25 01:13:38.982128 easy-hmac-0.0.4/PKG-INFO
--rw-r--r--   0 garrethcain   (501) staff       (20)      104 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/pyproject.toml
--rw-r--r--   0 garrethcain   (501) staff       (20)      841 2023-04-25 01:13:38.982451 easy-hmac-0.0.4/setup.cfg
--rw-r--r--   0 garrethcain   (501) staff       (20)       37 2023-04-25 00:03:31.000000 easy-hmac-0.0.4/setup.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:13:38.978946 easy-hmac-0.0.4/src/
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:13:38.980538 easy-hmac-0.0.4/src/easy_hmac/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/src/easy_hmac/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     3605 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/src/easy_hmac/core.py
--rw-r--r--   0 garrethcain   (501) staff       (20)      101 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/src/easy_hmac/exceptions.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:13:38.981510 easy-hmac-0.0.4/src/easy_hmac/utils/
--rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/src/easy_hmac/utils/__init__.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     2790 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/src/easy_hmac/utils/http.py
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:13:38.981284 easy-hmac-0.0.4/src/easy_hmac.egg-info/
--rw-r--r--   0 garrethcain   (501) staff       (20)      725 2023-04-25 01:13:38.000000 easy-hmac-0.0.4/src/easy_hmac.egg-info/PKG-INFO
--rw-r--r--   0 garrethcain   (501) staff       (20)      384 2023-04-25 01:13:38.000000 easy-hmac-0.0.4/src/easy_hmac.egg-info/SOURCES.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)        1 2023-04-25 01:13:38.000000 easy-hmac-0.0.4/src/easy_hmac.egg-info/dependency_links.txt
--rw-r--r--   0 garrethcain   (501) staff       (20)       10 2023-04-25 01:13:38.000000 easy-hmac-0.0.4/src/easy_hmac.egg-info/top_level.txt
-drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:13:38.981849 easy-hmac-0.0.4/test/
--rw-r--r--   0 garrethcain   (501) staff       (20)     8371 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/test/test_easy_hmac.py
--rw-r--r--   0 garrethcain   (501) staff       (20)     1650 2023-04-24 23:50:44.000000 easy-hmac-0.0.4/test/test_utils_http.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:24:05.717118 easy-hmac-0.0.5/
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1264 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/LICENSE
+-rw-r--r--   0 garrethcain   (501) staff       (20)       25 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/MANIFEST.in
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1844 2023-04-25 01:24:05.717203 easy-hmac-0.0.5/PKG-INFO
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1118 2023-04-24 23:53:57.000000 easy-hmac-0.0.5/README.md
+-rw-r--r--   0 garrethcain   (501) staff       (20)      104 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/pyproject.toml
+-rw-r--r--   0 garrethcain   (501) staff       (20)      841 2023-04-25 01:24:05.717517 easy-hmac-0.0.5/setup.cfg
+-rw-r--r--   0 garrethcain   (501) staff       (20)       37 2023-04-25 00:03:31.000000 easy-hmac-0.0.5/setup.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:24:05.713876 easy-hmac-0.0.5/src/
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:24:05.715530 easy-hmac-0.0.5/src/easy_hmac/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/src/easy_hmac/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     3605 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/src/easy_hmac/core.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)      101 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/src/easy_hmac/exceptions.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:24:05.716500 easy-hmac-0.0.5/src/easy_hmac/utils/
+-rw-r--r--   0 garrethcain   (501) staff       (20)        0 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/src/easy_hmac/utils/__init__.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     2790 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/src/easy_hmac/utils/http.py
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:24:05.716268 easy-hmac-0.0.5/src/easy_hmac.egg-info/
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1844 2023-04-25 01:24:05.000000 easy-hmac-0.0.5/src/easy_hmac.egg-info/PKG-INFO
+-rw-r--r--   0 garrethcain   (501) staff       (20)      394 2023-04-25 01:24:05.000000 easy-hmac-0.0.5/src/easy_hmac.egg-info/SOURCES.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)        1 2023-04-25 01:24:05.000000 easy-hmac-0.0.5/src/easy_hmac.egg-info/dependency_links.txt
+-rw-r--r--   0 garrethcain   (501) staff       (20)       10 2023-04-25 01:24:05.000000 easy-hmac-0.0.5/src/easy_hmac.egg-info/top_level.txt
+drwxr-xr-x   0 garrethcain   (501) staff       (20)        0 2023-04-25 01:24:05.716938 easy-hmac-0.0.5/test/
+-rw-r--r--   0 garrethcain   (501) staff       (20)     8371 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/test/test_easy_hmac.py
+-rw-r--r--   0 garrethcain   (501) staff       (20)     1650 2023-04-24 23:50:44.000000 easy-hmac-0.0.5/test/test_utils_http.py
```

### Comparing `easy-hmac-0.0.4/LICENSE` & `easy-hmac-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-hmac-0.0.4/setup.cfg` & `easy-hmac-0.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easy-hmac
-version = 0.0.4
+version = 0.0.5
 description = A python package that creates and verifies HMAC signatures
 long_description = file: README.md
 long_description_content_type = text/markdown
 readme = "README.md"
 url = https://github.com/garrethcain/easy-hmac/
 author = Garreth Cain
 author_email = garrethccain@gmail.com
```

### Comparing `easy-hmac-0.0.4/src/easy_hmac/core.py` & `easy-hmac-0.0.5/src/easy_hmac/core.py`

 * *Files identical despite different names*

### Comparing `easy-hmac-0.0.4/src/easy_hmac/utils/http.py` & `easy-hmac-0.0.5/src/easy_hmac/utils/http.py`

 * *Files identical despite different names*

### Comparing `easy-hmac-0.0.4/test/test_easy_hmac.py` & `easy-hmac-0.0.5/test/test_easy_hmac.py`

 * *Files identical despite different names*

### Comparing `easy-hmac-0.0.4/test/test_utils_http.py` & `easy-hmac-0.0.5/test/test_utils_http.py`

 * *Files identical despite different names*

