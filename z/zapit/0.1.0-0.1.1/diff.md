# Comparing `tmp/zapit-0.1.0.tar.gz` & `tmp/zapit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zapit-0.1.0.tar", max compression
+gzip compressed data, was "zapit-0.1.1.tar", max compression
```

## Comparing `zapit-0.1.0.tar` & `zapit-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      720 2023-04-25 01:53:33.711296 zapit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      373 2023-04-25 03:16:52.120685 zapit-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-21 10:44:03.019693 zapit-0.1.0/zapit/__init__.py
--rw-r--r--   0        0        0      248 2023-04-25 02:02:10.126299 zapit-0.1.0/zapit/exceptions.py
--rw-r--r--   0        0        0     1834 2023-04-25 05:09:56.559735 zapit-0.1.0/zapit/models/network.py
--rw-r--r--   0        0        0     1226 2023-04-24 08:52:14.840087 zapit-0.1.0/zapit/models/network_member.py
--rw-r--r--   0        0        0      713 2023-04-23 07:09:10.857454 zapit-0.1.0/zapit/models/organizations.py
--rw-r--r--   0        0        0      617 2023-04-25 05:12:29.402936 zapit-0.1.0/zapit/models/user.py
--rw-r--r--   0        0        0      365 2023-04-25 02:05:06.142297 zapit-0.1.0/zapit/models/util.py
--rw-r--r--   0        0        0     1714 2023-04-25 05:09:37.535736 zapit-0.1.0/zapit/requestor.py
--rw-r--r--   0        0        0     8295 2023-04-25 05:12:40.632938 zapit-0.1.0/zapit/zapit.py
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 zapit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-04-25 05:49:46.732956 zapit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      374 2023-04-25 05:45:54.423955 zapit-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 10:44:03.019693 zapit-0.1.1/zapit/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-25 02:02:10.126299 zapit-0.1.1/zapit/exceptions.py
+-rw-r--r--   0        0        0     1834 2023-04-25 05:09:56.559735 zapit-0.1.1/zapit/models/network.py
+-rw-r--r--   0        0        0     1226 2023-04-24 08:52:14.840087 zapit-0.1.1/zapit/models/network_member.py
+-rw-r--r--   0        0        0      713 2023-04-23 07:09:10.857454 zapit-0.1.1/zapit/models/organizations.py
+-rw-r--r--   0        0        0      617 2023-04-25 05:12:29.402936 zapit-0.1.1/zapit/models/user.py
+-rw-r--r--   0        0        0      365 2023-04-25 02:05:06.142297 zapit-0.1.1/zapit/models/util.py
+-rw-r--r--   0        0        0     1808 2023-04-25 05:47:08.188956 zapit-0.1.1/zapit/requestor.py
+-rw-r--r--   0        0        0     8295 2023-04-25 05:12:40.632938 zapit-0.1.1/zapit/zapit.py
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 zapit-0.1.1/PKG-INFO
```

### Comparing `zapit-0.1.0/pyproject.toml` & `zapit-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zapit"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Zerotier API wrapper."
 authors = ["Macleay Stephenson <macleays@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `zapit-0.1.0/zapit/models/network.py` & `zapit-0.1.1/zapit/models/network.py`

 * *Files identical despite different names*

### Comparing `zapit-0.1.0/zapit/models/network_member.py` & `zapit-0.1.1/zapit/models/network_member.py`

 * *Files identical despite different names*

### Comparing `zapit-0.1.0/zapit/models/organizations.py` & `zapit-0.1.1/zapit/models/organizations.py`

 * *Files identical despite different names*

### Comparing `zapit-0.1.0/zapit/models/user.py` & `zapit-0.1.1/zapit/models/user.py`

 * *Files identical despite different names*

### Comparing `zapit-0.1.0/zapit/requestor.py` & `zapit-0.1.1/zapit/requestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         auth_headers.update(headers)
         return self._make_request(
             method,
             url,
             auth_headers,
             data,
             timeout=timeout,
+            *args,
+            **kwargs,
         )
 
     def _make_request(
         self,
         method,
         url,
         headers,
@@ -58,10 +60,12 @@
             logger.info(f"headers: {headers}")
             return self._http.request(
                 method,
                 url,
                 headers=headers,
                 data=data,
                 timeout=timeout or self.timeout,
+                *args,
+                **kwargs,
             )
         except Exception as exc:
             raise RequestException(exc, args, kwargs)
```

### Comparing `zapit-0.1.0/zapit/zapit.py` & `zapit-0.1.1/zapit/zapit.py`

 * *Files identical despite different names*

### Comparing `zapit-0.1.0/PKG-INFO` & `zapit-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zapit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Zerotier API wrapper.
 License: MIT
 Author: Macleay Stephenson
 Author-email: macleays@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,27 +19,27 @@
 
 # Zapit
 
 Zapit, a Zerotier API wrapper for Python.
 
 ## Installation
 
-Zapit is supported on 3.7+. The recommended way to install Zapit is via pip.
+Zapit is supported on 3.8+. The recommended way to install Zapit is via pip.
 
 ``` bash
 pip install zapit
 ```
 
 ## Quickstart
 
 ``` python
 
 import zapit
 
 ztcentral = zapit.Central(
-    api_key = "API_KEY
+    api_key = "API_KEY"
 )
 
 # Get all the networks avaliable.
 networks = ztcentral.list_networks()
 ```
```

