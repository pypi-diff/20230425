# Comparing `tmp/skylab-0.1.0.tar.gz` & `tmp/skylab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skylab-0.1.0.tar", max compression
+gzip compressed data, was "skylab-0.1.1.tar", max compression
```

## Comparing `skylab-0.1.0.tar` & `skylab-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      652 2023-04-23 21:10:19.907374 skylab-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 12:22:31.765336 skylab-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-21 22:27:55.460381 skylab-0.1.0/skylab/__init__.py
--rw-r--r--   0        0        0      236 2023-04-23 20:49:08.128455 skylab-0.1.0/skylab/__main__.py
--rw-r--r--   0        0        0     1135 2023-04-23 20:33:27.980025 skylab-0.1.0/skylab/api.py
--rw-r--r--   0        0        0      356 2023-04-23 19:43:05.423689 skylab-0.1.0/skylab/css/styles.css
--rw-r--r--   0        0        0     4751 2023-04-23 20:33:24.736191 skylab-0.1.0/skylab/skylab.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 skylab-0.1.0/setup.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 skylab-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-23 21:28:56.735383 skylab-0.1.1/LICENSE
+-rw-r--r--   0        0        0      831 2023-04-25 12:00:39.422608 skylab-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      857 2023-04-24 19:11:31.739686 skylab-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 22:27:55.460381 skylab-0.1.1/skylab/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-23 22:12:51.429163 skylab-0.1.1/skylab/__main__.py
+-rw-r--r--   0        0        0     1112 2023-04-24 19:15:43.017845 skylab-0.1.1/skylab/api.py
+-rw-r--r--   0        0        0      424 2023-04-24 13:45:07.205633 skylab-0.1.1/skylab/css/styles.css
+-rw-r--r--   0        0        0     1668 2023-04-24 19:11:57.443257 skylab-0.1.1/skylab/models.py
+-rw-r--r--   0        0        0     5100 2023-04-24 14:45:36.607699 skylab-0.1.1/skylab/skylab.py
+-rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 skylab-0.1.1/setup.py
+-rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 skylab-0.1.1/PKG-INFO
```

### Comparing `skylab-0.1.0/skylab/api.py` & `skylab-0.1.1/skylab/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,30 @@
-import requests
-from pydantic import BaseModel
-
-GET_UPCOMING_LAUNCHES = "https://lldev.thespacedevs.com/2.2.0/launch/upcoming/"
-
-
-class LaunchProvier(BaseModel):
-    name: str
-    url: str
-
+"""Api module for receiving data from thespacedevs."""
 
-class Mission(BaseModel):
-    name: str
-    description: str
-
-
-class Rocket(BaseModel):
-    full_name: str
-    ...
+import requests
 
+from skylab.models import Launch
 
-class Launch(BaseModel):
-    name: str
-    net: str
-    rocket: Rocket
-    mission: Mission
-    launch_service_provider: LaunchProvier
+GET_UPCOMING_LAUNCHES = "https://lldev.thespacedevs.com/2.2.0/launch/upcoming/"
 
 
-def get_upcoming_laucnhes(url: str, timeout: float = 5.0) -> list:
+def get_upcoming_laucnhes(url: str, timeout: float = 5.0) -> dict:
     """Get request for upcoming launches."""
     response = requests.get(url, timeout=timeout)
     response.raise_for_status()
-    return response.json()["results"]
+    return response.json()
 
 
 def launch_factory() -> list[Launch]:
     """Makes a request for upcoming launches, modifies and validates them."""
-    results = get_upcoming_laucnhes(GET_UPCOMING_LAUNCHES)
+    results = get_upcoming_laucnhes(GET_UPCOMING_LAUNCHES)["results"]
     launches = []
     for launch_dict in results:
+        # removing "configuration" nested layer from given data
         rocket_config = launch_dict["rocket"].pop("configuration")
         launch_dict["rocket"].update(rocket_config)
+
+        # getting address name from "location" json
+        launch_pad_address = launch_dict["pad"].pop("location")["name"]
+        launch_dict["pad"]["address"] = launch_pad_address
         launches.append(Launch(**launch_dict))
     return launches
```

### Comparing `skylab-0.1.0/skylab/skylab.py` & `skylab-0.1.1/skylab/skylab.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import datetime
 import os
 import random
 import urllib.parse
 import webbrowser
 
-import skylab.api
 import tzlocal
-from skylab.api import Launch
 from textual.app import App, ComposeResult
 from textual.color import Color
 from textual.containers import Container
 from textual.reactive import reactive
 from textual.widgets import Button, Footer, Header, Static
 
+import skylab.api
+from skylab.models import Launch
+
 CURR_DIR = os.path.dirname(os.path.abspath(__file__))
 LOCAL_TIMEZONE = tzlocal.get_localzone()
 
 
 class TimeDisplay(Static):
     """Time till launch Static."""
 
@@ -59,32 +60,44 @@
 
     def __init__(self, *args, **kwargs) -> None:
         """Initialize LaunchWidget."""
         # remove launch object from kwargs before doing super()
         self.launch: Launch = kwargs.pop("launch")
         super().__init__(*args, **kwargs)
         self._net = datetime.datetime.fromisoformat(self.launch.net[:-1])
+        self._launch_time = Static(
+            f"{LOCAL_TIMEZONE.localize(self._net)}\n", classes="launch-time"
+        )
+        self._launch_provider = Static(f"{self.launch.launch_service_provider.name}\n")
+        self._rocket_name = Static(f"{self.launch.rocket.full_name}\n")
+        self._launch_pad = Static(
+            f"{self.launch.pad.name}, {self.launch.pad.address}\n"
+        )
         self._description = Static(f"{self.launch.mission.description}")
-        self._rocket_name = Static(f"Rocket: {self.launch.rocket.full_name}\n")
-        self._launch_time = Static(f"{LOCAL_TIMEZONE.localize(self._net)}\n")
 
     def on_button_pressed(self) -> None:
         """
         Event handler called when a button is pressed.
         On press creates a youtube search query for upcoming launch.
         """
         query = f"{self.launch.name} {self._net}"
         launch_url = (
             f"{self.youtube_url}/results?search_query={urllib.parse.quote(query)}"
         )
         webbrowser.open(launch_url, new=2)
 
     def compose(self) -> ComposeResult:
         """Creates a child widget of LaunchWidget."""
-        yield Container(self._launch_time, self._rocket_name, self._description)
+        yield Container(
+            self._launch_time,
+            self._launch_provider,
+            self._rocket_name,
+            self._launch_pad,
+            self._description,
+        )
         yield Container(
             TimeDisplay(launch_time=self._net, id="time-left"),
             Button("Watch", id="watch_button"),
         )
 
 
 class SkylabApp(App):
@@ -104,20 +117,20 @@
     def on_mount(self) -> None:
         """
         Event handler for when widget added to the app.
         Changes style of given LaunchWidgets such as border,
         background-color, border_title, etc.
         """
         for launch_widget in self.launch_widget_list:
-            colors = [
+            launch_widget.styles.background = Color(
                 random.randint(0, 255),
                 random.randint(0, 255),
                 random.randint(0, 255),
-            ]
-            launch_widget.styles.background = Color(*colors, a=0.45)
+                0.45,
+            )
             launch_widget.styles.border = ("round", "white")
             launch_widget.border_title = launch_widget.launch.name
             launch_widget.styles.border_title_align = "left"
 
     def action_exit(self) -> None:
         """Bindings action method for app exit."""
         self.exit()
```

