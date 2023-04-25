# Comparing `tmp/teslajsonpy-3.8.0.tar.gz` & `tmp/teslajsonpy-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teslajsonpy-3.8.0.tar", max compression
+gzip compressed data, was "teslajsonpy-3.8.1.tar", max compression
```

## Comparing `teslajsonpy-3.8.0.tar` & `teslajsonpy-3.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    23941 2023-03-26 03:47:03.767671 teslajsonpy-3.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-03-26 03:46:39.550903 teslajsonpy-3.8.0/LICENSE
--rw-r--r--   0        0        0     2391 2023-03-26 03:46:39.550903 teslajsonpy-3.8.0/README.md
--rw-r--r--   0        0        0     1558 2023-03-26 03:47:03.779672 teslajsonpy-3.8.0/pyproject.toml
--rw-r--r--   0        0        0      916 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/__init__.py
--rw-r--r--   0        0        0      222 2023-03-26 03:47:03.779672 teslajsonpy-3.8.0/teslajsonpy/__version__.py
--rw-r--r--   0        0        0    46760 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/car.py
--rw-r--r--   0        0        0    25716 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/connection.py
--rw-r--r--   0        0        0     1377 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/const.py
--rw-r--r--   0        0        0    53186 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/controller.py
--rw-r--r--   0        0        0    52966 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/endpoints.json
--rw-r--r--   0        0        0     9422 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/energy.py
--rw-r--r--   0        0        0     3382 2023-03-26 03:46:39.626906 teslajsonpy-3.8.0/teslajsonpy/exceptions.py
--rw-r--r--   0        0        0     7696 2023-03-26 03:46:39.630906 teslajsonpy-3.8.0/teslajsonpy/teslaproxy.py
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 teslajsonpy-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0    24168 2023-04-25 05:23:35.542426 teslajsonpy-3.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-04-25 05:23:04.142299 teslajsonpy-3.8.1/LICENSE
+-rw-r--r--   0        0        0     2391 2023-04-25 05:23:04.142299 teslajsonpy-3.8.1/README.md
+-rw-r--r--   0        0        0     1558 2023-04-25 05:23:35.554427 teslajsonpy-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0      916 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-25 05:23:35.554427 teslajsonpy-3.8.1/teslajsonpy/__version__.py
+-rw-r--r--   0        0        0    46764 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/car.py
+-rw-r--r--   0        0        0    25716 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/connection.py
+-rw-r--r--   0        0        0     1377 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/const.py
+-rw-r--r--   0        0        0    53186 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/controller.py
+-rw-r--r--   0        0        0    52966 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/endpoints.json
+-rw-r--r--   0        0        0     9422 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/energy.py
+-rw-r--r--   0        0        0     3382 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/exceptions.py
+-rw-r--r--   0        0        0     7696 2023-04-25 05:23:04.222300 teslajsonpy-3.8.1/teslajsonpy/teslaproxy.py
+-rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 teslajsonpy-3.8.1/PKG-INFO
```

### Comparing `teslajsonpy-3.8.0/CHANGELOG.md` & `teslajsonpy-3.8.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v3.8.1 (2023-04-25)
+### Fix
+* Handle missing climate_state ([#404](https://github.com/zabuldon/teslajsonpy/issues/404)) ([`342a2ef`](https://github.com/zabuldon/teslajsonpy/commit/342a2ef03c2ccd8b4281fb815107d423f3c1bddc))
+
 ## v3.8.0 (2023-03-26)
 ### Feature
 * Add energy_site_ids and vins to update to limit updating to specific devices ([#402](https://github.com/zabuldon/teslajsonpy/issues/402)) ([`e97ccaf`](https://github.com/zabuldon/teslajsonpy/commit/e97ccaf41dcc3df0dc526882a5b85c14480ac672))
 
 ## v3.7.5 (2023-03-21)
 ### Fix
 * Update endpoints.json for sharing ([#399](https://github.com/zabuldon/teslajsonpy/issues/399)) ([`e46d0d9`](https://github.com/zabuldon/teslajsonpy/commit/e46d0d968024107f7897dbb27387bf34a1fa0b87))
```

### Comparing `teslajsonpy-3.8.0/LICENSE` & `teslajsonpy-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/README.md` & `teslajsonpy-3.8.1/README.md`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/pyproject.toml` & `teslajsonpy-3.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "teslajsonpy"
-version = "3.8.0"
+version = "3.8.1"
 description = "A library to work with Tesla API."
 authors = ["Sergey Isachenko <sergey.isachenkol@bool.by>"]
 license = "Apache-2.0"
 repository = "https://github.com/zabuldon/teslajsonpy"
 readme = "README.md"
 homepage = "https://github.com/zabuldon/teslajsonpy"
 documentation = "https://teslajsonpy.readthedocs.io"
```

### Comparing `teslajsonpy-3.8.0/teslajsonpy/__init__.py` & `teslajsonpy-3.8.1/teslajsonpy/__init__.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/car.py` & `teslajsonpy-3.8.1/teslajsonpy/car.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,15 +870,15 @@
             params = {f"seat_heater_{SEAT_ID_MAP[seat_id]}": level}
             self._vehicle_data["climate_state"].update(params)
 
     def get_seat_heater_status(self, seat_id: int) -> int:
         """Return status of seat heater for a given seat."""
         seat_id = f"seat_heater_{SEAT_ID_MAP[seat_id]}"
         if self.data_available:
-            return self._vehicle_data.get("climate_state").get(seat_id)
+            return self._vehicle_data.get("climate_state", {}).get(seat_id)
         return None
 
     async def schedule_software_update(self, offset_sec: Optional[int] = 0) -> None:
         """Send command to install software update."""
         await self._send_command("SCHEDULE_SOFTWARE_UPDATE", offset_sec=offset_sec)
 
     async def set_charging_amps(self, value: float) -> None:
```

### Comparing `teslajsonpy-3.8.0/teslajsonpy/connection.py` & `teslajsonpy-3.8.1/teslajsonpy/connection.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/const.py` & `teslajsonpy-3.8.1/teslajsonpy/const.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/controller.py` & `teslajsonpy-3.8.1/teslajsonpy/controller.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/endpoints.json` & `teslajsonpy-3.8.1/teslajsonpy/endpoints.json`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/energy.py` & `teslajsonpy-3.8.1/teslajsonpy/energy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/exceptions.py` & `teslajsonpy-3.8.1/teslajsonpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/teslajsonpy/teslaproxy.py` & `teslajsonpy-3.8.1/teslajsonpy/teslaproxy.py`

 * *Files identical despite different names*

### Comparing `teslajsonpy-3.8.0/PKG-INFO` & `teslajsonpy-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teslajsonpy
-Version: 3.8.0
+Version: 3.8.1
 Summary: A library to work with Tesla API.
 Home-page: https://github.com/zabuldon/teslajsonpy
 License: Apache-2.0
 Author: Sergey Isachenko
 Author-email: sergey.isachenkol@bool.by
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

