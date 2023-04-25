# Comparing `tmp/hsso-0.5.tar.gz` & `tmp/hsso-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsso-0.5.tar", last modified: Tue Apr 25 08:01:49 2023, max compression
+gzip compressed data, was "hsso-0.6.tar", last modified: Tue Apr 25 08:43:42 2023, max compression
```

## Comparing `hsso-0.5.tar` & `hsso-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-25 08:01:49.619266 hsso-0.5/
--rw-rw----   0 root         (0) everybody  (9997)      324 2023-04-25 08:01:49.619266 hsso-0.5/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-25 08:01:49.619266 hsso-0.5/hsso.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      324 2023-04-25 08:01:49.000000 hsso-0.5/hsso.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      193 2023-04-25 08:01:49.000000 hsso-0.5/hsso.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-25 08:01:49.000000 hsso-0.5/hsso.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-25 08:01:49.000000 hsso-0.5/hsso.egg-info/not-zip-safe
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-04-25 08:01:49.000000 hsso-0.5/hsso.egg-info/top_level.txt
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-25 08:01:49.619266 hsso-0.5/hssoIN/
--rw-rw----   0 root         (0) everybody  (9997)       29 2023-04-25 07:50:54.000000 hsso-0.5/hssoIN/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      728 2023-04-25 07:55:29.000000 hsso-0.5/hssoIN/hs_tik.py
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-25 08:01:49.623266 hsso-0.5/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      379 2023-04-25 07:58:37.000000 hsso-0.5/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-25 08:43:42.105443 hsso-0.6/
+-rw-rw----   0 root         (0) everybody  (9997)      324 2023-04-25 08:43:42.105443 hsso-0.6/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-25 08:43:42.101443 hsso-0.6/hsso.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      324 2023-04-25 08:43:41.000000 hsso-0.6/hsso.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      193 2023-04-25 08:43:41.000000 hsso-0.6/hsso.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-25 08:43:41.000000 hsso-0.6/hsso.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-25 08:43:41.000000 hsso-0.6/hsso.egg-info/not-zip-safe
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-04-25 08:43:41.000000 hsso-0.6/hsso.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-25 08:43:42.105443 hsso-0.6/hssoIN/
+-rw-rw----   0 root         (0) everybody  (9997)       25 2023-04-25 08:37:14.000000 hsso-0.6/hssoIN/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      716 2023-04-25 08:36:53.000000 hsso-0.6/hssoIN/hs_tik.py
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-25 08:43:42.105443 hsso-0.6/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      379 2023-04-25 08:37:53.000000 hsso-0.6/setup.py
```

### Comparing `hsso-0.5/hssoIN/hs_tik.py` & `hsso-0.6/hssoIN/hs_tik.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
-def hsInfoTik(username):
-    res = requests.get(f'https://api.dlyar-dev.tk/info-tiktok.json?user={username}').json()
+def hsTik(user):
+    res = requests.get(f'https://api.dlyar-dev.tk/info-tiktok.json?user={user}').json()
     if resp4['status'] == True:
         idd = resp4['id']
         namee = resp4['name']
         countryy = resp4['country']
         code-countryy = resp4['code-country']
         flagg = resp4['flag']
         followw = resp4['followers']
```

