# Comparing `tmp/openai_forward-0.1.0.tar.gz` & `tmp/openai_forward-0.1.1.tar.gz`

## Comparing `openai_forward-0.1.0.tar` & `openai_forward-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/__init__.py
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/__main__.py
--rwxr-xr-x   0        0        0     3101 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/_base.py
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/app.py
--rwxr-xr-x   0        0        0     2611 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/config.py
--rwxr-xr-x   0        0        0      808 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/openai.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/content/__init__.py
--rwxr-xr-x   0        0        0     3327 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/content/chat.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/content/image.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/routers/__init__.py
--rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/routers/openai_v1.py
--rwxr-xr-x   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.1.0/openai_forward/routers/schemas.py
--rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.0/.gitignore
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     5470 2020-02-02 00:00:00.000000 openai_forward-0.1.0/README.md
--rwxr-xr-x   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 openai_forward-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/__main__.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/_base.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/app.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/config.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.1.1/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 openai_forward-0.1.1/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 openai_forward-0.1.1/PKG-INFO
```

### Comparing `openai_forward-0.1.0/openai_forward/_base.py` & `openai_forward-0.1.1/openai_forward/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from .content.chat import log_chat_completions, ChatSaver
 
 
 class OpenaiBase:
     default_api_key = os.environ.get("OPENAI_API_KEY", "")
     base_url = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com")
     LOG_CHAT = os.environ.get("LOG_CHAT", "False").lower() == "true"
+    ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "")
+    if ROUTE_PREFIX:
+        if ROUTE_PREFIX.endswith('/'):
+            ROUTE_PREFIX = ROUTE_PREFIX[:-1]
+        if not ROUTE_PREFIX.startswith('/'):
+            ROUTE_PREFIX = '/' + ROUTE_PREFIX
     stream_timeout = 20
     timeout = 30
     non_stream_timeout = 30
     allow_ips = []
     chatsaver = ChatSaver(save_interval=10)
 
     def add_allowed_ip(self, ip: str):
@@ -44,15 +50,17 @@
             cls.log_chat_completions(bytes_)
         except Exception as e:
             logger.warning(e)
 
     @classmethod
     async def _reverse_proxy(cls, request: Request):
         client: httpx.AsyncClient = request.app.state.client
-        url = httpx.URL(path=request.url.path, query=request.url.query.encode('utf-8'))
+        url_path = request.url.path
+        url_path = url_path[len(cls.ROUTE_PREFIX):]
+        url = httpx.URL(path=url_path, query=request.url.query.encode('utf-8'))
         headers = dict(request.headers)
         auth = headers.pop("authorization", None)
         if auth and str(auth).startswith("Bearer sk-"):
             tmp_headers = {'Authorization': auth}
         elif cls.default_api_key:
             auth = "Bearer " + cls.default_api_key
             tmp_headers = {'Authorization': auth}
```

### Comparing `openai_forward-0.1.0/openai_forward/app.py` & `openai_forward-0.1.1/openai_forward/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 
 
 @app.on_event('shutdown')
 async def shutdown_event():
     await app.state.client.aclose()
 
 
-app.add_route('/{api_path:path}', openai.reverse_proxy,
-              ['GET', 'POST', 'PUT', 'DELETE', 'OPTIONS', 'HEAD', 'PATCH', 'TRACE'])
+app.add_route(openai.ROUTE_PREFIX+'/{api_path:path}', openai.reverse_proxy,
+              methods=['GET', 'POST', 'PUT', 'DELETE', 'OPTIONS', 'HEAD', 'PATCH', 'TRACE'])
 app.include_router(router_v1)
```

### Comparing `openai_forward-0.1.0/openai_forward/config.py` & `openai_forward-0.1.1/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/openai_forward/openai.py` & `openai_forward-0.1.1/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/openai_forward/content/chat.py` & `openai_forward-0.1.1/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/openai_forward/routers/schemas.py` & `openai_forward-0.1.1/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/.gitignore` & `openai_forward-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/LICENSE` & `openai_forward-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/README.md` & `openai_forward-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,23 +37,25 @@
 Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions 
 
 # Table of Contents 
 
 - [Features](#Features) 
 - [Usage](#Usage) 
 - [Service Deployment](#Service-Deployment) 
-- [Service Usage](#Service Usage) 
+- [Service Usage](#Service-Usage) 
 
 # Features 
 - [x] Supports forwarding of all OpenAI interfaces 
 - [x] Supports request IP verification 
 - [x] Supports streaming forwarding 
 - [x] Supports default API key 
 - [x] pip installation and deployment 
 - [x] Docker deployment 
+- [x] Support for multiple worker processes
+- [x] Support for specifying the forwarding routing prefix.
 - [ ] Chat content security: Chat content streaming filtering 
 
 # Usage 
 > Here, the proxy address set up by the individual, https://caloi.top, is used as an example 
 
 ### Image Generation (DALL-E):
 ```bash 
@@ -78,35 +80,35 @@
 ```bash 
 docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
 ``` 
 
 
 ### Using in a module 
 
-**Used in JS/TS** 
+**JS/TS** 
 ```typescript 
 import { Configuration } from "openai"; 
 
 const configuration = new Configuration({ 
     basePath: "https://caloi.top", 
     apiKey: "sk-******", 
 
 }); 
 ``` 
-**Used in Python** 
+**Python** 
 ```python 
 import openai 
 openai.api_base = "https://caloi.top" 
 openai.api_key = "sk-******" 
 ``` 
 
 # Service Deployment 
 Two service deployment methods are provided, choose one 
 
-## Method 1: pip 
+## Use `pip` 
 **Installation** 
 ```bash 
 pip install openai-forward 
 ``` 
 **Run forwarding service** 
 The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be specified through `--workers`, which defaults to `1`. 
 ```bash 
@@ -117,15 +119,15 @@
 Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client does not need to pass in the Authorization in the header when requesting the relevant route. 
 Startup command with default API key: 
 ```bash 
 OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1 
 ``` 
 Note: If both the default API key and the API key passed in the request header exist, the API key in the request header will override the default API key. 
 
-## Method 2: Docker (recommended) 
+## Use Docker (recommended) 
 ```bash 
 docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
 ``` 
 The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`. 
 Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command. 
 
 # Service Usage
```

### Comparing `openai_forward-0.1.0/pyproject.toml` & `openai_forward-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.0/PKG-INFO` & `openai_forward-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.0
+Version: 0.1.1
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -69,23 +69,25 @@
 Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions 
 
 # Table of Contents 
 
 - [Features](#Features) 
 - [Usage](#Usage) 
 - [Service Deployment](#Service-Deployment) 
-- [Service Usage](#Service Usage) 
+- [Service Usage](#Service-Usage) 
 
 # Features 
 - [x] Supports forwarding of all OpenAI interfaces 
 - [x] Supports request IP verification 
 - [x] Supports streaming forwarding 
 - [x] Supports default API key 
 - [x] pip installation and deployment 
 - [x] Docker deployment 
+- [x] Support for multiple worker processes
+- [x] Support for specifying the forwarding routing prefix.
 - [ ] Chat content security: Chat content streaming filtering 
 
 # Usage 
 > Here, the proxy address set up by the individual, https://caloi.top, is used as an example 
 
 ### Image Generation (DALL-E):
 ```bash 
@@ -110,35 +112,35 @@
 ```bash 
 docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
 ``` 
 
 
 ### Using in a module 
 
-**Used in JS/TS** 
+**JS/TS** 
 ```typescript 
 import { Configuration } from "openai"; 
 
 const configuration = new Configuration({ 
     basePath: "https://caloi.top", 
     apiKey: "sk-******", 
 
 }); 
 ``` 
-**Used in Python** 
+**Python** 
 ```python 
 import openai 
 openai.api_base = "https://caloi.top" 
 openai.api_key = "sk-******" 
 ``` 
 
 # Service Deployment 
 Two service deployment methods are provided, choose one 
 
-## Method 1: pip 
+## Use `pip` 
 **Installation** 
 ```bash 
 pip install openai-forward 
 ``` 
 **Run forwarding service** 
 The port number can be specified through `--port`, which defaults to `8000`, and the number of worker processes can be specified through `--workers`, which defaults to `1`. 
 ```bash 
@@ -149,15 +151,15 @@
 Of course, OPENAI_API_KEY can also be passed in as an environment variable as the default API key, so that the client does not need to pass in the Authorization in the header when requesting the relevant route. 
 Startup command with default API key: 
 ```bash 
 OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --workers=1 
 ``` 
 Note: If both the default API key and the API key passed in the request header exist, the API key in the request header will override the default API key. 
 
-## Method 2: Docker (recommended) 
+## Use Docker (recommended) 
 ```bash 
 docker run --name="openai-forward" -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
 ``` 
 The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`. 
 Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command. 
 
 # Service Usage
```

