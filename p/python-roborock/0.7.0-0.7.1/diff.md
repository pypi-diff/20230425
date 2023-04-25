# Comparing `tmp/python_roborock-0.7.0.tar.gz` & `tmp/python_roborock-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.7.0.tar", max compression
+gzip compressed data, was "python_roborock-0.7.1.tar", max compression
```

## Comparing `python_roborock-0.7.0.tar` & `python_roborock-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-25 02:42:06.085425 python_roborock-0.7.0/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-25 02:42:06.085425 python_roborock-0.7.0/README.md
--rw-r--r--   0        0        0     1370 2023-04-25 02:42:06.857436 python_roborock-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/__init__.py
--rw-r--r--   0        0        0    19384 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/cli.py
--rw-r--r--   0        0        0     8241 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/cloud_api.py
--rw-r--r--   0        0        0     4283 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/code_mappings.py
--rw-r--r--   0        0        0     9872 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/exceptions.py
--rw-r--r--   0        0        0     6178 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/local_api.py
--rw-r--r--   0        0        0      694 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/roborock_future.py
--rw-r--r--   0        0        0     6115 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/roborock_message.py
--rw-r--r--   0        0        0    12220 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/typing.py
--rw-r--r--   0        0        0      754 2023-04-25 02:42:06.085425 python_roborock-0.7.0/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-25 03:16:51.837758 python_roborock-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-25 03:16:51.837758 python_roborock-0.7.1/README.md
+-rw-r--r--   0        0        0     1370 2023-04-25 03:16:52.585765 python_roborock-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/__init__.py
+-rw-r--r--   0        0        0    19384 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/cli.py
+-rw-r--r--   0        0        0     8241 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4283 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9872 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/exceptions.py
+-rw-r--r--   0        0        0     6178 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6232 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/roborock_message.py
+-rw-r--r--   0        0        0    12155 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/typing.py
+-rw-r--r--   0        0        0      754 2023-04-25 03:16:51.837758 python_roborock-0.7.1/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.7.1/PKG-INFO
```

### Comparing `python_roborock-0.7.0/LICENSE` & `python_roborock-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/README.md` & `python_roborock-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/pyproject.toml` & `python_roborock-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.7.0"
+version = "0.7.1"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.7.0/roborock/api.py` & `python_roborock-0.7.1/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/cli.py` & `python_roborock-0.7.1/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/cloud_api.py` & `python_roborock-0.7.1/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/code_mappings.py` & `python_roborock-0.7.1/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/containers.py` & `python_roborock-0.7.1/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/exceptions.py` & `python_roborock-0.7.1/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/local_api.py` & `python_roborock-0.7.1/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/roborock_future.py` & `python_roborock-0.7.1/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/roborock/roborock_message.py` & `python_roborock-0.7.1/roborock/roborock_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
     @staticmethod
     def encode(roborock_messages: list[RoborockMessage] | RoborockMessage, local_key: str):
         if isinstance(roborock_messages, RoborockMessage):
             roborock_messages = [roborock_messages]
 
         msg = b""
         for roborock_message in roborock_messages:
+            if len(roborock_message.prefix) not in [0, 4]:
+                raise RoborockException("Invalid prefix")
             aes_key = md5bin(encode_timestamp(roborock_message.timestamp) + local_key + salt)
             cipher = AES.new(aes_key, AES.MODE_ECB)
             payload = roborock_message.payload
             if payload:
                 payload = pad(roborock_message.payload, AES.block_size)
             encrypted = cipher.encrypt(payload)
             encrypted_len = len(encrypted)
```

### Comparing `python_roborock-0.7.0/roborock/typing.py` & `python_roborock-0.7.1/roborock/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     GET_COLLISION_AVOID_STATUS = "get_collision_avoid_status"
     CLOSE_VALLEY_ELECTRICITY_TIMER = "close_valley_electricity_timer"
     GET_VALLEY_ELECTRICITY_TIMER = "get_valley_electricity_timer"
     SET_CLEAN_MOTOR_MODE = "set_clean_motor_mode"
     SET_LED_STATUS = "set_led_status"
     GET_CAMERA_STATUS = "get_camera_status"
     CLOSE_DND_TIMER = "close_dnd_timer"
-    GET_MULTI_MAP = "get_multi_map"
     SET_COLLISION_AVOID_STATUS = "set_collision_avoid_status"
     SET_IDENTIFY_GROUND_MATERIAL_STATUS = "set_identify_ground_material_status"
     GET_IDENTIFY_GROUND_MATERIAL_STATUS = "get_identify_ground_material_status"
     SET_VALLEY_ELECTRICITY_TIMER = "set_valley_electricity_timer"
     SWITCH_WATER_MARK = "switch_water_mark"
     SET_IDENTIFY_FURNITURE_STATUS = "set_identify_furniture_status"
     GET_CLEAN_RECORD_MAP = "get_clean_record_map"
@@ -117,15 +116,15 @@
 
 
 CommandInfoMap: dict[RoborockCommand, CommandInfo] = {
     RoborockCommand.GET_PROP: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x77"),
     RoborockCommand.SET_CUSTOM_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.GET_CHILD_LOCK_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
-    RoborockCommand.GET_MULTI_MAPS_LIST: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.GET_MULTI_MAPS_LIST: CommandInfo(prefix=b"\x00\x00\x00\xd7"),
     RoborockCommand.GET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.SET_WATER_BOX_CUSTOM_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_CLEAN_SEQUENCE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_CUSTOMIZE_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_CARPET_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.SET_CAMERA_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.SET_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x87"),
@@ -150,47 +149,46 @@
     RoborockCommand.CLOSE_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_WAKEUP_ROBOT: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.SET_MOP_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.GET_DND_TIMER: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.GET_CARPET_MODE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.GET_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.SET_CARPET_MODE: CommandInfo(prefix=b"\x00\x00\x00\xd7"),
-    RoborockCommand.GET_MULTI_MAP: CommandInfo(prefix=b"\x00\x00\x00\xd7"),
-    RoborockCommand.SET_COLLISION_AVOID_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.SET_CARPET_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.SET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.GET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.SET_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.SWITCH_WATER_MARK: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.SET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.SET_CHILD_LOCK_STATUS: CommandInfo(prefix=b"\x00\x00\x97"),
-    RoborockCommand.GET_CLEAN_RECORD_MAP: CommandInfo(prefix=b"\x00\x00\xe7"),
+    RoborockCommand.SET_COLLISION_AVOID_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SET_CARPET_CLEAN_MODE: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.GET_IDENTIFY_GROUND_MATERIAL_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SET_VALLEY_ELECTRICITY_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SWITCH_WATER_MARK: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SET_IDENTIFY_FURNITURE_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.SET_CHILD_LOCK_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x97"),
+    RoborockCommand.GET_CLEAN_RECORD_MAP: CommandInfo(prefix=b"\x00\x00\x00\xe7"),
     RoborockCommand.APP_START: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_STOP: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_CHARGE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_SPOT: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.FIND_ME: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.RESUME_ZONED_CLEAN: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.RESUME_SEGMENT_CLEAN: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.RESET_CONSUMABLE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.LOAD_MULTI_MAP: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_RC_START: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_RC_END: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_RC_MOVE: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_GOTO_TARGET: CommandInfo(prefix=b"\x00\x00\x00\x87"),
-    RoborockCommand.APP_SEGMENT_CLEAN: CommandInfo(prefix=b"\x00\x00\x00\xc7"),
-    RoborockCommand.APP_ZONED_CLEAN: CommandInfo(prefix=b"\x00\x00\x00w"),
+    RoborockCommand.APP_SEGMENT_CLEAN: CommandInfo(prefix=b"\x00\x00\x00\x87"),
+    RoborockCommand.APP_ZONED_CLEAN: CommandInfo(prefix=b"\x00\x00\x00\x97"),
     RoborockCommand.APP_START_WASH: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.APP_STOP_WASH: CommandInfo(prefix=b"\x00\x00\x00w"),
-    RoborockCommand.SET_FDS_ENDPOINT: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_FDS_ENDPOINT: CommandInfo(prefix=b"\x00\x00\x00\x97"),
     RoborockCommand.ENABLE_LOG_UPLOAD: CommandInfo(prefix=b"\x00\x00\x87"),
     RoborockCommand.GET_SOUND_VOLUME: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.TEST_SOUND_VOLUME: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.UPD_SERVER_TIMER: CommandInfo(prefix=b"\x00\x00\x00\x97"),
-    RoborockCommand.SET_APP_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x97"),
+    RoborockCommand.SET_APP_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x00\x97"),
     RoborockCommand.CHANGE_SOUND_VOLUME: CommandInfo(prefix=b"\x00\x00\x00\x87"),
     RoborockCommand.GET_SOUND_PROGRESS: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.SET_SERVER_TIMER: CommandInfo(prefix=b"\x00\x00\x00\xc7"),
     RoborockCommand.GET_ROOM_MAPPING: CommandInfo(prefix=b"\x00\x00\x00w"),
     RoborockCommand.NAME_SEGMENT: CommandInfo(prefix=b"\x00\x00\x027"),
     RoborockCommand.SET_TIMEZONE: CommandInfo(prefix=b"\x00\x00\x00\x97"),
     RoborockCommand.GET_HOMESEC_CONNECT_STATUS: CommandInfo(prefix=b"\x00\x00\x00\x87"),
```

### Comparing `python_roborock-0.7.0/roborock/util.py` & `python_roborock-0.7.1/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.7.0/PKG-INFO` & `python_roborock-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.7.0
+Version: 0.7.1
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
-Metadata-Version: 2.1 Name: python-roborock Version: 0.7.0 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.7.1 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

