# Comparing `tmp/shadpy-2.1.0.tar.gz` & `tmp/shadpy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadpy-2.1.0.tar", last modified: Mon Apr 24 12:25:24 2023, max compression
+gzip compressed data, was "shadpy-2.1.1.tar", last modified: Mon Apr 24 12:32:18 2023, max compression
```

## Comparing `shadpy-2.1.0.tar` & `shadpy-2.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.371544 shadpy-2.1.0/
--rw-rw-rw-   0        0        0     3350 2023-04-24 12:25:24.371544 shadpy-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2206 2023-04-24 12:24:15.000000 shadpy-2.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 12:25:24.371544 shadpy-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1542 2023-04-24 12:25:07.000000 shadpy-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.230565 shadpy-2.1.0/shadpy/
--rw-rw-rw-   0        0        0      240 2023-04-24 00:07:06.000000 shadpy-2.1.0/shadpy/__init__.py
--rw-rw-rw-   0        0        0    29264 2023-04-24 00:05:02.000000 shadpy-2.1.0/shadpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.277427 shadpy-2.1.0/shadpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.309063 shadpy-2.1.0/shadpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 shadpy-2.1.0/shadpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25880 2023-04-24 12:22:04.000000 shadpy-2.1.0/shadpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 shadpy-2.1.0/shadpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.324683 shadpy-2.1.0/shadpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 shadpy-2.1.0/shadpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.340304 shadpy-2.1.0/shadpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.371544 shadpy-2.1.0/shadpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 shadpy-2.1.0/shadpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 shadpy-2.1.0/shadpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-24 12:25:24.261807 shadpy-2.1.0/shadpy.egg-info/
--rw-rw-rw-   0        0        0     3350 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 12:25:24.000000 shadpy-2.1.0/shadpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.310031 shadpy-2.1.1/
+-rw-rw-rw-   0        0        0     3350 2023-04-24 12:32:18.310031 shadpy-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2206 2023-04-24 12:24:15.000000 shadpy-2.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:32:18.310031 shadpy-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1542 2023-04-24 12:29:43.000000 shadpy-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.278400 shadpy-2.1.1/shadpy/
+-rw-rw-rw-   0        0        0      240 2023-04-24 12:29:14.000000 shadpy-2.1.1/shadpy/__init__.py
+-rw-rw-rw-   0        0        0    29263 2023-04-24 12:32:02.000000 shadpy-2.1.1/shadpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.294020 shadpy-2.1.1/shadpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.294020 shadpy-2.1.1/shadpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 shadpy-2.1.1/shadpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25880 2023-04-24 12:22:04.000000 shadpy-2.1.1/shadpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 shadpy-2.1.1/shadpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.294020 shadpy-2.1.1/shadpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10587 2023-04-24 12:28:52.000000 shadpy-2.1.1/shadpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.305026 shadpy-2.1.1/shadpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.305026 shadpy-2.1.1/shadpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 shadpy-2.1.1/shadpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 shadpy-2.1.1/shadpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:32:18.278400 shadpy-2.1.1/shadpy.egg-info/
+-rw-rw-rw-   0        0        0     3350 2023-04-24 12:32:18.000000 shadpy-2.1.1/shadpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-04-24 12:32:18.000000 shadpy-2.1.1/shadpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:32:18.000000 shadpy-2.1.1/shadpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-24 12:32:18.000000 shadpy-2.1.1/shadpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 12:32:18.000000 shadpy-2.1.1/shadpy.egg-info/top_level.txt
```

### Comparing `shadpy-2.1.0/PKG-INFO` & `shadpy-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadpy
-Version: 2.1.0
+Version: 2.1.1
 Summary: This is an unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: shad,rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shadpy Version: 2.1.0 Summary: This is an
+Metadata-Version: 2.1 Name: shadpy Version: 2.1.1 Summary: This is an
 unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 shad,rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `shadpy-2.1.0/README.md` & `shadpy-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/setup.py` & `shadpy-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'shadpy',
-    version = '2.1.0',
+    version = '2.1.1',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Shad accounts.',
     keywords = ['shad', 'rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

### Comparing `shadpy-2.1.0/shadpy/client.py` & `shadpy-2.1.1/shadpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,42 +6,42 @@
 from .network import Connection, Proxies
 from .gadgets import exceptions, methods, thumbnail
 from .sessions import StringSession, SQLiteSession
 
 
 class Client:
     configuire = {
-        'package': 'web.rubika.ir',
+        'package': 'web.shad.ir',
         'platform': 'Web',
         'app_name': 'Main',
         'user_agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
                        'AppleWebKit/537.36 (KHTML, like Gecko)'
                        'Chrome/102.0.0.0 Safari/537.36'),
         'api_version': '5',
-        'app_version': '4.2.0'
+        'app_version': '4.1.16'
     }
 
     def __init__(self,
         session,
         proxy=None,
         logger=None,
         timeout=20,
         lang_code='fa',
         user_agent=None,
         request_retries=5, *args, **kwargs):
 
         """Client
             Args:
-                session_name (`str` | `rubika.sessions.StringSession`):
+                session_name (`str` | `shadpy.sessions.StringSession`):
                     The file name of the session file that is used
                     if there is a string Given (may be a complete path)
                     or it could be a string session
-                    [rubika.sessions.StringSession]
+                    [shadpy.sessions.StringSession]
 
-                proxy (` rubika.network.Proxies `, optional): To set up a proxy
+                proxy (` shadpy.network.Proxies `, optional): To set up a proxy
 
                 user_agent (`str`, optional):
                     Client uses the web version, You can set the usr-user_agent
 
                 timeout (`int` | `float`, optional):
                     To set the timeout `` default( `20 seconds` )``
 
@@ -53,22 +53,22 @@
         """
 
         if isinstance(session, str):
             session = SQLiteSession(session)
 
         elif not isinstance(session, StringSession):
             raise TypeError('The given session must be a '
-                            'str or [rubika.sessions.StringSession]')
+                            'str or [shadpy.sessions.StringSession]')
 
         if not isinstance(logger, logging.Logger):
             logger = logging.getLogger(logger_name)
 
         if proxy and not isinstance(proxy, Proxies):
             raise TypeError(
-                'The given proxy must be a [rubika.network.Proxies]')
+                'The given proxy must be a [shadpy.network.Proxies]')
 
         self._dcs = None
         self._key = None
         self._auth = None
         self._guid = None
         self._proxy = proxy
         self._logger = logger
```

### Comparing `shadpy-2.1.0/shadpy/crypto/crypto.py` & `shadpy-2.1.1/shadpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/gadgets/classino.py` & `shadpy-2.1.1/shadpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/gadgets/exceptions.py` & `shadpy-2.1.1/shadpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/gadgets/grouping.py` & `shadpy-2.1.1/shadpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/gadgets/methods.py` & `shadpy-2.1.1/shadpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/gadgets/thumbnail.py` & `shadpy-2.1.1/shadpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/network/connection.py` & `shadpy-2.1.1/shadpy/network/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     """Internal class"""
 
     def __init__(self, client):
         self._client = client
         self._connection = aiohttp.ClientSession(
             connector=self._client._proxy,
             headers={'user-agent': self._client._user_agent,
-            	'origin': 'https://web.rubika.ir',
-            	'referer': 'https://web.rubika.ir/'},
+            	'origin': 'https://web.shad.ir',
+            	'referer': 'https://web.shad.ir/'},
             timeout=aiohttp.ClientTimeout(total=self._client._timeout))
 
     async def _dcs(self):
         if not self._client._dcs:
             self._client._dcs = await self.execute(
                 methods.authorisations.GetDCs())
```

### Comparing `shadpy-2.1.0/shadpy/network/proxies.py` & `shadpy-2.1.1/shadpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/sessions/sqliteSession.py` & `shadpy-2.1.1/shadpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/sessions/stringSession.py` & `shadpy-2.1.1/shadpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/structs/handlers.py` & `shadpy-2.1.1/shadpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/structs/models.py` & `shadpy-2.1.1/shadpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/structs/results.py` & `shadpy-2.1.1/shadpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy/structs/struct.py` & `shadpy-2.1.1/shadpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.0/shadpy.egg-info/PKG-INFO` & `shadpy-2.1.1/shadpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadpy
-Version: 2.1.0
+Version: 2.1.1
 Summary: This is an unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: shad,rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shadpy Version: 2.1.0 Summary: This is an
+Metadata-Version: 2.1 Name: shadpy Version: 2.1.1 Summary: This is an
 unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 shad,rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `shadpy-2.1.0/shadpy.egg-info/SOURCES.txt` & `shadpy-2.1.1/shadpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

