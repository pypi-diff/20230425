# Comparing `tmp/python_roborock-0.7.1.tar.gz` & `tmp/python_roborock-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.7.1.tar", max compression
+gzip compressed data, was "python_roborock-0.7.2.tar", max compression
```

## Comparing `python_roborock-0.7.1.tar` & `python_roborock-0.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-25 03:16:51.837758 python_roborock-0.7.1/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-25 03:16:51.837758 python_roborock-0.7.1/README.md
--rw-r--r--   0        0        0     1370 2023-04-25 03:16:52.585765 python_roborock-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/__init__.py
--rw-r--r--   0        0        0    19384 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/cloud_api.py
--rw-r--r--   0        0        0     4283 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/code_mappings.py
--rw-r--r--   0        0        0     9872 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/exceptions.py
--rw-r--r--   0        0        0     6178 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/roborock_future.py
--rw-r--r--   0        0        0     6232 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/roborock_message.py
--rw-r--r--   0        0        0    12155 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/typing.py
--rw-r--r--   0        0        0      754 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-25 11:57:05.494174 python_roborock-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-25 11:57:05.494174 python_roborock-0.7.2/README.md
+-rw-r--r--   0        0        0     1370 2023-04-25 11:57:06.242186 python_roborock-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-25 11:57:05.494174 python_roborock-0.7.2/roborock/__init__.py
+-rw-r--r--   0        0        0    19300 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/cli.py
+-rw-r--r--   0        0        0     8241 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4283 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9872 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/exceptions.py
+-rw-r--r--   0        0        0     6178 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12103 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/typing.py
+-rw-r--r--   0        0        0      754 2023-04-25 11:57:05.498174 python_roborock-0.7.2/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.2/PKG-INFO
```

### Comparing `python_roborock-0.7.1/LICENSE` & `python_roborock-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/README.md` & `python_roborock-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/pyproject.toml` & `python_roborock-0.7.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.7.1"
+version = "0.7.2"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.7.1/roborock/api.py` & `python_roborock-0.7.2/roborock/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,21 +270,20 @@
 
             return DockSummary(dust_collection_mode, wash_towel_mode, smart_wash_params)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
     async def get_prop(self, device_id: str) -> DeviceProp | None:
-        [status, dnd_timer, clean_summary, consumable, multi_maps_list] = await asyncio.gather(
+        [status, dnd_timer, clean_summary, consumable] = await asyncio.gather(
             *[
                 self.get_status(device_id),
                 self.get_dnd_timer(device_id),
                 self.get_clean_summary(device_id),
-                self.get_consumable(device_id),
-                self.get_multi_maps_list(device_id)
+                self.get_consumable(device_id)
             ]
         )
         last_clean_record = None
         if clean_summary and clean_summary.records and len(clean_summary.records) > 0:
             last_clean_record = await self.get_clean_record(device_id, clean_summary.records[0])
         dock_summary = None
         if status and status.dock_type is not None and status.dock_type != RoborockDockTypeCode["0"]:
@@ -293,15 +292,14 @@
             return DeviceProp(
                 status,
                 dnd_timer,
                 clean_summary,
                 consumable,
                 last_clean_record,
                 dock_summary,
-                multi_maps_list
             )
         return None
 
     async def get_multi_maps_list(self, device_id) -> MultiMapsList | None:
         try:
             multi_maps_list = await self.send_command(device_id, RoborockCommand.GET_MULTI_MAPS_LIST)
             if isinstance(multi_maps_list, dict):
@@ -320,15 +318,15 @@
         return None
 
     async def get_room_mapping(self, device_id: str) -> list[RoomMapping]:
         """Gets the mapping from segment id -> iot id. Only works on local api."""
         mapping = await self.send_command(device_id, RoborockCommand.GET_ROOM_MAPPING)
         if isinstance(mapping, list):
             return [
-                RoomMapping(segment_id, iot_id)
+                RoomMapping(segment_id=segment_id, iot_id=segment_id)  # type: ignore
                 for segment_id, iot_id in [unpack_list(room, 2) for room in mapping]
             ]
         return []
 
 
 class RoborockApiClient:
     def __init__(self, username: str, base_url=None) -> None:
@@ -459,16 +457,15 @@
         )
         mac = base64.b64encode(hmac.new(rriot.h.encode(), prestr.encode(), hashlib.sha256).digest()).decode()
         if rriot.r.a is None:
             raise RoborockException("Missing field 'a' in rriot reference")
         home_request = PreparedRequest(
             rriot.r.a,
             {
-                "Authorization": f'Hawk id="{rriot.u}", s="{rriot.s}", ts="{timestamp}", nonce="{nonce}", '
-                f'mac="{mac}"',
+                "Authorization": f'Hawk id="{rriot.u}", s="{rriot.s}", ts="{timestamp}", nonce="{nonce}", mac="{mac}"',
             },
         )
         home_response = await home_request.request("get", "/user/homes/" + str(home_id))
         if not home_response.get("success"):
             raise RoborockException(home_response)
         home_data = home_response.get("result")
         if isinstance(home_data, dict):
```

### Comparing `python_roborock-0.7.1/roborock/cli.py` & `python_roborock-0.7.2/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/cloud_api.py` & `python_roborock-0.7.2/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/code_mappings.py` & `python_roborock-0.7.2/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/containers.py` & `python_roborock-0.7.2/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/exceptions.py` & `python_roborock-0.7.2/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/local_api.py` & `python_roborock-0.7.2/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/roborock_future.py` & `python_roborock-0.7.2/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/roborock_message.py` & `python_roborock-0.7.2/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/roborock/typing.py` & `python_roborock-0.7.2/roborock/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 
 CommandInfoMap: dict[RoborockCommand, CommandInfo] = {
     RoborockCommand.GET_PROP: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x77"),
     RoborockCommand.SET_CUSTOM_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.GET_CHILD_LOCK_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
-    RoborockCommand.GET_MULTI_MAPS_LIST: CommandInfo(prefix=b"\x00\x00\x00\xd7"),
+    RoborockCommand.GET_MULTI_MAPS_LIST: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.SET_WATER_BOX_CUSTOM_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_CLEAN_SEQUENCE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_CUSTOMIZE_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_CARPET_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.SET_CAMERA_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.SET_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x87"),
@@ -219,8 +219,7 @@
 class DeviceProp:
     status: Optional[Status] = None
     dnd_timer: Optional[DNDTimer] = None
     clean_summary: Optional[CleanSummary] = None
     consumable: Optional[Consumable] = None
     last_clean_record: Optional[CleanRecord] = None
     dock_summary: Optional[DockSummary] = None
-    multi_maps_list: Optional[MultiMapsList] = None
```

### Comparing `python_roborock-0.7.1/roborock/util.py` & `python_roborock-0.7.2/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.1/PKG-INFO` & `python_roborock-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.7.1
+Version: 0.7.2
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.7.1 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.7.2 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

