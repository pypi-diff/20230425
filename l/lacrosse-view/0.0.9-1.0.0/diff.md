# Comparing `tmp/lacrosse_view-0.0.9.tar.gz` & `tmp/lacrosse_view-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacrosse_view-0.0.9.tar", last modified: Tue Jul 26 22:16:35 2022, max compression
+gzip compressed data, was "lacrosse_view-1.0.0.tar", last modified: Mon Apr 24 23:09:20 2023, max compression
```

## Comparing `lacrosse_view-0.0.9.tar` & `lacrosse_view-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-26 22:16:35.464048 lacrosse_view-0.0.9/
--rw-r--r--   0 pi        (1000) pi        (1000)     1064 2022-06-28 16:42:09.000000 lacrosse_view-0.0.9/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     2128 2022-07-26 22:16:35.464048 lacrosse_view-0.0.9/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1592 2022-06-28 16:42:09.000000 lacrosse_view-0.0.9/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      103 2022-06-28 16:42:09.000000 lacrosse_view-0.0.9/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)      769 2022-07-26 22:16:35.474048 lacrosse_view-0.0.9/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-26 22:16:35.444049 lacrosse_view-0.0.9/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-26 22:16:35.454048 lacrosse_view-0.0.9/src/lacrosse_view/
--rw-r--r--   0 pi        (1000) pi        (1000)    11393 2022-07-26 22:14:10.000000 lacrosse_view-0.0.9/src/lacrosse_view/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2022-06-28 16:42:09.000000 lacrosse_view-0.0.9/src/lacrosse_view/py.typed
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-07-26 22:16:35.464048 lacrosse_view-0.0.9/src/lacrosse_view.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2128 2022-07-26 22:16:35.000000 lacrosse_view-0.0.9/src/lacrosse_view.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      303 2022-07-26 22:16:35.000000 lacrosse_view-0.0.9/src/lacrosse_view.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-07-26 22:16:35.000000 lacrosse_view-0.0.9/src/lacrosse_view.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       36 2022-07-26 22:16:35.000000 lacrosse_view-0.0.9/src/lacrosse_view.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       14 2022-07-26 22:16:35.000000 lacrosse_view-0.0.9/src/lacrosse_view.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:09:20.658281 lacrosse_view-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-24 23:09:20.658281 lacrosse_view-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-24 23:09:20.658281 lacrosse_view-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:09:20.654281 lacrosse_view-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:09:20.654281 lacrosse_view-1.0.0/src/lacrosse_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/src/lacrosse_view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/src/lacrosse_view/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/src/lacrosse_view/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-24 23:09:09.000000 lacrosse_view-1.0.0/src/lacrosse_view/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:09:20.658281 lacrosse_view-1.0.0/src/lacrosse_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-24 23:09:20.000000 lacrosse_view-1.0.0/src/lacrosse_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 23:09:20.000000 lacrosse_view-1.0.0/src/lacrosse_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:09:20.000000 lacrosse_view-1.0.0/src/lacrosse_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 23:09:20.000000 lacrosse_view-1.0.0/src/lacrosse_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 23:09:20.000000 lacrosse_view-1.0.0/src/lacrosse_view.egg-info/top_level.txt
```

### Comparing `lacrosse_view-0.0.9/LICENSE` & `lacrosse_view-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lacrosse_view-0.0.9/PKG-INFO` & `lacrosse_view-1.0.0/src/lacrosse_view.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lacrosse_view
-Version: 0.0.9
+Name: lacrosse-view
+Version: 1.0.0
 Summary: Client for retrieving data from the La Crosse View cloud
 Home-page: https://github.com/IceBotYT/lacrosse_view
 Author: IceBotYT
 Author-email: icebotyt@outlook.com
 Project-URL: Bug Tracker, https://github.com/IceBotYT/lacrosse_view/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,32 +29,42 @@
 pip install lacrosse_view
 ```
 
 ## Usage
 
 This example shows how to get the latest data from every sensor connected to the first location on your account.
 ```python
+
 from lacrosse_view import LaCrosse
 import asyncio
+from datetime import datetime, timedelta
+import time
 
 async def get_data():
     api = LaCrosse()
     # Log in to your LaCrosse View account
-    await api.login('paulus@home-assistant.io', 'password')
+    await api.login('username', 'password')
     # Get the sensors from the first location on the account
     locations = await api.get_locations()
-    sensors = await api.get_sensors(locations[0], tz="America/New_York", start=datetime.now() - timedelta(minutes=1), end=datetime.now())
+    startTime = datetime.now() - timedelta(minutes=1)
+    endTime = datetime.now()
+    startTimeUnix = time.mktime(startTime.timetuple())
+    endTimeUnix = time.mktime(endTime.timetuple())
+    sensors = await api.get_sensors(locations[0], tz="America/Vancouver", start=startTimeUnix, end=endTimeUnix)
  
     for sensor in sensors:
         for field in sensor.sensor_field_names:
             # Each value is a dictionary with keys "s" and "u". "s" is the value and "u" is the Unix timestamp for it.
+            value = sensor.data[field]["values"][-1]["s"]
             print(
-                f"{sensor.name} {field}: {sensor.data[field]["values"][-1]["s"]}"
+                f"{sensor.name} {field}: {value}"
             )
     
     await api.logout()
 
 asyncio.run(get_data())
+
+
 ```
 
 ## Questions?
 If you have any questions, please, don't hesitate to [open an issue](https://github.com/IceBotYT/lacrosse_view/issues/new).
```

### Comparing `lacrosse_view-0.0.9/README.md` & `lacrosse_view-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: lacrosse_view
+Version: 1.0.0
+Summary: Client for retrieving data from the La Crosse View cloud
+Home-page: https://github.com/IceBotYT/lacrosse_view
+Author: IceBotYT
+Author-email: icebotyt@outlook.com
+Project-URL: Bug Tracker, https://github.com/IceBotYT/lacrosse_view/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # La Crosse View
 
 A library for retrieving data from [La Crosse View-connected sensors](https://www.lacrossetechnology.com/collections/lacrosse-view-connected).
 
 ## Disclaimer
 
 This library is **NOT** for the Jeelink LaCrosse sensors. You can find that library [here](https://pypi.org/project/pylacrosse/).
@@ -14,32 +29,42 @@
 pip install lacrosse_view
 ```
 
 ## Usage
 
 This example shows how to get the latest data from every sensor connected to the first location on your account.
 ```python
+
 from lacrosse_view import LaCrosse
 import asyncio
+from datetime import datetime, timedelta
+import time
 
 async def get_data():
     api = LaCrosse()
     # Log in to your LaCrosse View account
-    await api.login('paulus@home-assistant.io', 'password')
+    await api.login('username', 'password')
     # Get the sensors from the first location on the account
     locations = await api.get_locations()
-    sensors = await api.get_sensors(locations[0], tz="America/New_York", start=datetime.now() - timedelta(minutes=1), end=datetime.now())
+    startTime = datetime.now() - timedelta(minutes=1)
+    endTime = datetime.now()
+    startTimeUnix = time.mktime(startTime.timetuple())
+    endTimeUnix = time.mktime(endTime.timetuple())
+    sensors = await api.get_sensors(locations[0], tz="America/Vancouver", start=startTimeUnix, end=endTimeUnix)
  
     for sensor in sensors:
         for field in sensor.sensor_field_names:
             # Each value is a dictionary with keys "s" and "u". "s" is the value and "u" is the Unix timestamp for it.
+            value = sensor.data[field]["values"][-1]["s"]
             print(
-                f"{sensor.name} {field}: {sensor.data[field]["values"][-1]["s"]}"
+                f"{sensor.name} {field}: {value}"
             )
     
     await api.logout()
 
 asyncio.run(get_data())
+
+
 ```
 
 ## Questions?
-If you have any questions, please, don't hesitate to [open an issue](https://github.com/IceBotYT/lacrosse_view/issues/new).
+If you have any questions, please, don't hesitate to [open an issue](https://github.com/IceBotYT/lacrosse_view/issues/new).
```

### Comparing `lacrosse_view-0.0.9/setup.cfg` & `lacrosse_view-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lacrosse_view
-version = 0.0.9
+version = 1.0.0
 author = IceBotYT
 author_email = icebotyt@outlook.com
 description = Client for retrieving data from the La Crosse View cloud
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IceBotYT/lacrosse_view
 project_urls =
```

### Comparing `lacrosse_view-0.0.9/src/lacrosse_view.egg-info/PKG-INFO` & `lacrosse_view-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: lacrosse-view
-Version: 0.0.9
-Summary: Client for retrieving data from the La Crosse View cloud
-Home-page: https://github.com/IceBotYT/lacrosse_view
-Author: IceBotYT
-Author-email: icebotyt@outlook.com
-Project-URL: Bug Tracker, https://github.com/IceBotYT/lacrosse_view/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # La Crosse View
 
 A library for retrieving data from [La Crosse View-connected sensors](https://www.lacrossetechnology.com/collections/lacrosse-view-connected).
 
 ## Disclaimer
 
 This library is **NOT** for the Jeelink LaCrosse sensors. You can find that library [here](https://pypi.org/project/pylacrosse/).
@@ -29,32 +14,42 @@
 pip install lacrosse_view
 ```
 
 ## Usage
 
 This example shows how to get the latest data from every sensor connected to the first location on your account.
 ```python
+
 from lacrosse_view import LaCrosse
 import asyncio
+from datetime import datetime, timedelta
+import time
 
 async def get_data():
     api = LaCrosse()
     # Log in to your LaCrosse View account
-    await api.login('paulus@home-assistant.io', 'password')
+    await api.login('username', 'password')
     # Get the sensors from the first location on the account
     locations = await api.get_locations()
-    sensors = await api.get_sensors(locations[0], tz="America/New_York", start=datetime.now() - timedelta(minutes=1), end=datetime.now())
+    startTime = datetime.now() - timedelta(minutes=1)
+    endTime = datetime.now()
+    startTimeUnix = time.mktime(startTime.timetuple())
+    endTimeUnix = time.mktime(endTime.timetuple())
+    sensors = await api.get_sensors(locations[0], tz="America/Vancouver", start=startTimeUnix, end=endTimeUnix)
  
     for sensor in sensors:
         for field in sensor.sensor_field_names:
             # Each value is a dictionary with keys "s" and "u". "s" is the value and "u" is the Unix timestamp for it.
+            value = sensor.data[field]["values"][-1]["s"]
             print(
-                f"{sensor.name} {field}: {sensor.data[field]["values"][-1]["s"]}"
+                f"{sensor.name} {field}: {value}"
             )
     
     await api.logout()
 
 asyncio.run(get_data())
+
+
 ```
 
 ## Questions?
-If you have any questions, please, don't hesitate to [open an issue](https://github.com/IceBotYT/lacrosse_view/issues/new).
+If you have any questions, please, don't hesitate to [open an issue](https://github.com/IceBotYT/lacrosse_view/issues/new).
```

