# Comparing `tmp/audiconnectpy-1.3.0.tar.gz` & `tmp/audiconnectpy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.0.tar", last modified: Mon Apr 24 06:34:42 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.1.tar", last modified: Tue Apr 25 06:27:56 2023, max compression
```

## Comparing `audiconnectpy-1.3.0.tar` & `audiconnectpy-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:42.346585 audiconnectpy-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-24 06:34:42.346585 audiconnectpy-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:42.346585 audiconnectpy-1.3.0/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/audiconnectpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:42.346585 audiconnectpy-1.3.0/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-24 06:34:42.000000 audiconnectpy-1.3.0/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 06:34:42.000000 audiconnectpy-1.3.0/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:34:42.000000 audiconnectpy-1.3.0/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:34:42.000000 audiconnectpy-1.3.0/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 06:34:42.000000 audiconnectpy-1.3.0/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:34:42.346585 audiconnectpy-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-24 06:34:41.000000 audiconnectpy-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:34:42.346585 audiconnectpy-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 06:34:30.000000 audiconnectpy-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22748 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29813 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30342 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/audiconnectpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 06:27:56.000000 audiconnectpy-1.3.1/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-25 06:27:55.000000 audiconnectpy-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:27:56.660131 audiconnectpy-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-25 06:27:45.000000 audiconnectpy-1.3.1/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.0/LICENSE` & `audiconnectpy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/PKG-INFO` & `audiconnectpy-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.0/README.md` & `audiconnectpy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/audiconnectpy/api.py` & `audiconnectpy-1.3.1/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/audiconnectpy/auth.py` & `audiconnectpy-1.3.1/audiconnectpy/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -496,17 +496,22 @@
             username_post_url = url_parts.scheme + "://" + url_parts.netloc + action
         else:
             raise AudiException(f"Unknown form action: {action}")
         return username_post_url
 
     async def _async_get_azs_token(self, access_token: str) -> Any:
         """Get AZS Token."""
-        headers = await self.async_get_headers(
-            token_type="no", headers={"Content-Type": "application/json"}
-        )
+        headers = {
+            "Accept": "application/json",
+            "Accept-Charset": "utf-8",
+            "User-Agent": HDR_USER_AGENT,
+            "X-App-Name": "myAudi",
+            "X-App-Version": HDR_XAPP_VERSION,
+            "Content-Type": "application/json",
+        }
         asz_req_data = {
             "token": access_token,
             "grant_type": "id_token",
             "stage": "live",
             "config": "myaudi",
         }
         azs_token_rsptxt = await self.request(
@@ -522,18 +527,20 @@
         return azs_token_json
 
     async def _async_get_idk_token(self, **kwargs: Any) -> Any:
         """Get IDK Token."""
         refresh_token = kwargs.get("refresh_token")
         code = kwargs.get("code")
         code_verifier = kwargs.get("code_verifier")
-        headers = await self.async_get_headers(
-            token_type="no",
-            headers={"Content-Type": "application/x-www-form-urlencoded"},
-        )
+        headers = {
+            "Accept": "application/json",
+            "Accept-Charset": "utf-8",
+            "User-Agent": HDR_USER_AGENT,
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
         # IDK token request data
         if refresh_token:
             idk_data = {
                 "client_id": self._client_id,
                 "grant_type": "refresh_token",
                 "refresh_token": refresh_token,
                 "response_type": "token id_token",
@@ -562,17 +569,20 @@
         _LOGGER.debug("IDK Token: %s", idk_token_json)
 
         return idk_token_json
 
     async def _async_register_idk(self) -> Any:
         """Register IDK."""
         # mbboauth client register
-        headers = await self.async_get_headers(
-            token_type="no", headers={"Content-Type": "application/json"}
-        )
+        headers = {
+            "Accept": "application/json",
+            "Accept-Charset": "utf-8",
+            "User-Agent": HDR_USER_AGENT,
+            "Content-Type": "application/json",
+        }
         mbboauth_reg_data = {
             "client_name": "SM-A405FN",
             "platform": "google",
             "client_brand": "Audi",
             "appName": "myAudi",
             "appVersion": HDR_XAPP_VERSION,
             "appId": "de.myaudi.mobile.assistant",
@@ -586,18 +596,23 @@
         mbboauth_client_reg_json = jload(mbboauth_client_reg_rsptxt)
         return mbboauth_client_reg_json.get("client_id")
 
     async def _async_get_mbb_token(self, **kwargs: Any) -> Any:
         """Authentification to IDK."""
         refresh_token = kwargs.get("refresh_token")
         id_token = kwargs.get("id_token")
-        headers = await self.async_get_headers(
-            token_type="no",
-            headers={"Content-Type": "application/x-www-form-urlencoded"},
-        )
+        headers = {
+            "Accept": "application/json",
+            "Accept-Charset": "utf-8",
+            "User-Agent": HDR_USER_AGENT,
+            "X-App-Name": "myAudi",
+            "X-App-Version": HDR_XAPP_VERSION,
+            "X-Client-ID": self._x_client_id,
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
         if refresh_token:
             mbboauth_data = {
                 "grant_type": "refresh_token",
                 "token": refresh_token,
                 "scope": "sc2:fal",
                 # "vin": vin,  << App uses a dedicated VIN here, but it works without, don't know
             }
```

### Comparing `audiconnectpy-1.3.0/audiconnectpy/models.py` & `audiconnectpy-1.3.1/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/audiconnectpy/services.py` & `audiconnectpy-1.3.1/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/audiconnectpy/util.py` & `audiconnectpy-1.3.1/audiconnectpy/util.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.1/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.0/pyproject.toml` & `audiconnectpy-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.0/setup.py` & `audiconnectpy-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.0",
+    version="1.3.1",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

