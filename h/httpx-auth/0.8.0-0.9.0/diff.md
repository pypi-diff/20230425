# Comparing `tmp/httpx_auth-0.8.0.tar.gz` & `tmp/httpx_auth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/httpx_auth-0.8.0.tar", last modified: Sun Nov 15 14:36:54 2020, max compression
+gzip compressed data, was "dist/httpx_auth-0.9.0.tar", last modified: Mon Mar  1 01:49:44 2021, max compression
```

## Comparing `httpx_auth-0.8.0.tar` & `httpx_auth-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    56839 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    49191 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth/
--rw-rw-r--   0 travis    (2000) travis    (2000)      789 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61148 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/authentication.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9960 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/aws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6418 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8789 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/oauth2_authentication_responses_server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7614 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/oauth2_tokens.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4972 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/testing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/httpx_auth/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    56839 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      403 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/httpx_auth.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-11-15 14:36:54.000000 httpx_auth-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2181 2020-11-15 14:36:28.000000 httpx_auth-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56839 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49191 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      789 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61148 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/authentication.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9960 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/aws.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6418 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8789 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/oauth2_authentication_responses_server.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7614 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/oauth2_tokens.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4972 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/testing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      371 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/httpx_auth/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56839 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      403 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/httpx_auth.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-01 01:49:44.000000 httpx_auth-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2181 2021-03-01 01:49:17.000000 httpx_auth-0.9.0/setup.py
```

### Comparing `httpx_auth-0.8.0/PKG-INFO` & `httpx_auth-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx_auth
-Version: 0.8.0
+Version: 0.9.0
 Summary: Authentication for HTTPX
 Home-page: https://colin-b.github.io/httpx_auth/
 Author: Colin Bounouar
 Author-email: colin.bounouar.dev@gmail.com
 Maintainer: Colin Bounouar
 Maintainer-email: colin.bounouar.dev@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpx_auth Version: 0.8.0 Summary: Authentication
+Metadata-Version: 2.1 Name: httpx_auth Version: 0.9.0 Summary: Authentication
 for HTTPX Home-page: https://colin-b.github.io/httpx_auth/ Author: Colin
 Bounouar Author-email: colin.bounouar.dev@gmail.com Maintainer: Colin Bounouar
 Maintainer-email: colin.bounouar.dev@gmail.com License: MIT Download-URL:
 https://pypi.org/project/httpx-auth/ Project-URL: GitHub, https://github.com/
 Colin-b/httpx_auth Project-URL: Changelog, https://github.com/Colin-b/
 httpx_auth/blob/master/CHANGELOG.md Project-URL: Issues, https://github.com/
 Colin-b/httpx_auth/issues Description:
```

### Comparing `httpx_auth-0.8.0/README.md` & `httpx_auth-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/__init__.py` & `httpx_auth-0.9.0/httpx_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/authentication.py` & `httpx_auth-0.9.0/httpx_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/aws.py` & `httpx_auth-0.9.0/httpx_auth/aws.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/errors.py` & `httpx_auth-0.9.0/httpx_auth/errors.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/oauth2_authentication_responses_server.py` & `httpx_auth-0.9.0/httpx_auth/oauth2_authentication_responses_server.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/oauth2_tokens.py` & `httpx_auth-0.9.0/httpx_auth/oauth2_tokens.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth/testing.py` & `httpx_auth-0.9.0/httpx_auth/testing.py`

 * *Files identical despite different names*

### Comparing `httpx_auth-0.8.0/httpx_auth.egg-info/PKG-INFO` & `httpx_auth-0.9.0/httpx_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-auth
-Version: 0.8.0
+Version: 0.9.0
 Summary: Authentication for HTTPX
 Home-page: https://colin-b.github.io/httpx_auth/
 Author: Colin Bounouar
 Author-email: colin.bounouar.dev@gmail.com
 Maintainer: Colin Bounouar
 Maintainer-email: colin.bounouar.dev@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpx-auth Version: 0.8.0 Summary: Authentication
+Metadata-Version: 2.1 Name: httpx-auth Version: 0.9.0 Summary: Authentication
 for HTTPX Home-page: https://colin-b.github.io/httpx_auth/ Author: Colin
 Bounouar Author-email: colin.bounouar.dev@gmail.com Maintainer: Colin Bounouar
 Maintainer-email: colin.bounouar.dev@gmail.com License: MIT Download-URL:
 https://pypi.org/project/httpx-auth/ Project-URL: GitHub, https://github.com/
 Colin-b/httpx_auth Project-URL: Changelog, https://github.com/Colin-b/
 httpx_auth/blob/master/CHANGELOG.md Project-URL: Issues, https://github.com/
 Colin-b/httpx_auth/issues Description:
```

### Comparing `httpx_auth-0.8.0/setup.py` & `httpx_auth-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Build Tools",
     ],
     keywords=["authentication", "oauth2", "aws", "okta", "aad"],
     packages=find_packages(exclude=["tests*"]),
     install_requires=[
         # Used for Base Authentication and to communicate with OAuth2 servers
-        "httpx==0.16.*"
+        "httpx==0.17.*"
     ],
     extras_require={
         "testing": [
             # Used to generate test tokens
             "pyjwt==1.*",
             # Used to mock httpx
-            "pytest_httpx==0.10.*",
+            "pytest_httpx==0.11.*",
             # Used to check coverage
             "pytest-cov==2.*",
         ]
     },
     python_requires=">=3.6",
     project_urls={
         "GitHub": "https://github.com/Colin-b/httpx_auth",
```

