# Comparing `tmp/altvmasterlist-2.4.5.tar.gz` & `tmp/altvmasterlist-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altvmasterlist-2.4.5.tar", max compression
+gzip compressed data, was "altvmasterlist-2.4.6.tar", max compression
```

## Comparing `altvmasterlist-2.4.5.tar` & `altvmasterlist-2.4.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/LICENSE
--rw-r--r--   0        0        0      425 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/README.md
--rw-r--r--   0        0        0     1053 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/pyproject.toml
--rw-r--r--   0        0        0      402 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/__init__.py
--rw-r--r--   0        0        0     6982 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/altstats.py
--rw-r--r--   0        0        0     9681 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/masterlist.py
--rw-r--r--   0        0        0    10516 2023-04-20 11:21:43.722667 altvmasterlist-2.4.5/src/altvmasterlist/shared.py
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 altvmasterlist-2.4.5/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/LICENSE
+-rw-r--r--   0        0        0      425 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/README.md
+-rw-r--r--   0        0        0     1053 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/__init__.py
+-rw-r--r--   0        0        0     6960 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/altstats.py
+-rw-r--r--   0        0        0     9658 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/masterlist.py
+-rw-r--r--   0        0        0    10974 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/shared.py
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 altvmasterlist-2.4.6/PKG-INFO
```

### Comparing `altvmasterlist-2.4.5/LICENSE` & `altvmasterlist-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.5/pyproject.toml` & `altvmasterlist-2.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altvmasterlist"
-version = "2.4.5"
+version = "2.4.6"
 description = "A package to use the alt:V Masterlist api."
 authors = ["Nickwasused <contact.nickwasused.fa6c8@simplelogin.co>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/Nickwasused/altv-python-masterlist"
 documentation = "https://nickwasused.github.io/altv-python-masterlist/"
 classifiers = [
```

### Comparing `altvmasterlist-2.4.5/src/altvmasterlist/altstats.py` & `altvmasterlist-2.4.6/src/altvmasterlist/altstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from dataclasses import dataclass
 from re import compile
 import logging
 import sys
 
 logging.basicConfig(level=logging.INFO)
 logging.getLogger().setLevel(logging.INFO)
-logging.debug(f'starting with base link: {shared.AltstatsUrls.base_link}')
 """You can find the altstats api docs here: https://docs.altv.mp/articles/master_list_api.html#information-1"""
 
 
 @dataclass
 class Server:
     """This is the server object. All values will be fetched from the api
         in the __init__ function. You just need to provide the id like this: Server("example_id")
@@ -57,15 +56,15 @@
     Version: float = 0.0
 
     def __init__(self, server_id: int, no_fetch: bool = False) -> None:
         """Update the server data using the api."""
         self.Id = server_id
 
         if not no_fetch:
-            temp_data = shared.request(shared.AltstatsUrls.server_link.format(self.Id))
+            temp_data = shared.request(shared.AltstatsUrls.specific_server.value.format(self.Id))
             if temp_data is None or temp_data == {} or not temp_data["LastUpdate"]:
                 # the api returned no data or the server is offline
                 self.LastActivity = False
                 self.Players = 0
             else:
                 self.FoundAt = temp_data["FoundAt"]
                 self.LastActivity = temp_data["LastActivity"]
@@ -105,15 +104,16 @@
     def update(self) -> None:
         """Update the server data using the api."""
         self.__init__(self.Id)
 
     @property
     def connect_json(self) -> dict | None:
         """Get the connect.json of the server."""
-        return shared.fetch_connect_json(self.UseCdn, self.Locked, self.LastFetchOnline, self.Ip, self.Port, self.CdnUrl)
+        return shared.fetch_connect_json(self.UseCdn, self.Locked, self.LastFetchOnline,
+                                         self.Ip, self.Port, self.CdnUrl)
 
     @property
     def permissions(self) -> shared.Permissions | None:
         """Get the permissions of the server."""
         return shared.get_permissions(self.connect_json)
 
     def get_dtc_url(self, password: str = None) -> str | None:
@@ -128,15 +128,15 @@
 def get_server_stats() -> dict | None:
     """Statistics - Player Count across all servers & The amount of servers online
 
     Returns:
         None: When an error occurs
         dict: The stats
     """
-    data = shared.request(shared.AltstatsUrls.all_server_stats_link)
+    data = shared.request(shared.AltstatsUrls.all_server_stats.value)
     if data is None:
         return None
     else:
         return data
 
 
 def get_servers() -> list[Server] | None:
@@ -144,15 +144,15 @@
         Note that the server objects returned are not complete!
 
     Returns:
         None: When an error occurs
         list: List object that contains all servers.
     """
     return_servers = []
-    servers = shared.request(shared.AltstatsUrls.all_servers_link)
+    servers = shared.request(shared.AltstatsUrls.all_servers.value)
     if servers is None or servers == "{}":
         return None
     else:
         for server in servers:
             tmp_server = Server(server["id"], True)
             tmp_server.Name = server["name"]
             tmp_server.Locked = bool(server["locked"])
```

### Comparing `altvmasterlist-2.4.5/src/altvmasterlist/masterlist.py` & `altvmasterlist-2.4.6/src/altvmasterlist/masterlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from dataclasses import dataclass
 from re import compile
 import logging
 import sys
 
 logging.basicConfig(level=logging.INFO)
 logging.getLogger().setLevel(logging.INFO)
-logging.debug(f'starting with base link: {shared.MasterlistUrls.base_link}')
 """You can find the masterlist api docs here: https://docs.altv.mp/articles/master_list_api.html"""
 
 
 @dataclass
 class Server:
     """This is the server object. All values will be fetched from the api
     in the __init__ function. You just need to provide the id like this: Server("example_id")
@@ -47,15 +46,15 @@
     lastUpdate: int = 0
 
     def __init__(self, server_id: str, no_fetch: bool = False) -> None:
         """Update the server data using the api."""
         self.id = server_id
 
         if not no_fetch:
-            temp_data = shared.request(shared.MasterlistUrls.server_link.format(self.id))
+            temp_data = shared.request(shared.MasterlistUrls.specific_server.value.format(self.id))
             if temp_data is None or temp_data == {} or not temp_data["active"]:
                 # the api returned no data or the server is offline
                 self.active = False
                 self.players = 0
             else:
                 self.active = temp_data["active"]
                 self.maxPlayers = temp_data["info"]["maxPlayers"]
@@ -92,29 +91,29 @@
         Args:
             time (str): The timerange of the data. Can be 1d, 7d, 31d.
 
         Returns:
             None: When an error occurs
             dict: The maximum player data
         """
-        return shared.request(shared.MasterlistUrls.server_max_link.format(self.id, time))
+        return shared.request(shared.MasterlistUrls.specific_server_maximum.value.format(self.id, time))
 
     def get_avg(self, time: str = "1d", return_result: bool = False) -> dict | int | None:
         """Averages - Returns averages data about the specified server (TIME = 1d, 7d, 31d)
 
         Args:
             time (str): The timerange of the data. Can be 1d, 7d, 31d.
             return_result (bool): Define if you want the overall average.
 
         Returns:
             None: When an error occurs
             dict: The maximum player data
             int: Overall average of defined timerange
         """
-        average_data = shared.request(shared.MasterlistUrls.server_average_link.format(self.id, time))
+        average_data = shared.request(shared.MasterlistUrls.specific_server_average.value.format(self.id, time))
         if not average_data:
             return None
 
         if return_result:
             players_all = 0
             for entry in average_data:
                 players_all = players_all + entry["c"]
@@ -145,15 +144,15 @@
 def get_server_stats() -> dict | None:
     """Statistics - Player Count across all servers & The amount of servers online
 
     Returns:
         None: When an error occurs
         dict: The stats
     """
-    data = shared.request(shared.MasterlistUrls.all_server_stats_link)
+    data = shared.request(shared.MasterlistUrls.all_server_stats.value)
     if data is None:
         return None
     else:
         return data
 
 
 def get_servers() -> list[Server] | None:
@@ -161,15 +160,15 @@
     Note that the server objects returned are not complete!
 
     Returns:
         None: When an error occurs
         list: List object that contains all servers.
     """
     return_servers = []
-    servers = shared.request(shared.MasterlistUrls.all_servers_link)
+    servers = shared.request(shared.MasterlistUrls.all_servers.value)
     if servers is None or servers == "{}":
         return None
     else:
         for server in servers:
             tmp_server = Server(server["id"], no_fetch=True)
             tmp_server.active = True
             tmp_server.maxPlayers = server["maxPlayers"]
@@ -223,15 +222,15 @@
     """Get a list of all available launcher skins.
 
     Returns:
         json: A json array of all launcher skins.
 
     The elements have the following keys: serverId, xxHash64 and fileName.
     """
-    skins = shared.request(shared.MasterlistUrls.launcher_skins)
+    skins = shared.request(shared.MasterlistUrls.launcher_skins.value)
 
     if skins is None or skins == "{}":
         return None
     else:
         return skins["indexEntries"]
 
 
@@ -257,15 +256,15 @@
             - imageLogo64: base64 Logo
             - imageBackground64: base64 background image
 
     """
     if not filename or filename == "":
         return None
 
-    skin = shared.request(shared.MasterlistUrls.launcher_file.format(filename))
+    skin = shared.request(shared.MasterlistUrls.launcher_skins_file.value.format(filename))
 
     if skin is None or skin == {}:
         return None
     else:
         return skin
```

### Comparing `altvmasterlist-2.4.5/src/altvmasterlist/shared.py` & `altvmasterlist-2.4.6/src/altvmasterlist/shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 #!/usr/bin/env python3
 from urllib.request import urlopen, Request
 from dataclasses import dataclass
 from json import dumps, loads
 from io import StringIO
+from enum import Enum
 import logging
 import secrets
 
 logging.basicConfig(level=logging.INFO)
 logging.getLogger().setLevel(logging.INFO)
 
 
-@dataclass
-class MasterlistUrls:
+class MasterlistUrls(Enum):
     """This class is used for the masterlist submodule. It provides all urls needed."""
-    base_link: str = "https://api.alt-mp.com"
-    base_cdn: str = "https://cdn.alt-mp.com"
-    all_server_stats_link: str = f"{base_link}/servers"
-    all_servers_link: str = f"{base_link}/servers/list"
-    server_link: str = f"{base_link}/server" + "/{}"
-    server_average_link: str = f"{base_link}/avg" + "/{}/{}"
-    server_max_link: str = f"{base_link}/max" + "/{}/{}"
-    launcher_skins: str = f"{base_cdn}/launcher-skins/index.json"
-    launcher_file: str = f"{base_cdn}/launcher-skins/files/" + "{}"
+    all_server_stats = "https://api.alt-mp.com/servers"
+    all_servers = "https://api.alt-mp.com/servers/list"
+    specific_server = "https://api.alt-mp.com/server/{}"
+    specific_server_average = "https://api.alt-mp.com/avg/{}/{}"
+    specific_server_maximum = "https://api.alt-mp.com/max/{}/{}"
+    launcher_skins = "https://cdn.alt-mp.com/launcher-skins/index.json"
+    launcher_skins_file = "https://cdn.alt-mp.com/launcher-skins/files/{}"
 
 
-@dataclass
-class AltstatsUrls:
+class AltstatsUrls(Enum):
     """This class is used for the altstats submodule. It provides all urls needed."""
-    base_link: str = "https://api.altstats.net/api/v1/"
-    all_server_stats_link: str = f"{base_link}/master"
-    all_servers_link: str = f"{base_link}/server"
-    server_link: str = f"{base_link}/server/" + "{}"
+    all_server_stats = "https://api.altstats.net/api/v1//master"
+    all_servers = "https://api.altstats.net/api/v1//server"
+    specific_server = "https://api.altstats.net/api/v1//server/{}"
+
+
+class Extra(Enum):
+    """This class defines extra values."""
+    user_agent = "AltPublicAgent"
+    default_password = "17241709254077376921"
 
 
 @dataclass
 class RequestHeaders:
     """These are the common request headers used by the request function.
     They are commonly used to emulate an alt:V client.
     """
     host: str = "",
-    user_agent: str = 'AltPublicAgent',
+    user_agent: str = Extra.user_agent.value,
     accept: str = '*/*',
     alt_debug: str = 'false',
-    alt_password: str = '17241709254077376921',
+    alt_password: str = Extra.default_password.value,
     alt_branch: str = "",
     alt_version: str = "",
     alt_player_name: str = secrets.token_urlsafe(10),
     alt_social_id: str = secrets.token_hex(9),
     alt_hardware_id2: str = secrets.token_hex(19),
     alt_hardware_id: str = secrets.token_hex(19)
 
@@ -85,15 +87,15 @@
     """
     # Use the User-Agent: AltPublicAgent, because some servers protect their CDN with
     # a simple User-Agent check e.g. https://luckyv.de does that
     if "http://" in url and cdn:
         req_headers = RequestHeaders(server.version, server.branch)
     else:
         req_headers = {
-            'User-Agent': 'AltPublicAgent',
+            'User-Agent': Extra.user_agent.value,
             'content-type': 'application/json; charset=utf-8'
         }
 
     try:
         api_request = Request(url, headers=req_headers, method="GET")
         with urlopen(api_request, timeout=60) as api_data:
             if api_data.status != 200:
@@ -109,15 +111,15 @@
 def get_dtc_url(use_cdn: bool, cdn_url: str, host: str, port: int, locked: bool, password: str = None) -> str | None:
     """This function gets the direct connect protocol url of an alt:V Server.
         (https://docs.altv.mp/articles/connectprotocol.html)
 
     Args:
         use_cdn (bool): Define if the Server is using a CDN.
         cdn_url (str): The CDN url of the server.
-        host (str): The host IP adress of the server.
+        host (str): The host IP address of the server.
         port (int): The port of the server.
         locked (bool): Define if the server is locked. Locked servers have a password.
         password (str): The password of the server.
 
     Returns:
         None: When an error occurred. But exceptions will still be logged!
         str: The direct connect protocol url.
@@ -144,15 +146,15 @@
 def fetch_connect_json(use_cdn: bool, locked: bool, active: bool, host: str, port: int, cdn_url: str) -> dict | None:
     """This function fetched the connect.json of an alt:V server.
 
     Args:
         use_cdn (bool): Define if the Server is using a CDN.
         locked (bool): Define if the server is locked. Locked servers have a password.
         active (bool): Define if the server is active. Active means Online.
-        host (str): The host IP adress of the server.
+        host (str): The host IP address of the server.
         port (int): The port of the server.
         cdn_url (str): The CDN url of the server.
 
     Returns:
         None: When an error occurred. But exceptions will still be logged!
         str: The direct connect protocol url.
     """
@@ -177,33 +179,34 @@
 class Permissions:
     """This is the Permission class used by get_permissions.
 
     Returns:
         Required: The required permissions of an alt:V server. Without them, you can not play on the server.
         Optional: The optional permissions of an alt:V server. You can play without them.
     """
-
     @dataclass
     class Required:
         """Required Permissions of an alt:V server.
 
         Attributes:
+        ----------
             screen_capture (bool): This allows a screenshot to be taken of the alt:V process (just GTA) and any webview
             webrtc (bool): This allows peer-to-peer RTC inside JS
             clipboard_access (bool): This allows to copy content to users clipboard
         """
         screen_capture: bool = False
         webrtc: bool = False
         clipboard_access: bool = False
 
     @dataclass
     class Optional:
         """Optional Permissions of an alt:V server.
 
         Attributes:
+        ----------
             screen_capture (bool): This allows a screenshot to be taken of the alt:V process (just GTA) and any webview
             webrtc (bool): This allows peer-to-peer RTC inside JS
             clipboard_access (bool): This allows to copy content to users clipboard
         """
         screen_capture: bool = False
         webrtc: bool = False
         clipboard_access: bool = False
@@ -216,51 +219,58 @@
         connect_json (json): The connect.json of the server. You can get the connect.json from the Server object
                                 e.g. Server(127).connect_json
 
     Returns:
         None: When an error occurred. But exceptions will still be logged!
         Permissions: The permissions of the server.
     """
+    class Permission(Enum):
+        screen_capture = "Screen Capture"
+        webrtc = "WebRTC"
+        clipboard_access = "Clipboard Access"
+        optional = "optional-permissions"
+        required = "required-permissions"
+
     if connect_json is None:
         return None
 
-    optional = connect_json["optional-permissions"]
-    required = connect_json["required-permissions"]
+    optional = connect_json[Permission.optional.value]
+    required = connect_json[Permission.required.value]
 
     permissions = Permissions()
 
     if optional is not []:
         try:
-            permissions.Optional.screen_capture = optional["Screen Capture"]
+            permissions.Optional.screen_capture = optional[Permission.screen_capture.value]
         except TypeError:
             pass
 
         try:
-            permissions.Optional.webrtc = optional["WebRTC"]
+            permissions.Optional.webrtc = optional[Permission.webrtc.value]
         except TypeError:
             pass
 
         try:
-            permissions.Optional.clipboard_access = optional["Clipboard Access"]
+            permissions.Optional.clipboard_access = optional[Permission.clipboard_access.value]
         except TypeError:
             pass
 
     if required is not []:
         try:
-            permissions.Required.screen_capture = required["Screen Capture"]
+            permissions.Required.screen_capture = required[Permission.screen_capture.value]
         except TypeError:
             pass
 
         try:
-            permissions.Required.webrtc = required["WebRTC"]
+            permissions.Required.webrtc = required[Permission.webrtc.value]
         except TypeError:
             pass
 
         try:
-            permissions.Required.clipboard_access = required["Clipboard Access"]
+            permissions.Required.clipboard_access = required[Permission.clipboard_access.value]
         except TypeError:
             pass
 
     return permissions
 
 
 def get_resource_size(use_cdn: bool, cdn_url: str, resource: str, host: str, port: int, decimal: int) -> float | None:
@@ -279,14 +289,14 @@
         float: The size of the resource.
     """
     if use_cdn:
         resource_url = f"{cdn_url}/{resource}.resource"
     else:
         resource_url = f"http://{host}:{port}/{resource}.resource"
 
-    size_request = Request(resource_url, headers={"User-Agent": "AltPublicAgent"}, method="HEAD")
+    size_request = Request(resource_url, headers={"User-Agent": Extra.user_agent.value}, method="HEAD")
 
     with urlopen(size_request, timeout=60) as size_data:
         if size_data.status == 200:
             return round((int(size_data.headers["Content-Length"]) / 1048576), decimal)
         else:
             return None
```

### Comparing `altvmasterlist-2.4.5/PKG-INFO` & `altvmasterlist-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altvmasterlist
-Version: 2.4.5
+Version: 2.4.6
 Summary: A package to use the alt:V Masterlist api.
 Home-page: https://github.com/Nickwasused/altv-python-masterlist
 License: MPL-2.0
 Author: Nickwasused
 Author-email: contact.nickwasused.fa6c8@simplelogin.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
```

